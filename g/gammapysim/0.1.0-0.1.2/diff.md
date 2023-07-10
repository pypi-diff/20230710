# Comparing `tmp/gammapysim-0.1.0.tar.gz` & `tmp/gammapysim-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammapysim-0.1.0.tar", last modified: Thu Mar  9 14:40:45 2023, max compression
+gzip compressed data, was "gammapysim-0.1.2.tar", max compression
```

## Comparing `gammapysim-0.1.0.tar` & `gammapysim-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,4 @@
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-03-09 14:40:45.936194 gammapysim-0.1.0/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       54 2023-03-09 14:40:45.936194 gammapysim-0.1.0/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        0 2023-02-22 17:45:22.000000 gammapysim-0.1.0/README.md
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-03-09 14:40:45.936194 gammapysim-0.1.0/gammapysim.egg-info/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       54 2023-03-09 14:40:45.000000 gammapysim-0.1.0/gammapysim.egg-info/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      198 2023-03-09 14:40:45.000000 gammapysim-0.1.0/gammapysim.egg-info/SOURCES.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2023-03-09 14:40:45.000000 gammapysim-0.1.0/gammapysim.egg-info/dependency_links.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2023-03-09 14:40:45.000000 gammapysim-0.1.0/gammapysim.egg-info/top_level.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     4100 2023-02-22 17:44:20.000000 gammapysim-0.1.0/gammapysim.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     4936 2023-02-22 17:28:10.000000 gammapysim-0.1.0/gammapysim.xml
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      287 2023-02-22 17:34:14.000000 gammapysim-0.1.0/pyproject.toml
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       38 2023-03-09 14:40:45.936194 gammapysim-0.1.0/setup.cfg
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      129 2023-03-09 14:37:21.000000 gammapysim-0.1.0/setup.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:21:41.429993 gammapysim-0.1.2/README.md
+-rw-r--r--   0        0        0     4115 2023-07-10 13:39:14.192117 gammapysim-0.1.2/gammapysim.py
+-rw-r--r--   0        0        0      338 2023-07-10 13:54:05.995332 gammapysim-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 gammapysim-0.1.2/PKG-INFO
```

### Comparing `gammapysim-0.1.0/gammapysim.py` & `gammapysim-0.1.2/gammapysim.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,132 +1,127 @@
-
-import matplotlib.pyplot as plt
 from pathlib import Path
+import click
+
 import numpy as np
-from astropy.coordinates import SkyCoord
 import astropy.units as u
+from astropy.coordinates import SkyCoord
+import matplotlib.pyplot as plt
 from astropy.io import fits
-from astropy.table import Table
-from astropy.time import Time
-from astropy.coordinates import SkyCoord, Angle
-from regions import CircleSkyRegion
-from gammapy.data import DataStore, Observation
+
+# %matplotlib inline
+from IPython.display import display
+from gammapy.data import Observation, observatory_locations
 from gammapy.datasets import MapDataset, MapDatasetEventSampler
-from gammapy.estimators import LightCurveEstimator
-from gammapy.maps import MapAxis, WcsGeom, Map, RegionGeom
-from gammapy.irf import load_cta_irfs
-from gammapy.makers import MapDatasetMaker
+from gammapy.irf import load_irf_dict_from_file
+from gammapy.makers import MapDatasetMaker, SafeMaskMaker
+from gammapy.maps import MapAxis, WcsGeom
 from gammapy.modeling import Fit
 from gammapy.modeling.models import (
-    Model,
+    FoVBackgroundModel,
+    GaussianSpatialModel,
     Models,
-    SkyModel,
     PowerLawSpectralModel,
-    PowerLawNormSpectralModel,
-    TemplateSpectralModel,
-    PointSpatialModel,
-    GaussianSpatialModel,
-    TemplateSpatialModel,
-    ConstantTemporalModel,
-    ExpDecayTemporalModel,
-    LightCurveTemplateTemporalModel,
-    FoVBackgroundModel,
+    SkyModel,
 )
-from regions import CircleSkyRegion, PointSkyRegion
-
-def save_events(events, dataset, number):
-    """Save simulated event list.
 
-    Input
+   
+def synth_for_pointing(livetime, pointing):
+    # Loading IRFs
+    irfs = load_irf_dict_from_file(
+        "$GAMMAPY_DATA/cta-1dc/caldb/data/cta/1dc/bcf/South_z20_50h/irf_file.fits"
+    )
 
-    events: ~gammapy.EventList
-    dataset: ~gammapy.Dataset
-    number: identifier
-    """
-    primary_hdu = fits.PrimaryHDU()
-    hdu_evt = fits.BinTableHDU(events.table)
-    hdu_gti = fits.BinTableHDU(dataset.gti.table, name="GTI")
-    hdu_all = fits.HDUList([primary_hdu, hdu_evt, hdu_gti])
-    hdu_all.writeto(f"./events_{number}.fits", overwrite=True)
+    # Define map geometry for binned simulation
+    energy_reco = MapAxis.from_edges(
+        np.logspace(-1.0, 1.0, 10), unit="TeV", name="energy", interp="log"
+    )
+    geom = WcsGeom.create(
+        skydir=(0, 0),
+        binsz=0.02,
+        width=(6, 6),
+        frame="galactic",
+        axes=[energy_reco],
+    )
+    # It is usually useful to have a separate binning for the true energy axis
+    energy_true = MapAxis.from_edges(
+        np.logspace(-1.5, 1.5, 30), unit="TeV", name="energy_true", interp="log"
+    )
 
-filename = "data/Prod5-North-20deg-AverageAz-4LSTs09MSTs.180000s-v0.1.fits.gz"
-IRFS = load_cta_irfs(filename)
+    migra_axis = MapAxis.from_bounds(0.5, 2, nbin=150, node_type="edges", name="migra")
 
+    empty = MapDataset.create(geom, name="dataset-simu", energy_axis_true=energy_true, migra_axis=migra_axis)
 
-from gammapy.modeling.models import PowerLawSpectralModel
-from gammapy.modeling.models import GaussianSpatialModel
+    # Define sky model to used simulate the data.
+    # Here we use a Gaussian spatial model and a Power Law spectral model.
+    spatial_model = GaussianSpatialModel(
+        lon_0="0.2 deg", lat_0="0.1 deg", sigma="0.3 deg", frame="galactic"
+    )
+    spectral_model = PowerLawSpectralModel(
+        index=3, amplitude="1e-11 cm-2 s-1 TeV-1", reference="1 TeV"
+    )
+    model_simu = SkyModel(
+        spatial_model=spatial_model,
+        spectral_model=spectral_model,
+        name="model-simu",
+    )
 
+    bkg_model = FoVBackgroundModel(dataset_name="dataset-simu")
 
-pwl = PowerLawSpectralModel(amplitude="2.7e-12 TeV-1 cm-2 s-1", index=2.2)
-gauss = GaussianSpatialModel(
-    lon_0="0 deg", lat_0="0 deg", sigma="0.2 deg", frame="galactic"
-)
+    models = Models([model_simu, bkg_model])
+    print(models)
 
-modelsky = SkyModel(spectral_model=pwl, spatial_model=gauss, name="my-source")
-print(modelsky)
+    file_model = "point-pwl.yaml"
+    models.write(file_model, overwrite=True)
 
-bkg_model = FoVBackgroundModel(dataset_name="my-dataset")
+    # Create an in-memory observation
+    location = observatory_locations["cta_south"]
+    obs = Observation.create(
+        pointing=pointing, livetime=livetime, irfs=irfs, location=location
+    )
+    print(obs)
 
-# modelsky.append(bkg_model)
+    # Make the MapDataset
+    maker = MapDatasetMaker(selection=["exposure", "background", "psf", "edisp"])
 
-   
-def synth_for_pointing(i, pointing):
-    print(f"Make the observation for pointing {i}...")
-    observation = Observation.create(
-                      obs_id="{:06d}".format(i), pointing=pointing, 
-                      livetime="0.01 hr", 
-                      irfs=IRFS
-                      )
-
-    print(f"Create the dataset for {pointing}")
-    energy_axis = MapAxis.from_energy_bounds(
-        "0.012 TeV", "100 TeV", nbin=2, per_decade=True
-        )
-    energy_axis_true = MapAxis.from_energy_bounds(
-        "0.001 TeV", "300 TeV", nbin=5, per_decade=True, name="energy_true"
-        )
-    migra_axis = MapAxis.from_bounds(
-        0.5, 2, nbin=15, node_type="edges", name="migra"
-        )
+    maker_safe_mask = SafeMaskMaker(methods=["offset-max"], offset_max=4.0 * u.deg)
 
-    geom = WcsGeom.create(
-        skydir=pointing,
-        width=(12, 12),
-        binsz=0.02,
-        frame="icrs",
-        axes=[energy_axis],
-    )
+    dataset = maker.run(empty, obs)
+    dataset = maker_safe_mask.run(dataset, obs)
+    print(dataset)
 
-    empty = MapDataset.create(
-            geom,
-            energy_axis_true=energy_axis_true,
-            migra_axis=migra_axis,
-            name="my-dataset",
-                )
-    maker = MapDatasetMaker(selection=["exposure", "background", "psf", "edisp"])
-    dataset = maker.run(empty, observation)
+    Path("event_sampling").mkdir(exist_ok=True)
+    dataset.write("./event_sampling/dataset.fits", overwrite=True)
 
-    rad_size = 1
-    region_sky = CircleSkyRegion(center=pointing, radius=rad_size * u.deg)
-    mask_map = dataset.geoms["geom"].region_mask(region_sky)
-    mod = modelsky.select_mask(mask_map)
+    # Add the model on the dataset and Poisson fluctuate
+    dataset.models = models
+    dataset.fake()
+    # Do a print on the dataset - there is now a counts maps
+    print(dataset)
 
-    bkg_idx = np.where(np.array(modelsky.names) == 'my-dataset-bkg')
-    mod.append(modelsky[int(bkg_idx[0][0])])
+    sampler = MapDatasetEventSampler(random_state=0)
+    events = sampler.run(dataset, obs)
 
-    dataset.models = mod
+    print(f"Source events: {(events.table['MC_ID'] == 1).sum()}")
+    print(f"Background events: {(events.table['MC_ID'] == 0).sum()}")
 
-    for m in dataset.models[:-1]:
-        sep = m.spatial_model.position.separation(pointing).deg
-        print(f"This is the spatial separation of {m.name} from the pointing direction: {sep}")
+    events.peek()
+    plt.savefig("peek.png")
+    events.select_offset([0, 1] * u.deg).peek()
+    plt.savefig("peek-focus.png")
 
-    print("Simulate...")
-    sampler = MapDatasetEventSampler(random_state=i)
-    events = sampler.run(dataset, observation)
+    # To plot, eg, counts:
+    # dataset.counts.smooth(0.05 * u.deg).plot_interactive(add_cbar=True, stretch="linear")
+    # plt.savefig("counts.png")
 
-    print(f"Save events {i}...")
-    save_events(events, dataset, "{:06d}".format(i))
 
-pointing = SkyCoord(0.0, 0.0, unit="deg", frame="galactic")
+@click.command()
+@click.option("--obs_id", default=1, help="Observation ID")
+@click.option("--livetime-hr", default=1, help="Livetime (hours)")
+@click.option("--pointing-coord", default="0 0", help="Pointing coordinate (SkyCoord)")
+def main(obs_id, livetime_hr, pointing_coord):
+    livetime = livetime_hr * u.hr
+    pointing = SkyCoord(pointing_coord, unit="deg", frame="galactic")
 
-synth_for_pointing(0, pointing)
+    synth_for_pointing(livetime, pointing)
 
+if __name__ == "__main__":
+    main()
```

