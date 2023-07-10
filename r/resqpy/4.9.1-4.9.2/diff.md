# Comparing `tmp/resqpy-4.9.1.tar.gz` & `tmp/resqpy-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resqpy-4.9.1.tar", max compression
+gzip compressed data, was "resqpy-4.9.2.tar", max compression
```

## Comparing `resqpy-4.9.1.tar` & `resqpy-4.9.2.tar`

### file list

```diff
@@ -1,198 +1,198 @@
--rw-r--r--   0        0        0     1059 2023-07-05 08:19:11.161633 resqpy-4.9.1/LICENSE
--rw-r--r--   0        0        0     2893 2023-07-05 08:19:11.161633 resqpy-4.9.1/README.md
--rw-r--r--   0        0        0     3354 2023-07-05 08:19:26.629743 resqpy-4.9.1/pyproject.toml
--rw-r--r--   0        0        0      555 2023-07-05 08:19:26.629743 resqpy-4.9.1/resqpy/__init__.py
--rw-r--r--   0        0        0    24782 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/crs.py
--rw-r--r--   0        0        0     1982 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/__init__.py
--rw-r--r--   0        0        0     6410 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_add_edges_per_column_property_array.py
--rw-r--r--   0        0        0    21022 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_add_faults.py
--rw-r--r--   0        0        0     6417 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_add_one_blocked_well_property.py
--rw-r--r--   0        0        0     8657 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_add_one_grid_property_array.py
--rw-r--r--   0        0        0     2431 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_add_single_cell_grid.py
--rw-r--r--   0        0        0     5495 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_add_wells_from_ascii_file.py
--rw-r--r--   0        0        0     6037 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_add_zone_by_layer_property.py
--rw-r--r--   0        0        0    11586 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_coarsened_grid.py
--rw-r--r--   0        0        0    10520 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_common.py
--rw-r--r--   0        0        0     3730 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_copy_grid.py
--rw-r--r--   0        0        0    11731 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_drape_to_surface.py
--rw-r--r--   0        0        0    16391 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_extract_box.py
--rw-r--r--   0        0        0    22969 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_extract_box_for_well.py
--rw-r--r--   0        0        0    20325 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_fault_throw_scaling.py
--rw-r--r--   0        0        0     7157 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_gather_ensemble.py
--rw-r--r--   0        0        0    17929 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_interpolated_grid.py
--rw-r--r--   0        0        0     9876 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_local_depth_adjustment.py
--rw-r--r--   0        0        0    20513 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_refined_grid.py
--rw-r--r--   0        0        0     5166 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_tilted_grid.py
--rw-r--r--   0        0        0     4792 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_unsplit_grid.py
--rw-r--r--   0        0        0    18825 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_zonal_grid.py
--rw-r--r--   0        0        0     4358 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/derived_model/_zone_layer_ranges_from_array.py
--rw-r--r--   0        0        0      996 2023-07-05 08:19:11.177633 resqpy-4.9.1/resqpy/fault/__init__.py
--rw-r--r--   0        0        0    29402 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/fault/_gcs_functions.py
--rw-r--r--   0        0        0   109110 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/fault/_grid_connection_set.py
--rw-r--r--   0        0        0      692 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/__init__.py
--rw-r--r--   0        0        0    20689 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_cell_properties.py
--rw-r--r--   0        0        0    10120 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_connection_sets.py
--rw-r--r--   0        0        0    19936 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_create_grid_xml.py
--rw-r--r--   0        0        0    32064 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_defined_geometry.py
--rw-r--r--   0        0        0    28203 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_extract_functions.py
--rw-r--r--   0        0        0    16516 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_face_functions.py
--rw-r--r--   0        0        0    12236 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_faults.py
--rw-r--r--   0        0        0   127766 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_grid.py
--rw-r--r--   0        0        0     3544 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_grid_types.py
--rw-r--r--   0        0        0      338 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_intervals_info.py
--rw-r--r--   0        0        0      604 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_moved_functions.py
--rw-r--r--   0        0        0     7243 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_pillars.py
--rw-r--r--   0        0        0     5386 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_pixel_maps.py
--rw-r--r--   0        0        0    65440 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_points_functions.py
--rw-r--r--   0        0        0    45761 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_regular_grid.py
--rw-r--r--   0        0        0    19413 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_transmissibility.py
--rw-r--r--   0        0        0     7944 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_write_hdf5_from_caches.py
--rw-r--r--   0        0        0     6147 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_write_nexus_corp.py
--rw-r--r--   0        0        0    13087 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid/_xyz.py
--rw-r--r--   0        0        0     2593 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid_surface/__init__.py
--rw-r--r--   0        0        0    35739 2023-07-05 08:19:11.181633 resqpy-4.9.1/resqpy/grid_surface/_blocked_well_populate.py
--rw-r--r--   0        0        0    64016 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/grid_surface/_find_faces.py
--rw-r--r--   0        0        0    26056 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/grid_surface/_grid_skin.py
--rw-r--r--   0        0        0    14379 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/grid_surface/_grid_surface.py
--rw-r--r--   0        0        0    22498 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/grid_surface/_trajectory_intersects.py
--rw-r--r--   0        0        0    39760 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/grid_surface/grid_surface_cuda.py
--rw-r--r--   0        0        0      539 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/lines/__init__.py
--rw-r--r--   0        0        0    11960 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/lines/_common.py
--rw-r--r--   0        0        0    42464 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/lines/_polyline.py
--rw-r--r--   0        0        0    27721 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/lines/_polyline_set.py
--rw-r--r--   0        0        0      378 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/model/__init__.py
--rw-r--r--   0        0        0    30205 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/model/_catalogue.py
--rw-r--r--   0        0        0     2840 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/model/_context.py
--rw-r--r--   0        0        0    34552 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/model/_forestry.py
--rw-r--r--   0        0        0     3371 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/model/_grids.py
--rw-r--r--   0        0        0    14238 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/model/_hdf5.py
--rw-r--r--   0        0        0   103055 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/model/_model.py
--rw-r--r--   0        0        0    23589 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/model/_xml.py
--rw-r--r--   0        0        0      909 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/multi_processing/__init__.py
--rw-r--r--   0        0        0     7301 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/multi_processing/_multiprocessing.py
--rw-r--r--   0        0        0       72 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/multi_processing/wrappers/__init__.py
--rw-r--r--   0        0        0     5952 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/multi_processing/wrappers/blocked_well_mp.py
--rw-r--r--   0        0        0    21156 2023-07-05 08:19:11.185633 resqpy-4.9.1/resqpy/multi_processing/wrappers/grid_surface_mp.py
--rw-r--r--   0        0        0     5793 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/multi_processing/wrappers/mesh_mp.py
--rw-r--r--   0        0        0       84 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/__init__.py
--rw-r--r--   0        0        0     2147 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/ab_toolbox.py
--rw-r--r--   0        0        0     7521 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/base.py
--rw-r--r--   0        0        0    20925 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/box_utilities.py
--rw-r--r--   0        0        0     5935 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/class_dict.py
--rw-r--r--   0        0        0     9489 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/consolidation.py
--rw-r--r--   0        0        0     5177 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/data/build.py
--rw-r--r--   0        0        0   498136 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/data/properties.json
--rw-r--r--   0        0        0    19836 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/dataframe.py
--rw-r--r--   0        0        0      307 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/exceptions.py
--rw-r--r--   0        0        0     1313 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/factors.py
--rw-r--r--   0        0        0    24541 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/fine_coarse.py
--rw-r--r--   0        0        0    27669 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/grid_functions.py
--rw-r--r--   0        0        0    20158 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/intersection.py
--rw-r--r--   0        0        0     8408 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/keyword_files.py
--rw-r--r--   0        0        0    19210 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/load_data.py
--rw-r--r--   0        0        0     6628 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/point_inclusion.py
--rw-r--r--   0        0        0     1103 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/random_seed.py
--rw-r--r--   0        0        0     5441 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/read_nexus_fault.py
--rw-r--r--   0        0        0    17083 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/relperm.py
--rw-r--r--   0        0        0    12189 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/simple_lines.py
--rw-r--r--   0        0        0      760 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/time.py
--rw-r--r--   0        0        0      822 2023-07-05 08:19:11.189633 resqpy-4.9.1/resqpy/olio/trademark.py
--rw-r--r--   0        0        0    61869 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/transmission.py
--rw-r--r--   0        0        0    44768 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/triangulation.py
--rw-r--r--   0        0        0     7324 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/uuid.py
--rw-r--r--   0        0        0    45231 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/vdb.py
--rw-r--r--   0        0        0    46253 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/vector_utilities.py
--rw-r--r--   0        0        0     6185 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/volume.py
--rw-r--r--   0        0        0    26220 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/wellspec_keywords.py
--rw-r--r--   0        0        0     5142 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/write_data.py
--rw-r--r--   0        0        0    19055 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/write_hdf5.py
--rw-r--r--   0        0        0    24925 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/xml_et.py
--rw-r--r--   0        0        0     1824 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/xml_namespaces.py
--rw-r--r--   0        0        0     5709 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/olio/zmap_reader.py
--rw-r--r--   0        0        0     2206 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/__init__.py
--rw-r--r--   0        0        0     2937 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/_utils.py
--rw-r--r--   0        0        0     1685 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/boundary_feature.py
--rw-r--r--   0        0        0     5190 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/boundary_feature_interpretation.py
--rw-r--r--   0        0        0     6186 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/earth_model_interpretation.py
--rw-r--r--   0        0        0    12457 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/fault_interpretation.py
--rw-r--r--   0        0        0     2757 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/fluid_boundary_feature.py
--rw-r--r--   0        0        0     1702 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/frontier_feature.py
--rw-r--r--   0        0        0     4498 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/generic_interpretation.py
--rw-r--r--   0        0        0     3771 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/genetic_boundary_feature.py
--rw-r--r--   0        0        0     8605 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/geobody_boundary_interpretation.py
--rw-r--r--   0        0        0     1836 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/geobody_feature.py
--rw-r--r--   0        0        0     8052 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/geobody_interpretation.py
--rw-r--r--   0        0        0     1739 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/geologic_unit_feature.py
--rw-r--r--   0        0        0     8346 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/horizon_interpretation.py
--rw-r--r--   0        0        0     2697 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/organization_feature.py
--rw-r--r--   0        0        0     5565 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/rock_fluid_unit_feature.py
--rw-r--r--   0        0        0     1802 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/structural_organization_interpretation.py
--rw-r--r--   0        0        0     2675 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/tectonic_boundary_feature.py
--rw-r--r--   0        0        0     1843 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/wellbore_feature.py
--rw-r--r--   0        0        0     6973 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/organize/wellbore_interpretation.py
--rw-r--r--   0        0        0     2155 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/property/__init__.py
--rw-r--r--   0        0        0    16961 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/property/_collection_add_part.py
--rw-r--r--   0        0        0    12926 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/property/_collection_create_xml.py
--rw-r--r--   0        0        0    32165 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/property/_collection_get_attributes.py
--rw-r--r--   0        0        0     5889 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/property/_collection_support.py
--rw-r--r--   0        0        0    24426 2023-07-05 08:19:11.193633 resqpy-4.9.1/resqpy/property/_property.py
--rw-r--r--   0        0        0    66946 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/property/grid_property_collection.py
--rw-r--r--   0        0        0   143771 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/property/property_collection.py
--rw-r--r--   0        0        0    36370 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/property/property_common.py
--rw-r--r--   0        0        0     5557 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/property/property_kind.py
--rw-r--r--   0        0        0     7737 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/property/string_lookup.py
--rw-r--r--   0        0        0     1077 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/property/well_interval_property.py
--rw-r--r--   0        0        0     1610 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/property/well_interval_property_collection.py
--rw-r--r--   0        0        0     1205 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/property/well_log.py
--rw-r--r--   0        0        0     7633 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/property/well_log_collection.py
--rw-r--r--   0        0        0      713 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/rq_import/__init__.py
--rw-r--r--   0        0        0     4493 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/rq_import/_add_ab_properties.py
--rw-r--r--   0        0        0     6067 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/rq_import/_add_surfaces.py
--rw-r--r--   0        0        0    32019 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/rq_import/_grid_from_cp.py
--rw-r--r--   0        0        0    34317 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/rq_import/_import_nexus.py
--rw-r--r--   0        0        0     6306 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/rq_import/_import_vdb_all_grids.py
--rw-r--r--   0        0        0    21372 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/rq_import/_import_vdb_ensemble.py
--rw-r--r--   0        0        0     1311 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/strata/__init__.py
--rw-r--r--   0        0        0     8861 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/strata/_binary_contact_interpretation.py
--rw-r--r--   0        0        0    10381 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/strata/_geologic_unit_interpretation.py
--rw-r--r--   0        0        0     1772 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/strata/_strata_common.py
--rw-r--r--   0        0        0     6797 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/strata/_stratigraphic_column.py
--rw-r--r--   0        0        0    13322 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/strata/_stratigraphic_column_rank.py
--rw-r--r--   0        0        0     7432 2023-07-05 08:19:11.197633 resqpy-4.9.1/resqpy/strata/_stratigraphic_unit_feature.py
--rw-r--r--   0        0        0    10167 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/strata/_stratigraphic_unit_interpretation.py
--rw-r--r--   0        0        0      696 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/surface/__init__.py
--rw-r--r--   0        0        0     2331 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/surface/_base_surface.py
--rw-r--r--   0        0        0     3082 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/surface/_combined_surface.py
--rw-r--r--   0        0        0    42192 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/surface/_mesh.py
--rw-r--r--   0        0        0    27024 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/surface/_pointset.py
--rw-r--r--   0        0        0    58417 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/surface/_surface.py
--rw-r--r--   0        0        0    24315 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/surface/_tri_mesh.py
--rw-r--r--   0        0        0    25907 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/surface/_triangulated_patch.py
--rw-r--r--   0        0        0     1074 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/time_series/__init__.py
--rw-r--r--   0        0        0     8595 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/time_series/_any_time_series.py
--rw-r--r--   0        0        0     6617 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/time_series/_from_nexus_summary.py
--rw-r--r--   0        0        0     6366 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/time_series/_functions.py
--rw-r--r--   0        0        0     3311 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/time_series/_geologic_time_series.py
--rw-r--r--   0        0        0     2759 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/time_series/_time_duration.py
--rw-r--r--   0        0        0    10818 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/time_series/_time_series.py
--rw-r--r--   0        0        0      603 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/unstructured/__init__.py
--rw-r--r--   0        0        0    15328 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/unstructured/_hexa_grid.py
--rw-r--r--   0        0        0    35856 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/unstructured/_prism_grid.py
--rw-r--r--   0        0        0     7862 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/unstructured/_pyramid_grid.py
--rw-r--r--   0        0        0    10208 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/unstructured/_tetra_grid.py
--rw-r--r--   0        0        0    51550 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/unstructured/_unstructured_grid.py
--rw-r--r--   0        0        0     1135 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/weights_and_measures/__init__.py
--rw-r--r--   0        0        0     5434 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/weights_and_measures/nexus_units.py
--rw-r--r--   0        0        0    16186 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/weights_and_measures/weights_and_measures.py
--rw-r--r--   0        0        0      990 2023-07-05 08:19:11.201633 resqpy-4.9.1/resqpy/well/__init__.py
--rw-r--r--   0        0        0   188822 2023-07-05 08:19:11.205633 resqpy-4.9.1/resqpy/well/_blocked_well.py
--rw-r--r--   0        0        0    22138 2023-07-05 08:19:11.205633 resqpy-4.9.1/resqpy/well/_deviation_survey.py
--rw-r--r--   0        0        0     7154 2023-07-05 08:19:11.205633 resqpy-4.9.1/resqpy/well/_md_datum.py
--rw-r--r--   0        0        0    50015 2023-07-05 08:19:11.205633 resqpy-4.9.1/resqpy/well/_trajectory.py
--rw-r--r--   0        0        0    15192 2023-07-05 08:19:11.205633 resqpy-4.9.1/resqpy/well/_wellbore_frame.py
--rw-r--r--   0        0        0     8403 2023-07-05 08:19:11.205633 resqpy-4.9.1/resqpy/well/_wellbore_marker.py
--rw-r--r--   0        0        0    20933 2023-07-05 08:19:11.205633 resqpy-4.9.1/resqpy/well/_wellbore_marker_frame.py
--rw-r--r--   0        0        0    22555 2023-07-05 08:19:11.205633 resqpy-4.9.1/resqpy/well/blocked_well_frame.py
--rw-r--r--   0        0        0    24703 2023-07-05 08:19:11.205633 resqpy-4.9.1/resqpy/well/well_object_funcs.py
--rw-r--r--   0        0        0     5969 2023-07-05 08:19:11.205633 resqpy-4.9.1/resqpy/well/well_utils.py
--rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 resqpy-4.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-10 17:57:21.955560 resqpy-4.9.2/LICENSE
+-rw-r--r--   0        0        0     2893 2023-07-10 17:57:21.955560 resqpy-4.9.2/README.md
+-rw-r--r--   0        0        0     3354 2023-07-10 17:57:40.111832 resqpy-4.9.2/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-07-10 17:57:40.111832 resqpy-4.9.2/resqpy/__init__.py
+-rw-r--r--   0        0        0    24782 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/crs.py
+-rw-r--r--   0        0        0     1982 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/__init__.py
+-rw-r--r--   0        0        0     6410 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_add_edges_per_column_property_array.py
+-rw-r--r--   0        0        0    21022 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_add_faults.py
+-rw-r--r--   0        0        0     6417 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_add_one_blocked_well_property.py
+-rw-r--r--   0        0        0     8657 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_add_one_grid_property_array.py
+-rw-r--r--   0        0        0     2431 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_add_single_cell_grid.py
+-rw-r--r--   0        0        0     5495 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_add_wells_from_ascii_file.py
+-rw-r--r--   0        0        0     6037 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_add_zone_by_layer_property.py
+-rw-r--r--   0        0        0    11586 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_coarsened_grid.py
+-rw-r--r--   0        0        0    10520 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_common.py
+-rw-r--r--   0        0        0     3730 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_copy_grid.py
+-rw-r--r--   0        0        0    11731 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_drape_to_surface.py
+-rw-r--r--   0        0        0    16391 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_extract_box.py
+-rw-r--r--   0        0        0    22969 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_extract_box_for_well.py
+-rw-r--r--   0        0        0    20325 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_fault_throw_scaling.py
+-rw-r--r--   0        0        0     7157 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_gather_ensemble.py
+-rw-r--r--   0        0        0    17929 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_interpolated_grid.py
+-rw-r--r--   0        0        0     9876 2023-07-10 17:57:21.971560 resqpy-4.9.2/resqpy/derived_model/_local_depth_adjustment.py
+-rw-r--r--   0        0        0    20513 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/derived_model/_refined_grid.py
+-rw-r--r--   0        0        0     5166 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/derived_model/_tilted_grid.py
+-rw-r--r--   0        0        0     4792 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/derived_model/_unsplit_grid.py
+-rw-r--r--   0        0        0    18825 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/derived_model/_zonal_grid.py
+-rw-r--r--   0        0        0     4358 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/derived_model/_zone_layer_ranges_from_array.py
+-rw-r--r--   0        0        0      996 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/fault/__init__.py
+-rw-r--r--   0        0        0    29616 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/fault/_gcs_functions.py
+-rw-r--r--   0        0        0   109110 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/fault/_grid_connection_set.py
+-rw-r--r--   0        0        0      692 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/__init__.py
+-rw-r--r--   0        0        0    20689 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_cell_properties.py
+-rw-r--r--   0        0        0    10120 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_connection_sets.py
+-rw-r--r--   0        0        0    19936 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_create_grid_xml.py
+-rw-r--r--   0        0        0    32064 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_defined_geometry.py
+-rw-r--r--   0        0        0    28203 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_extract_functions.py
+-rw-r--r--   0        0        0    16516 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_face_functions.py
+-rw-r--r--   0        0        0    12236 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_faults.py
+-rw-r--r--   0        0        0   129211 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_grid.py
+-rw-r--r--   0        0        0     3544 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_grid_types.py
+-rw-r--r--   0        0        0      338 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_intervals_info.py
+-rw-r--r--   0        0        0      604 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_moved_functions.py
+-rw-r--r--   0        0        0     7243 2023-07-10 17:57:21.975560 resqpy-4.9.2/resqpy/grid/_pillars.py
+-rw-r--r--   0        0        0     5386 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid/_pixel_maps.py
+-rw-r--r--   0        0        0    65440 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid/_points_functions.py
+-rw-r--r--   0        0        0    45761 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid/_regular_grid.py
+-rw-r--r--   0        0        0    22575 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid/_transmissibility.py
+-rw-r--r--   0        0        0     7944 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid/_write_hdf5_from_caches.py
+-rw-r--r--   0        0        0     6147 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid/_write_nexus_corp.py
+-rw-r--r--   0        0        0    13087 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid/_xyz.py
+-rw-r--r--   0        0        0     2593 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid_surface/__init__.py
+-rw-r--r--   0        0        0    35739 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid_surface/_blocked_well_populate.py
+-rw-r--r--   0        0        0    64016 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid_surface/_find_faces.py
+-rw-r--r--   0        0        0    26056 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid_surface/_grid_skin.py
+-rw-r--r--   0        0        0    14379 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid_surface/_grid_surface.py
+-rw-r--r--   0        0        0    22498 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid_surface/_trajectory_intersects.py
+-rw-r--r--   0        0        0    39760 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/grid_surface/grid_surface_cuda.py
+-rw-r--r--   0        0        0      539 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/lines/__init__.py
+-rw-r--r--   0        0        0    11960 2023-07-10 17:57:21.979560 resqpy-4.9.2/resqpy/lines/_common.py
+-rw-r--r--   0        0        0    42464 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/lines/_polyline.py
+-rw-r--r--   0        0        0    27721 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/lines/_polyline_set.py
+-rw-r--r--   0        0        0      378 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/model/__init__.py
+-rw-r--r--   0        0        0    30205 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/model/_catalogue.py
+-rw-r--r--   0        0        0     2840 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/model/_context.py
+-rw-r--r--   0        0        0    34552 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/model/_forestry.py
+-rw-r--r--   0        0        0     3371 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/model/_grids.py
+-rw-r--r--   0        0        0    14238 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/model/_hdf5.py
+-rw-r--r--   0        0        0   103055 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/model/_model.py
+-rw-r--r--   0        0        0    23589 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/model/_xml.py
+-rw-r--r--   0        0        0      909 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/multi_processing/__init__.py
+-rw-r--r--   0        0        0     7301 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/multi_processing/_multiprocessing.py
+-rw-r--r--   0        0        0       72 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/multi_processing/wrappers/__init__.py
+-rw-r--r--   0        0        0     5952 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/multi_processing/wrappers/blocked_well_mp.py
+-rw-r--r--   0        0        0    21156 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/multi_processing/wrappers/grid_surface_mp.py
+-rw-r--r--   0        0        0     5793 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/multi_processing/wrappers/mesh_mp.py
+-rw-r--r--   0        0        0       84 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/olio/__init__.py
+-rw-r--r--   0        0        0     2147 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/olio/ab_toolbox.py
+-rw-r--r--   0        0        0     7521 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/olio/base.py
+-rw-r--r--   0        0        0    20925 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/olio/box_utilities.py
+-rw-r--r--   0        0        0     5935 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/olio/class_dict.py
+-rw-r--r--   0        0        0     9489 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/olio/consolidation.py
+-rw-r--r--   0        0        0     5177 2023-07-10 17:57:21.983560 resqpy-4.9.2/resqpy/olio/data/build.py
+-rw-r--r--   0        0        0   498136 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/data/properties.json
+-rw-r--r--   0        0        0    19836 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/dataframe.py
+-rw-r--r--   0        0        0      307 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/exceptions.py
+-rw-r--r--   0        0        0     1313 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/factors.py
+-rw-r--r--   0        0        0    24541 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/fine_coarse.py
+-rw-r--r--   0        0        0    27669 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/grid_functions.py
+-rw-r--r--   0        0        0    20158 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/intersection.py
+-rw-r--r--   0        0        0     8408 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/keyword_files.py
+-rw-r--r--   0        0        0    19210 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/load_data.py
+-rw-r--r--   0        0        0     6628 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/point_inclusion.py
+-rw-r--r--   0        0        0     1103 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/random_seed.py
+-rw-r--r--   0        0        0     5441 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/read_nexus_fault.py
+-rw-r--r--   0        0        0    17083 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/relperm.py
+-rw-r--r--   0        0        0    12189 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/simple_lines.py
+-rw-r--r--   0        0        0      760 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/time.py
+-rw-r--r--   0        0        0      822 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/trademark.py
+-rw-r--r--   0        0        0    61869 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/transmission.py
+-rw-r--r--   0        0        0    44768 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/triangulation.py
+-rw-r--r--   0        0        0     7324 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/uuid.py
+-rw-r--r--   0        0        0    45231 2023-07-10 17:57:21.987560 resqpy-4.9.2/resqpy/olio/vdb.py
+-rw-r--r--   0        0        0    46253 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/olio/vector_utilities.py
+-rw-r--r--   0        0        0     6185 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/olio/volume.py
+-rw-r--r--   0        0        0    26220 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/olio/wellspec_keywords.py
+-rw-r--r--   0        0        0     5142 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/olio/write_data.py
+-rw-r--r--   0        0        0    19055 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/olio/write_hdf5.py
+-rw-r--r--   0        0        0    24925 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/olio/xml_et.py
+-rw-r--r--   0        0        0     1824 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/olio/xml_namespaces.py
+-rw-r--r--   0        0        0     5709 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/olio/zmap_reader.py
+-rw-r--r--   0        0        0     2206 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/__init__.py
+-rw-r--r--   0        0        0     2937 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/_utils.py
+-rw-r--r--   0        0        0     1685 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/boundary_feature.py
+-rw-r--r--   0        0        0     5190 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/boundary_feature_interpretation.py
+-rw-r--r--   0        0        0     6186 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/earth_model_interpretation.py
+-rw-r--r--   0        0        0    12457 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/fault_interpretation.py
+-rw-r--r--   0        0        0     2757 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/fluid_boundary_feature.py
+-rw-r--r--   0        0        0     1702 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/frontier_feature.py
+-rw-r--r--   0        0        0     4498 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/generic_interpretation.py
+-rw-r--r--   0        0        0     3771 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/genetic_boundary_feature.py
+-rw-r--r--   0        0        0     8605 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/geobody_boundary_interpretation.py
+-rw-r--r--   0        0        0     1836 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/geobody_feature.py
+-rw-r--r--   0        0        0     8052 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/geobody_interpretation.py
+-rw-r--r--   0        0        0     1739 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/geologic_unit_feature.py
+-rw-r--r--   0        0        0     8346 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/horizon_interpretation.py
+-rw-r--r--   0        0        0     2697 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/organization_feature.py
+-rw-r--r--   0        0        0     5565 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/rock_fluid_unit_feature.py
+-rw-r--r--   0        0        0     1802 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/structural_organization_interpretation.py
+-rw-r--r--   0        0        0     2675 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/tectonic_boundary_feature.py
+-rw-r--r--   0        0        0     1843 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/wellbore_feature.py
+-rw-r--r--   0        0        0     6973 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/organize/wellbore_interpretation.py
+-rw-r--r--   0        0        0     2155 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/property/__init__.py
+-rw-r--r--   0        0        0    16961 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/property/_collection_add_part.py
+-rw-r--r--   0        0        0    12926 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/property/_collection_create_xml.py
+-rw-r--r--   0        0        0    32444 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/property/_collection_get_attributes.py
+-rw-r--r--   0        0        0     5889 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/property/_collection_support.py
+-rw-r--r--   0        0        0    24426 2023-07-10 17:57:21.991560 resqpy-4.9.2/resqpy/property/_property.py
+-rw-r--r--   0        0        0    66946 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/property/grid_property_collection.py
+-rw-r--r--   0        0        0   143771 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/property/property_collection.py
+-rw-r--r--   0        0        0    36370 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/property/property_common.py
+-rw-r--r--   0        0        0     5557 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/property/property_kind.py
+-rw-r--r--   0        0        0     7737 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/property/string_lookup.py
+-rw-r--r--   0        0        0     1077 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/property/well_interval_property.py
+-rw-r--r--   0        0        0     1610 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/property/well_interval_property_collection.py
+-rw-r--r--   0        0        0     1205 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/property/well_log.py
+-rw-r--r--   0        0        0     7633 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/property/well_log_collection.py
+-rw-r--r--   0        0        0      713 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/rq_import/__init__.py
+-rw-r--r--   0        0        0     4493 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/rq_import/_add_ab_properties.py
+-rw-r--r--   0        0        0     6067 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/rq_import/_add_surfaces.py
+-rw-r--r--   0        0        0    32019 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/rq_import/_grid_from_cp.py
+-rw-r--r--   0        0        0    34317 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/rq_import/_import_nexus.py
+-rw-r--r--   0        0        0     6306 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/rq_import/_import_vdb_all_grids.py
+-rw-r--r--   0        0        0    21372 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/rq_import/_import_vdb_ensemble.py
+-rw-r--r--   0        0        0     1311 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/strata/__init__.py
+-rw-r--r--   0        0        0     8861 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/strata/_binary_contact_interpretation.py
+-rw-r--r--   0        0        0    10381 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/strata/_geologic_unit_interpretation.py
+-rw-r--r--   0        0        0     1772 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/strata/_strata_common.py
+-rw-r--r--   0        0        0     6797 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/strata/_stratigraphic_column.py
+-rw-r--r--   0        0        0    13322 2023-07-10 17:57:21.995560 resqpy-4.9.2/resqpy/strata/_stratigraphic_column_rank.py
+-rw-r--r--   0        0        0     7432 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/strata/_stratigraphic_unit_feature.py
+-rw-r--r--   0        0        0    10167 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/strata/_stratigraphic_unit_interpretation.py
+-rw-r--r--   0        0        0      696 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/surface/__init__.py
+-rw-r--r--   0        0        0     2331 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/surface/_base_surface.py
+-rw-r--r--   0        0        0     3082 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/surface/_combined_surface.py
+-rw-r--r--   0        0        0    42192 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/surface/_mesh.py
+-rw-r--r--   0        0        0    27024 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/surface/_pointset.py
+-rw-r--r--   0        0        0    58417 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/surface/_surface.py
+-rw-r--r--   0        0        0    24315 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/surface/_tri_mesh.py
+-rw-r--r--   0        0        0    25907 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/surface/_triangulated_patch.py
+-rw-r--r--   0        0        0     1074 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/time_series/__init__.py
+-rw-r--r--   0        0        0     8595 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/time_series/_any_time_series.py
+-rw-r--r--   0        0        0     6617 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/time_series/_from_nexus_summary.py
+-rw-r--r--   0        0        0     6366 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/time_series/_functions.py
+-rw-r--r--   0        0        0     3311 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/time_series/_geologic_time_series.py
+-rw-r--r--   0        0        0     2759 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/time_series/_time_duration.py
+-rw-r--r--   0        0        0    10818 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/time_series/_time_series.py
+-rw-r--r--   0        0        0      603 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/unstructured/__init__.py
+-rw-r--r--   0        0        0    15328 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/unstructured/_hexa_grid.py
+-rw-r--r--   0        0        0    35856 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/unstructured/_prism_grid.py
+-rw-r--r--   0        0        0     7862 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/unstructured/_pyramid_grid.py
+-rw-r--r--   0        0        0    10208 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/unstructured/_tetra_grid.py
+-rw-r--r--   0        0        0    51550 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/unstructured/_unstructured_grid.py
+-rw-r--r--   0        0        0     1135 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/weights_and_measures/__init__.py
+-rw-r--r--   0        0        0     5434 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/weights_and_measures/nexus_units.py
+-rw-r--r--   0        0        0    16186 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/weights_and_measures/weights_and_measures.py
+-rw-r--r--   0        0        0      990 2023-07-10 17:57:21.999560 resqpy-4.9.2/resqpy/well/__init__.py
+-rw-r--r--   0        0        0   188822 2023-07-10 17:57:22.003560 resqpy-4.9.2/resqpy/well/_blocked_well.py
+-rw-r--r--   0        0        0    22138 2023-07-10 17:57:22.003560 resqpy-4.9.2/resqpy/well/_deviation_survey.py
+-rw-r--r--   0        0        0     7154 2023-07-10 17:57:22.003560 resqpy-4.9.2/resqpy/well/_md_datum.py
+-rw-r--r--   0        0        0    50015 2023-07-10 17:57:22.003560 resqpy-4.9.2/resqpy/well/_trajectory.py
+-rw-r--r--   0        0        0    15192 2023-07-10 17:57:22.003560 resqpy-4.9.2/resqpy/well/_wellbore_frame.py
+-rw-r--r--   0        0        0     8403 2023-07-10 17:57:22.003560 resqpy-4.9.2/resqpy/well/_wellbore_marker.py
+-rw-r--r--   0        0        0    20933 2023-07-10 17:57:22.003560 resqpy-4.9.2/resqpy/well/_wellbore_marker_frame.py
+-rw-r--r--   0        0        0    22555 2023-07-10 17:57:22.003560 resqpy-4.9.2/resqpy/well/blocked_well_frame.py
+-rw-r--r--   0        0        0    24703 2023-07-10 17:57:22.003560 resqpy-4.9.2/resqpy/well/well_object_funcs.py
+-rw-r--r--   0        0        0     5969 2023-07-10 17:57:22.003560 resqpy-4.9.2/resqpy/well/well_utils.py
+-rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 resqpy-4.9.2/PKG-INFO
```

### Comparing `resqpy-4.9.1/LICENSE` & `resqpy-4.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/README.md` & `resqpy-4.9.2/README.md`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/pyproject.toml` & `resqpy-4.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["poetry>=1.0.2", "poetry-dynamic-versioning"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "resqpy"
-version = "4.9.1" # Set at build time
+version = "4.9.2" # Set at build time
 description = "Python API for working with RESQML models"
 authors = ["BP"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bp/resqpy"
 documentation = "https://resqpy.readthedocs.io/en/latest/"
 keywords = ["RESQML"]
```

### Comparing `resqpy-4.9.1/resqpy/__init__.py` & `resqpy-4.9.2/resqpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,10 +24,10 @@
     weights_and_measures
     well
     olio
 """
 
 import logging
 
-__version__ = "4.9.1"  # Set at build time
+__version__ = "4.9.2"  # Set at build time
 log = logging.getLogger(__name__)
 log.info(f"Imported resqpy version {__version__}")
```

### Comparing `resqpy-4.9.1/resqpy/crs.py` & `resqpy-4.9.2/resqpy/crs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/__init__.py` & `resqpy-4.9.2/resqpy/derived_model/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_add_edges_per_column_property_array.py` & `resqpy-4.9.2/resqpy/derived_model/_add_edges_per_column_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_add_faults.py` & `resqpy-4.9.2/resqpy/derived_model/_add_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_add_one_blocked_well_property.py` & `resqpy-4.9.2/resqpy/derived_model/_add_one_blocked_well_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_add_one_grid_property_array.py` & `resqpy-4.9.2/resqpy/derived_model/_add_one_grid_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_add_single_cell_grid.py` & `resqpy-4.9.2/resqpy/derived_model/_add_single_cell_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_add_wells_from_ascii_file.py` & `resqpy-4.9.2/resqpy/derived_model/_add_wells_from_ascii_file.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_add_zone_by_layer_property.py` & `resqpy-4.9.2/resqpy/derived_model/_add_zone_by_layer_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_coarsened_grid.py` & `resqpy-4.9.2/resqpy/derived_model/_coarsened_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_common.py` & `resqpy-4.9.2/resqpy/derived_model/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_copy_grid.py` & `resqpy-4.9.2/resqpy/derived_model/_copy_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_drape_to_surface.py` & `resqpy-4.9.2/resqpy/derived_model/_drape_to_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_extract_box.py` & `resqpy-4.9.2/resqpy/derived_model/_extract_box.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_extract_box_for_well.py` & `resqpy-4.9.2/resqpy/derived_model/_extract_box_for_well.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_fault_throw_scaling.py` & `resqpy-4.9.2/resqpy/derived_model/_fault_throw_scaling.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_gather_ensemble.py` & `resqpy-4.9.2/resqpy/derived_model/_gather_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_interpolated_grid.py` & `resqpy-4.9.2/resqpy/derived_model/_interpolated_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_local_depth_adjustment.py` & `resqpy-4.9.2/resqpy/derived_model/_local_depth_adjustment.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_refined_grid.py` & `resqpy-4.9.2/resqpy/derived_model/_refined_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_tilted_grid.py` & `resqpy-4.9.2/resqpy/derived_model/_tilted_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_unsplit_grid.py` & `resqpy-4.9.2/resqpy/derived_model/_unsplit_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_zonal_grid.py` & `resqpy-4.9.2/resqpy/derived_model/_zonal_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/derived_model/_zone_layer_ranges_from_array.py` & `resqpy-4.9.2/resqpy/derived_model/_zone_layer_ranges_from_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/fault/__init__.py` & `resqpy-4.9.2/resqpy/fault/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/fault/_gcs_functions.py` & `resqpy-4.9.2/resqpy/fault/_gcs_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,17 @@
 
     returns:
         triple numpy float arrays being transmissibility multipliers for K, J, and I grid faces; arrays have
             shapes (nk + 1, nj, ni), (nk, nj + 1, ni), and (nk, nj, ni + 1) respectively
 
     notes:
         each gcs, which is the supporting representation for each input tr mult property, must be for a single
-        grid and that grid must be the same for all the gcs'es
+        grid and that grid must be the same for all the gcs'es;
+        the three arrays returned by this function can be flattened and concatenated to create a composite
+        array compatible with RESQML documentation for grid properties with indexable elmement of 'faces'
     """
 
     assert merge_mode in ['minimum', 'multiply', 'maximum', 'exception']
     assert gcs_tr_mult_uuid_list is not None and len(gcs_tr_mult_uuid_list) > 0
     if sided is None:
         sided = (merge_mode != 'multiply')
     elif sided and merge_mode == 'multiply':
```

### Comparing `resqpy-4.9.1/resqpy/fault/_grid_connection_set.py` & `resqpy-4.9.2/resqpy/fault/_grid_connection_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/__init__.py` & `resqpy-4.9.2/resqpy/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_cell_properties.py` & `resqpy-4.9.2/resqpy/grid/_cell_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_connection_sets.py` & `resqpy-4.9.2/resqpy/grid/_connection_sets.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_create_grid_xml.py` & `resqpy-4.9.2/resqpy/grid/_create_grid_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_defined_geometry.py` & `resqpy-4.9.2/resqpy/grid/_defined_geometry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_extract_functions.py` & `resqpy-4.9.2/resqpy/grid/_extract_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_face_functions.py` & `resqpy-4.9.2/resqpy/grid/_face_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_faults.py` & `resqpy-4.9.2/resqpy/grid/_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_grid.py` & `resqpy-4.9.2/resqpy/grid/_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -2145,15 +2145,16 @@
                                                    gcs_uuid_list = None,
                                                    realization = None,
                                                    merge_mode = 'minimum',
                                                    sided = None,
                                                    fill_value = 1.0,
                                                    active_only = True,
                                                    apply_baffles = False,
-                                                   baffle_triplet = None):
+                                                   baffle_triplet = None,
+                                                   composite_property = False):
         """Add triplet of transmissibility multiplier properties by combining gcs properties.
 
         arguments:
             gcs_uuid_list (list of UUID, optional): if None, all grid connection sets related to this grid will
                 be used
             realization (int, optional): if present, is used to filter tranmissibility multiplier input
                 properties and is added to the output properties
@@ -2167,25 +2168,30 @@
                 then only active faces are used when combining to make the grid face properties
             apply_baffles (bool, default False): if True, where a baffle property exists for a grid connection
                 set, a transmissibility multiplier of zero will be used for faces marked as True, overriding the
                 multiplier property values at such faces
             baffle_triplet (triplet of numpy bool arrays, optional): if present, boolean masks over the grid
                 internal faces; where True, a value of zero will be enforced for the multipliers regardless
                 of the grid connection set properties
+            composite_property (bool, default False): if True, the transmissibility data is stored in a single
+                property with no direction facet (in accordance with the RESQML standard); if False, a separate
+                property is generated for each of the three directions
 
         returns:
-            list of 3 uuids, one for each of the newly created transmissibility multiplier properties
+            list of 3 uuids, one for each of the newly created transmissibility multiplier properties; or
+            a list with just one uuid, if composite_property is True
 
         notes:
             each grid connection set must refer to this grid only;
             the generated properties have indexable element 'faces', not 'faces per cell', so may not be
             suitable for faulted grids;
             the baffle_triplet arrays, if provided, must be for internal faces only, so have extents of
             (nk - 1, nj, ni), (nk, nj - 1, ni), (nk, nj, ni -1); note that this is a different protocol
-            than the indexable element of faces, which includes external faces
+            than the indexable element of faces, which includes external faces;
+            set composite_property True for compatibility with shape information indicated in RESQML documentation
         """
 
         if not gcs_uuid_list:
             gcs_uuid_list = self.model.uuids(obj_type = 'GridConnectionSetRepresentation', related_uuid = self.uuid)
         assert gcs_uuid_list, 'no grid connections sets identified for transmissibility multiplier combining'
 
         if baffle_triplet is not None:
@@ -2220,26 +2226,39 @@
         pc = self.extract_property_collection()
 
         if baffle_triplet is not None:
             trm_k[1:-1] = np.where(baffle_triplet[0], 0.0, trm_k[1:-1])
             trm_j[:, 1:-1] = np.where(baffle_triplet[1], 0.0, trm_j[:, 1:-1])
             trm_i[:, :, 1:-1] = np.where(baffle_triplet[2], 0.0, trm_i[:, :, 1:-1])
 
-        for axis, trm in enumerate((trm_k, trm_j, trm_i)):
-            axis_ch = 'KJI'[axis]
-            pc.add_cached_array_to_imported_list(trm,
+        if composite_property:
+            tr_composite = np.concatenate((trm_k.flat, trm_j.flat, trm_i.flat))
+            pc.add_cached_array_to_imported_list(tr_composite,
                                                  'combined from gcs tr mults',
-                                                 'TMULT' + axis_ch,
+                                                 'TMULT',
                                                  discrete = False,
                                                  uom = 'Euc',
                                                  property_kind = 'transmissibility multiplier',
-                                                 facet_type = 'direction',
-                                                 facet = axis_ch,
+                                                 facet_type = None,
+                                                 facet = None,
                                                  realization = realization,
                                                  indexable_element = 'faces')
+        else:
+            for axis, trm in enumerate((trm_k, trm_j, trm_i)):
+                axis_ch = 'KJI'[axis]
+                pc.add_cached_array_to_imported_list(trm,
+                                                     'combined from gcs tr mults',
+                                                     'TMULT' + axis_ch,
+                                                     discrete = False,
+                                                     uom = 'Euc',
+                                                     property_kind = 'transmissibility multiplier',
+                                                     facet_type = 'direction',
+                                                     facet = axis_ch,
+                                                     realization = realization,
+                                                     indexable_element = 'faces')
 
         pc.write_hdf5_for_imported_list()
         return pc.create_xml_for_imported_list_and_add_parts_to_model()
 
     def _add_geom_points_xml(self, geom_node, ext_uuid):
         """Generate geometry points node in xml, called during create_xml, overridden for RegularGrid."""
         return _add_pillar_points_xml(self, geom_node, ext_uuid)
```

### Comparing `resqpy-4.9.1/resqpy/grid/_grid_types.py` & `resqpy-4.9.2/resqpy/grid/_grid_types.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_moved_functions.py` & `resqpy-4.9.2/resqpy/grid/_moved_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_pillars.py` & `resqpy-4.9.2/resqpy/grid/_pillars.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_pixel_maps.py` & `resqpy-4.9.2/resqpy/grid/_pixel_maps.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_points_functions.py` & `resqpy-4.9.2/resqpy/grid/_points_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_regular_grid.py` & `resqpy-4.9.2/resqpy/grid/_regular_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_transmissibility.py` & `resqpy-4.9.2/resqpy/grid/_transmissibility.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,21 +25,21 @@
           possible transmissibility arrays and if found, they are used instead of calculation; note that
           when this argument is False, the property collection is still used for the feed arrays to the
           calculation
        realization (int, optional) if present, only properties with this realization number will be used;
           applies to pre-computed transmissibility properties or permeability and net to gross ratio
           properties when computing
        modifier_mode (string, optional): if None, no transmissibility modifiers are applied; other
-          options are: 'faces multiplier', for which directional transmissibility properties with indexable
-          element of 'faces' will be used; 'faces per cell multiplier', in which case a transmissibility
-          property with 'faces per cell' as the indexable element will be used to modify the half cell
-          transmissibilities prior to combination; or 'absolute' in which case directional properties
-          of local property kind 'fault transmissibility' (or 'mat transmissibility') and indexable
-          element of 'faces' will be used as a third transmissibility term along with the two half
-          cell transmissibilities at each face; see also the notes below
+          options are: 'faces multiplier', for which transmissibility properties with indexable
+          element of 'faces' will be used (directional or composite); 'faces per cell multiplier',
+          in which case a transmissibility property with 'faces per cell' as the indexable element
+          will be used to modify the half cell transmissibilities prior to combination;
+          or 'absolute' in which case directional properties of local property kind 'fault transmissibility'
+          (or 'mat transmissibility') and indexable element of 'faces' will be used as a third transmissibility
+          term along with the two half cell transmissibilities at each face; see also the notes below
 
     returns:
        3 numpy float arrays of shape (nk + 1, nj, ni), (nk, nj + 1, ni), (nk, nj, ni + 1) being the
        neighbourly transmissibilities in K, J & I axes respectively
 
     notes:
        the 3 permeability arrays (and net to gross ratio if in use) must be identifiable in the property
@@ -48,18 +48,18 @@
        bbl.cP/(psi.d) if length units are feet; the computation is compatible with the Nexus NEWTRAN formulation;
        values will be zero at pinchouts, and at column edges where there is a split pillar, even if there is
        juxtapostion of faces; the same is true of K gap faces (even where the gap is zero); NaNs in any of
        the feed properties also result in transmissibility values of zero;
        outer facing values will always be zero (included to be in accordance with RESQML faces properties);
        array caching in the grid object will only be used if realization is None; if a modifier mode of
        'faces multiplier' or 'faces per cell multiplier' is specified, properties will be searched for with
-       local property kind 'transmissibility multiplier' and the appropriate indexable element (and direction
-       facet in the case of 'faces multiplier'); the modifier mode of 'absolute' can be used to model the
-       effect of faults and thin shales, tar mats etc. in a way which is independent of cell size;
-       for 'aboslute' directional properties with indexable element of 'faces' and local property kind
+       local property kind 'transmissibility multiplier' and the appropriate indexable element (and optionally
+       the direction facet in the case of 'faces multiplier'); the modifier mode of 'absolute' can be used to
+       model the effect of faults and thin shales, tar mats etc. in a way which is independent of cell size;
+       for 'aboslute' properties with indexable element of 'faces' (optionally directional) and local property kind
        'fault transmissibility' (or 'mat transmissibility') will be used; such absolute faces transmissibilities
        should have a value of np.inf or np.nan where no modification is required; note that this method is only
        dealing with logically neighbouring cells and will not compute values for faces with a split pillar,
        which should be handled elsewhere
     """
 
     # todo: improve handling of units: check uom for half cell transmissibility property and for absolute modifiers
@@ -74,48 +74,63 @@
         if hasattr(grid, 'array_i_transmissibility') and grid.array_i_transmissibility is not None:
             i_tr = grid.array_i_transmissibility
 
     if use_tr_properties and (k_tr is None or j_tr is None or i_tr is None):
 
         pc = grid.extract_property_collection()
 
+        composite_tr = pc.single_array_ref(property_kind = 'transmissibility',
+                                           realization = realization,
+                                           continuous = True,
+                                           indexable = 'faces',
+                                           facet_type = 'none',
+                                           facet = 'none')
         if k_tr is None:
             k_tr = pc.single_array_ref(property_kind = 'transmissibility',
                                        realization = realization,
                                        continuous = True,
                                        count = 1,
                                        indexable = 'faces',
                                        facet_type = 'direction',
                                        facet = 'K')
+            if k_tr is None and composite_tr is not None:
+                k_tr = composite_tr[:(grid.nk + 1) * grid.nj * grid.ni].reshape((grid.nk + 1, grid.nj, grid.ni))
             if k_tr is not None:
                 assert k_tr.shape == (grid.nk + 1, grid.nj, grid.ni)
                 if realization is None:
                     grid.array_k_transmissibility = k_tr
 
         if j_tr is None:
             j_tr = pc.single_array_ref(property_kind = 'transmissibility',
                                        realization = realization,
                                        continuous = True,
                                        count = 1,
                                        indexable = 'faces',
                                        facet_type = 'direction',
                                        facet = 'J')
+            if j_tr is None and composite_tr is not None:
+                offset = (grid.nk + 1) * grid.nj * grid.ni
+                j_tr = composite_tr[offset:offset + grid.nk * (grid.nj + 1) * grid.ni].reshape(
+                    (grid.nk, grid.nj + 1, grid.ni))
             if j_tr is not None:
                 assert j_tr.shape == (grid.nk, grid.nj + 1, grid.ni)
                 if realization is None:
                     grid.array_j_transmissibility = j_tr
 
         if i_tr is None:
             i_tr = pc.single_array_ref(property_kind = 'transmissibility',
                                        realization = realization,
                                        continuous = True,
                                        count = 1,
                                        indexable = 'faces',
                                        facet_type = 'direction',
                                        facet = 'I')
+            if i_tr is None and composite_tr is not None:
+                offset = (grid.nk + 1) * grid.nj * grid.ni + grid.nk * (grid.nj + 1) * grid.ni
+                i_tr = composite_tr[offset:].reshape((grid.nk, grid.nj, grid.ni + 1))
             if i_tr is not None:
                 assert i_tr.shape == (grid.nk, grid.nj, grid.ni + 1)
                 if realization is None:
                     grid.array_i_transmissibility = i_tr
 
     if k_tr is None or j_tr is None or i_tr is None:
 
@@ -176,14 +191,24 @@
                                       realization = realization,
                                       facet_type = 'direction',
                                       facet = 'I',
                                       continuous = True,
                                       count = 1,
                                       indexable = 'faces')
         if tr_mult is None:
+            tr_composite = pc.single_array_ref(property_kind = 'transmissibility multiplier',
+                                               realization = realization,
+                                               facet_type = 'none',
+                                               facet = 'none',
+                                               continuous = True,
+                                               indexable = 'faces')
+            if tr_composite is not None:
+                offset = (grid.nk + 1) * grid.nj * grid.ni + grid.nk * (grid.nj + 1) * grid.ni
+                tr_mult = tr_composite[offset:].reshape((grid.nk, grid.nj, grid.ni + 1))
+        if tr_mult is None:
             log.warning('no I direction faces transmissibility multiplier found when calculating transmissibilities')
         else:
             assert tr_mult.shape == (grid.nk, grid.nj, grid.ni + 1)
             internal_zero_mask = np.logical_or(internal_zero_mask, np.isnan(tr_mult[:, :, 1:-1]))
     if tr_mult is None:
         tr_mult = 1.0
     tr_abs_r = 0.0
@@ -218,14 +243,25 @@
                                       realization = realization,
                                       facet_type = 'direction',
                                       facet = 'J',
                                       continuous = True,
                                       count = 1,
                                       indexable = 'faces')
         if tr_mult is None:
+            tr_composite = pc.single_array_ref(property_kind = 'transmissibility multiplier',
+                                               realization = realization,
+                                               facet_type = 'none',
+                                               facet = 'none',
+                                               continuous = True,
+                                               indexable = 'faces')
+            if tr_composite is not None:
+                offset = (grid.nk + 1) * grid.nj * grid.ni
+                tr_mult = tr_composite[offset:offset + grid.nk * (grid.nj + 1) * grid.ni].reshape(
+                    (grid.nk, grid.nj + 1, grid.ni))
+        if tr_mult is None:
             log.warning('no J direction faces transmissibility multiplier found when calculating transmissibilities')
         else:
             assert tr_mult.shape == (grid.nk, grid.nj + 1, grid.ni)
             internal_zero_mask = np.logical_or(internal_zero_mask, np.isnan(tr_mult[:, 1:-1, :]))
     if tr_mult is None:
         tr_mult = 1.0
     tr_abs_r = 0.0
@@ -261,14 +297,24 @@
         tr_mult = pc.single_array_ref(property_kind = 'transmissibility multiplier',
                                       realization = realization,
                                       facet_type = 'direction',
                                       facet = 'K',
                                       continuous = True,
                                       count = 1,
                                       indexable = 'faces')
+        if tr_mult is None:
+            tr_composite = pc.single_array_ref(property_kind = 'transmissibility multiplier',
+                                               realization = realization,
+                                               facet_type = 'none',
+                                               facet = 'none',
+                                               continuous = True,
+                                               indexable = 'faces')
+            if tr_composite is not None:
+                size = (grid.nk + 1) * grid.nj * grid.ni
+                tr_mult = tr_composite[:size].reshape((grid.nk + 1, grid.nj, grid.ni))
         if tr_mult is not None:
             assert tr_mult.shape == (grid.nk + 1, grid.nj, grid.ni)
             internal_zero_mask = np.logical_or(internal_zero_mask, np.isnan(tr_mult[1:-1, :, :]))
     if tr_mult is None:
         tr_mult = 1.0
     tr_abs_r = 0.0
     if modifier_mode == 'absolute':
```

### Comparing `resqpy-4.9.1/resqpy/grid/_write_hdf5_from_caches.py` & `resqpy-4.9.2/resqpy/grid/_write_hdf5_from_caches.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_write_nexus_corp.py` & `resqpy-4.9.2/resqpy/grid/_write_nexus_corp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid/_xyz.py` & `resqpy-4.9.2/resqpy/grid/_xyz.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid_surface/__init__.py` & `resqpy-4.9.2/resqpy/grid_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid_surface/_blocked_well_populate.py` & `resqpy-4.9.2/resqpy/grid_surface/_blocked_well_populate.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid_surface/_find_faces.py` & `resqpy-4.9.2/resqpy/grid_surface/_find_faces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid_surface/_grid_skin.py` & `resqpy-4.9.2/resqpy/grid_surface/_grid_skin.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid_surface/_grid_surface.py` & `resqpy-4.9.2/resqpy/grid_surface/_grid_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid_surface/_trajectory_intersects.py` & `resqpy-4.9.2/resqpy/grid_surface/_trajectory_intersects.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/grid_surface/grid_surface_cuda.py` & `resqpy-4.9.2/resqpy/grid_surface/grid_surface_cuda.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/lines/__init__.py` & `resqpy-4.9.2/resqpy/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/lines/_common.py` & `resqpy-4.9.2/resqpy/lines/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/lines/_polyline.py` & `resqpy-4.9.2/resqpy/lines/_polyline.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/lines/_polyline_set.py` & `resqpy-4.9.2/resqpy/lines/_polyline_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/model/_catalogue.py` & `resqpy-4.9.2/resqpy/model/_catalogue.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/model/_context.py` & `resqpy-4.9.2/resqpy/model/_context.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/model/_forestry.py` & `resqpy-4.9.2/resqpy/model/_forestry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/model/_grids.py` & `resqpy-4.9.2/resqpy/model/_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/model/_hdf5.py` & `resqpy-4.9.2/resqpy/model/_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/model/_model.py` & `resqpy-4.9.2/resqpy/model/_model.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/model/_xml.py` & `resqpy-4.9.2/resqpy/model/_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/multi_processing/__init__.py` & `resqpy-4.9.2/resqpy/multi_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/multi_processing/_multiprocessing.py` & `resqpy-4.9.2/resqpy/multi_processing/_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/multi_processing/wrappers/blocked_well_mp.py` & `resqpy-4.9.2/resqpy/multi_processing/wrappers/blocked_well_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/multi_processing/wrappers/grid_surface_mp.py` & `resqpy-4.9.2/resqpy/multi_processing/wrappers/grid_surface_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/multi_processing/wrappers/mesh_mp.py` & `resqpy-4.9.2/resqpy/multi_processing/wrappers/mesh_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/ab_toolbox.py` & `resqpy-4.9.2/resqpy/olio/ab_toolbox.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/base.py` & `resqpy-4.9.2/resqpy/olio/base.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/box_utilities.py` & `resqpy-4.9.2/resqpy/olio/box_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/class_dict.py` & `resqpy-4.9.2/resqpy/olio/class_dict.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/consolidation.py` & `resqpy-4.9.2/resqpy/olio/consolidation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/data/build.py` & `resqpy-4.9.2/resqpy/olio/data/build.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/data/properties.json` & `resqpy-4.9.2/resqpy/olio/data/properties.json`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/dataframe.py` & `resqpy-4.9.2/resqpy/olio/dataframe.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/factors.py` & `resqpy-4.9.2/resqpy/olio/factors.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/fine_coarse.py` & `resqpy-4.9.2/resqpy/olio/fine_coarse.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/grid_functions.py` & `resqpy-4.9.2/resqpy/olio/grid_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/intersection.py` & `resqpy-4.9.2/resqpy/olio/intersection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/keyword_files.py` & `resqpy-4.9.2/resqpy/olio/keyword_files.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/load_data.py` & `resqpy-4.9.2/resqpy/olio/load_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/point_inclusion.py` & `resqpy-4.9.2/resqpy/olio/point_inclusion.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/random_seed.py` & `resqpy-4.9.2/resqpy/olio/random_seed.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/read_nexus_fault.py` & `resqpy-4.9.2/resqpy/olio/read_nexus_fault.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/relperm.py` & `resqpy-4.9.2/resqpy/olio/relperm.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/simple_lines.py` & `resqpy-4.9.2/resqpy/olio/simple_lines.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/time.py` & `resqpy-4.9.2/resqpy/olio/time.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/trademark.py` & `resqpy-4.9.2/resqpy/olio/trademark.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/transmission.py` & `resqpy-4.9.2/resqpy/olio/transmission.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/triangulation.py` & `resqpy-4.9.2/resqpy/olio/triangulation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/uuid.py` & `resqpy-4.9.2/resqpy/olio/uuid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/vdb.py` & `resqpy-4.9.2/resqpy/olio/vdb.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/vector_utilities.py` & `resqpy-4.9.2/resqpy/olio/vector_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/volume.py` & `resqpy-4.9.2/resqpy/olio/volume.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/wellspec_keywords.py` & `resqpy-4.9.2/resqpy/olio/wellspec_keywords.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/write_data.py` & `resqpy-4.9.2/resqpy/olio/write_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/write_hdf5.py` & `resqpy-4.9.2/resqpy/olio/write_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/xml_et.py` & `resqpy-4.9.2/resqpy/olio/xml_et.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/xml_namespaces.py` & `resqpy-4.9.2/resqpy/olio/xml_namespaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/olio/zmap_reader.py` & `resqpy-4.9.2/resqpy/olio/zmap_reader.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/__init__.py` & `resqpy-4.9.2/resqpy/organize/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/_utils.py` & `resqpy-4.9.2/resqpy/organize/_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/boundary_feature.py` & `resqpy-4.9.2/resqpy/organize/boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/boundary_feature_interpretation.py` & `resqpy-4.9.2/resqpy/organize/boundary_feature_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/earth_model_interpretation.py` & `resqpy-4.9.2/resqpy/organize/earth_model_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/fault_interpretation.py` & `resqpy-4.9.2/resqpy/organize/fault_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/fluid_boundary_feature.py` & `resqpy-4.9.2/resqpy/organize/fluid_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/frontier_feature.py` & `resqpy-4.9.2/resqpy/organize/frontier_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/generic_interpretation.py` & `resqpy-4.9.2/resqpy/organize/generic_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/genetic_boundary_feature.py` & `resqpy-4.9.2/resqpy/organize/genetic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/geobody_boundary_interpretation.py` & `resqpy-4.9.2/resqpy/organize/geobody_boundary_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/geobody_feature.py` & `resqpy-4.9.2/resqpy/organize/geobody_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/geobody_interpretation.py` & `resqpy-4.9.2/resqpy/organize/geobody_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/geologic_unit_feature.py` & `resqpy-4.9.2/resqpy/organize/geologic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/horizon_interpretation.py` & `resqpy-4.9.2/resqpy/organize/horizon_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/organization_feature.py` & `resqpy-4.9.2/resqpy/organize/organization_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/rock_fluid_unit_feature.py` & `resqpy-4.9.2/resqpy/organize/rock_fluid_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/structural_organization_interpretation.py` & `resqpy-4.9.2/resqpy/organize/structural_organization_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/tectonic_boundary_feature.py` & `resqpy-4.9.2/resqpy/organize/tectonic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/wellbore_feature.py` & `resqpy-4.9.2/resqpy/organize/wellbore_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/organize/wellbore_interpretation.py` & `resqpy-4.9.2/resqpy/organize/wellbore_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/__init__.py` & `resqpy-4.9.2/resqpy/property/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/_collection_add_part.py` & `resqpy-4.9.2/resqpy/property/_collection_add_part.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/_collection_create_xml.py` & `resqpy-4.9.2/resqpy/property/_collection_create_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/_collection_get_attributes.py` & `resqpy-4.9.2/resqpy/property/_collection_get_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,18 +435,26 @@
         shape_list = [support.nk, support.nj]
     else:
         raise ValueError(f'unsupported grid indexable element: {indexable_element}')
     return shape_list
 
 
 def _supporting_shape_grid_faces(direction, support):
-    assert direction is not None and direction.upper() in 'IJK'
-    axis = 'KJI'.index(direction.upper())
-    shape_list = [support.nk, support.nj, support.ni]
-    shape_list[axis] += 1  # note: properties for grid faces include outer faces
+    if direction is None:  # a composite 1D array (the RESQML standard)
+        count = 0
+        for axis in range(3):
+            batch = np.array(support.extent_kji, dtype = int)
+            batch[axis] += 1
+            count += np.product(batch)
+        shape_list = [count]
+    else:
+        assert direction.upper() in 'IJK'
+        axis = 'KJI'.index(direction.upper())
+        shape_list = [support.nk, support.nj, support.ni]
+        shape_list[axis] += 1  # note: properties for grid faces include outer faces
     return shape_list
 
 
 def _supporting_shape_grid_nodes(support):
     shape_list = None
     assert not support.k_gaps, 'indexable element of nodes not currently supported for grids with K gaps'
     if support.has_split_coordinate_lines:
```

### Comparing `resqpy-4.9.1/resqpy/property/_collection_support.py` & `resqpy-4.9.2/resqpy/property/_collection_support.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/_property.py` & `resqpy-4.9.2/resqpy/property/_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/grid_property_collection.py` & `resqpy-4.9.2/resqpy/property/grid_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/property_collection.py` & `resqpy-4.9.2/resqpy/property/property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/property_common.py` & `resqpy-4.9.2/resqpy/property/property_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/property_kind.py` & `resqpy-4.9.2/resqpy/property/property_kind.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/string_lookup.py` & `resqpy-4.9.2/resqpy/property/string_lookup.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/well_interval_property.py` & `resqpy-4.9.2/resqpy/property/well_interval_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/well_interval_property_collection.py` & `resqpy-4.9.2/resqpy/property/well_interval_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/well_log.py` & `resqpy-4.9.2/resqpy/property/well_log.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/property/well_log_collection.py` & `resqpy-4.9.2/resqpy/property/well_log_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/rq_import/__init__.py` & `resqpy-4.9.2/resqpy/rq_import/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/rq_import/_add_ab_properties.py` & `resqpy-4.9.2/resqpy/rq_import/_add_ab_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/rq_import/_add_surfaces.py` & `resqpy-4.9.2/resqpy/rq_import/_add_surfaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/rq_import/_grid_from_cp.py` & `resqpy-4.9.2/resqpy/rq_import/_grid_from_cp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/rq_import/_import_nexus.py` & `resqpy-4.9.2/resqpy/rq_import/_import_nexus.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/rq_import/_import_vdb_all_grids.py` & `resqpy-4.9.2/resqpy/rq_import/_import_vdb_all_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/rq_import/_import_vdb_ensemble.py` & `resqpy-4.9.2/resqpy/rq_import/_import_vdb_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/strata/__init__.py` & `resqpy-4.9.2/resqpy/strata/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/strata/_binary_contact_interpretation.py` & `resqpy-4.9.2/resqpy/strata/_binary_contact_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/strata/_geologic_unit_interpretation.py` & `resqpy-4.9.2/resqpy/strata/_geologic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/strata/_strata_common.py` & `resqpy-4.9.2/resqpy/strata/_strata_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/strata/_stratigraphic_column.py` & `resqpy-4.9.2/resqpy/strata/_stratigraphic_column.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/strata/_stratigraphic_column_rank.py` & `resqpy-4.9.2/resqpy/strata/_stratigraphic_column_rank.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/strata/_stratigraphic_unit_feature.py` & `resqpy-4.9.2/resqpy/strata/_stratigraphic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/strata/_stratigraphic_unit_interpretation.py` & `resqpy-4.9.2/resqpy/strata/_stratigraphic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/surface/__init__.py` & `resqpy-4.9.2/resqpy/surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/surface/_base_surface.py` & `resqpy-4.9.2/resqpy/surface/_base_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/surface/_combined_surface.py` & `resqpy-4.9.2/resqpy/surface/_combined_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/surface/_mesh.py` & `resqpy-4.9.2/resqpy/surface/_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/surface/_pointset.py` & `resqpy-4.9.2/resqpy/surface/_pointset.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/surface/_surface.py` & `resqpy-4.9.2/resqpy/surface/_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/surface/_tri_mesh.py` & `resqpy-4.9.2/resqpy/surface/_tri_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/surface/_triangulated_patch.py` & `resqpy-4.9.2/resqpy/surface/_triangulated_patch.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/time_series/__init__.py` & `resqpy-4.9.2/resqpy/time_series/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/time_series/_any_time_series.py` & `resqpy-4.9.2/resqpy/time_series/_any_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/time_series/_from_nexus_summary.py` & `resqpy-4.9.2/resqpy/time_series/_from_nexus_summary.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/time_series/_functions.py` & `resqpy-4.9.2/resqpy/time_series/_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/time_series/_geologic_time_series.py` & `resqpy-4.9.2/resqpy/time_series/_geologic_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/time_series/_time_duration.py` & `resqpy-4.9.2/resqpy/time_series/_time_duration.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/time_series/_time_series.py` & `resqpy-4.9.2/resqpy/time_series/_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/unstructured/__init__.py` & `resqpy-4.9.2/resqpy/unstructured/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/unstructured/_hexa_grid.py` & `resqpy-4.9.2/resqpy/unstructured/_hexa_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/unstructured/_prism_grid.py` & `resqpy-4.9.2/resqpy/unstructured/_prism_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/unstructured/_pyramid_grid.py` & `resqpy-4.9.2/resqpy/unstructured/_pyramid_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/unstructured/_tetra_grid.py` & `resqpy-4.9.2/resqpy/unstructured/_tetra_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/unstructured/_unstructured_grid.py` & `resqpy-4.9.2/resqpy/unstructured/_unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/weights_and_measures/__init__.py` & `resqpy-4.9.2/resqpy/weights_and_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/weights_and_measures/nexus_units.py` & `resqpy-4.9.2/resqpy/weights_and_measures/nexus_units.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/weights_and_measures/weights_and_measures.py` & `resqpy-4.9.2/resqpy/weights_and_measures/weights_and_measures.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/__init__.py` & `resqpy-4.9.2/resqpy/well/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/_blocked_well.py` & `resqpy-4.9.2/resqpy/well/_blocked_well.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/_deviation_survey.py` & `resqpy-4.9.2/resqpy/well/_deviation_survey.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/_md_datum.py` & `resqpy-4.9.2/resqpy/well/_md_datum.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/_trajectory.py` & `resqpy-4.9.2/resqpy/well/_trajectory.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/_wellbore_frame.py` & `resqpy-4.9.2/resqpy/well/_wellbore_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/_wellbore_marker.py` & `resqpy-4.9.2/resqpy/well/_wellbore_marker.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/_wellbore_marker_frame.py` & `resqpy-4.9.2/resqpy/well/_wellbore_marker_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/blocked_well_frame.py` & `resqpy-4.9.2/resqpy/well/blocked_well_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/well_object_funcs.py` & `resqpy-4.9.2/resqpy/well/well_object_funcs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/resqpy/well/well_utils.py` & `resqpy-4.9.2/resqpy/well/well_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.9.1/PKG-INFO` & `resqpy-4.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resqpy
-Version: 4.9.1
+Version: 4.9.2
 Summary: Python API for working with RESQML models
 Home-page: https://github.com/bp/resqpy
 License: MIT
 Keywords: RESQML
 Author: BP
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 5 - Production/Stable
```

