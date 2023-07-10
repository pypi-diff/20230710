# Comparing `tmp/querychart_package-2.0.2.tar.gz` & `tmp/querychart_package-2.0.3.tar.gz`

## Comparing `querychart_package-2.0.2.tar` & `querychart_package-2.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 querychart_package-2.0.2/test.csv
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/.schemawiz_config3
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/data.csv
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/fieldcounts.tsv
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/gant_data.csv
--rw-r--r--   0        0        0    11206 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/ganter.py
--rw-r--r--   0        0        0   200704 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/local_sqlite_db
--rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/plan.xlsx
--rw-r--r--   0        0        0    15204 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/querychart.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/sales.csv
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/sampledata.csv
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-2.0.2/src/querychart_package/widesales.csv
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-2.0.2/tests/.schemawiz_config3
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 querychart_package-2.0.2/tests/chart_csv_columns.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 querychart_package-2.0.2/tests/chart_csv_rows.py
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 querychart_package-2.0.2/tests/local_sqlite_db
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-2.0.2/tests/sales.csv
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 querychart_package-2.0.2/tests/tester.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-2.0.2/tests/widesales.csv
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 querychart_package-2.0.2/.gitignore
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 querychart_package-2.0.2/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 querychart_package-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 querychart_package-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 querychart_package-2.0.3/test.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/.schemawiz_config3
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/data.csv
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/fieldcounts.tsv
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/gant_data.csv
+-rw-r--r--   0        0        0    11206 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/ganter.py
+-rw-r--r--   0        0        0   200704 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/local_sqlite_db
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/plan.xlsx
+-rw-r--r--   0        0        0    15999 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/querychart.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/sales.csv
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/sampledata.csv
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-2.0.3/src/querychart_package/widesales.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-2.0.3/tests/.schemawiz_config3
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 querychart_package-2.0.3/tests/chart_csv_columns.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 querychart_package-2.0.3/tests/chart_csv_rows.py
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 querychart_package-2.0.3/tests/local_sqlite_db
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-2.0.3/tests/sales.csv
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 querychart_package-2.0.3/tests/tester.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-2.0.3/tests/widesales.csv
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 querychart_package-2.0.3/.gitignore
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 querychart_package-2.0.3/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 querychart_package-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 querychart_package-2.0.3/PKG-INFO
```

### Comparing `querychart_package-2.0.2/src/querychart_package/data.csv` & `querychart_package-2.0.3/src/querychart_package/data.csv`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.2/src/querychart_package/ganter.py` & `querychart_package-2.0.3/src/querychart_package/ganter.py`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.2/src/querychart_package/local_sqlite_db` & `querychart_package-2.0.3/src/querychart_package/local_sqlite_db`

 * *Format-specific differences are supported for SQLite databases but no file-specific differences were detected; falling back to a binary diff. file(1) reports: SQLite 3.x database, last written using SQLite version 3039004, file counter 948, database pages 49, 1st free page 49, free pages 1, cookie 0x1c4, schema 4, UTF-8, version-valid-for 948*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5351 4c69 7465 2066 6f72 6d61 7420 3300  SQLite format 3.
-00000010: 1000 0101 0040 2020 0000 03b4 0000 0031  .....@  .......1
-00000020: 0000 0031 0000 0001 0000 01c4 0000 0004  ...1............
+00000010: 1000 0101 0040 2020 0000 03fc 0000 0031  .....@  .......1
+00000020: 0000 0031 0000 0001 0000 01e8 0000 0004  ...1............
 00000030: 0000 0000 0000 0000 0000 0001 0000 0000  ................
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000050: 0000 0000 0000 0000 0000 0000 0000 03b4  ................
+00000050: 0000 0000 0000 0000 0000 0000 0000 03fc  ................
 00000060: 002e 5f1c 0500 0000 020f f600 0000 0026  .._............&
 00000070: 0ffb 0ff6 0b96 0ab4 09d2 08f0 080e 072c  ...............,
 00000080: 0629 0526 0423 0320 021d 011a 0112 0000  .).&.#. ........
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -9468,15 +9468,15 @@
 00024fb0: 1713 1f1f 081b 5453 4b20 0f05 0321 0250  ......TSK ...!.P
 00024fc0: 6f70 756c 6174 696f 6e0f 390d 0403 1d02  opulation.9.....
 00024fd0: 4469 7374 7269 6374 0557 1003 0323 0243  District.W...#.C
 00024fe0: 6f75 6e74 7279 436f 6465 00e8 0902 0315  ountryCode......
 00024ff0: 024e 616d 650f 9e07 0103 1102 6964 0fef  .Name.......id..
 00025000: 0d00 0000 1202 a800 0f15 0e2a 0d3f 0c51  ...........*.?.Q
 00025010: 0b63 0a3c 0915 0880 07eb 0756 06c1 062c  .c.<.......V...,
-00025020: 0594 04fc 0467 03d2 033d 02a8 01a5 0000  .....g...=......
+00025020: 0594 04fc 0467 03d2 033d 02a8 0213 0000  .....g...=......
 00025030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00025040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00025050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00025060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00025070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00025080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00025090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -9499,24 +9499,24 @@
 000251a0: 0000 0000 0000 0001 0317 3333 0183 2774  ..........33..'t
 000251b0: 6162 6c65 7462 6c63 7376 5f32 3032 3330  abletblcsv_20230
 000251c0: 3731 3031 3131 3274 626c 6373 765f 3230  7101112tblcsv_20
 000251d0: 3233 3037 3130 3131 3132 3143 5245 4154  23071011121CREAT
 000251e0: 4520 5441 424c 4520 7462 6c63 7376 5f32  E TABLE tblcsv_2
 000251f0: 3032 3330 3731 3031 3131 3228 0a09 6361  02307101112(..ca
 00025200: 6c5f 6474 2074 6578 7420 0909 2f2a 2065  l_dt text ../* e
-00025210: 672e 2032 3032 332f 3033 2f32 3920 2a2f  g. 2023/03/29 */
-00025220: 202c 0a09 7072 6f64 7563 7420 7465 7874   ,..product text
-00025230: 2009 092f 2a20 6567 2e20 666f 6f64 202a   ../* eg. food *
-00025240: 2f20 2c0a 0963 7573 746f 6d65 7220 7465  / ,..customer te
-00025250: 7874 2009 092f 2a20 6567 2e20 6461 7665  xt ../* eg. dave
-00025260: 202a 2f20 2c0a 0973 616c 6573 5f61 6d74   */ ,..sales_amt
-00025270: 2072 6561 6c20 0909 2f2a 2065 672e 2031   real ../* eg. 1
-00025280: 302e 3939 202a 2f20 2c0a 0963 6f73 7420  0.99 */ ,..cost 
-00025290: 7265 616c 2009 092f 2a20 6567 2e20 382e  real ../* eg. 8.
-000252a0: 3535 202a 2f20 0a29 8112 2c07 1731 3101  55 */ .)..,..11.
+00025210: 0000 0000 0000 9517 3131 0181 4f74 6162  ........11..Otab
+00025220: 6c65 7462 6c63 7376 5f32 3032 3330 3731  letblcsv_2023071
+00025230: 3031 3230 7462 6c63 7376 5f32 3032 3330  0120tblcsv_20230
+00025240: 3731 3031 3230 3143 5245 4154 4520 5441  7101201CREATE TA
+00025250: 424c 4520 7462 6c63 7376 5f32 3032 3330  BLE tblcsv_20230
+00025260: 3731 3031 3230 280a 0966 6965 6c64 2074  710120(..field t
+00025270: 6578 7420 0909 2f2a 2065 672e 2069 6420  ext ../* eg. id 
+00025280: 2a2f 202c 0a09 636f 756e 7473 2069 6e74  */ ,..counts int
+00025290: 6567 6572 2009 092f 2a20 6567 2e20 3430  eger ../* eg. 40
+000252a0: 3739 202a 2f20 0a29 8112 2c07 1731 3101  79 */ .)..,..11.
 000252b0: 814f 7461 626c 6574 626c 6373 765f 3230  .Otabletblcsv_20
 000252c0: 3233 3037 3130 3131 3674 626c 6373 765f  230710116tblcsv_
 000252d0: 3230 3233 3037 3130 3131 3630 4352 4541  202307101160CREA
 000252e0: 5445 2054 4142 4c45 2074 626c 6373 765f  TE TABLE tblcsv_
 000252f0: 3230 3233 3037 3130 3131 3628 0a09 6669  20230710116(..fi
 00025300: 656c 6420 7465 7874 2009 092f 2a20 6567  eld text ../* eg
 00025310: 2e20 6964 202a 2f20 2c0a 0963 6f75 6e74  . id */ ,..count
@@ -12282,16 +12282,16 @@
 0002ff90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0002ffa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0002ffb0: 0000 0000 0000 0000 0000 0f05 0321 0250  .............!.P
 0002ffc0: 6f70 756c 6174 696f 6e0f 390d 0403 1d02  opulation.9.....
 0002ffd0: 4469 7374 7269 6374 0557 1003 0323 0243  District.W...#.C
 0002ffe0: 6f75 6e74 7279 436f 6465 00e8 0902 0315  ountryCode......
 0002fff0: 024e 616d 650f 9e07 0103 1102 6964 0fef  .Name.......id..
-00030000: 0000 0000 0000 0000 0fd6 0fa5 0f7a 0f50  .............z.P
-00030010: 0f1f 0eee 0ebd 0e92 0e61 0e36 0e0c 0ddb  .........a.6....
+00030000: 0000 0000 0000 0000 0ff7 0fec 0fda 0fcb  ................
+00030010: 0fba 0eee 0ebd 0e92 0e61 0e36 0e0c 0ddb  .........a.6....
 00030020: 0daa 0000 0000 0000 0000 0000 0000 0000  ................
 00030030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00030040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00030050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00030060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00030070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00030080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -12533,12 +12533,12 @@
 00030f40: 4021 fae1 47ae 147b 4021 b333 3333 3333  @!..G..{@!.33333
 00030f50: 2804 0621 1515 0707 3230 3233 2f30 342f  (..!....2023/04/
 00030f60: 3031 666f 6f64 6461 7665 4017 f5c2 8f5c  01fooddave@....\
 00030f70: 28f6 4045 a000 0000 0000 2903 0621 1715  (.@E......)..!..
 00030f80: 0707 3230 3233 2f30 332f 3331 626f 6f7a  ..2023/03/31booz
 00030f90: 6564 6176 6540 34fd 70a3 d70a 3d40 02cc  edave@4.p...=@..
 00030fa0: cccc cccc cd2f 0206 2123 1507 0732 3032  ...../..!#...202
-00030fb0: 332f 3033 2f33 3065 6c65 6374 726f 6e69  3/03/30electroni
-00030fc0: 6373 6461 7665 402f fae1 47ae 147b 4032  csdave@/..G..{@2
-00030fd0: 7333 3333 3333 2801 0621 1515 0707 3230  s33333(..!....20
-00030fe0: 3233 2f30 332f 3239 666f 6f64 6461 7665  23/03/29fooddave
-00030ff0: 4025 fae1 47ae 147b 4021 1999 9999 999a  @%..G..{@!......
+00030fb0: 332f 3033 2f33 3065 6c65 0f05 0321 0250  3/03/30ele...!.P
+00030fc0: 6f70 756c 6174 696f 6e0f 390d 0403 1d02  opulation.9.....
+00030fd0: 4469 7374 7269 6374 0557 1003 0323 0243  District.W...#.C
+00030fe0: 6f75 6e74 7279 436f 6465 00e8 0902 0315  ountryCode......
+00030ff0: 024e 616d 650f 9e07 0103 1102 6964 0fef  .Name.......id..
```

### Comparing `querychart_package-2.0.2/src/querychart_package/plan.xlsx` & `querychart_package-2.0.3/src/querychart_package/plan.xlsx`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.2/src/querychart_package/querychart.py` & `querychart_package-2.0.3/src/querychart_package/querychart.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 	#charter().showcsv('sales.csv','SELECT cal_dt FROM sales.csv ORDER BY cal_dt')
 	#charter().showcsv('widesales.csv','SELECT * FROM widesales.csv')
 
 	#name,start_dt,end_dt,progress_pct
 	#charter().progresscsv('gant_data.csv')
 
 	#charter().csv_querypiechart('fieldcounts.tsv','SELECT field,counts FROM fieldcounts.tsv ORDER BY field')
-	#charter().csv_querybarchart('SELECT cal_dt,sales_amt,cost FROM sales.csv ORDER BY cal_dt','sales.csv','this is my title','xlabel','ylabel',1,8)
-	#charter().csv_querybarchart('SELECT field,counts FROM fieldcounts.tsv','fieldcounts.tsv','this is my title','xlabel','ylabel',3,5)
+	#charter().csv_querybarchart('SELECT cal_dt,sales_amt,cost FROM sales.csv ORDER BY cal_dt','sales.csv','this is my title','xlabel','ylabel')
+	#charter().csv_querybarchart('SELECT field,counts FROM fieldcounts.tsv','fieldcounts.tsv','this is my title','xlabel','ylabel',-1)
 	#charter().tester('SELECT field,counts FROM fieldcounts.tsv','fieldcounts.tsv','this is my title','xlabel','ylabel')
 
 class charter():
 	def __init__(self):
 		self.schwiz = schemawiz()
 
 	# Stages	start_dt	end_dt	progress_pct
@@ -214,50 +214,86 @@
 	#
 	# cal_dt,product,customer,sales_amt,cost
 	# 2023/03/29,food,dave,10.99,8.55
 	# 2023/03/30,electronics,dave,15.99,18.45
 	# 2023/03/31,booze,dave,20.99,2.35
 	# 2023/04/01,food,dave,5.99,43.25
 	#
-	def csv_querybarchart(self,query,csv_filename='',ptitle='',xlabel='',ylabel='',grph_rowstrt=-1,grph_rowend=-1):
+	def csv_querybarchart(self,query,csv_filename='',ptitle='',xlabel='',ylabel='',ipagesize=-1):
 
 		field_label = xlabel
 		measure_label = ylabel
 		title = ptitle
 
 		if csv_filename != '':
 			self.schwiz.createload_sqlite_from_csv(csv_filename)
 			tablename = self.schwiz.lastcall_tablename
 			newquery = query.replace(csv_filename,tablename)
 		else:
 			newquery = query
 
 		chartdata = self.schwiz.dbthings.sqlite_db.query(newquery)
-		chartfields = []
-		chartcounts = []
-		colhdr = []
-
-		for k in [i[0] for i in chartdata.description]:
-			colhdr.append(k)
+		
+		if ipagesize == -1:
+			pagesize = chartdata.rowcount
+		else:
+			pagesize = ipagesize
 
-		rows = 1
-		for row in chartdata:
-			rows += 1
-			if (grph_rowstrt == -1) or (rows > grph_rowstrt):
-				if (grph_rowend == -1) or (rows <= grph_rowend+1):
+		at_least_cnt = int(chartdata.rowcount / pagesize)
+		remainder_cnt = chartdata.rowcount % pagesize
+		for i in range(0,at_least_cnt):
+			gstrt = 1 + i*pagesize
+			gend = gstrt + pagesize - 1
+			#print('gstrt:',gstrt)
+			#print('gend:',gend)
+
+			chartfields = []
+			chartcounts = []
+
+			rows = 0
+			for row in chartdata:
+				rows += 1
+				if (rows >= gstrt) and (rows <= gend):
+					# first col will be label
+					chartfields.append(row[0])
+					chartcounts.append(row[1])
+			
+			if rows > 7:
+				fig = plt.figure(figsize = (14, 5))
+			else:
+				fig = plt.figure(figsize = (5, 5))
+
+
+			plt.bar(chartfields, chartcounts, color = "red")
+			plt.title(title)
+			plt.xlabel(field_label)
+			plt.ylabel(measure_label)
+
+			fig.show()
+		gstrt = at_least_cnt*pagesize
+		if gstrt < chartdata.rowcount:
+			chartfields = []
+			chartcounts = []
+			rows = 0
+
+			for row in chartdata:
+				#print(rows,' - ',row[0])
+				rows += 1
+				if (rows > (at_least_cnt*pagesize)):
 					# first col will be label
 					chartfields.append(row[0])
 					chartcounts.append(row[1])
 
-		fig = plt.figure(figsize = (14, 5))
+			fig = plt.figure(figsize = (5, 5))
+			plt.bar(chartfields, chartcounts, color = "red")
+			plt.title(title)
+			plt.xlabel(field_label)
+			plt.ylabel(measure_label)
 
-		plt.bar(chartfields, chartcounts, color = "red")
-		plt.title(title)
-		plt.xlabel(field_label)
-		plt.ylabel(measure_label)
+			fig.show()
 
 		plt.show()
 
 		if csv_filename != '':
 			self.schwiz.dbthings.sqlite_db.execute('DROP TABLE ' + tablename)
```

### Comparing `querychart_package-2.0.2/src/querychart_package/sales.csv` & `querychart_package-2.0.3/src/querychart_package/sales.csv`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.2/src/querychart_package/sampledata.csv` & `querychart_package-2.0.3/src/querychart_package/sampledata.csv`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.2/tests/local_sqlite_db` & `querychart_package-2.0.3/tests/local_sqlite_db`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.2/tests/sales.csv` & `querychart_package-2.0.3/tests/sales.csv`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.2/pyproject.toml` & `querychart_package-2.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","schemawizard_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "querychart_package"
-version = "2.0.2"
+version = "2.0.3"
 dependencies = [
   'schemawizard_package >= 2.3.5'
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
 description = "A wrapper for simplified matplotlib usage"
```

### Comparing `querychart_package-2.0.2/PKG-INFO` & `querychart_package-2.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querychart_package
-Version: 2.0.2
+Version: 2.0.3
 Summary: A wrapper for simplified matplotlib usage
 Project-URL: Homepage, https://github.com/daveskura/querychart
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

