# Comparing `tmp/chess-board-0.3.1.tar.gz` & `tmp/chess-board-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess-board-0.3.1.tar", last modified: Tue Jul 12 13:33:16 2022, max compression
+gzip compressed data, was "chess-board-0.4.0.tar", last modified: Mon Jul 10 20:46:59 2023, max compression
```

## Comparing `chess-board-0.3.1.tar` & `chess-board-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-07-12 13:33:16.739504 chess-board-0.3.1/
--rw-rw-rw-   0        0        0    35128 2022-04-10 11:32:03.000000 chess-board-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       28 2022-05-15 10:49:54.000000 chess-board-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2371 2022-07-12 13:33:16.739504 chess-board-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1676 2022-04-10 11:32:04.000000 chess-board-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2022-07-12 13:33:16.718909 chess-board-0.3.1/chess_board.egg-info/
--rw-rw-rw-   0        0        0     2371 2022-07-12 13:33:16.000000 chess-board-0.3.1/chess_board.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      722 2022-07-12 13:33:16.000000 chess-board-0.3.1/chess_board.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-12 13:33:16.000000 chess-board-0.3.1/chess_board.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-07-12 13:33:16.000000 chess-board-0.3.1/chess_board.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-07-12 13:33:16.000000 chess-board-0.3.1/chess_board.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-12 13:33:16.730480 chess-board-0.3.1/chessboard/
--rw-rw-rw-   0        0        0        0 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/__init__.py
--rw-rw-rw-   0        0        0     4713 2022-07-12 13:32:23.000000 chess-board-0.3.1/chessboard/board.py
--rw-rw-rw-   0        0        0      244 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/constants.py
--rw-rw-rw-   0        0        0     1067 2022-07-12 13:32:23.000000 chess-board-0.3.1/chessboard/display.py
--rw-rw-rw-   0        0        0      893 2022-04-10 11:32:04.000000 chess-board-0.3.1/chessboard/fenparser.py
-drwxrwxrwx   0        0        0        0 2022-07-12 13:33:16.739504 chess-board-0.3.1/chessboard/images/
--rw-rw-rw-   0        0        0      905 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/bB.png
--rw-rw-rw-   0        0        0     1955 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/bK.png
--rw-rw-rw-   0        0        0     1239 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/bN.png
--rw-rw-rw-   0        0        0      561 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/bP.png
--rw-rw-rw-   0        0        0     1797 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/bQ.png
--rw-rw-rw-   0        0        0      652 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/bR.png
--rw-rw-rw-   0        0        0      330 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/btile.png
--rw-rw-rw-   0        0        0     1475 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/wB.png
--rw-rw-rw-   0        0        0     1910 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/wK.png
--rw-rw-rw-   0        0        0     1508 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/wN.png
--rw-rw-rw-   0        0        0      988 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/wP.png
--rw-rw-rw-   0        0        0     2288 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/wQ.png
--rw-rw-rw-   0        0        0     1043 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/wR.png
--rw-rw-rw-   0        0        0      208 2022-04-10 11:32:03.000000 chess-board-0.3.1/chessboard/images/wtile.png
--rw-rw-rw-   0        0        0     2869 2022-07-12 13:32:23.000000 chess-board-0.3.1/chessboard/pieces.py
--rw-rw-rw-   0        0        0       66 2022-04-10 11:32:58.000000 chess-board-0.3.1/chessboard/utils.py
--rw-rw-rw-   0        0        0       42 2022-07-12 13:33:16.739504 chess-board-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     3823 2022-07-12 13:18:40.000000 chess-board-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:46:59.614145 chess-board-0.4.0/
+-rw-rw-rw-   0        0        0    35128 2022-04-10 11:32:03.000000 chess-board-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       28 2022-05-15 10:49:54.000000 chess-board-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2325 2023-07-10 20:46:59.614145 chess-board-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1655 2023-07-09 03:20:46.000000 chess-board-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 20:46:59.517675 chess-board-0.4.0/chess_board.egg-info/
+-rw-rw-rw-   0        0        0     2325 2023-07-10 20:46:59.000000 chess-board-0.4.0/chess_board.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2023-07-10 20:46:59.000000 chess-board-0.4.0/chess_board.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 20:46:59.000000 chess-board-0.4.0/chess_board.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 20:46:59.000000 chess-board-0.4.0/chess_board.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-10 20:46:59.000000 chess-board-0.4.0/chess_board.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 20:46:59.555510 chess-board-0.4.0/chessboard/
+-rw-rw-rw-   0        0        0        0 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/__init__.py
+-rw-rw-rw-   0        0        0     5106 2023-07-09 04:24:41.000000 chess-board-0.4.0/chessboard/board.py
+-rw-rw-rw-   0        0        0      244 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/constants.py
+-rw-rw-rw-   0        0        0     1194 2023-07-09 03:32:25.000000 chess-board-0.4.0/chessboard/display.py
+-rw-rw-rw-   0        0        0      787 2023-07-09 03:24:53.000000 chess-board-0.4.0/chessboard/fenparser.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:46:59.614145 chess-board-0.4.0/chessboard/images/
+-rw-rw-rw-   0        0        0      905 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bB.png
+-rw-rw-rw-   0        0        0     1955 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bK.png
+-rw-rw-rw-   0        0        0     1239 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bN.png
+-rw-rw-rw-   0        0        0      561 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bP.png
+-rw-rw-rw-   0        0        0     1797 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bQ.png
+-rw-rw-rw-   0        0        0      652 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bR.png
+-rw-rw-rw-   0        0        0      330 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/btile.png
+-rw-rw-rw-   0        0        0     1475 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wB.png
+-rw-rw-rw-   0        0        0     1910 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wK.png
+-rw-rw-rw-   0        0        0     1508 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wN.png
+-rw-rw-rw-   0        0        0      988 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wP.png
+-rw-rw-rw-   0        0        0     2288 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wQ.png
+-rw-rw-rw-   0        0        0     1043 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wR.png
+-rw-rw-rw-   0        0        0      208 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wtile.png
+-rw-rw-rw-   0        0        0     2869 2022-07-12 13:32:23.000000 chess-board-0.4.0/chessboard/pieces.py
+-rw-rw-rw-   0        0        0       66 2022-04-10 11:32:58.000000 chess-board-0.4.0/chessboard/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 20:46:59.614145 chess-board-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     3823 2023-07-10 20:42:22.000000 chess-board-0.4.0/setup.py
```

### Comparing `chess-board-0.3.1/LICENSE` & `chess-board-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/PKG-INFO` & `chess-board-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: chess-board
-Version: 0.3.1
+Version: 0.4.0
 Summary: A python chessboard library for representing game positions.
 Home-page: https://github.com/ahira-justice/chess-board
 Author: Ahira Adefokun
 Author-email: justiceahira@gmail.com
 License: GPLv3
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,16 +60,14 @@
 
 game_board = display.start()
 
 while True:
     display.check_for_quit()
     display.update(valid_fen, game_board)
 
-display.terminate()
-
 ```
 
 ## Installation
 Download and install the latest release:
 ```sh
 
 # install into virtualenv
@@ -104,9 +101,7 @@
 
 ```
 **chess-board** installation automatically installs latest **pygame** version.
 
 ## License
 
 [GNU GENERAL PUBLIC LICENSE](LICENSE)
-
-
```

### Comparing `chess-board-0.3.1/README.md` & `chess-board-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,14 @@
 
 game_board = display.start()
 
 while True:
     display.check_for_quit()
     display.update(valid_fen, game_board)
 
-display.terminate()
-
 ```
 
 ## Installation
 Download and install the latest release:
 ```sh
 
 # install into virtualenv
```

### Comparing `chess-board-0.3.1/chess_board.egg-info/PKG-INFO` & `chess-board-0.4.0/chess_board.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: chess-board
-Version: 0.3.1
+Version: 0.4.0
 Summary: A python chessboard library for representing game positions.
 Home-page: https://github.com/ahira-justice/chess-board
 Author: Ahira Adefokun
 Author-email: justiceahira@gmail.com
 License: GPLv3
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,16 +60,14 @@
 
 game_board = display.start()
 
 while True:
     display.check_for_quit()
     display.update(valid_fen, game_board)
 
-display.terminate()
-
 ```
 
 ## Installation
 Download and install the latest release:
 ```sh
 
 # install into virtualenv
@@ -104,9 +101,7 @@
 
 ```
 **chess-board** installation automatically installs latest **pygame** version.
 
 ## License
 
 [GNU GENERAL PUBLIC LICENSE](LICENSE)
-
-
```

### Comparing `chess-board-0.3.1/chess_board.egg-info/SOURCES.txt` & `chess-board-0.4.0/chess_board.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/board.py` & `chess-board-0.4.0/chessboard/board.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     w_tile = pygame.image.load(os.path.join(IMAGE_DIR, 'wtile.png'))
 
     def __init__(self, bg_color, display_surf):
         self.bg_color = bg_color
         self.display_surf = display_surf
 
         self.piece_rect = []
+        self.current_fen = ''
+        self.flipped = False
+        self.fp = FenParser()
 
     def display_board(self):
         self.display_surf.fill(self.bg_color)
         pygame.draw.rect(self.display_surf, Color.BLACK, (95, 95, 410, 410), 10)
 
         self.draw_tiles()
 
@@ -54,17 +57,22 @@
                 elif not is_odd(i):
                     if is_odd(j):
                         self.display_surf.blit(Board.b_tile, Board.board_rect[i - 1][j - 1])
                     else:
                         self.display_surf.blit(Board.w_tile, Board.board_rect[i - 1][j - 1])
 
     def update_pieces(self, fen):
+        self.current_fen = fen
         self.display_board()
         self.draw_pieces(fen)
 
+    def flip(self):
+        self.flipped = not self.flipped
+        self.update_pieces(self.current_fen)
+
     def create_piece(self, color, piece_type, position):
         piece = Piece(color, piece_type, self.display_surf)
         piece.set_position(position)
         return piece
 
     def create_piece_for_side(self, board_piece, color, position):
         if board_piece == 'b':
@@ -87,18 +95,24 @@
             piece = self.create_piece(color, PieceType.QUEEN, position)
             self.piece_rect.append(piece)
 
         if board_piece == 'r':
             piece = self.create_piece(color, PieceType.ROOK, position)
             self.piece_rect.append(piece)
 
+    def parse_fen(self, fen):
+        return self.fp.parse(fen)
+
     def draw_pieces(self, fen):
         self.piece_rect = []
-        fp = FenParser(fen)
-        fen_board = fp.parse()
+        fen_board = self.fp.parse(fen)
+
+        if self.flipped:
+            fen_board.reverse()
+            fen_board = list(map(lambda x: x[::-1], fen_board))
 
         for i in range(len(fen_board)):
             for j in range(len(fen_board[i])):
                 if fen_board[i][j].isupper():
                     self.create_piece_for_side(fen_board[i][j].lower(), PieceColor.WHITE, Board.board_rect[i][j])
 
                 if fen_board[i][j].islower():
```

### Comparing `chess-board-0.3.1/chessboard/display.py` & `chess-board-0.4.0/chessboard/display.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,7 +42,15 @@
 
 def update(fen, game_board):
     check_for_quit()
     game_board.update_pieces(fen)
 
     pygame.display.update()
     fps_clock.tick(FPS)
+
+
+def flip(game_board: Board):
+    check_for_quit()
+    game_board.flip()
+
+    pygame.display.update()
+    fps_clock.tick(FPS)
```

### Comparing `chess-board-0.3.1/chessboard/fenparser.py` & `chess-board-0.4.0/chessboard/fenparser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-"""
-    https://github.com/tlehman/fenparser
-"""
-
-
 import re
 from itertools import chain
 
 
 class FenParser():
-  def __init__(self, fen_str):
-    self.fen_str = fen_str
-
 
-  def parse(self):
-    ranks = self.fen_str.split(" ")[0].split("/")
+  def parse(self, fen_str):
+    ranks = fen_str.split(" ")[0].split("/")
     pieces_on_all_ranks = [self.parse_rank(rank) for rank in ranks]
     return pieces_on_all_ranks
 
 
   def parse_rank(self, rank):
     rank_re = re.compile(r"(\d|[kqbnrpKQBNRP])")
     piece_tokens = rank_re.findall(rank)
```

### Comparing `chess-board-0.3.1/chessboard/images/bB.png` & `chess-board-0.4.0/chessboard/images/bB.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/bK.png` & `chess-board-0.4.0/chessboard/images/bK.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/bN.png` & `chess-board-0.4.0/chessboard/images/bN.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/bP.png` & `chess-board-0.4.0/chessboard/images/bP.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/bQ.png` & `chess-board-0.4.0/chessboard/images/bQ.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/bR.png` & `chess-board-0.4.0/chessboard/images/bR.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/wB.png` & `chess-board-0.4.0/chessboard/images/wB.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/wK.png` & `chess-board-0.4.0/chessboard/images/wK.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/wN.png` & `chess-board-0.4.0/chessboard/images/wN.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/wP.png` & `chess-board-0.4.0/chessboard/images/wP.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/wQ.png` & `chess-board-0.4.0/chessboard/images/wQ.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/images/wR.png` & `chess-board-0.4.0/chessboard/images/wR.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/chessboard/pieces.py` & `chess-board-0.4.0/chessboard/pieces.py`

 * *Files identical despite different names*

### Comparing `chess-board-0.3.1/setup.py` & `chess-board-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'chess-board'
 DESCRIPTION = 'A python chessboard library for representing game positions.'
 URL = 'https://github.com/ahira-justice/chess-board'
 EMAIL = 'justiceahira@gmail.com'
 AUTHOR = 'Ahira Adefokun'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.1'
+VERSION = '0.4.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pygame'
 ]
 
 # What packages are optional?
```

