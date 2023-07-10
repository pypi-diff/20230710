# Comparing `tmp/darwinio-0.1.1.tar.gz` & `tmp/darwinio-0.2.0.tar.gz`

## Comparing `darwinio-0.1.1.tar` & `darwinio-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.1.1/CONTRIBUTING.md
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.1.1/requirements.txt
--rwxr-xr-x   0        0        0      404 2020-02-02 00:00:00.000000 darwinio-0.1.1/todo.org
--rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.1.1/documentation/characteristics.ods
--rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.1.1/documentation/doc.md
--rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.1.1/documentation/doc.pdf
--rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.1.1/documentation/earlystages.md
--rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.1.1/documentation/implementation.md
--rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.1.1/documentation/graphical_interface/empty_window.png
--rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.1.1/documentation/graphical_interface/main_game.png
--rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.1.1/documentation/graphical_interface/starting_window.png
--rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.1.1/documentation/screenshot/main_game_play.png
--rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.1.1/documentation/screenshot/titlescreen.png
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/__init__.py
--rwxr-xr-x   0        0        0     3664 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/__main__.py
--rwxr-xr-x   0        0        0     5467 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/brain.py
--rwxr-xr-x   0        0        0     2313 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/constants.py
--rwxr-xr-x   0        0        0    16167 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/distribution.py
--rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/genome.py
--rwxr-xr-x   0        0        0    18325 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/graphical_sim.py
--rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/organism.py
--rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/text_sim.py
--rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/archaebacteria_halophile.png
--rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/archaebacteria_methanogen.png
--rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
--rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/eubacteria_BGA.png
--rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/eubacteria_mycoplasma.png
--rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
--rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/fungi-ascomycetes.png
--rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/fungi-basidiomycetes.png
--rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/fungi-deuteromycetes.png
--rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/fungi-phycomycetes.png
--rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/metaphyta-algae.png
--rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/metaphyta-angiospermae.png
--rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/metaphyta-bryophyta.png
--rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/metaphyta-gymnospermae.png
--rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/metaphyta-pterdiophyta.png
--rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/protista_dinoflagellate.png
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/protista_euglena.png
--rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/protista_protozoan.png
--rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/protista_slimemould.png
--rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/art/theme.json
--rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.1.1/src/darwinio/assets/audio/Darwinio.mp3
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.1.1/.gitignore
--rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.1.1/LICENSE.md
--rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.1.1/README.md
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 darwinio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 darwinio-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.2.0/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.2.0/requirements.txt
+-rwxr-xr-x   0        0        0      475 2020-02-02 00:00:00.000000 darwinio-0.2.0/todo.org
+-rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.2.0/documentation/characteristics.ods
+-rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.2.0/documentation/doc.md
+-rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.2.0/documentation/doc.pdf
+-rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.2.0/documentation/earlystages.md
+-rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.2.0/documentation/implementation.md
+-rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.2.0/documentation/graphical_interface/empty_window.png
+-rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.2.0/documentation/graphical_interface/main_game.png
+-rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.2.0/documentation/graphical_interface/starting_window.png
+-rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.2.0/documentation/screenshot/main_game_play.png
+-rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.2.0/documentation/screenshot/titlescreen.png
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/__init__.py
+-rwxr-xr-x   0        0        0     3768 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/__main__.py
+-rwxr-xr-x   0        0        0     5467 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/brain.py
+-rwxr-xr-x   0        0        0     2313 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/constants.py
+-rwxr-xr-x   0        0        0    16167 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/distribution.py
+-rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/genome.py
+-rwxr-xr-x   0        0        0    18675 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/graphical_sim.py
+-rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/organism.py
+-rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/text_sim.py
+-rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/archaebacteria_halophile.png
+-rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/archaebacteria_methanogen.png
+-rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
+-rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/eubacteria_BGA.png
+-rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/eubacteria_mycoplasma.png
+-rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
+-rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/fungi-ascomycetes.png
+-rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/fungi-basidiomycetes.png
+-rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/fungi-deuteromycetes.png
+-rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/fungi-phycomycetes.png
+-rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/metaphyta-algae.png
+-rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/metaphyta-angiospermae.png
+-rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/metaphyta-bryophyta.png
+-rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/metaphyta-gymnospermae.png
+-rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/metaphyta-pterdiophyta.png
+-rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/protista_dinoflagellate.png
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/protista_euglena.png
+-rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/protista_protozoan.png
+-rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/protista_slimemould.png
+-rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/art/theme.json
+-rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.2.0/src/darwinio/assets/audio/Darwinio.mp3
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.2.0/.gitignore
+-rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.2.0/LICENSE.md
+-rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.2.0/README.md
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 darwinio-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 darwinio-0.2.0/PKG-INFO
```

### Comparing `darwinio-0.1.1/CONTRIBUTING.md` & `darwinio-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/documentation/characteristics.ods` & `darwinio-0.2.0/documentation/characteristics.ods`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/documentation/doc.md` & `darwinio-0.2.0/documentation/doc.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/documentation/doc.pdf` & `darwinio-0.2.0/documentation/doc.pdf`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/documentation/earlystages.md` & `darwinio-0.2.0/documentation/earlystages.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/documentation/implementation.md` & `darwinio-0.2.0/documentation/implementation.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/documentation/graphical_interface/empty_window.png` & `darwinio-0.2.0/documentation/graphical_interface/empty_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/documentation/graphical_interface/main_game.png` & `darwinio-0.2.0/documentation/graphical_interface/main_game.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/documentation/graphical_interface/starting_window.png` & `darwinio-0.2.0/documentation/graphical_interface/starting_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/documentation/screenshot/main_game_play.png` & `darwinio-0.2.0/documentation/screenshot/main_game_play.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/documentation/screenshot/titlescreen.png` & `darwinio-0.2.0/documentation/screenshot/titlescreen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/__main__.py` & `darwinio-0.2.0/src/darwinio/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 import pygame as pg
 import darwinio.graphical_sim as gsim
 import darwinio.constants as constants
+from importlib.metadata import version
 
 
 def main(resolution: tuple[int, int], fps: int, world_size: tuple[int, int]):
     """
     The main function that runs the game.
 
     Args:
@@ -33,30 +34,32 @@
 
     world_size (tuple[int, int]): The size of the world for simulation.
     """
 
     # Initialize Pygame
     pg.init()
     screen = pg.display.set_mode(resolution, pg.SCALED | pg.RESIZABLE)
-    pg.display.set_caption("darwinio")
+    pg.display.set_caption(f'darwinio v{version("darwinio")}')
     with gsim.get_asset_path("art", "eubacteria_BGA.png") as path:
         pg.display.set_icon(pg.image.load(path))
     clock = pg.time.Clock()
 
     # music
     music_playing = True
     with gsim.get_asset_path("audio", "Darwinio.mp3") as path:
         pg.mixer.music.load(path)
     pg.mixer.music.set_volume(1)
     pg.mixer.music.play()
 
     world = gsim.World(world_size, initial_temp_avg=45)
 
     # Create the states
-    title = gsim.TitleScreen(screen, constants.TITLE_ASCII_ART)
+    title = gsim.TitleScreen(
+        screen, constants.TITLE_ASCII_ART, f'v{version("darwinio")}'
+    )
     license_notice = gsim.TextScreen(screen, constants.LICENSE_NOTICE, 2)
     world_build = gsim.Organism_selection(screen, world, 4)
     init_help_screen = gsim.TextScreen(screen, constants.HELP, 3)
     help_screen = gsim.TextScreen(screen, constants.HELP, 5)
     with gsim.get_asset_path("art", "archaebacteria_halophile.png") as path:
         main_game = gsim.Simulation(screen, world, path)
```

### Comparing `darwinio-0.1.1/src/darwinio/brain.py` & `darwinio-0.2.0/src/darwinio/brain.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/constants.py` & `darwinio-0.2.0/src/darwinio/constants.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/distribution.py` & `darwinio-0.2.0/src/darwinio/distribution.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/genome.py` & `darwinio-0.2.0/src/darwinio/genome.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/graphical_sim.py` & `darwinio-0.2.0/src/darwinio/graphical_sim.py`

 * *Files 4% similar despite different names*

```diff
@@ -447,38 +447,53 @@
     font: The font used for rendering the title.
 
     title_surf: The rendered title surface.
 
     surface: The surface on which the state is rendered.
     """
 
-    def __init__(self, surface: pg.Surface, title_text: str) -> None:
+    def __init__(
+        self, surface: pg.Surface, title_text: str, subtitle_text: str
+    ) -> None:
         """
         Args:
         -----
         surface: The surface on which the state will be rendered.
 
         title_text: The text to be displayed as the title.
+
+        subtitle_text: The text to be displayed as the subtitle.
         """
-        self.font: pg.Font = pg.font.SysFont("monospace", 25)
-        self.title_surf: pg.Surface = self.font.render(
-            title_text, True, "white"
+
+        font: pg.Font = pg.font.SysFont("monospace", 25)
+        self.title_surf: pg.Surface = font.render(title_text, True, "white")
+
+        smallerfont: pg.Font = pg.font.SysFont("monospace", 12)
+        self.subtitle_surf: pg.Surface = smallerfont.render(
+            subtitle_text, True, "white"
         )
+
         self.surface: pg.Surface = surface
 
     def render(self) -> None:
         """Render the title screen state."""
         self.title_surf = pg.transform.scale(
             self.title_surf,
             (self.surface.get_width(), self.title_surf.get_height()),
         )
-        self.rect = self.title_surf.get_rect(
+        titlerect = self.title_surf.get_rect(
             center=self.surface.get_rect().center
         )
-        self.surface.blit(self.title_surf, self.rect)
+        self.surface.blit(self.title_surf, titlerect)
+
+        subtitlerect = self.subtitle_surf.get_rect(
+            center=self.surface.get_rect().center
+        )
+        subtitlerect.centery += 200
+        self.surface.blit(self.subtitle_surf, subtitlerect)
 
     def update(
         self, events: list[pg.Event], time_delta: float
     ) -> Union[int, None]:
         """
         Update the title screen state.
 
@@ -492,17 +507,14 @@
         -------
         int: The index of the next state to transition to, or None if no
         transition is needed.
         """
         for event in events:
             if event.type == pg.KEYDOWN:
                 return 1
-        self.rect = self.title_surf.get_rect(
-            center=self.surface.get_rect().center
-        )
         return None
 
 
 class TextScreen(State):
     """
     Represents a screen with text content.
```

### Comparing `darwinio-0.1.1/src/darwinio/organism.py` & `darwinio-0.2.0/src/darwinio/organism.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/text_sim.py` & `darwinio-0.2.0/src/darwinio/text_sim.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/archaebacteria_halophile.png` & `darwinio-0.2.0/src/darwinio/assets/art/archaebacteria_halophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/archaebacteria_methanogen.png` & `darwinio-0.2.0/src/darwinio/assets/art/archaebacteria_methanogen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/archaebacteria_thermoacidophile.png` & `darwinio-0.2.0/src/darwinio/assets/art/archaebacteria_thermoacidophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/eubacteria_BGA.png` & `darwinio-0.2.0/src/darwinio/assets/art/eubacteria_BGA.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/eubacteria_mycoplasma.png` & `darwinio-0.2.0/src/darwinio/assets/art/eubacteria_mycoplasma.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/eubacteroa_chemosynthetic.png` & `darwinio-0.2.0/src/darwinio/assets/art/eubacteroa_chemosynthetic.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/fungi-ascomycetes.png` & `darwinio-0.2.0/src/darwinio/assets/art/fungi-ascomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/fungi-basidiomycetes.png` & `darwinio-0.2.0/src/darwinio/assets/art/fungi-basidiomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/fungi-deuteromycetes.png` & `darwinio-0.2.0/src/darwinio/assets/art/fungi-deuteromycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/fungi-phycomycetes.png` & `darwinio-0.2.0/src/darwinio/assets/art/fungi-phycomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/metaphyta-algae.png` & `darwinio-0.2.0/src/darwinio/assets/art/metaphyta-algae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/metaphyta-angiospermae.png` & `darwinio-0.2.0/src/darwinio/assets/art/metaphyta-angiospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/metaphyta-bryophyta.png` & `darwinio-0.2.0/src/darwinio/assets/art/metaphyta-bryophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/metaphyta-gymnospermae.png` & `darwinio-0.2.0/src/darwinio/assets/art/metaphyta-gymnospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/metaphyta-pterdiophyta.png` & `darwinio-0.2.0/src/darwinio/assets/art/metaphyta-pterdiophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/protista_dinoflagellate.png` & `darwinio-0.2.0/src/darwinio/assets/art/protista_dinoflagellate.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/protista_euglena.png` & `darwinio-0.2.0/src/darwinio/assets/art/protista_euglena.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/protista_protozoan.png` & `darwinio-0.2.0/src/darwinio/assets/art/protista_protozoan.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/protista_slimemould.png` & `darwinio-0.2.0/src/darwinio/assets/art/protista_slimemould.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/art/theme.json` & `darwinio-0.2.0/src/darwinio/assets/art/theme.json`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/src/darwinio/assets/audio/Darwinio.mp3` & `darwinio-0.2.0/src/darwinio/assets/audio/Darwinio.mp3`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/LICENSE.md` & `darwinio-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/README.md` & `darwinio-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.1.1/pyproject.toml` & `darwinio-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [tool.hatch.build]
 exclude = [
   "*.wav",
 ]
 
 [project]
 name = "darwinio"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Tushar Maharana", email="tusharhero@sdf.org" },
   { name="Mihir Nallagonda", email="adhikshithamihir@gmail.com" },
 ]
 description = "An evolution simulator"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `darwinio-0.1.1/PKG-INFO` & `darwinio-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwinio
-Version: 0.1.1
+Version: 0.2.0
 Summary: An evolution simulator
 Project-URL: Homepage, https://github.com/tusharhero/darwinio
 Project-URL: Bug Tracker, https://github.com/tusharhero/darwinio/issues
 Author-email: Tushar Maharana <tusharhero@sdf.org>, Mihir Nallagonda <adhikshithamihir@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

