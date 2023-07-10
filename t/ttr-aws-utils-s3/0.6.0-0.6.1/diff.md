# Comparing `tmp/ttr_aws_utils_s3-0.6.0.tar.gz` & `tmp/ttr_aws_utils_s3-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttr_aws_utils_s3-0.6.0.tar", last modified: Sat Jul  1 22:37:07 2023, max compression
+gzip compressed data, was "ttr_aws_utils_s3-0.6.1.tar", last modified: Mon Jul 10 15:14:50 2023, max compression
```

## Comparing `ttr_aws_utils_s3-0.6.0.tar` & `ttr_aws_utils_s3-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,16 @@
--rw-r--r--   0        0        0      250 2023-06-30 20:46:21.594945 ttr_aws_utils_s3-0.6.0/AUTHORS
--rw-r--r--   0        0        0     1590 2017-05-09 23:34:02.826309 ttr_aws_utils_s3-0.6.0/LICENSE.rst
--rw-r--r--   0        0        0     9640 2023-07-01 22:31:08.760778 ttr_aws_utils_s3-0.6.0/README.rst
--rw-r--r--   0        0        0      283 2023-07-01 22:25:59.534302 ttr_aws_utils_s3-0.6.0/noxfile.py
--rw-r--r--   0        0        0     1587 2023-07-01 22:37:07.163274 ttr_aws_utils_s3-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1847 2020-06-23 18:04:12.897439 ttr_aws_utils_s3-0.6.0/tests/test_fname_factory.py
--rw-r--r--   0        0        0     1130 2019-02-27 19:42:31.563499 ttr_aws_utils_s3-0.6.0/tests/test_from_to.py
--rw-r--r--   0        0        0     1852 2017-05-09 23:34:02.830309 ttr_aws_utils_s3-0.6.0/tests/test_parsetime.py
--rw-r--r--   0        0        0    10370 1970-01-01 00:00:00.000000 ttr_aws_utils_s3-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      250 2023-06-30 21:06:14.342275 ttr_aws_utils_s3-0.6.1/AUTHORS
+-rw-r--r--   0        0        0     1618 2023-06-19 12:26:44.291809 ttr_aws_utils_s3-0.6.1/LICENSE.rst
+-rw-r--r--   0        0        0     9893 2023-07-10 14:09:54.346598 ttr_aws_utils_s3-0.6.1/README.rst
+-rw-r--r--   0        0        0     1586 2023-07-10 15:14:50.831581 ttr_aws_utils_s3-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1895 2023-06-19 12:26:44.296810 ttr_aws_utils_s3-0.6.1/tests/test_fname_factory.py
+-rw-r--r--   0        0        0     1168 2023-06-19 12:26:44.297809 ttr_aws_utils_s3-0.6.1/tests/test_from_to.py
+-rw-r--r--   0        0        0     1902 2023-06-19 12:26:44.297809 ttr_aws_utils_s3-0.6.1/tests/test_parsetime.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:26:44.299810 ttr_aws_utils_s3-0.6.1/ttr/aws/utils/s3/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:26:44.300809 ttr_aws_utils_s3-0.6.1/ttr/aws/utils/s3/cli/__init__.py
+-rw-r--r--   0        0        0     1779 2023-06-19 12:26:44.300809 ttr_aws_utils_s3-0.6.1/ttr/aws/utils/s3/cli/chart.html
+-rw-r--r--   0        0        0     3663 2023-06-19 12:26:44.300809 ttr_aws_utils_s3-0.6.1/ttr/aws/utils/s3/cli/getvers.py
+-rw-r--r--   0        0        0     8589 2023-07-10 14:09:54.355620 ttr_aws_utils_s3-0.6.1/ttr/aws/utils/s3/cli/lsvers.py
+-rw-r--r--   0        0        0     3392 2023-07-10 14:09:54.356596 ttr_aws_utils_s3-0.6.1/ttr/aws/utils/s3/cli/tmpgen.py
+-rw-r--r--   0        0        0     5045 2023-06-19 12:26:44.301810 ttr_aws_utils_s3-0.6.1/ttr/aws/utils/s3/saver.py
+-rw-r--r--   0        0        0     2092 2023-06-19 12:26:44.302809 ttr_aws_utils_s3-0.6.1/ttr/aws/utils/s3/utils.py
+-rw-r--r--   0        0        0    10370 1970-01-01 00:00:00.000000 ttr_aws_utils_s3-0.6.1/PKG-INFO
```

### Comparing `ttr_aws_utils_s3-0.6.0/LICENSE.rst` & `ttr_aws_utils_s3-0.6.1/LICENSE.rst`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Copyright (c) 2011, Jan Vlcinsky
-Copyright (c) 2012-2017, TamTam Research s.r.o. http://www.tamtamresearch.com
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS
-BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
-
-The views and conclusions contained in the software and documentation are
-those of the authors and should not be interpreted as representing official
-policies, either expressed or implied, of the FreeBSD Project.
+Copyright (c) 2011, Jan Vlcinsky
+Copyright (c) 2012-2017, TamTam Research s.r.o. http://www.tamtamresearch.com
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS
+BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE.
+
+The views and conclusions contained in the software and documentation are
+those of the authors and should not be interpreted as representing official
+policies, either expressed or implied, of the FreeBSD Project.
```

### Comparing `ttr_aws_utils_s3-0.6.0/README.rst` & `ttr_aws_utils_s3-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: ttr.aws.utils.s3
+Version: 0.6.1
+Summary: CLI to list and fetch objects from versioned S3 buckets. Plus get tmp url.
+Keywords: aws s3
+Home-page: https://gitlab.com/tamtamresearch-public/pypi/ttr.aws.utils.s3
+Author: Jan Vlcinsky
+Author-Email: Unknown <jan.vlcinsky@tamtamresearch.com>
+License: BSD
+Project-URL: Homepage, https://gitlab.com/tamtamresearch-public/pypi/ttr.aws.utils.s3
+Requires-Python: >=3.8
+Requires-Dist: PyYAML==6.0
+Requires-Dist: boto3==1.26.165
+Requires-Dist: plac==1.3.5
+Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: pytz
+Requires-Dist: pendulum==2.1.2; extra == "test"
+Requires-Dist: pytest==7.4.0; extra == "test"
+Provides-Extra: test
+Description-Content-Type: text/x-rst
+
 ============
 AWS Utils S3
 ============
 
 Tools to list and fetch objects from versioned AWS_ S3_ bucket:
 
 * `s3lsvers`: List object versions, see versioning_
```

### Comparing `ttr_aws_utils_s3-0.6.0/pyproject.toml` & `ttr_aws_utils_s3-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "PyYAML==6.0",
     "boto3==1.26.165",
     "plac==1.3.5",
     "python-dateutil==2.8.2",
     "pytz",
 ]
 requires-python = ">=3.8"
-version = "0.6.0"
+version = "0.6.1"
 
 [project.license]
 text = "BSD"
 
 [project.optional-dependencies]
 test = [
     "pendulum==2.1.2",
@@ -56,12 +56,14 @@
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
-[tool.pdm]
-package-dir = "ttr/aws/utils/s3"
+[tool.pdm.build]
+includes = [
+    "ttr",
+]
 
 [tool.pdm.version]
 source = "scm"
```

### Comparing `ttr_aws_utils_s3-0.6.0/tests/test_fname_factory.py` & `ttr_aws_utils_s3-0.6.1/tests/test_fname_factory.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# import dateutil.parser
-import pendulum
-from ttr.aws.utils.s3.saver import FnameFactory
-import pytest
-
-
-def get_last_modified_scenarios():
-    plan = [["buck/k/n.json:1234aaa:2017-05-15T20:25:07Z",
-             "n.2017-05-15T20_25_07Z.json"],
-            ["buck/d.json:1234aaa:1970-01-01T00:00:00Z",
-             "d.1970-01-01T00_00_00Z.json"],
-            ]
-    for objver, expected in plan:
-        obj, version_id, dtstr = objver.split(":", 2)
-        bucket_name, key_name = obj.split("/", 1)
-        dt = pendulum.parse(dtstr)
-        objverdct = {"LastModified": dt, "VersionId": version_id}
-        yield bucket_name, key_name, version_id, objverdct, expected
-
-
-@pytest.mark.parametrize("scenario", list(get_last_modified_scenarios()))
-def test_last_modified(scenario):
-    bucket_name, key_name, version_id, objdict, expected = scenario
-    fname_factory = FnameFactory().last_modified
-    fname = fname_factory(bucket_name, key_name, version_id, objdict)
-    assert fname == expected
-
-
-def get_version_id_scenarios():
-    plan = [["buck/k/n.json:1234aaa:2017-05-15T20:25:07Z",
-             "n.1234aaa.json"],
-            ["buck/d.json:1234aaa:1970-01-01T00:00:00Z",
-             "d.1234aaa.json"],
-            ]
-    for objver, expected in plan:
-        obj, version_id, dtstr = objver.split(":", 2)
-        bucket_name, key_name = obj.split("/", 1)
-        dt = pendulum.parse(dtstr)
-        objverdct = {"LastModified": dt, "VersionId": version_id}
-        yield bucket_name, key_name, version_id, objverdct, expected
-
-
-@pytest.mark.parametrize("scenario", list(get_version_id_scenarios()))
-def test_version_id(scenario):
-    bucket_name, key_name, version_id, objdict, expected = scenario
-    fname_factory = FnameFactory().version_id
-    fname = fname_factory(bucket_name, key_name, version_id, objdict)
-    assert fname == expected
+# import dateutil.parser
+import pendulum
+from ttr.aws.utils.s3.saver import FnameFactory
+import pytest
+
+
+def get_last_modified_scenarios():
+    plan = [["buck/k/n.json:1234aaa:2017-05-15T20:25:07Z",
+             "n.2017-05-15T20_25_07Z.json"],
+            ["buck/d.json:1234aaa:1970-01-01T00:00:00Z",
+             "d.1970-01-01T00_00_00Z.json"],
+            ]
+    for objver, expected in plan:
+        obj, version_id, dtstr = objver.split(":", 2)
+        bucket_name, key_name = obj.split("/", 1)
+        dt = pendulum.parse(dtstr)
+        objverdct = {"LastModified": dt, "VersionId": version_id}
+        yield bucket_name, key_name, version_id, objverdct, expected
+
+
+@pytest.mark.parametrize("scenario", list(get_last_modified_scenarios()))
+def test_last_modified(scenario):
+    bucket_name, key_name, version_id, objdict, expected = scenario
+    fname_factory = FnameFactory().last_modified
+    fname = fname_factory(bucket_name, key_name, version_id, objdict)
+    assert fname == expected
+
+
+def get_version_id_scenarios():
+    plan = [["buck/k/n.json:1234aaa:2017-05-15T20:25:07Z",
+             "n.1234aaa.json"],
+            ["buck/d.json:1234aaa:1970-01-01T00:00:00Z",
+             "d.1234aaa.json"],
+            ]
+    for objver, expected in plan:
+        obj, version_id, dtstr = objver.split(":", 2)
+        bucket_name, key_name = obj.split("/", 1)
+        dt = pendulum.parse(dtstr)
+        objverdct = {"LastModified": dt, "VersionId": version_id}
+        yield bucket_name, key_name, version_id, objverdct, expected
+
+
+@pytest.mark.parametrize("scenario", list(get_version_id_scenarios()))
+def test_version_id(scenario):
+    bucket_name, key_name, version_id, objdict, expected = scenario
+    fname_factory = FnameFactory().version_id
+    fname = fname_factory(bucket_name, key_name, version_id, objdict)
+    assert fname == expected
```

### Comparing `ttr_aws_utils_s3-0.6.0/tests/test_from_to.py` & `ttr_aws_utils_s3-0.6.1/tests/test_from_to.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import pytest
-from datetime import datetime
-import pytz
-from ttr.aws.utils.s3.utils import check_from_to
-
-
-def utc(*args, **kwargs):
-    res = datetime(*args, **kwargs)
-    return res.replace(tzinfo=pytz.UTC)
-
-
-scenarios = [
-    ["2015-08-15T00:00:00Z", "2015-09-15T00:00:00Z",
-     (utc(2015, 8, 15, 0, 0, 0),
-      utc(2015, 9, 15, 0, 0, 0))],
-    ["", "", (None, None)],
-    ["", "2015-09-15T00:00:00Z", (None, utc(2015, 9, 15, 0, 0, 0))],
-    ["2015-08-15T00:00:00Z", "", (utc(2015, 8, 15, 0, 0, 0),
-                                  None)],
-    pytest.param(
-        ["2015-09-15T00:00:00Z", "2015-08-15T00:00:00Z",
-         (utc(2015, 8, 15, 0, 0, 0),
-          utc(2015, 9, 15, 0, 0, 0))],
-        marks=pytest.mark.xfail), ]
-
-
-def scen_id(scenario):
-    from_txt = scenario[0]
-    to_txt = scenario[1]
-    return "{from_txt}-{to_txt}".format(from_txt=from_txt,
-                                        to_txt=to_txt)
-
-
-@pytest.mark.parametrize("scenario", scenarios, ids=scen_id)
-def test_from_to(scenario):
-    from_time, to_time, expected = scenario
-    res = check_from_to(from_time, to_time)
-    assert res == expected
+import pytest
+from datetime import datetime
+import pytz
+from ttr.aws.utils.s3.utils import check_from_to
+
+
+def utc(*args, **kwargs):
+    res = datetime(*args, **kwargs)
+    return res.replace(tzinfo=pytz.UTC)
+
+
+scenarios = [
+    ["2015-08-15T00:00:00Z", "2015-09-15T00:00:00Z",
+     (utc(2015, 8, 15, 0, 0, 0),
+      utc(2015, 9, 15, 0, 0, 0))],
+    ["", "", (None, None)],
+    ["", "2015-09-15T00:00:00Z", (None, utc(2015, 9, 15, 0, 0, 0))],
+    ["2015-08-15T00:00:00Z", "", (utc(2015, 8, 15, 0, 0, 0),
+                                  None)],
+    pytest.param(
+        ["2015-09-15T00:00:00Z", "2015-08-15T00:00:00Z",
+         (utc(2015, 8, 15, 0, 0, 0),
+          utc(2015, 9, 15, 0, 0, 0))],
+        marks=pytest.mark.xfail), ]
+
+
+def scen_id(scenario):
+    from_txt = scenario[0]
+    to_txt = scenario[1]
+    return "{from_txt}-{to_txt}".format(from_txt=from_txt,
+                                        to_txt=to_txt)
+
+
+@pytest.mark.parametrize("scenario", scenarios, ids=scen_id)
+def test_from_to(scenario):
+    from_time, to_time, expected = scenario
+    res = check_from_to(from_time, to_time)
+    assert res == expected
```

### Comparing `ttr_aws_utils_s3-0.6.0/PKG-INFO` & `ttr_aws_utils_s3-0.6.1/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,274 +1,253 @@
-Metadata-Version: 2.1
-Name: ttr.aws.utils.s3
-Version: 0.6.0
-Summary: CLI to list and fetch objects from versioned S3 buckets. Plus get tmp url.
-Keywords: aws s3
-Home-page: https://gitlab.com/tamtamresearch-public/pypi/ttr.aws.utils.s3
-Author: Jan Vlcinsky
-Author-Email: Unknown <jan.vlcinsky@tamtamresearch.com>
-License: BSD
-Project-URL: Homepage, https://gitlab.com/tamtamresearch-public/pypi/ttr.aws.utils.s3
-Requires-Python: >=3.8
-Requires-Dist: PyYAML==6.0
-Requires-Dist: boto3==1.26.165
-Requires-Dist: plac==1.3.5
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: pytz
-Requires-Dist: pendulum==2.1.2; extra == "test"
-Requires-Dist: pytest==7.4.0; extra == "test"
-Provides-Extra: test
-Description-Content-Type: text/x-rst
-
-============
-AWS Utils S3
-============
-
-Tools to list and fetch objects from versioned AWS_ S3_ bucket:
-
-* `s3lsvers`: List object versions, see versioning_
-* `s3getvers`: Fetch specified object versions
-* `s3tmpgen`: Generate temporary url links to objects
-
-.. contents:: Table of Contents
-
-Installation
-============
-Using `pip`::
-
-  $ pip install ttr.aws.utils.s3
-
-Using `pipx`::
-
-  $ pipx install ttr.aws.utils.s3
-    
-Quick start
-===========
-We want to fetch versions of feed in bucket `mybucket` named `my/versioned/feed.xml`
-
-1. Configure AWSCLI credentials to allow access to your buckets and objects. E.g. using `AWS_DEFAULT_PROFILE`. See AWS_config_.
-
-2. create csv file for given feed and time period::
-
-    $ s3lsvers -from 2012-05-24T00:15 -to 2012-05-24T01:15 -list-file list.csv mybucket/my/versioned/feed.xml
-
-   You shall then find file `list.csv` on your disk.
-
-3. Review records in `list.csv` and delete all lines with version, which are not of your interest.
-
-4. Using `list.csv`, ask s3getvers to fetch all versions specified in the file. Be sure to run it on empty directory::
-
-    $ s3getvers mybucket list.csv
-
-   You will see, how is each version downloaded and saved to your current directory.
-
-5. Finally, you can try generating temorary url to your feed (showing the latest existing)::
-
-    $ s3tmpgen 2014-09-30T00:00:00Z mybucket my/versioned/feed.xml
-    https://mybucket.s3.amazonaws.com/my/versioned/feed.xml?Signature=kOCwz%2FkanVWX8O15dlXhy4jrbwY%3D&Expires=1412031600&AWSAccessKeyId=AKIAxyzxyzxyzEQA
-
-   Note, that the url does not include VersionId, so it will always point to the most up todate version (in case the key happens to be on versioned bucket).
-
-Provided commands
-=================
-
-s3lsvers
---------
-List versions of some feed. Could output into CSV file (-list-file) and/or html chart (-html-file).::
-
-    $ s3lsvers -h
-    usage: s3lsvers [-h] [-from None] [-to None] [-list-file None]
-                    [-html-file None] [-version-id None] [-profile-name None]
-                    [-aws-access-key-id None] [-aws-secret-access-key None]
-                    bucket_key
-
-    List object versions stored on versioned S3 bucket, create CSV and/or HTML file.
-        CSV file can be used e.g. by `s3getvers` command.
-        HTML file allows showing feed size and update period in chart.
-
-        Version can be limited by time range `from` - `to`.
-        `version-id` allow starting from specific version (back to the past,
-        excluding given version).
-
-        Object key is defined either as {bucket_name}/{key_name} or as alias from .s3lsvers file.
-
-        Times are expressed in RFC 3339 format using Zulu (UTC) timezone, possibly truncated.
-        For truncated time strings, maximal time extent is used.
-
-        Listing has records with structure:
-          `{key_name};{version_id};{size};{last_modified};{age}`
-            - key_name: name of the key (excluding bucket name).
-            - version_id: unique identifier for given version on given bucket.
-            - size: size of key object in bytes
-            - last_modified: RFC 3339 formated object modification time
-            - age: update interval [s] for given version
-
-        Examples:
-
-            Lists all versions of given `keyname` on `bucket`::
-
-                $ s3lsvers bucketname/keyname
-
-            Lists all versions in period betwen `from` and `to` time::
-
-                $ s3lsvers -from 2010-01-01 -to 2011-07-19T12:00:00 bucket/key
-
-            Lists all versions and writes them into csv file named `versions.csv`::
-
-                $ s3lsvers -list-file versions.csv bucketname/keyname
-
-            Lists all versions and write them into html chart file `chart.html`::
-
-                $ s3lsvers -html-file chart.html bucketname/keyname
-
-        Using bucket/key_name aliases in .s3lsvers file
-
-            Aliases are specified in file .s3lsvers, which may be located in
-            currect directory, home directory or /etc/s3lsvers"
-
-            `.s3lsvers` example::
-
-                #.s3lsversrc - definition of some preconfigured bucket/key values
-                [DEFAULT]
-                pl-base: pl-base.dp.tamtamresearch.com
-                cz-base: cz-base.dp.tamtamresearch.com
-
-                # alias name must not contain "/"
-                [aliases]
-                plcsr: %(pl-base)s/region/pl/ConsumerServiceReady.xml
-                czcsr: %(cz-base)s/region/cz/ConsumerServiceReady.xml
-
-            The format follows SafeConfigParser rules, see
-            http://docs.python.org/2/library/configparser.html#safeconfigparser-objects
-
-            To list all versions of czcsr alias::
-
-                $ s3lsvers czcsr
-
-
-    positional arguments:
-      bucket_key            {bucket_name}/{key_name} for the key to list
-
-    optional arguments:
-      -h, --help            show this help message and exit
-      -from None, --from-time None
-                            start of version modification time range (default:
-                            oldest version)
-      -to None, --to-time None
-                            end of version modification time range (default: now)
-      -list-file None       Name of output CSV file.
-      -html-file None       Name of output HTML file.
-      -version-id None      version-id to start after
-      -profile-name None    AWSCLI profile name
-      -aws-access-key-id None
-                            AWS Access Key ID
-      -aws-secret-access-key None
-                            AWS Secret Access Key
-
-s3getvers
----------
-::
-
-    $ s3getvers -h
-    usage: s3getvers [-h] [-output-version-id-names] [-no-decompression]
-                     [-profile-name None] [-aws-access-key-id None]
-                     [-aws-secret-access-key None]
-                     bucket_name csv_version_file
-
-    Fetch S3 object versions as listed in a csv file
-
-        Typical csv file (as by default produced by s3lsvers) is:
-
-            m/y.xml;OrUr6XO8KSKEHbd8mQ.MloGcGlsh7Sir;191;2012-05-23T20:45:10.000Z;39
-            m/y.xml;xhkVOy.dJfjSfUwse8tsieqjDicp0owq;192;2012-05-23T20:44:31.000Z;62
-            m/y.xml;oKneK.N2wS8pW8.EmLqjldYlgcFwxN3V;193;2012-05-23T20:43:29.000Z;58
-
-        for `s3getvers` only the first two columns are significant:
-        :key_name: name of the object (not containing the bucket name itself)
-        :version_id: string, identifying unique version.
-
-        Typical use (assuming, above csv file is available under name verlist.csv)::
-
-            $ s3getvers yourbucketname verlist.csv
-
-        What will create following files in current directory:
-
-        * f.2012-05-23T20_45_10.xml
-        * f.2012-05-23T20_44_31.xml
-        * f.2012-05-23T20_43_29.xml
-
-        Files are (by default) saved decompressed (even if gzipped on the bucket)
-
-
-    positional arguments:
-      bucket_name           bucket name (default: None)
-      csv_version_file      name of CSV file with version_id
-
-    optional arguments:
-      -h, --help            show this help message and exit
-      -output-version-id-names
-                            Resulting file names shall use version_id to become
-                            distinguished (default is to use timestamp of file
-                            creation)
-      -no-decompression     Keeps the files as they come, do not decompress, if
-                            they come compressed
-      -profile-name None    Name of AWSCLI profile to use for credentials
-      -aws-access-key-id None
-                            Your AWS Access Key ID
-      -aws-secret-access-key None
-                            Your AWS Secret Access Key
-
-s3tmpgen
---------
-
-
-::
-
-  $ s3tmpgen -h
-  usage: s3tmpgen [-h] [-profile-name None] [-aws-access-key-id None] [-aws-secret-access-key None] [-validate-bucket] [-validate-key] [-http] expire_dt bucket_name [key_names [key_names ...]]
-
-  Generate temporary url for accessing content of AWS S3 key.
-
-      Temporary url includes expiration time, after which it rejects serving the
-      content.
-
-      Urls are printed one per line to stdout.
-
-      For missing key names empty line is printed and error goes to stderr.
-
-      If the bucket is versioned, tmp url will serve the latest version
-      at the moment of request (version_id is not part of generated url).
-
-      By default, bucket and key name existnence is not verified.
-
-      Url is using https, unless `-http` is used.
-    
-
-  positional arguments:
-    expire_dt             ISO formatted time of expiration, full seconds, 'Z' is obligatory, e.g. '2014-02-14T21:47:16Z'
-    bucket_name           name of bucket
-    key_names             key names to generate tmpurl for
-
-  optional arguments:
-    -h, --help            show this help message and exit
-    -profile-name None    Name of AWSCLI profile to use for credentials
-    -aws-access-key-id None
-                          Your AWS Access Key ID
-    -aws-secret-access-key None
-                          Your AWS Secret Access Key
-    -validate-bucket      Make sure, the bucket really exists
-    -validate-key         Make sure, the key really exists
-    -http                 Force the url to use http and not https
-  
-
-Configuring AWS S3 credentials
-==============================
-
-Configure the credentials as you would do for using AWS CLI.
-
-If you configure profiles, you may use switch `-profile` when calling the commands.
-
-
-.. _AWS: http://aws.amazon.com/
-.. _S3: http://aws.amazon.com/s3/
-.. _versioning: http://aws.amazon.com/about-aws/whats-new/2010/02/08/versioning-feature-for-amazon-s3-now-available/
-.. _AWS_config: http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html
+============
+AWS Utils S3
+============
+
+Tools to list and fetch objects from versioned AWS_ S3_ bucket:
+
+* `s3lsvers`: List object versions, see versioning_
+* `s3getvers`: Fetch specified object versions
+* `s3tmpgen`: Generate temporary url links to objects
+
+.. contents:: Table of Contents
+
+Installation
+============
+Using `pip`::
+
+  $ pip install ttr.aws.utils.s3
+
+Using `pipx`::
+
+  $ pipx install ttr.aws.utils.s3
+    
+Quick start
+===========
+We want to fetch versions of feed in bucket `mybucket` named `my/versioned/feed.xml`
+
+1. Configure AWSCLI credentials to allow access to your buckets and objects. E.g. using `AWS_DEFAULT_PROFILE`. See AWS_config_.
+
+2. create csv file for given feed and time period::
+
+    $ s3lsvers -from 2012-05-24T00:15 -to 2012-05-24T01:15 -list-file list.csv mybucket/my/versioned/feed.xml
+
+   You shall then find file `list.csv` on your disk.
+
+3. Review records in `list.csv` and delete all lines with version, which are not of your interest.
+
+4. Using `list.csv`, ask s3getvers to fetch all versions specified in the file. Be sure to run it on empty directory::
+
+    $ s3getvers mybucket list.csv
+
+   You will see, how is each version downloaded and saved to your current directory.
+
+5. Finally, you can try generating temorary url to your feed (showing the latest existing)::
+
+    $ s3tmpgen 2014-09-30T00:00:00Z mybucket my/versioned/feed.xml
+    https://mybucket.s3.amazonaws.com/my/versioned/feed.xml?Signature=kOCwz%2FkanVWX8O15dlXhy4jrbwY%3D&Expires=1412031600&AWSAccessKeyId=AKIAxyzxyzxyzEQA
+
+   Note, that the url does not include VersionId, so it will always point to the most up todate version (in case the key happens to be on versioned bucket).
+
+Provided commands
+=================
+
+s3lsvers
+--------
+List versions of some feed. Could output into CSV file (-list-file) and/or html chart (-html-file).::
+
+    $ s3lsvers -h
+    usage: s3lsvers [-h] [-from None] [-to None] [-list-file None]
+                    [-html-file None] [-version-id None] [-profile-name None]
+                    [-aws-access-key-id None] [-aws-secret-access-key None]
+                    bucket_key
+
+    List object versions stored on versioned S3 bucket, create CSV and/or HTML file.
+        CSV file can be used e.g. by `s3getvers` command.
+        HTML file allows showing feed size and update period in chart.
+
+        Version can be limited by time range `from` - `to`.
+        `version-id` allow starting from specific version (back to the past,
+        excluding given version).
+
+        Object key is defined either as {bucket_name}/{key_name} or as alias from .s3lsvers file.
+
+        Times are expressed in RFC 3339 format using Zulu (UTC) timezone, possibly truncated.
+        For truncated time strings, maximal time extent is used.
+
+        Listing has records with structure:
+          `{key_name};{version_id};{size};{last_modified};{age}`
+            - key_name: name of the key (excluding bucket name).
+            - version_id: unique identifier for given version on given bucket.
+            - size: size of key object in bytes
+            - last_modified: RFC 3339 formated object modification time
+            - age: update interval [s] for given version
+
+        Examples:
+
+            Lists all versions of given `keyname` on `bucket`::
+
+                $ s3lsvers bucketname/keyname
+
+            Lists all versions in period betwen `from` and `to` time::
+
+                $ s3lsvers -from 2010-01-01 -to 2011-07-19T12:00:00 bucket/key
+
+            Lists all versions and writes them into csv file named `versions.csv`::
+
+                $ s3lsvers -list-file versions.csv bucketname/keyname
+
+            Lists all versions and write them into html chart file `chart.html`::
+
+                $ s3lsvers -html-file chart.html bucketname/keyname
+
+        Using bucket/key_name aliases in .s3lsvers file
+
+            Aliases are specified in file .s3lsvers, which may be located in
+            currect directory, home directory or /etc/s3lsvers"
+
+            `.s3lsvers` example::
+
+                #.s3lsversrc - definition of some preconfigured bucket/key values
+                [DEFAULT]
+                pl-base: pl-base.dp.tamtamresearch.com
+                cz-base: cz-base.dp.tamtamresearch.com
+
+                # alias name must not contain "/"
+                [aliases]
+                plcsr: %(pl-base)s/region/pl/ConsumerServiceReady.xml
+                czcsr: %(cz-base)s/region/cz/ConsumerServiceReady.xml
+
+            The format follows SafeConfigParser rules, see
+            http://docs.python.org/2/library/configparser.html#safeconfigparser-objects
+
+            To list all versions of czcsr alias::
+
+                $ s3lsvers czcsr
+
+
+    positional arguments:
+      bucket_key            {bucket_name}/{key_name} for the key to list
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      -from None, --from-time None
+                            start of version modification time range (default:
+                            oldest version)
+      -to None, --to-time None
+                            end of version modification time range (default: now)
+      -list-file None       Name of output CSV file.
+      -html-file None       Name of output HTML file.
+      -version-id None      version-id to start after
+      -profile-name None    AWSCLI profile name
+      -aws-access-key-id None
+                            AWS Access Key ID
+      -aws-secret-access-key None
+                            AWS Secret Access Key
+
+s3getvers
+---------
+::
+
+    $ s3getvers -h
+    usage: s3getvers [-h] [-output-version-id-names] [-no-decompression]
+                     [-profile-name None] [-aws-access-key-id None]
+                     [-aws-secret-access-key None]
+                     bucket_name csv_version_file
+
+    Fetch S3 object versions as listed in a csv file
+
+        Typical csv file (as by default produced by s3lsvers) is:
+
+            m/y.xml;OrUr6XO8KSKEHbd8mQ.MloGcGlsh7Sir;191;2012-05-23T20:45:10.000Z;39
+            m/y.xml;xhkVOy.dJfjSfUwse8tsieqjDicp0owq;192;2012-05-23T20:44:31.000Z;62
+            m/y.xml;oKneK.N2wS8pW8.EmLqjldYlgcFwxN3V;193;2012-05-23T20:43:29.000Z;58
+
+        for `s3getvers` only the first two columns are significant:
+        :key_name: name of the object (not containing the bucket name itself)
+        :version_id: string, identifying unique version.
+
+        Typical use (assuming, above csv file is available under name verlist.csv)::
+
+            $ s3getvers yourbucketname verlist.csv
+
+        What will create following files in current directory:
+
+        * f.2012-05-23T20_45_10.xml
+        * f.2012-05-23T20_44_31.xml
+        * f.2012-05-23T20_43_29.xml
+
+        Files are (by default) saved decompressed (even if gzipped on the bucket)
+
+
+    positional arguments:
+      bucket_name           bucket name (default: None)
+      csv_version_file      name of CSV file with version_id
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      -output-version-id-names
+                            Resulting file names shall use version_id to become
+                            distinguished (default is to use timestamp of file
+                            creation)
+      -no-decompression     Keeps the files as they come, do not decompress, if
+                            they come compressed
+      -profile-name None    Name of AWSCLI profile to use for credentials
+      -aws-access-key-id None
+                            Your AWS Access Key ID
+      -aws-secret-access-key None
+                            Your AWS Secret Access Key
+
+s3tmpgen
+--------
+
+
+::
+
+  $ s3tmpgen -h
+  usage: s3tmpgen [-h] [-profile-name None] [-aws-access-key-id None] [-aws-secret-access-key None] [-validate-bucket] [-validate-key] [-http] expire_dt bucket_name [key_names [key_names ...]]
+
+  Generate temporary url for accessing content of AWS S3 key.
+
+      Temporary url includes expiration time, after which it rejects serving the
+      content.
+
+      Urls are printed one per line to stdout.
+
+      For missing key names empty line is printed and error goes to stderr.
+
+      If the bucket is versioned, tmp url will serve the latest version
+      at the moment of request (version_id is not part of generated url).
+
+      By default, bucket and key name existnence is not verified.
+
+      Url is using https, unless `-http` is used.
+    
+
+  positional arguments:
+    expire_dt             ISO formatted time of expiration, full seconds, 'Z' is obligatory, e.g. '2014-02-14T21:47:16Z'
+    bucket_name           name of bucket
+    key_names             key names to generate tmpurl for
+
+  optional arguments:
+    -h, --help            show this help message and exit
+    -profile-name None    Name of AWSCLI profile to use for credentials
+    -aws-access-key-id None
+                          Your AWS Access Key ID
+    -aws-secret-access-key None
+                          Your AWS Secret Access Key
+    -validate-bucket      Make sure, the bucket really exists
+    -validate-key         Make sure, the key really exists
+    -http                 Force the url to use http and not https
+  
+
+Configuring AWS S3 credentials
+==============================
+
+Configure the credentials as you would do for using AWS CLI.
+
+If you configure profiles, you may use switch `-profile` when calling the commands.
+
+
+.. _AWS: http://aws.amazon.com/
+.. _S3: http://aws.amazon.com/s3/
+.. _versioning: http://aws.amazon.com/about-aws/whats-new/2010/02/08/versioning-feature-for-amazon-s3-now-available/
+.. _AWS_config: http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html
```

