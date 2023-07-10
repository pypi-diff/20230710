# Comparing `tmp/pmdsky_debug_py-7.0.1-py3-none-any.whl.zip` & `tmp/pmdsky_debug_py-7.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 852335 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Jul-09 04:27 pmdsky_debug_py/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 23-Jul-09 04:27 pmdsky_debug_py/_release.py
--rw-r--r--  2.0 unx   783396 b- defN 23-Jul-09 04:27 pmdsky_debug_py/eu.py
--rw-r--r--  2.0 unx   750244 b- defN 23-Jul-09 04:27 pmdsky_debug_py/eu_itcm.py
--rw-r--r--  2.0 unx   771294 b- defN 23-Jul-09 04:27 pmdsky_debug_py/jp.py
--rw-r--r--  2.0 unx   750244 b- defN 23-Jul-09 04:27 pmdsky_debug_py/jp_itcm.py
--rw-r--r--  2.0 unx   790641 b- defN 23-Jul-09 04:27 pmdsky_debug_py/na.py
--rw-r--r--  2.0 unx   750255 b- defN 23-Jul-09 04:27 pmdsky_debug_py/na_itcm.py
--rw-r--r--  2.0 unx   244540 b- defN 23-Jul-09 04:27 pmdsky_debug_py/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 04:27 pmdsky_debug_py/py.typed
--rw-r--r--  2.0 unx     1320 b- defN 23-Jul-09 04:28 pmdsky_debug_py-7.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 04:28 pmdsky_debug_py-7.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-09 04:28 pmdsky_debug_py-7.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 23-Jul-09 04:28 pmdsky_debug_py-7.0.1.dist-info/RECORD
-14 files, 4845058 bytes uncompressed, 850437 bytes compressed:  82.4%
+Zip file size: 857096 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jul-10 04:28 pmdsky_debug_py/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Jul-10 04:28 pmdsky_debug_py/_release.py
+-rw-r--r--  2.0 unx   786958 b- defN 23-Jul-10 04:28 pmdsky_debug_py/eu.py
+-rw-r--r--  2.0 unx   753491 b- defN 23-Jul-10 04:28 pmdsky_debug_py/eu_itcm.py
+-rw-r--r--  2.0 unx   774541 b- defN 23-Jul-10 04:28 pmdsky_debug_py/jp.py
+-rw-r--r--  2.0 unx   753491 b- defN 23-Jul-10 04:28 pmdsky_debug_py/jp_itcm.py
+-rw-r--r--  2.0 unx   793949 b- defN 23-Jul-10 04:28 pmdsky_debug_py/na.py
+-rw-r--r--  2.0 unx   753502 b- defN 23-Jul-10 04:28 pmdsky_debug_py/na_itcm.py
+-rw-r--r--  2.0 unx   245945 b- defN 23-Jul-10 04:28 pmdsky_debug_py/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 04:28 pmdsky_debug_py/py.typed
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jul-10 04:28 pmdsky_debug_py-7.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 04:28 pmdsky_debug_py-7.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-10 04:28 pmdsky_debug_py-7.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 23-Jul-10 04:28 pmdsky_debug_py-7.0.2.dist-info/RECORD
+14 files, 4866321 bytes uncompressed, 855198 bytes compressed:  82.4%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pmdsky_debug_py/protocol.py
 Comment: 
 
 Filename: pmdsky_debug_py/py.typed
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.1.dist-info/METADATA
+Filename: pmdsky_debug_py-7.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.1.dist-info/WHEEL
+Filename: pmdsky_debug_py-7.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.1.dist-info/top_level.txt
+Filename: pmdsky_debug_py-7.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.1.dist-info/RECORD
+Filename: pmdsky_debug_py-7.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmdsky_debug_py/_release.py

```diff
@@ -1 +1 @@
-RELEASE = "v0.7.0+1c49ae6a6d"
+RELEASE = "v0.7.0+2479362776"
```

## pmdsky_debug_py/eu.py

```diff
@@ -2718,14 +2718,31 @@
         [0x1A99C], [0x201A99C], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     StopSe = Symbol(
         [0x1AA80], [0x201AA80], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
+    InitAnimationControl = Symbol(
+        [0x1C0EC],
+        [0x201C0EC],
+        None,
+        "Initialize the animation_control structure\n\nr0: animation_control",
+    )
+
+    InitAnimationControlWithSet = Symbol(
+        [0x1C14C, 0x1C168],
+        [0x201C14C, 0x201C168],
+        None,
+        (
+            "Initialize the animation_control structure, and set a certain value in a"
+            " bitflag to 1\n\nr0: animation_control"
+        ),
+    )
+
     DeleteWanTableEntry = Symbol(
         [0x1D278],
         [0x201D278],
         None,
         (
             "Always delete an entry if the file is allocated externally"
             " (file_externally_allocated is set), otherwise, decrease the reference"
@@ -3293,28 +3310,48 @@
         None,
         (
             "Gets field_0xc from the dialog box of the given ID.\n\nr0:"
             " dbox_id\nreturn: field_0xc"
         ),
     )
 
+    LoadCursors = Symbol(
+        [0x29800],
+        [0x2029800],
+        None,
+        (
+            "Load and initialise the cursor and cursor16 sprites, storing the result in"
+            " CURSOR_ANIMATION_CONTROL and CURSOR_16_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     Arm9LoadUnkFieldNa0x2029EC8 = Symbol(
         [0x2A1BC],
         [0x202A1BC],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id",
     )
 
     Arm9StoreUnkFieldNa0x2029ED8 = Symbol(
         [0x2A1CC],
         [0x202A1CC],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nr1: value",
     )
 
+    LoadAlert = Symbol(
+        [0x2A1DC],
+        [0x202A1DC],
+        None,
+        (
+            "Load and initialise the alert sprite, storing the result in"
+            " ALERT_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     CreateNormalMenu = Symbol(
         [0x2B3E0],
         [0x202B3E0],
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0:"
             " layout_struct_ptr\nr1: menu_flags\nr2: additional_info_ptr\nr3:"
@@ -6521,14 +6558,34 @@
     UpdateChannels = Symbol(
         [0x74824],
         [0x2074824],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nNo params.",
     )
 
+    EnableVramBanksInSetDontSave = Symbol(
+        [0x76744],
+        [0x2076744],
+        None,
+        (
+            "Enable the VRAM bank marked in the input set, but don’t mark them as"
+            " enabled in ENABLED_VRAM_BANKS\n\nr0: vram_banks_set"
+        ),
+    )
+
+    EnableVramBanksInSet = Symbol(
+        [0x77460],
+        [0x2077460],
+        None,
+        (
+            "Enable the VRAM banks in the input set. Will reset the pointed set to 0,"
+            " and update ENABLED_VRAM_BANKS\n\nr0: vram_banks_set *"
+        ),
+    )
+
     ClearIrqFlag = Symbol(
         [0x7BB68],
         [0x207BB68],
         None,
         (
             "Enables processor interrupts by clearing the i flag in the program status"
             " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
@@ -14122,14 +14179,34 @@
         None,
         (
             "Initialize the partner follow data structure, without allocating it (in"
             " GROUND_STATE_PTRS)\n\nNo params."
         ),
     )
 
+    GetDirectionLiveActor = Symbol(
+        [0x20FC8],
+        [0x22FDB48],
+        None,
+        (
+            "Put the direction of the actor in the destination\n\nr0: live actor\nr1:"
+            " destination address (1 byte)"
+        ),
+    )
+
+    SetDirectionLiveActor = Symbol(
+        [0x20FD8],
+        [0x22FDB58],
+        None,
+        (
+            "Store the direction in the actor structure\n-1 input is ignored\nUnsure if"
+            " this change the animation\n\nr0: live actor\nr1: direction"
+        ),
+    )
+
     SprintfStatic = Symbol(
         [0x2CCE8],
         [0x2309868],
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -17061,15 +17138,15 @@
         ),
     )
 
     ChangeDungeonMusic = Symbol(
         [0xEC44],
         [0x22EB7C4],
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: music ID",
+        "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
     TrySwitchPlace = Symbol(
         [0xEFA8],
         [0x22EBB28],
         None,
         (
@@ -23403,14 +23480,25 @@
         None,
         (
             "Logs a message in the message log.\n\nr0: user entity pointer\nr1: message"
             " ID\nr2: bool, whether or not to present a message popup"
         ),
     )
 
+    InitPortraitDungeon = Symbol(
+        [0x6FB40],
+        [0x234C6C0],
+        None,
+        (
+            "Initialize the portrait box structure for the given monster and"
+            " expression\n\nr0: pointer the portrait box data structure to"
+            " initialize\nr1: monster id\nr2: emotion id"
+        ),
+    )
+
     OpenMessageLog = Symbol(
         [0x6FBDC], [0x234C75C], None, "Opens the message log window.\n\nr0: ?\nr1: ?"
     )
 
     RunDungeonMode = Symbol(
         [0x6FFA8],
         [0x234CB28],
@@ -23461,15 +23549,16 @@
 
     DisplayMessage = Symbol(
         [0x712D8],
         [0x234DE58],
         None,
         (
             "Displays a message in a dialogue box that optionally waits for player"
-            " input before closing.\n\nr0: ?\nr1: ID of the string to display\nr2: True"
+            " input before closing.\n\nr0: pointer to the structure representing the"
+            " desired state of the portrait\nr1: ID of the string to display\nr2: True"
             " to wait for player input before closing the dialogue box, false to close"
             " it automatically once all the characters get printed."
         ),
     )
 
     DisplayMessage2 = Symbol(
         [0x7132C], [0x234DEAC], None, "Very similar to DisplayMessage"
@@ -23495,15 +23584,16 @@
         (
             "Called by DisplayMessage. Seems to be the function that handles the"
             " display of the dialogue box. It won't return until all the characters"
             " have been written and after the player manually closes the dialogue box"
             " (if the corresponding parameter was set).\n\nr0: ID of the string to"
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
-            " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
+            " printed.\nr2: pointer to the structure representing the desired state of"
+            " the portrait\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
     OpenMenu = Symbol(
         [0x71E74],
         [0x234E9F4],
         None,
@@ -25338,14 +25428,47 @@
     MONEY_STORED = Symbol(
         [0x2A5504],
         [0x22A5504],
         0x4,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    CURSOR_16_SPRITE_ID = Symbol(
+        [0x2AB5A4],
+        [0x22AB5A4],
+        0x2,
+        "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE",
+    )
+
+    CURSOR_SPRITE_ID = Symbol(
+        [0x2AB5A6],
+        [0x22AB5A6],
+        0x2,
+        "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE",
+    )
+
+    CURSOR_ANIMATION_CONTROL = Symbol(
+        [0x2AB5C0], [0x22AB5C0], 0x7C, "animation_control of 'FONT/cursor.wan'"
+    )
+
+    CURSOR_16_ANIMATION_CONTROL = Symbol(
+        [0x2AB63C], [0x22AB63C], 0x7C, "animation_control of 'FONT/cursor_16.wan'"
+    )
+
+    ALERT_SPRITE_ID = Symbol(
+        [0x2AB6B8],
+        [0x22AB6B8],
+        0x2,
+        "Id of the 'FONT/alert.wan' sprite loaded in WAN_TABLE",
+    )
+
+    ALERT_ANIMATION_CONTROL = Symbol(
+        [0x2AB6BC], [0x22AB6BC], 0x7C, "animation_control of 'FONT/alter.wan'"
+    )
+
     DIALOG_BOX_LIST = Symbol(None, None, None, "Array of allocated dialog box structs.")
 
     LAST_NEW_MOVE = Symbol(
         [0x2AB78C],
         [0x22AB78C],
         0x8,
         (
@@ -25445,14 +25568,21 @@
             "Table with all team members, persistent information about them, and"
             " information about which ones are currently active.\n\nSee the comments on"
             " struct team_member_table for more information.\n\ntype: struct"
             " team_member_table"
         ),
     )
 
+    ENABLED_VRAM_BANKS = Symbol(
+        [0x2B9ECC],
+        [0x22B9ECC],
+        0x2,
+        "Bitset of enabled VRAM banks\n\ntype: vram_banks_set",
+    )
+
     FRAMES_SINCE_LAUNCH_TIMES_THREE = Symbol(
         [0x2BA304],
         [0x22BA304],
         0x4,
         (
             "Starts at 0 when the game is first launched, and ticks up by 3 per frame"
             " while the game is running."
```

## pmdsky_debug_py/eu_itcm.py

```diff
@@ -2631,14 +2631,31 @@
 
     SeChangePan = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     StopSe = Symbol(None, None, None, "Note: unverified, ported from Irdkwia's notes")
 
+    InitAnimationControl = Symbol(
+        None,
+        None,
+        None,
+        "Initialize the animation_control structure\n\nr0: animation_control",
+    )
+
+    InitAnimationControlWithSet = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the animation_control structure, and set a certain value in a"
+            " bitflag to 1\n\nr0: animation_control"
+        ),
+    )
+
     DeleteWanTableEntry = Symbol(
         None,
         None,
         None,
         (
             "Always delete an entry if the file is allocated externally"
             " (file_externally_allocated is set), otherwise, decrease the reference"
@@ -3197,25 +3214,45 @@
         None,
         (
             "Gets field_0xc from the dialog box of the given ID.\n\nr0:"
             " dbox_id\nreturn: field_0xc"
         ),
     )
 
+    LoadCursors = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load and initialise the cursor and cursor16 sprites, storing the result in"
+            " CURSOR_ANIMATION_CONTROL and CURSOR_16_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     Arm9LoadUnkFieldNa0x2029EC8 = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nr0: id"
     )
 
     Arm9StoreUnkFieldNa0x2029ED8 = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nr1: value",
     )
 
+    LoadAlert = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load and initialise the alert sprite, storing the result in"
+            " ALERT_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     CreateNormalMenu = Symbol(
         None,
         None,
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0:"
             " layout_struct_ptr\nr1: menu_flags\nr2: additional_info_ptr\nr3:"
@@ -6323,14 +6360,34 @@
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     UpdateChannels = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nNo params."
     )
 
+    EnableVramBanksInSetDontSave = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enable the VRAM bank marked in the input set, but don’t mark them as"
+            " enabled in ENABLED_VRAM_BANKS\n\nr0: vram_banks_set"
+        ),
+    )
+
+    EnableVramBanksInSet = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enable the VRAM banks in the input set. Will reset the pointed set to 0,"
+            " and update ENABLED_VRAM_BANKS\n\nr0: vram_banks_set *"
+        ),
+    )
+
     ClearIrqFlag = Symbol(
         None,
         None,
         None,
         (
             "Enables processor interrupts by clearing the i flag in the program status"
             " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
@@ -13826,14 +13883,34 @@
         None,
         (
             "Initialize the partner follow data structure, without allocating it (in"
             " GROUND_STATE_PTRS)\n\nNo params."
         ),
     )
 
+    GetDirectionLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Put the direction of the actor in the destination\n\nr0: live actor\nr1:"
+            " destination address (1 byte)"
+        ),
+    )
+
+    SetDirectionLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Store the direction in the actor structure\n-1 input is ignored\nUnsure if"
+            " this change the animation\n\nr0: live actor\nr1: direction"
+        ),
+    )
+
     SprintfStatic = Symbol(
         None,
         None,
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -16620,15 +16697,15 @@
         ),
     )
 
     ChangeDungeonMusic = Symbol(
         None,
         None,
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: music ID",
+        "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
     TrySwitchPlace = Symbol(
         None,
         None,
         None,
         (
@@ -22898,14 +22975,25 @@
         None,
         (
             "Logs a message in the message log.\n\nr0: user entity pointer\nr1: message"
             " ID\nr2: bool, whether or not to present a message popup"
         ),
     )
 
+    InitPortraitDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the portrait box structure for the given monster and"
+            " expression\n\nr0: pointer the portrait box data structure to"
+            " initialize\nr1: monster id\nr2: emotion id"
+        ),
+    )
+
     OpenMessageLog = Symbol(
         None, None, None, "Opens the message log window.\n\nr0: ?\nr1: ?"
     )
 
     RunDungeonMode = Symbol(
         None,
         None,
@@ -22956,15 +23044,16 @@
 
     DisplayMessage = Symbol(
         None,
         None,
         None,
         (
             "Displays a message in a dialogue box that optionally waits for player"
-            " input before closing.\n\nr0: ?\nr1: ID of the string to display\nr2: True"
+            " input before closing.\n\nr0: pointer to the structure representing the"
+            " desired state of the portrait\nr1: ID of the string to display\nr2: True"
             " to wait for player input before closing the dialogue box, false to close"
             " it automatically once all the characters get printed."
         ),
     )
 
     DisplayMessage2 = Symbol(None, None, None, "Very similar to DisplayMessage")
 
@@ -22988,15 +23077,16 @@
         (
             "Called by DisplayMessage. Seems to be the function that handles the"
             " display of the dialogue box. It won't return until all the characters"
             " have been written and after the player manually closes the dialogue box"
             " (if the corresponding parameter was set).\n\nr0: ID of the string to"
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
-            " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
+            " printed.\nr2: pointer to the structure representing the desired state of"
+            " the portrait\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
     OpenMenu = Symbol(
         None,
         None,
         None,
@@ -24705,14 +24795,38 @@
     MONEY_STORED = Symbol(
         None,
         None,
         None,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    CURSOR_16_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE"
+    )
+
+    CURSOR_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE"
+    )
+
+    CURSOR_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/cursor.wan'"
+    )
+
+    CURSOR_16_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/cursor_16.wan'"
+    )
+
+    ALERT_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/alert.wan' sprite loaded in WAN_TABLE"
+    )
+
+    ALERT_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/alter.wan'"
+    )
+
     DIALOG_BOX_LIST = Symbol(None, None, None, "Array of allocated dialog box structs.")
 
     LAST_NEW_MOVE = Symbol(
         None,
         None,
         None,
         (
@@ -24812,14 +24926,18 @@
             "Table with all team members, persistent information about them, and"
             " information about which ones are currently active.\n\nSee the comments on"
             " struct team_member_table for more information.\n\ntype: struct"
             " team_member_table"
         ),
     )
 
+    ENABLED_VRAM_BANKS = Symbol(
+        None, None, None, "Bitset of enabled VRAM banks\n\ntype: vram_banks_set"
+    )
+
     FRAMES_SINCE_LAUNCH_TIMES_THREE = Symbol(
         None,
         None,
         None,
         (
             "Starts at 0 when the game is first launched, and ticks up by 3 per frame"
             " while the game is running."
```

## pmdsky_debug_py/jp.py

```diff
@@ -2716,14 +2716,31 @@
         [0x1A958], [0x201A958], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     StopSe = Symbol(
         [0x1AA3C], [0x201AA3C], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
+    InitAnimationControl = Symbol(
+        None,
+        None,
+        None,
+        "Initialize the animation_control structure\n\nr0: animation_control",
+    )
+
+    InitAnimationControlWithSet = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the animation_control structure, and set a certain value in a"
+            " bitflag to 1\n\nr0: animation_control"
+        ),
+    )
+
     DeleteWanTableEntry = Symbol(
         [0x1D234],
         [0x201D234],
         None,
         (
             "Always delete an entry if the file is allocated externally"
             " (file_externally_allocated is set), otherwise, decrease the reference"
@@ -3291,28 +3308,48 @@
         None,
         (
             "Gets field_0xc from the dialog box of the given ID.\n\nr0:"
             " dbox_id\nreturn: field_0xc"
         ),
     )
 
+    LoadCursors = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load and initialise the cursor and cursor16 sprites, storing the result in"
+            " CURSOR_ANIMATION_CONTROL and CURSOR_16_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     Arm9LoadUnkFieldNa0x2029EC8 = Symbol(
         [0x2A220],
         [0x202A220],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id",
     )
 
     Arm9StoreUnkFieldNa0x2029ED8 = Symbol(
         [0x2A230],
         [0x202A230],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nr1: value",
     )
 
+    LoadAlert = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load and initialise the alert sprite, storing the result in"
+            " ALERT_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     CreateNormalMenu = Symbol(
         [0x2B444],
         [0x202B444],
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0:"
             " layout_struct_ptr\nr1: menu_flags\nr2: additional_info_ptr\nr3:"
@@ -6519,14 +6556,34 @@
     UpdateChannels = Symbol(
         [0x74774],
         [0x2074774],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nNo params.",
     )
 
+    EnableVramBanksInSetDontSave = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enable the VRAM bank marked in the input set, but don’t mark them as"
+            " enabled in ENABLED_VRAM_BANKS\n\nr0: vram_banks_set"
+        ),
+    )
+
+    EnableVramBanksInSet = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enable the VRAM banks in the input set. Will reset the pointed set to 0,"
+            " and update ENABLED_VRAM_BANKS\n\nr0: vram_banks_set *"
+        ),
+    )
+
     ClearIrqFlag = Symbol(
         None,
         None,
         None,
         (
             "Enables processor interrupts by clearing the i flag in the program status"
             " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
@@ -14058,14 +14115,34 @@
         None,
         (
             "Initialize the partner follow data structure, without allocating it (in"
             " GROUND_STATE_PTRS)\n\nNo params."
         ),
     )
 
+    GetDirectionLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Put the direction of the actor in the destination\n\nr0: live actor\nr1:"
+            " destination address (1 byte)"
+        ),
+    )
+
+    SetDirectionLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Store the direction in the actor structure\n-1 input is ignored\nUnsure if"
+            " this change the animation\n\nr0: live actor\nr1: direction"
+        ),
+    )
+
     SprintfStatic = Symbol(
         [0x2CB98],
         [0x230A478],
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -16864,15 +16941,15 @@
         ),
     )
 
     ChangeDungeonMusic = Symbol(
         [0xEB9C],
         [0x22EC47C],
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: music ID",
+        "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
     TrySwitchPlace = Symbol(
         [0xEF00],
         [0x22EC7E0],
         None,
         (
@@ -23157,14 +23234,25 @@
         None,
         (
             "Logs a message in the message log.\n\nr0: user entity pointer\nr1: message"
             " ID\nr2: bool, whether or not to present a message popup"
         ),
     )
 
+    InitPortraitDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the portrait box structure for the given monster and"
+            " expression\n\nr0: pointer the portrait box data structure to"
+            " initialize\nr1: monster id\nr2: emotion id"
+        ),
+    )
+
     OpenMessageLog = Symbol(
         [0x6F4E0], [0x234CDC0], None, "Opens the message log window.\n\nr0: ?\nr1: ?"
     )
 
     RunDungeonMode = Symbol(
         [0x6F8AC],
         [0x234D18C],
@@ -23215,15 +23303,16 @@
 
     DisplayMessage = Symbol(
         [0x70C04],
         [0x234E4E4],
         None,
         (
             "Displays a message in a dialogue box that optionally waits for player"
-            " input before closing.\n\nr0: ?\nr1: ID of the string to display\nr2: True"
+            " input before closing.\n\nr0: pointer to the structure representing the"
+            " desired state of the portrait\nr1: ID of the string to display\nr2: True"
             " to wait for player input before closing the dialogue box, false to close"
             " it automatically once all the characters get printed."
         ),
     )
 
     DisplayMessage2 = Symbol(
         [0x70C58], [0x234E538], None, "Very similar to DisplayMessage"
@@ -23249,15 +23338,16 @@
         (
             "Called by DisplayMessage. Seems to be the function that handles the"
             " display of the dialogue box. It won't return until all the characters"
             " have been written and after the player manually closes the dialogue box"
             " (if the corresponding parameter was set).\n\nr0: ID of the string to"
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
-            " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
+            " printed.\nr2: pointer to the structure representing the desired state of"
+            " the portrait\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
     OpenMenu = Symbol(
         [0x717A0],
         [0x234F080],
         None,
@@ -24969,14 +25059,38 @@
     MONEY_STORED = Symbol(
         None,
         None,
         None,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    CURSOR_16_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE"
+    )
+
+    CURSOR_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE"
+    )
+
+    CURSOR_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/cursor.wan'"
+    )
+
+    CURSOR_16_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/cursor_16.wan'"
+    )
+
+    ALERT_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/alert.wan' sprite loaded in WAN_TABLE"
+    )
+
+    ALERT_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/alter.wan'"
+    )
+
     DIALOG_BOX_LIST = Symbol(None, None, None, "Array of allocated dialog box structs.")
 
     LAST_NEW_MOVE = Symbol(
         None,
         None,
         None,
         (
@@ -25076,14 +25190,18 @@
             "Table with all team members, persistent information about them, and"
             " information about which ones are currently active.\n\nSee the comments on"
             " struct team_member_table for more information.\n\ntype: struct"
             " team_member_table"
         ),
     )
 
+    ENABLED_VRAM_BANKS = Symbol(
+        None, None, None, "Bitset of enabled VRAM banks\n\ntype: vram_banks_set"
+    )
+
     FRAMES_SINCE_LAUNCH_TIMES_THREE = Symbol(
         None,
         None,
         None,
         (
             "Starts at 0 when the game is first launched, and ticks up by 3 per frame"
             " while the game is running."
```

## pmdsky_debug_py/jp_itcm.py

```diff
@@ -2631,14 +2631,31 @@
 
     SeChangePan = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     StopSe = Symbol(None, None, None, "Note: unverified, ported from Irdkwia's notes")
 
+    InitAnimationControl = Symbol(
+        None,
+        None,
+        None,
+        "Initialize the animation_control structure\n\nr0: animation_control",
+    )
+
+    InitAnimationControlWithSet = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the animation_control structure, and set a certain value in a"
+            " bitflag to 1\n\nr0: animation_control"
+        ),
+    )
+
     DeleteWanTableEntry = Symbol(
         None,
         None,
         None,
         (
             "Always delete an entry if the file is allocated externally"
             " (file_externally_allocated is set), otherwise, decrease the reference"
@@ -3197,25 +3214,45 @@
         None,
         (
             "Gets field_0xc from the dialog box of the given ID.\n\nr0:"
             " dbox_id\nreturn: field_0xc"
         ),
     )
 
+    LoadCursors = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load and initialise the cursor and cursor16 sprites, storing the result in"
+            " CURSOR_ANIMATION_CONTROL and CURSOR_16_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     Arm9LoadUnkFieldNa0x2029EC8 = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nr0: id"
     )
 
     Arm9StoreUnkFieldNa0x2029ED8 = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nr1: value",
     )
 
+    LoadAlert = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load and initialise the alert sprite, storing the result in"
+            " ALERT_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     CreateNormalMenu = Symbol(
         None,
         None,
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0:"
             " layout_struct_ptr\nr1: menu_flags\nr2: additional_info_ptr\nr3:"
@@ -6323,14 +6360,34 @@
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     UpdateChannels = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nNo params."
     )
 
+    EnableVramBanksInSetDontSave = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enable the VRAM bank marked in the input set, but don’t mark them as"
+            " enabled in ENABLED_VRAM_BANKS\n\nr0: vram_banks_set"
+        ),
+    )
+
+    EnableVramBanksInSet = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enable the VRAM banks in the input set. Will reset the pointed set to 0,"
+            " and update ENABLED_VRAM_BANKS\n\nr0: vram_banks_set *"
+        ),
+    )
+
     ClearIrqFlag = Symbol(
         None,
         None,
         None,
         (
             "Enables processor interrupts by clearing the i flag in the program status"
             " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
@@ -13826,14 +13883,34 @@
         None,
         (
             "Initialize the partner follow data structure, without allocating it (in"
             " GROUND_STATE_PTRS)\n\nNo params."
         ),
     )
 
+    GetDirectionLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Put the direction of the actor in the destination\n\nr0: live actor\nr1:"
+            " destination address (1 byte)"
+        ),
+    )
+
+    SetDirectionLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Store the direction in the actor structure\n-1 input is ignored\nUnsure if"
+            " this change the animation\n\nr0: live actor\nr1: direction"
+        ),
+    )
+
     SprintfStatic = Symbol(
         None,
         None,
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -16620,15 +16697,15 @@
         ),
     )
 
     ChangeDungeonMusic = Symbol(
         None,
         None,
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: music ID",
+        "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
     TrySwitchPlace = Symbol(
         None,
         None,
         None,
         (
@@ -22898,14 +22975,25 @@
         None,
         (
             "Logs a message in the message log.\n\nr0: user entity pointer\nr1: message"
             " ID\nr2: bool, whether or not to present a message popup"
         ),
     )
 
+    InitPortraitDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the portrait box structure for the given monster and"
+            " expression\n\nr0: pointer the portrait box data structure to"
+            " initialize\nr1: monster id\nr2: emotion id"
+        ),
+    )
+
     OpenMessageLog = Symbol(
         None, None, None, "Opens the message log window.\n\nr0: ?\nr1: ?"
     )
 
     RunDungeonMode = Symbol(
         None,
         None,
@@ -22956,15 +23044,16 @@
 
     DisplayMessage = Symbol(
         None,
         None,
         None,
         (
             "Displays a message in a dialogue box that optionally waits for player"
-            " input before closing.\n\nr0: ?\nr1: ID of the string to display\nr2: True"
+            " input before closing.\n\nr0: pointer to the structure representing the"
+            " desired state of the portrait\nr1: ID of the string to display\nr2: True"
             " to wait for player input before closing the dialogue box, false to close"
             " it automatically once all the characters get printed."
         ),
     )
 
     DisplayMessage2 = Symbol(None, None, None, "Very similar to DisplayMessage")
 
@@ -22988,15 +23077,16 @@
         (
             "Called by DisplayMessage. Seems to be the function that handles the"
             " display of the dialogue box. It won't return until all the characters"
             " have been written and after the player manually closes the dialogue box"
             " (if the corresponding parameter was set).\n\nr0: ID of the string to"
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
-            " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
+            " printed.\nr2: pointer to the structure representing the desired state of"
+            " the portrait\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
     OpenMenu = Symbol(
         None,
         None,
         None,
@@ -24705,14 +24795,38 @@
     MONEY_STORED = Symbol(
         None,
         None,
         None,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    CURSOR_16_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE"
+    )
+
+    CURSOR_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE"
+    )
+
+    CURSOR_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/cursor.wan'"
+    )
+
+    CURSOR_16_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/cursor_16.wan'"
+    )
+
+    ALERT_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/alert.wan' sprite loaded in WAN_TABLE"
+    )
+
+    ALERT_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/alter.wan'"
+    )
+
     DIALOG_BOX_LIST = Symbol(None, None, None, "Array of allocated dialog box structs.")
 
     LAST_NEW_MOVE = Symbol(
         None,
         None,
         None,
         (
@@ -24812,14 +24926,18 @@
             "Table with all team members, persistent information about them, and"
             " information about which ones are currently active.\n\nSee the comments on"
             " struct team_member_table for more information.\n\ntype: struct"
             " team_member_table"
         ),
     )
 
+    ENABLED_VRAM_BANKS = Symbol(
+        None, None, None, "Bitset of enabled VRAM banks\n\ntype: vram_banks_set"
+    )
+
     FRAMES_SINCE_LAUNCH_TIMES_THREE = Symbol(
         None,
         None,
         None,
         (
             "Starts at 0 when the game is first launched, and ticks up by 3 per frame"
             " while the game is running."
```

## pmdsky_debug_py/na.py

```diff
@@ -2718,14 +2718,31 @@
         [0x1A900], [0x201A900], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     StopSe = Symbol(
         [0x1A9E4], [0x201A9E4], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
+    InitAnimationControl = Symbol(
+        None,
+        None,
+        None,
+        "Initialize the animation_control structure\n\nr0: animation_control",
+    )
+
+    InitAnimationControlWithSet = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the animation_control structure, and set a certain value in a"
+            " bitflag to 1\n\nr0: animation_control"
+        ),
+    )
+
     DeleteWanTableEntry = Symbol(
         [0x1D1DC],
         [0x201D1DC],
         None,
         (
             "Always delete an entry if the file is allocated externally"
             " (file_externally_allocated is set), otherwise, decrease the reference"
@@ -3293,28 +3310,48 @@
         None,
         (
             "Gets field_0xc from the dialog box of the given ID.\n\nr0:"
             " dbox_id\nreturn: field_0xc"
         ),
     )
 
+    LoadCursors = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load and initialise the cursor and cursor16 sprites, storing the result in"
+            " CURSOR_ANIMATION_CONTROL and CURSOR_16_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     Arm9LoadUnkFieldNa0x2029EC8 = Symbol(
         [0x29EC8],
         [0x2029EC8],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id",
     )
 
     Arm9StoreUnkFieldNa0x2029ED8 = Symbol(
         [0x29ED8],
         [0x2029ED8],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nr1: value",
     )
 
+    LoadAlert = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load and initialise the alert sprite, storing the result in"
+            " ALERT_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     CreateNormalMenu = Symbol(
         [0x2B0EC],
         [0x202B0EC],
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0:"
             " layout_struct_ptr\nr1: menu_flags\nr2: additional_info_ptr\nr3:"
@@ -6521,14 +6558,34 @@
     UpdateChannels = Symbol(
         [0x7448C],
         [0x207448C],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nNo params.",
     )
 
+    EnableVramBanksInSetDontSave = Symbol(
+        [0x763AC],
+        [0x20763AC],
+        None,
+        (
+            "Enable the VRAM bank marked in the input set, but don’t mark them as"
+            " enabled in ENABLED_VRAM_BANKS\n\nr0: vram_banks_set"
+        ),
+    )
+
+    EnableVramBanksInSet = Symbol(
+        [0x770C8],
+        [0x20770C8],
+        None,
+        (
+            "Enable the VRAM banks in the input set. Will reset the pointed set to 0,"
+            " and update ENABLED_VRAM_BANKS\n\nr0: vram_banks_set *"
+        ),
+    )
+
     ClearIrqFlag = Symbol(
         [0x7B7D0],
         [0x207B7D0],
         None,
         (
             "Enables processor interrupts by clearing the i flag in the program status"
             " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
@@ -14177,14 +14234,34 @@
         None,
         (
             "Initialize the partner follow data structure, without allocating it (in"
             " GROUND_STATE_PTRS)\n\nNo params."
         ),
     )
 
+    GetDirectionLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Put the direction of the actor in the destination\n\nr0: live actor\nr1:"
+            " destination address (1 byte)"
+        ),
+    )
+
+    SetDirectionLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Store the direction in the actor structure\n-1 input is ignored\nUnsure if"
+            " this change the animation\n\nr0: live actor\nr1: direction"
+        ),
+    )
+
     SprintfStatic = Symbol(
         [0x2CC8C],
         [0x2308ECC],
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -17145,15 +17222,15 @@
         ),
     )
 
     ChangeDungeonMusic = Symbol(
         [0xEBD4],
         [0x22EAE14],
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: music ID",
+        "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
     TrySwitchPlace = Symbol(
         [0xEF38],
         [0x22EB178],
         None,
         (
@@ -23487,14 +23564,25 @@
         None,
         (
             "Logs a message in the message log.\n\nr0: user entity pointer\nr1: message"
             " ID\nr2: bool, whether or not to present a message popup"
         ),
     )
 
+    InitPortraitDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the portrait box structure for the given monster and"
+            " expression\n\nr0: pointer the portrait box data structure to"
+            " initialize\nr1: monster id\nr2: emotion id"
+        ),
+    )
+
     OpenMessageLog = Symbol(
         [0x6F91C], [0x234BB5C], None, "Opens the message log window.\n\nr0: ?\nr1: ?"
     )
 
     RunDungeonMode = Symbol(
         [0x6FCE8],
         [0x234BF28],
@@ -23545,15 +23633,16 @@
 
     DisplayMessage = Symbol(
         [0x71018],
         [0x234D258],
         None,
         (
             "Displays a message in a dialogue box that optionally waits for player"
-            " input before closing.\n\nr0: ?\nr1: ID of the string to display\nr2: True"
+            " input before closing.\n\nr0: pointer to the structure representing the"
+            " desired state of the portrait\nr1: ID of the string to display\nr2: True"
             " to wait for player input before closing the dialogue box, false to close"
             " it automatically once all the characters get printed."
         ),
     )
 
     DisplayMessage2 = Symbol(
         [0x7106C], [0x234D2AC], None, "Very similar to DisplayMessage"
@@ -23579,15 +23668,16 @@
         (
             "Called by DisplayMessage. Seems to be the function that handles the"
             " display of the dialogue box. It won't return until all the characters"
             " have been written and after the player manually closes the dialogue box"
             " (if the corresponding parameter was set).\n\nr0: ID of the string to"
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
-            " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
+            " printed.\nr2: pointer to the structure representing the desired state of"
+            " the portrait\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
     OpenMenu = Symbol(
         [0x71BB4],
         [0x234DDF4],
         None,
@@ -25425,14 +25515,38 @@
     MONEY_STORED = Symbol(
         [0x2A4BC4],
         [0x22A4BC4],
         0x4,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    CURSOR_16_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE"
+    )
+
+    CURSOR_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE"
+    )
+
+    CURSOR_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/cursor.wan'"
+    )
+
+    CURSOR_16_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/cursor_16.wan'"
+    )
+
+    ALERT_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/alert.wan' sprite loaded in WAN_TABLE"
+    )
+
+    ALERT_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/alter.wan'"
+    )
+
     DIALOG_BOX_LIST = Symbol(
         [0x2A88DC], [0x22A88DC], None, "Array of allocated dialog box structs."
     )
 
     LAST_NEW_MOVE = Symbol(
         [0x2AAE4C],
         [0x22AAE4C],
@@ -25534,14 +25648,21 @@
             "Table with all team members, persistent information about them, and"
             " information about which ones are currently active.\n\nSee the comments on"
             " struct team_member_table for more information.\n\ntype: struct"
             " team_member_table"
         ),
     )
 
+    ENABLED_VRAM_BANKS = Symbol(
+        [0x2B958C],
+        [0x22B958C],
+        0x2,
+        "Bitset of enabled VRAM banks\n\ntype: vram_banks_set",
+    )
+
     FRAMES_SINCE_LAUNCH_TIMES_THREE = Symbol(
         [0x2B99C4],
         [0x22B99C4],
         0x4,
         (
             "Starts at 0 when the game is first launched, and ticks up by 3 per frame"
             " while the game is running."
```

## pmdsky_debug_py/na_itcm.py

```diff
@@ -2631,14 +2631,31 @@
 
     SeChangePan = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     StopSe = Symbol(None, None, None, "Note: unverified, ported from Irdkwia's notes")
 
+    InitAnimationControl = Symbol(
+        None,
+        None,
+        None,
+        "Initialize the animation_control structure\n\nr0: animation_control",
+    )
+
+    InitAnimationControlWithSet = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the animation_control structure, and set a certain value in a"
+            " bitflag to 1\n\nr0: animation_control"
+        ),
+    )
+
     DeleteWanTableEntry = Symbol(
         None,
         None,
         None,
         (
             "Always delete an entry if the file is allocated externally"
             " (file_externally_allocated is set), otherwise, decrease the reference"
@@ -3197,25 +3214,45 @@
         None,
         (
             "Gets field_0xc from the dialog box of the given ID.\n\nr0:"
             " dbox_id\nreturn: field_0xc"
         ),
     )
 
+    LoadCursors = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load and initialise the cursor and cursor16 sprites, storing the result in"
+            " CURSOR_ANIMATION_CONTROL and CURSOR_16_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     Arm9LoadUnkFieldNa0x2029EC8 = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nr0: id"
     )
 
     Arm9StoreUnkFieldNa0x2029ED8 = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nr1: value",
     )
 
+    LoadAlert = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load and initialise the alert sprite, storing the result in"
+            " ALERT_ANIMATION_CONTROL\n\nNo params."
+        ),
+    )
+
     CreateNormalMenu = Symbol(
         None,
         None,
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0:"
             " layout_struct_ptr\nr1: menu_flags\nr2: additional_info_ptr\nr3:"
@@ -6323,14 +6360,34 @@
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     UpdateChannels = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nNo params."
     )
 
+    EnableVramBanksInSetDontSave = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enable the VRAM bank marked in the input set, but don’t mark them as"
+            " enabled in ENABLED_VRAM_BANKS\n\nr0: vram_banks_set"
+        ),
+    )
+
+    EnableVramBanksInSet = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enable the VRAM banks in the input set. Will reset the pointed set to 0,"
+            " and update ENABLED_VRAM_BANKS\n\nr0: vram_banks_set *"
+        ),
+    )
+
     ClearIrqFlag = Symbol(
         None,
         None,
         None,
         (
             "Enables processor interrupts by clearing the i flag in the program status"
             " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
@@ -13826,14 +13883,34 @@
         None,
         (
             "Initialize the partner follow data structure, without allocating it (in"
             " GROUND_STATE_PTRS)\n\nNo params."
         ),
     )
 
+    GetDirectionLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Put the direction of the actor in the destination\n\nr0: live actor\nr1:"
+            " destination address (1 byte)"
+        ),
+    )
+
+    SetDirectionLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Store the direction in the actor structure\n-1 input is ignored\nUnsure if"
+            " this change the animation\n\nr0: live actor\nr1: direction"
+        ),
+    )
+
     SprintfStatic = Symbol(
         None,
         None,
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -16620,15 +16697,15 @@
         ),
     )
 
     ChangeDungeonMusic = Symbol(
         None,
         None,
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: music ID",
+        "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
     TrySwitchPlace = Symbol(
         None,
         None,
         None,
         (
@@ -22898,14 +22975,25 @@
         None,
         (
             "Logs a message in the message log.\n\nr0: user entity pointer\nr1: message"
             " ID\nr2: bool, whether or not to present a message popup"
         ),
     )
 
+    InitPortraitDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the portrait box structure for the given monster and"
+            " expression\n\nr0: pointer the portrait box data structure to"
+            " initialize\nr1: monster id\nr2: emotion id"
+        ),
+    )
+
     OpenMessageLog = Symbol(
         None, None, None, "Opens the message log window.\n\nr0: ?\nr1: ?"
     )
 
     RunDungeonMode = Symbol(
         None,
         None,
@@ -22956,15 +23044,16 @@
 
     DisplayMessage = Symbol(
         None,
         None,
         None,
         (
             "Displays a message in a dialogue box that optionally waits for player"
-            " input before closing.\n\nr0: ?\nr1: ID of the string to display\nr2: True"
+            " input before closing.\n\nr0: pointer to the structure representing the"
+            " desired state of the portrait\nr1: ID of the string to display\nr2: True"
             " to wait for player input before closing the dialogue box, false to close"
             " it automatically once all the characters get printed."
         ),
     )
 
     DisplayMessage2 = Symbol(None, None, None, "Very similar to DisplayMessage")
 
@@ -22988,15 +23077,16 @@
         (
             "Called by DisplayMessage. Seems to be the function that handles the"
             " display of the dialogue box. It won't return until all the characters"
             " have been written and after the player manually closes the dialogue box"
             " (if the corresponding parameter was set).\n\nr0: ID of the string to"
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
-            " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
+            " printed.\nr2: pointer to the structure representing the desired state of"
+            " the portrait\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
     OpenMenu = Symbol(
         None,
         None,
         None,
@@ -24705,14 +24795,38 @@
     MONEY_STORED = Symbol(
         None,
         None,
         None,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    CURSOR_16_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE"
+    )
+
+    CURSOR_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE"
+    )
+
+    CURSOR_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/cursor.wan'"
+    )
+
+    CURSOR_16_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/cursor_16.wan'"
+    )
+
+    ALERT_SPRITE_ID = Symbol(
+        None, None, None, "Id of the 'FONT/alert.wan' sprite loaded in WAN_TABLE"
+    )
+
+    ALERT_ANIMATION_CONTROL = Symbol(
+        None, None, None, "animation_control of 'FONT/alter.wan'"
+    )
+
     DIALOG_BOX_LIST = Symbol(None, None, None, "Array of allocated dialog box structs.")
 
     LAST_NEW_MOVE = Symbol(
         None,
         None,
         None,
         (
@@ -24812,14 +24926,18 @@
             "Table with all team members, persistent information about them, and"
             " information about which ones are currently active.\n\nSee the comments on"
             " struct team_member_table for more information.\n\ntype: struct"
             " team_member_table"
         ),
     )
 
+    ENABLED_VRAM_BANKS = Symbol(
+        None, None, None, "Bitset of enabled VRAM banks\n\ntype: vram_banks_set"
+    )
+
     FRAMES_SINCE_LAUNCH_TIMES_THREE = Symbol(
         None,
         None,
         None,
         (
             "Starts at 0 when the game is first launched, and ticks up by 3 per frame"
             " while the game is running."
```

## pmdsky_debug_py/protocol.py

```diff
@@ -1502,14 +1502,24 @@
     ]
 
     StopSe: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    InitAnimationControl: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    InitAnimationControlWithSet: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     DeleteWanTableEntry: Symbol[
         Optional[List[int]],
         None,
     ]
 
     AllocateWanTableEntry: Symbol[
         Optional[List[int]],
@@ -1782,24 +1792,34 @@
     ]
 
     GetDialogBoxField0xC: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    LoadCursors: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     Arm9LoadUnkFieldNa0x2029EC8: Symbol[
         Optional[List[int]],
         None,
     ]
 
     Arm9StoreUnkFieldNa0x2029ED8: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    LoadAlert: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     CreateNormalMenu: Symbol[
         Optional[List[int]],
         None,
     ]
 
     FreeNormalMenu: Symbol[
         Optional[List[int]],
@@ -3487,14 +3507,24 @@
     ]
 
     UpdateChannels: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    EnableVramBanksInSetDontSave: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    EnableVramBanksInSet: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ClearIrqFlag: Symbol[
         Optional[List[int]],
         None,
     ]
 
     EnableIrqFlag: Symbol[
         Optional[List[int]],
@@ -7625,14 +7655,24 @@
     ]
 
     InitPartnerFollowData: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetDirectionLiveActor: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    SetDirectionLiveActor: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     SprintfStatic: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetExclusiveItemRequirements: Symbol[
         Optional[List[int]],
@@ -12700,14 +12740,19 @@
     ]
 
     LogMessageById: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    InitPortraitDungeon: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     OpenMessageLog: Symbol[
         Optional[List[int]],
         None,
     ]
 
     RunDungeonMode: Symbol[
         Optional[List[int]],
@@ -13931,14 +13976,44 @@
     ]
 
     MONEY_STORED: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    CURSOR_16_SPRITE_ID: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
+    CURSOR_SPRITE_ID: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
+    CURSOR_ANIMATION_CONTROL: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
+    CURSOR_16_ANIMATION_CONTROL: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
+    ALERT_SPRITE_ID: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
+    ALERT_ANIMATION_CONTROL: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     DIALOG_BOX_LIST: Symbol[
         Optional[List[int]],
         None,
     ]
 
     LAST_NEW_MOVE: Symbol[
         Optional[List[int]],
@@ -13986,14 +14061,19 @@
     ]
 
     TEAM_MEMBER_TABLE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    ENABLED_VRAM_BANKS: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     FRAMES_SINCE_LAUNCH_TIMES_THREE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     SENTRY_DUTY_STRUCT: Symbol[
         Optional[List[int]],
```

## Comparing `pmdsky_debug_py-7.0.1.dist-info/METADATA` & `pmdsky_debug_py-7.0.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmdsky-debug-py
-Version: 7.0.1
+Version: 7.0.2
 Summary: pmdsky-debug symbols for Python.
 Author-email: Marco 'Capypara' Köpcke <hello@capypara.de>
 License: MIT
 Project-URL: repository, https://github.com/SkyTemple/pmdsky-debug-py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `pmdsky_debug_py-7.0.1.dist-info/RECORD` & `pmdsky_debug_py-7.0.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pmdsky_debug_py/__init__.py,sha256=xvXjdxEqeoQaaS6ssZYVI9jARzv5M4q6FNwA3Z6fOw4,1831
-pmdsky_debug_py/_release.py,sha256=eiEejP9c6MjL_RP69ds8WoRbpi5D6dQAtKjexznU0JA,30
-pmdsky_debug_py/eu.py,sha256=ySPE2oo7vxIW7DraZzjWRUNUuDrEoruzApYmSehhzlY,783396
-pmdsky_debug_py/eu_itcm.py,sha256=sbOpMgZZ4ngkEZ-9mzH91PyU-ledOsNgqu0o4NpUu7Q,750244
-pmdsky_debug_py/jp.py,sha256=-RbWeoSUAlDB-HdF3r9Jjy-wxB_Ups366pC5U9w-OV0,771294
-pmdsky_debug_py/jp_itcm.py,sha256=A9YBLEEZ_MmxejflO130cQdKG4Km9q_F_kXrzSuAULA,750244
-pmdsky_debug_py/na.py,sha256=0Kre6uaOQRuyBe3vZGWqrbHPwQGXA8VXIFlVqIFDRrU,790641
-pmdsky_debug_py/na_itcm.py,sha256=9l5HKtYXBPVI8HWs1-ucf5ClgYGCb45cKOtreWiCPng,750255
-pmdsky_debug_py/protocol.py,sha256=hrXHe1kWpBxPESTPP-ceiCRPba5hi4SZ4zLqtL9pSKI,244540
+pmdsky_debug_py/_release.py,sha256=F2PBmAeoRytEwtSPDEVcxEyNqgXt4OJPE9ArIuqN7mc,30
+pmdsky_debug_py/eu.py,sha256=TUh7XRSsPc1nk5rZmkMA6hWy6Xh8enGCCyVn_3GZmjo,786958
+pmdsky_debug_py/eu_itcm.py,sha256=5Ony3Q0zpZEKgJ4wyum7iBpd0Nc8Wmf1wqxT4mfb7_E,753491
+pmdsky_debug_py/jp.py,sha256=5Bt7rYNa6UUOxjJr_QSjMLcPe90J872a7HCSxCXxUls,774541
+pmdsky_debug_py/jp_itcm.py,sha256=pCjussa1Irb3bWngR4HMawtITSMpg_YJBwa91z94hkY,753491
+pmdsky_debug_py/na.py,sha256=-DFdqVvKVUIZyhmW0P0h2QXhmCiuVhCxolqvuQMODZk,793949
+pmdsky_debug_py/na_itcm.py,sha256=DIFl-N-Rw0fXjiaxfR2JrrFCiJI-ZHncohsiBzxQlnY,753502
+pmdsky_debug_py/protocol.py,sha256=Redx2itj26LGVpQb1uC2azRbLAEd5Mlat1yDEpDh6dA,245945
 pmdsky_debug_py/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pmdsky_debug_py-7.0.1.dist-info/METADATA,sha256=5jQQkta8pH9ouxLWT8eJt1csfmga0XRHSk9vDS1KgDc,1320
-pmdsky_debug_py-7.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pmdsky_debug_py-7.0.1.dist-info/top_level.txt,sha256=cqvpcJbud2s8IyBAc1MfCySwniko_6qO5LWSSxNIoXI,16
-pmdsky_debug_py-7.0.1.dist-info/RECORD,,
+pmdsky_debug_py-7.0.2.dist-info/METADATA,sha256=kpjN71cGdZuQg_A9r2F98hRmivz90RZlI3Ju_chxgE0,1320
+pmdsky_debug_py-7.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pmdsky_debug_py-7.0.2.dist-info/top_level.txt,sha256=cqvpcJbud2s8IyBAc1MfCySwniko_6qO5LWSSxNIoXI,16
+pmdsky_debug_py-7.0.2.dist-info/RECORD,,
```

