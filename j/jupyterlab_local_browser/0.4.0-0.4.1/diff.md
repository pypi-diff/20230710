# Comparing `tmp/jupyterlab_local_browser-0.4.0.tar.gz` & `tmp/jupyterlab_local_browser-0.4.1.tar.gz`

## Comparing `jupyterlab_local_browser-0.4.0.tar` & `jupyterlab_local_browser-0.4.1.tar`

### file list

```diff
@@ -1,247 +1,247 @@
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/.copier-answers.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/RELEASE.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/Untitled.ipynb
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/babel.config.js
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jest.config.js
--rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/tsconfig.test.json
--rw-r--r--   0        0        0   356177 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/yarn.lock
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/_version.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/config.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/handlers.py
--rw-r--r--   0        0        0    21962 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/build_log.json
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/package.json
--rw-r--r--   0        0        0    14109 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0260d483d18d1b5881ab.js
--rw-r--r--   0        0        0    18058 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0260d483d18d1b5881ab.js.map
--rw-r--r--   0        0        0    16875 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0531ad9081f3b9910023.js
--rw-r--r--   0        0        0    20547 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0531ad9081f3b9910023.js.map
--rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.097dbaec2b4b7ab6bed1.js
--rw-r--r--   0        0        0    17991 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.097dbaec2b4b7ab6bed1.js.map
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0ae1bbc988abd77d7ce5.js
--rw-r--r--   0        0        0    19245 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0ae1bbc988abd77d7ce5.js.map
--rw-r--r--   0        0        0    17051 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.11db783c3fe24b6adc52.js
--rw-r--r--   0        0        0    20639 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.11db783c3fe24b6adc52.js.map
--rw-r--r--   0        0        0    14604 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.2f4a309cfaf1e44ea829.js
--rw-r--r--   0        0        0    19356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.2f4a309cfaf1e44ea829.js.map
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.30767f8725ca18bf459f.js
--rw-r--r--   0        0        0    18055 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.30767f8725ca18bf459f.js.map
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3885651e14bde39816d2.js
--rw-r--r--   0        0        0    18125 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3885651e14bde39816d2.js.map
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.38c8a7ef7cc34da00151.js
--rw-r--r--   0        0        0    18054 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.38c8a7ef7cc34da00151.js.map
--rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.393a277a4fd7125de295.js
--rw-r--r--   0        0        0    19445 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.393a277a4fd7125de295.js.map
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3c902412ec6167e454d2.js
--rw-r--r--   0        0        0    17972 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3c902412ec6167e454d2.js.map
--rw-r--r--   0        0        0    16444 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3cf287e5014b860e7ce4.js
--rw-r--r--   0        0        0    19691 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3cf287e5014b860e7ce4.js.map
--rw-r--r--   0        0        0    13984 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3e869e2d783bda32e86f.js
--rw-r--r--   0        0        0    17933 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3e869e2d783bda32e86f.js.map
--rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.44a50b4bec1243752537.js
--rw-r--r--   0        0        0    19632 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.44a50b4bec1243752537.js.map
--rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.45fac8fc3fc216764524.js
--rw-r--r--   0        0        0    20369 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.45fac8fc3fc216764524.js.map
--rw-r--r--   0        0        0    15591 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.467c52c0a48ceec9af7f.js
--rw-r--r--   0        0        0    19203 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.467c52c0a48ceec9af7f.js.map
--rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.478e2e857c30ab96296c.js
--rw-r--r--   0        0        0    18056 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.478e2e857c30ab96296c.js.map
--rw-r--r--   0        0        0    14211 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.482abf9339c01e5ba6c3.js
--rw-r--r--   0        0        0    17970 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.482abf9339c01e5ba6c3.js.map
--rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.48f290893b0d30b5c3f0.js
--rw-r--r--   0        0        0    19312 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.48f290893b0d30b5c3f0.js.map
--rw-r--r--   0        0        0    14563 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.4b5c73e1630f9c00d4b2.js
--rw-r--r--   0        0        0    18130 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.4b5c73e1630f9c00d4b2.js.map
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.515127fe21ef0f56a907.js
--rw-r--r--   0        0        0    19174 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.515127fe21ef0f56a907.js.map
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.581ab39f2e283a14aff7.js
--rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.581ab39f2e283a14aff7.js.map
--rw-r--r--   0        0        0    15041 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.664d52f84dba6d28ccf0.js
--rw-r--r--   0        0        0    19425 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.664d52f84dba6d28ccf0.js.map
--rw-r--r--   0        0        0    16802 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.66e30c2a4a85c03b58d9.js
--rw-r--r--   0        0        0    20364 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.66e30c2a4a85c03b58d9.js.map
--rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.6aa9131c23b373442af2.js
--rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.6aa9131c23b373442af2.js.map
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.6abf9ea20ee1c9c1dd6f.js
--rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.6abf9ea20ee1c9c1dd6f.js.map
--rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.7df68cc0bacbddb1774d.js
--rw-r--r--   0        0        0    19469 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.7df68cc0bacbddb1774d.js.map
--rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.7ebea98f752cde807697.js
--rw-r--r--   0        0        0    20585 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.7ebea98f752cde807697.js.map
--rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.8326cb8f3e2d1fd7e623.js
--rw-r--r--   0        0        0    19515 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.8326cb8f3e2d1fd7e623.js.map
--rw-r--r--   0        0        0    14211 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.861dea7bc7cb5f82903a.js
--rw-r--r--   0        0        0    17844 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.861dea7bc7cb5f82903a.js.map
--rw-r--r--   0        0        0    17051 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.8b369c4134033ffa5d52.js
--rw-r--r--   0        0        0    20550 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.8b369c4134033ffa5d52.js.map
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.9542c477b3765627ab36.js
--rw-r--r--   0        0        0    18014 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.9542c477b3765627ab36.js.map
--rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.99c52d2c6cf45f5e1f51.js
--rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.99c52d2c6cf45f5e1f51.js.map
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.9dfef7c94aafde75de43.js
--rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.9dfef7c94aafde75de43.js.map
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a0e6bae1dbf4e86bcdbe.js
--rw-r--r--   0        0        0    18045 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a0e6bae1dbf4e86bcdbe.js.map
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a219bfe4543e8c82a94a.js
--rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a219bfe4543e8c82a94a.js.map
--rw-r--r--   0        0        0    14109 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2370edcbfff0500a30c.js
--rw-r--r--   0        0        0    18048 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2370edcbfff0500a30c.js.map
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2b3b95e9ca37fdc24ab.js
--rw-r--r--   0        0        0    18090 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2b3b95e9ca37fdc24ab.js.map
--rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2c1b9df84931a8ef1cc.js
--rw-r--r--   0        0        0    18157 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2c1b9df84931a8ef1cc.js.map
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a31e48eff904a48bc2e4.js
--rw-r--r--   0        0        0    19058 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a31e48eff904a48bc2e4.js.map
--rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a518ab3a6e4d545b32ca.js
--rw-r--r--   0        0        0    19599 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a518ab3a6e4d545b32ca.js.map
--rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a535319a6e809944b995.js
--rw-r--r--   0        0        0    19520 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a535319a6e809944b995.js.map
--rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a60c60cdc4ea8d93e28c.js
--rw-r--r--   0        0        0    19579 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a60c60cdc4ea8d93e28c.js.map
--rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a75e33608a1ff124aac3.js
--rw-r--r--   0        0        0    20414 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a75e33608a1ff124aac3.js.map
--rw-r--r--   0        0        0    16858 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a7f7c111f8e36e37204b.js
--rw-r--r--   0        0        0    20471 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a7f7c111f8e36e37204b.js.map
--rw-r--r--   0        0        0    14462 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b40be2f2583322a7a84d.js
--rw-r--r--   0        0        0    19144 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b40be2f2583322a7a84d.js.map
--rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b40c42a822c1acaafe61.js
--rw-r--r--   0        0        0    19483 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b40c42a822c1acaafe61.js.map
--rw-r--r--   0        0        0    16802 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b6383d5778cb49254d99.js
--rw-r--r--   0        0        0    20368 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b6383d5778cb49254d99.js.map
--rw-r--r--   0        0        0    16875 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b79e606c604dff28cb73.js
--rw-r--r--   0        0        0    20583 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b79e606c604dff28cb73.js.map
--rw-r--r--   0        0        0    14604 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.bd37de52b78466a4f5d4.js
--rw-r--r--   0        0        0    19414 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.bd37de52b78466a4f5d4.js.map
--rw-r--r--   0        0        0    14462 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.bfbe76f93ff87e72e8d5.js
--rw-r--r--   0        0        0    19227 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.bfbe76f93ff87e72e8d5.js.map
--rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.c7e82623d55ff4a2402b.js
--rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.c7e82623d55ff4a2402b.js.map
--rw-r--r--   0        0        0    14563 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d0df2c2c41c52ce5e6bf.js
--rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d0df2c2c41c52ce5e6bf.js.map
--rw-r--r--   0        0        0    13984 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d1d9356b9fda6e7696e8.js
--rw-r--r--   0        0        0    17939 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d1d9356b9fda6e7696e8.js.map
--rw-r--r--   0        0        0    14563 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d4e0dbdaa229184ab605.js
--rw-r--r--   0        0        0    18132 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d4e0dbdaa229184ab605.js.map
--rw-r--r--   0        0        0    15591 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d8d5eef5f577cf52ed2e.js
--rw-r--r--   0        0        0    18165 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d8d5eef5f577cf52ed2e.js.map
--rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.dac0e43082d308e0e490.js
--rw-r--r--   0        0        0    19599 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.dac0e43082d308e0e490.js.map
--rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.deec7b1a19e037c57782.js
--rw-r--r--   0        0        0    18025 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.deec7b1a19e037c57782.js.map
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e1f82fcdb1df57164b69.js
--rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e1f82fcdb1df57164b69.js.map
--rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e2381d09a8797b4febd2.js
--rw-r--r--   0        0        0    19654 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e2381d09a8797b4febd2.js.map
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e2580aaee693c29e07cb.js
--rw-r--r--   0        0        0    18056 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e2580aaee693c29e07cb.js.map
--rw-r--r--   0        0        0    17188 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e8530757b556bf028152.js
--rw-r--r--   0        0        0    20706 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e8530757b556bf028152.js.map
--rw-r--r--   0        0        0    13984 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e9225fce3da73baaa974.js
--rw-r--r--   0        0        0    17911 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e9225fce3da73baaa974.js.map
--rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e9ea030b4a00ebbcf710.js
--rw-r--r--   0        0        0    19336 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e9ea030b4a00ebbcf710.js.map
--rw-r--r--   0        0        0    16926 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f23e1e8e2f15f4973b4d.js
--rw-r--r--   0        0        0    20391 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f23e1e8e2f15f4973b4d.js.map
--rw-r--r--   0        0        0    16434 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f8edc82fc51b7640b290.js
--rw-r--r--   0        0        0    19679 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f8edc82fc51b7640b290.js.map
--rw-r--r--   0        0        0    14563 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f94f1cfa271c209d2015.js
--rw-r--r--   0        0        0    18157 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f94f1cfa271c209d2015.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.059a5ab6fa0d40dc2ec5.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.05cdb0e2d59ddf299c2d.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.09954ab8aac77ff30097.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.158e6dc4043218c5fd93.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.192da90950725b39b157.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.1a998993d84da7b0a455.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.23e4fe60cdea9dc96d93.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.2e7b0d7b4fb0ed4dae07.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.30a762e9c23bdc35e52e.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.35249e44af8d1f7377c0.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.3842d1844bc92ce96c88.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.38bce3ca0ff07fde40d7.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.38bced12d1b42c4c1a31.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.3c2b1e1171eb58df862a.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.3e26fc8afccac357e6be.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.3e5cc4a2b41e91b597ab.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.3e9eac384c105b303e79.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.4312b39770d43fd0d656.js.map
--rw-r--r--   0        0        0    29704 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.431464fdcb2b990c3b1a.js
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.431464fdcb2b990c3b1a.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.4558ccb53085fe45df87.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.53de14fff371a123d029.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.5849cb718fc52ee6df46.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.5a10e773711543bda859.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.5ac71cfa716a71c030d6.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.5e9875f82a3ad5f97952.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.5f57ce37214d4953598d.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.6042c480082a224a48b9.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.643577e67810f43714a8.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.66304c18bf3697d2473c.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.66ffd46a03333ee56a42.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.69cb0d28c6d4f2854af1.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.75c1ff3819927bdbf902.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.766ed606d07a8b832abc.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.7acd16813491fa0ff615.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.7ba614e2875b1e9680ff.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.800679a3fe495198cfd2.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.82d9bc0bc37152ea73c7.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.84ceea7b4267012e84c7.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.86707e8d7112b13cc3ad.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.87cc3741e1b6de69aa89.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.8ecf538fde2ccfcf33fb.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.9f0a2eefe7aadb15ae41.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.a98bc4ff5170118ea64a.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.ab1975ca0d1b9df1f91b.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.b084e69afb14892a975c.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.b20eaff3587d6b3ac566.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.b75b1ac5e362e0ae72d6.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.bd557903020a2b46b920.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.bd670e7ca8849267ece7.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.c151b05f5da9fabb7410.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.c1f7ed49e666074234d9.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.c59ecde72df993d90563.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.c9fb1eac6c2c9fedd03a.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.d2fd8a3c468010c8e1a1.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.d80e408bab17a43c87c2.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.dcc6b30986c6497bca3c.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.dda78c3c2459e905f54c.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.de590b3308b7618cc4d7.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.e276b399887d08c35e71.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.e37bcd7c63c6418dfbb3.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.eda5332dafec41590e5b.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.f5c4021326e0456459a2.js.map
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.f5e261b210e647b2d4ba.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.f6f75a2ce44969d92c2c.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.f7bdba3f4581ac7e4ce9.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.fb4a4b567bf481c1d484.js.map
--rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.fe2870f0697685b06781.js.map
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/style.js
--rw-r--r--   0        0        0    19365 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/style_index_js.9cf61c47582680994e2f.js
--rw-r--r--   0        0        0    14835 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/style_index_js.9cf61c47582680994e2f.js.map
--rw-r--r--   0        0        0    33772 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.f87f93d906d92e4f7101.js
--rw-r--r--   0        0        0    25770 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.f87f93d906d92e4f7101.js.map
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/public/index.html
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/public/styles.css
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/src/icon.ts
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/src/index.ts
--rw-r--r--   0        0        0     7887 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/src/widget.tsx
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/src/__tests__/jupyterlab_local_browser.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/style/index.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/ui-tests/tests/jupyterlab_local_browser.spec.ts
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/LICENSE
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/README.md
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/.copier-answers.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/RELEASE.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/Untitled.ipynb
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/babel.config.js
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jest.config.js
+-rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/tsconfig.test.json
+-rw-r--r--   0        0        0   356177 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/yarn.lock
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/_version.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/config.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/handlers.py
+-rw-r--r--   0        0        0    21962 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/build_log.json
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/package.json
+-rw-r--r--   0        0        0    14109 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0260d483d18d1b5881ab.js
+-rw-r--r--   0        0        0    18058 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0260d483d18d1b5881ab.js.map
+-rw-r--r--   0        0        0    16875 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0531ad9081f3b9910023.js
+-rw-r--r--   0        0        0    20547 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0531ad9081f3b9910023.js.map
+-rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.097dbaec2b4b7ab6bed1.js
+-rw-r--r--   0        0        0    17991 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.097dbaec2b4b7ab6bed1.js.map
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0ae1bbc988abd77d7ce5.js
+-rw-r--r--   0        0        0    19245 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0ae1bbc988abd77d7ce5.js.map
+-rw-r--r--   0        0        0    17051 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.11db783c3fe24b6adc52.js
+-rw-r--r--   0        0        0    20639 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.11db783c3fe24b6adc52.js.map
+-rw-r--r--   0        0        0    14604 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.2f4a309cfaf1e44ea829.js
+-rw-r--r--   0        0        0    19356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.2f4a309cfaf1e44ea829.js.map
+-rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.30767f8725ca18bf459f.js
+-rw-r--r--   0        0        0    18055 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.30767f8725ca18bf459f.js.map
+-rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3885651e14bde39816d2.js
+-rw-r--r--   0        0        0    18125 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3885651e14bde39816d2.js.map
+-rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.38c8a7ef7cc34da00151.js
+-rw-r--r--   0        0        0    18054 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.38c8a7ef7cc34da00151.js.map
+-rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.393a277a4fd7125de295.js
+-rw-r--r--   0        0        0    19445 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.393a277a4fd7125de295.js.map
+-rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3c902412ec6167e454d2.js
+-rw-r--r--   0        0        0    17972 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3c902412ec6167e454d2.js.map
+-rw-r--r--   0        0        0    16444 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3cf287e5014b860e7ce4.js
+-rw-r--r--   0        0        0    19691 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3cf287e5014b860e7ce4.js.map
+-rw-r--r--   0        0        0    13984 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3e869e2d783bda32e86f.js
+-rw-r--r--   0        0        0    17933 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3e869e2d783bda32e86f.js.map
+-rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.44a50b4bec1243752537.js
+-rw-r--r--   0        0        0    19632 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.44a50b4bec1243752537.js.map
+-rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.45fac8fc3fc216764524.js
+-rw-r--r--   0        0        0    20369 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.45fac8fc3fc216764524.js.map
+-rw-r--r--   0        0        0    15591 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.467c52c0a48ceec9af7f.js
+-rw-r--r--   0        0        0    19203 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.467c52c0a48ceec9af7f.js.map
+-rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.478e2e857c30ab96296c.js
+-rw-r--r--   0        0        0    18056 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.478e2e857c30ab96296c.js.map
+-rw-r--r--   0        0        0    14211 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.482abf9339c01e5ba6c3.js
+-rw-r--r--   0        0        0    17970 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.482abf9339c01e5ba6c3.js.map
+-rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.48f290893b0d30b5c3f0.js
+-rw-r--r--   0        0        0    19312 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.48f290893b0d30b5c3f0.js.map
+-rw-r--r--   0        0        0    14563 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.4b5c73e1630f9c00d4b2.js
+-rw-r--r--   0        0        0    18130 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.4b5c73e1630f9c00d4b2.js.map
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.515127fe21ef0f56a907.js
+-rw-r--r--   0        0        0    19174 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.515127fe21ef0f56a907.js.map
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.581ab39f2e283a14aff7.js
+-rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.581ab39f2e283a14aff7.js.map
+-rw-r--r--   0        0        0    15041 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.664d52f84dba6d28ccf0.js
+-rw-r--r--   0        0        0    19425 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.664d52f84dba6d28ccf0.js.map
+-rw-r--r--   0        0        0    16802 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.66e30c2a4a85c03b58d9.js
+-rw-r--r--   0        0        0    20364 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.66e30c2a4a85c03b58d9.js.map
+-rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.6aa9131c23b373442af2.js
+-rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.6aa9131c23b373442af2.js.map
+-rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.6abf9ea20ee1c9c1dd6f.js
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.6abf9ea20ee1c9c1dd6f.js.map
+-rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.7df68cc0bacbddb1774d.js
+-rw-r--r--   0        0        0    19469 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.7df68cc0bacbddb1774d.js.map
+-rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.7ebea98f752cde807697.js
+-rw-r--r--   0        0        0    20585 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.7ebea98f752cde807697.js.map
+-rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.8326cb8f3e2d1fd7e623.js
+-rw-r--r--   0        0        0    19515 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.8326cb8f3e2d1fd7e623.js.map
+-rw-r--r--   0        0        0    14211 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.861dea7bc7cb5f82903a.js
+-rw-r--r--   0        0        0    17844 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.861dea7bc7cb5f82903a.js.map
+-rw-r--r--   0        0        0    17051 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.8b369c4134033ffa5d52.js
+-rw-r--r--   0        0        0    20550 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.8b369c4134033ffa5d52.js.map
+-rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.9542c477b3765627ab36.js
+-rw-r--r--   0        0        0    18014 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.9542c477b3765627ab36.js.map
+-rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.99c52d2c6cf45f5e1f51.js
+-rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.99c52d2c6cf45f5e1f51.js.map
+-rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.9dfef7c94aafde75de43.js
+-rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.9dfef7c94aafde75de43.js.map
+-rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a0e6bae1dbf4e86bcdbe.js
+-rw-r--r--   0        0        0    18045 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a0e6bae1dbf4e86bcdbe.js.map
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a219bfe4543e8c82a94a.js
+-rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a219bfe4543e8c82a94a.js.map
+-rw-r--r--   0        0        0    14109 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2370edcbfff0500a30c.js
+-rw-r--r--   0        0        0    18048 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2370edcbfff0500a30c.js.map
+-rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2b3b95e9ca37fdc24ab.js
+-rw-r--r--   0        0        0    18090 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2b3b95e9ca37fdc24ab.js.map
+-rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2c1b9df84931a8ef1cc.js
+-rw-r--r--   0        0        0    18157 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2c1b9df84931a8ef1cc.js.map
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a31e48eff904a48bc2e4.js
+-rw-r--r--   0        0        0    19058 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a31e48eff904a48bc2e4.js.map
+-rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a518ab3a6e4d545b32ca.js
+-rw-r--r--   0        0        0    19599 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a518ab3a6e4d545b32ca.js.map
+-rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a535319a6e809944b995.js
+-rw-r--r--   0        0        0    19520 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a535319a6e809944b995.js.map
+-rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a60c60cdc4ea8d93e28c.js
+-rw-r--r--   0        0        0    19579 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a60c60cdc4ea8d93e28c.js.map
+-rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a75e33608a1ff124aac3.js
+-rw-r--r--   0        0        0    20414 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a75e33608a1ff124aac3.js.map
+-rw-r--r--   0        0        0    16858 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a7f7c111f8e36e37204b.js
+-rw-r--r--   0        0        0    20471 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a7f7c111f8e36e37204b.js.map
+-rw-r--r--   0        0        0    14462 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b40be2f2583322a7a84d.js
+-rw-r--r--   0        0        0    19144 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b40be2f2583322a7a84d.js.map
+-rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b40c42a822c1acaafe61.js
+-rw-r--r--   0        0        0    19483 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b40c42a822c1acaafe61.js.map
+-rw-r--r--   0        0        0    16802 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b6383d5778cb49254d99.js
+-rw-r--r--   0        0        0    20368 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b6383d5778cb49254d99.js.map
+-rw-r--r--   0        0        0    16875 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b79e606c604dff28cb73.js
+-rw-r--r--   0        0        0    20583 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b79e606c604dff28cb73.js.map
+-rw-r--r--   0        0        0    14604 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.bd37de52b78466a4f5d4.js
+-rw-r--r--   0        0        0    19414 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.bd37de52b78466a4f5d4.js.map
+-rw-r--r--   0        0        0    14462 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.bfbe76f93ff87e72e8d5.js
+-rw-r--r--   0        0        0    19227 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.bfbe76f93ff87e72e8d5.js.map
+-rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.c7e82623d55ff4a2402b.js
+-rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.c7e82623d55ff4a2402b.js.map
+-rw-r--r--   0        0        0    14563 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d0df2c2c41c52ce5e6bf.js
+-rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d0df2c2c41c52ce5e6bf.js.map
+-rw-r--r--   0        0        0    13984 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d1d9356b9fda6e7696e8.js
+-rw-r--r--   0        0        0    17939 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d1d9356b9fda6e7696e8.js.map
+-rw-r--r--   0        0        0    14563 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d4e0dbdaa229184ab605.js
+-rw-r--r--   0        0        0    18132 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d4e0dbdaa229184ab605.js.map
+-rw-r--r--   0        0        0    15591 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d8d5eef5f577cf52ed2e.js
+-rw-r--r--   0        0        0    18165 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d8d5eef5f577cf52ed2e.js.map
+-rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.dac0e43082d308e0e490.js
+-rw-r--r--   0        0        0    19599 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.dac0e43082d308e0e490.js.map
+-rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.deec7b1a19e037c57782.js
+-rw-r--r--   0        0        0    18025 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.deec7b1a19e037c57782.js.map
+-rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e1f82fcdb1df57164b69.js
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e1f82fcdb1df57164b69.js.map
+-rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e2381d09a8797b4febd2.js
+-rw-r--r--   0        0        0    19654 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e2381d09a8797b4febd2.js.map
+-rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e2580aaee693c29e07cb.js
+-rw-r--r--   0        0        0    18056 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e2580aaee693c29e07cb.js.map
+-rw-r--r--   0        0        0    17188 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e8530757b556bf028152.js
+-rw-r--r--   0        0        0    20706 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e8530757b556bf028152.js.map
+-rw-r--r--   0        0        0    13984 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e9225fce3da73baaa974.js
+-rw-r--r--   0        0        0    17911 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e9225fce3da73baaa974.js.map
+-rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e9ea030b4a00ebbcf710.js
+-rw-r--r--   0        0        0    19336 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e9ea030b4a00ebbcf710.js.map
+-rw-r--r--   0        0        0    16926 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f23e1e8e2f15f4973b4d.js
+-rw-r--r--   0        0        0    20391 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f23e1e8e2f15f4973b4d.js.map
+-rw-r--r--   0        0        0    16434 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f8edc82fc51b7640b290.js
+-rw-r--r--   0        0        0    19679 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f8edc82fc51b7640b290.js.map
+-rw-r--r--   0        0        0    14563 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f94f1cfa271c209d2015.js
+-rw-r--r--   0        0        0    18157 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f94f1cfa271c209d2015.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.059a5ab6fa0d40dc2ec5.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.05cdb0e2d59ddf299c2d.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.09954ab8aac77ff30097.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.158e6dc4043218c5fd93.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.192da90950725b39b157.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.1a998993d84da7b0a455.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.23e4fe60cdea9dc96d93.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.2e7b0d7b4fb0ed4dae07.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.30a762e9c23bdc35e52e.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.35249e44af8d1f7377c0.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.3842d1844bc92ce96c88.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.38bce3ca0ff07fde40d7.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.38bced12d1b42c4c1a31.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.3c2b1e1171eb58df862a.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.3e26fc8afccac357e6be.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.3e5cc4a2b41e91b597ab.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.3e9eac384c105b303e79.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.4312b39770d43fd0d656.js.map
+-rw-r--r--   0        0        0    29704 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.431464fdcb2b990c3b1a.js
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.431464fdcb2b990c3b1a.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.4558ccb53085fe45df87.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.53de14fff371a123d029.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.5849cb718fc52ee6df46.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.5a10e773711543bda859.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.5ac71cfa716a71c030d6.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.5e9875f82a3ad5f97952.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.5f57ce37214d4953598d.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.6042c480082a224a48b9.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.643577e67810f43714a8.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.66304c18bf3697d2473c.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.66ffd46a03333ee56a42.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.69cb0d28c6d4f2854af1.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.75c1ff3819927bdbf902.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.766ed606d07a8b832abc.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.7acd16813491fa0ff615.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.7ba614e2875b1e9680ff.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.800679a3fe495198cfd2.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.82d9bc0bc37152ea73c7.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.84ceea7b4267012e84c7.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.86707e8d7112b13cc3ad.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.87cc3741e1b6de69aa89.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.8ecf538fde2ccfcf33fb.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.9f0a2eefe7aadb15ae41.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.a98bc4ff5170118ea64a.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.ab1975ca0d1b9df1f91b.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.b084e69afb14892a975c.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.b20eaff3587d6b3ac566.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.b75b1ac5e362e0ae72d6.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.bd557903020a2b46b920.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.bd670e7ca8849267ece7.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.c151b05f5da9fabb7410.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.c1f7ed49e666074234d9.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.c59ecde72df993d90563.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.c9fb1eac6c2c9fedd03a.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.d2fd8a3c468010c8e1a1.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.d80e408bab17a43c87c2.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.dcc6b30986c6497bca3c.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.dda78c3c2459e905f54c.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.de590b3308b7618cc4d7.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.e276b399887d08c35e71.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.e37bcd7c63c6418dfbb3.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.eda5332dafec41590e5b.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.f5c4021326e0456459a2.js.map
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.f5e261b210e647b2d4ba.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.f6f75a2ce44969d92c2c.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.f7bdba3f4581ac7e4ce9.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.fb4a4b567bf481c1d484.js.map
+-rw-r--r--   0        0        0    28590 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.fe2870f0697685b06781.js.map
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/style.js
+-rw-r--r--   0        0        0    19365 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/style_index_js.9cf61c47582680994e2f.js
+-rw-r--r--   0        0        0    14835 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/style_index_js.9cf61c47582680994e2f.js.map
+-rw-r--r--   0        0        0    33772 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.f87f93d906d92e4f7101.js
+-rw-r--r--   0        0        0    25770 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.f87f93d906d92e4f7101.js.map
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/public/index.html
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/public/styles.css
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/src/icon.ts
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/src/index.ts
+-rw-r--r--   0        0        0     7887 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/src/widget.tsx
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/src/__tests__/jupyterlab_local_browser.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/ui-tests/tests/jupyterlab_local_browser.spec.ts
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/README.md
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 jupyterlab_local_browser-0.4.1/PKG-INFO
```

### Comparing `jupyterlab_local_browser-0.4.0/RELEASE.md` & `jupyterlab_local_browser-0.4.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/Untitled.ipynb` & `jupyterlab_local_browser-0.4.1/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jest.config.js` & `jupyterlab_local_browser-0.4.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/package.json` & `jupyterlab_local_browser-0.4.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.4.1'"}*

```diff
@@ -183,9 +183,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `jupyterlab_local_browser-0.4.0/tsconfig.json` & `jupyterlab_local_browser-0.4.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/yarn.lock` & `jupyterlab_local_browser-0.4.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/__init__.py` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/handlers.py` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     @tornado.web.authenticated
     def get(self):
         ports = set()
         ports.update(self._config.persistent)
         ports.update([
             conn.laddr.port
             for conn in net_connections(kind='tcp')
-            if conn.laddr.ip == '127.0.0.1' and conn.status == 'LISTEN'
+            if (conn.laddr.ip == '127.0.0.1' or conn.laddr.ip == '0.0.0.0') and conn.status == 'LISTEN'
                 and conn.laddr.port not in self._config.hidden
         ])
         ports = list(ports)
         ports.sort()
         ports = [(str(port), self._config.labels[port] if port in self._config.labels else str(port)) for port in ports]
         self.finish(json.dumps(ports))
```

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/build_log.json` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/package.json` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0260d483d18d1b5881ab.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0260d483d18d1b5881ab.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0260d483d18d1b5881ab.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0260d483d18d1b5881ab.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0531ad9081f3b9910023.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0531ad9081f3b9910023.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0531ad9081f3b9910023.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0531ad9081f3b9910023.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.097dbaec2b4b7ab6bed1.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.097dbaec2b4b7ab6bed1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.097dbaec2b4b7ab6bed1.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.097dbaec2b4b7ab6bed1.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0ae1bbc988abd77d7ce5.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0ae1bbc988abd77d7ce5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.0ae1bbc988abd77d7ce5.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.0ae1bbc988abd77d7ce5.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.11db783c3fe24b6adc52.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.11db783c3fe24b6adc52.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.11db783c3fe24b6adc52.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.11db783c3fe24b6adc52.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.2f4a309cfaf1e44ea829.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.2f4a309cfaf1e44ea829.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.2f4a309cfaf1e44ea829.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.2f4a309cfaf1e44ea829.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.30767f8725ca18bf459f.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.30767f8725ca18bf459f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.30767f8725ca18bf459f.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.30767f8725ca18bf459f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3885651e14bde39816d2.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3885651e14bde39816d2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3885651e14bde39816d2.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3885651e14bde39816d2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.38c8a7ef7cc34da00151.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.38c8a7ef7cc34da00151.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.38c8a7ef7cc34da00151.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.38c8a7ef7cc34da00151.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.393a277a4fd7125de295.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.393a277a4fd7125de295.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.393a277a4fd7125de295.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.393a277a4fd7125de295.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3c902412ec6167e454d2.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3c902412ec6167e454d2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3c902412ec6167e454d2.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3c902412ec6167e454d2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3cf287e5014b860e7ce4.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3cf287e5014b860e7ce4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3cf287e5014b860e7ce4.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3cf287e5014b860e7ce4.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3e869e2d783bda32e86f.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3e869e2d783bda32e86f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.3e869e2d783bda32e86f.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.3e869e2d783bda32e86f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.44a50b4bec1243752537.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.44a50b4bec1243752537.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.44a50b4bec1243752537.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.44a50b4bec1243752537.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.45fac8fc3fc216764524.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.45fac8fc3fc216764524.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.45fac8fc3fc216764524.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.45fac8fc3fc216764524.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.467c52c0a48ceec9af7f.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.467c52c0a48ceec9af7f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.467c52c0a48ceec9af7f.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.467c52c0a48ceec9af7f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.478e2e857c30ab96296c.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.478e2e857c30ab96296c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.478e2e857c30ab96296c.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.478e2e857c30ab96296c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.482abf9339c01e5ba6c3.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.482abf9339c01e5ba6c3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.482abf9339c01e5ba6c3.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.482abf9339c01e5ba6c3.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.48f290893b0d30b5c3f0.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.48f290893b0d30b5c3f0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.48f290893b0d30b5c3f0.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.48f290893b0d30b5c3f0.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.4b5c73e1630f9c00d4b2.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.4b5c73e1630f9c00d4b2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.4b5c73e1630f9c00d4b2.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.4b5c73e1630f9c00d4b2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.515127fe21ef0f56a907.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.515127fe21ef0f56a907.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.515127fe21ef0f56a907.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.515127fe21ef0f56a907.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.581ab39f2e283a14aff7.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.581ab39f2e283a14aff7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.581ab39f2e283a14aff7.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.581ab39f2e283a14aff7.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.664d52f84dba6d28ccf0.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.664d52f84dba6d28ccf0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.664d52f84dba6d28ccf0.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.664d52f84dba6d28ccf0.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.66e30c2a4a85c03b58d9.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.66e30c2a4a85c03b58d9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.66e30c2a4a85c03b58d9.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.66e30c2a4a85c03b58d9.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.6aa9131c23b373442af2.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.6aa9131c23b373442af2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.6aa9131c23b373442af2.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.6aa9131c23b373442af2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.6abf9ea20ee1c9c1dd6f.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.6abf9ea20ee1c9c1dd6f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.6abf9ea20ee1c9c1dd6f.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.6abf9ea20ee1c9c1dd6f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.7df68cc0bacbddb1774d.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.7df68cc0bacbddb1774d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.7df68cc0bacbddb1774d.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.7df68cc0bacbddb1774d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.7ebea98f752cde807697.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.7ebea98f752cde807697.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.7ebea98f752cde807697.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.7ebea98f752cde807697.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.8326cb8f3e2d1fd7e623.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.8326cb8f3e2d1fd7e623.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.8326cb8f3e2d1fd7e623.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.8326cb8f3e2d1fd7e623.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.861dea7bc7cb5f82903a.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.861dea7bc7cb5f82903a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.861dea7bc7cb5f82903a.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.861dea7bc7cb5f82903a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.8b369c4134033ffa5d52.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.8b369c4134033ffa5d52.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.8b369c4134033ffa5d52.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.8b369c4134033ffa5d52.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.9542c477b3765627ab36.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.9542c477b3765627ab36.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.9542c477b3765627ab36.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.9542c477b3765627ab36.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.99c52d2c6cf45f5e1f51.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.99c52d2c6cf45f5e1f51.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.99c52d2c6cf45f5e1f51.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.99c52d2c6cf45f5e1f51.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.9dfef7c94aafde75de43.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.9dfef7c94aafde75de43.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.9dfef7c94aafde75de43.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.9dfef7c94aafde75de43.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a0e6bae1dbf4e86bcdbe.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a0e6bae1dbf4e86bcdbe.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a0e6bae1dbf4e86bcdbe.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a0e6bae1dbf4e86bcdbe.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a219bfe4543e8c82a94a.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a219bfe4543e8c82a94a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a219bfe4543e8c82a94a.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a219bfe4543e8c82a94a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2370edcbfff0500a30c.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2370edcbfff0500a30c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2370edcbfff0500a30c.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2370edcbfff0500a30c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2b3b95e9ca37fdc24ab.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2b3b95e9ca37fdc24ab.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2b3b95e9ca37fdc24ab.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2b3b95e9ca37fdc24ab.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2c1b9df84931a8ef1cc.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2c1b9df84931a8ef1cc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a2c1b9df84931a8ef1cc.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a2c1b9df84931a8ef1cc.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a31e48eff904a48bc2e4.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a31e48eff904a48bc2e4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a31e48eff904a48bc2e4.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a31e48eff904a48bc2e4.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a518ab3a6e4d545b32ca.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a518ab3a6e4d545b32ca.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a518ab3a6e4d545b32ca.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a518ab3a6e4d545b32ca.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a535319a6e809944b995.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a535319a6e809944b995.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a535319a6e809944b995.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a535319a6e809944b995.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a60c60cdc4ea8d93e28c.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a60c60cdc4ea8d93e28c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a60c60cdc4ea8d93e28c.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a60c60cdc4ea8d93e28c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a75e33608a1ff124aac3.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a75e33608a1ff124aac3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a75e33608a1ff124aac3.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a75e33608a1ff124aac3.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a7f7c111f8e36e37204b.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a7f7c111f8e36e37204b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.a7f7c111f8e36e37204b.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.a7f7c111f8e36e37204b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b40be2f2583322a7a84d.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b40be2f2583322a7a84d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b40be2f2583322a7a84d.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b40be2f2583322a7a84d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b40c42a822c1acaafe61.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b40c42a822c1acaafe61.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b40c42a822c1acaafe61.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b40c42a822c1acaafe61.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b6383d5778cb49254d99.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b6383d5778cb49254d99.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b6383d5778cb49254d99.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b6383d5778cb49254d99.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b79e606c604dff28cb73.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b79e606c604dff28cb73.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.b79e606c604dff28cb73.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.b79e606c604dff28cb73.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.bd37de52b78466a4f5d4.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.bd37de52b78466a4f5d4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.bd37de52b78466a4f5d4.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.bd37de52b78466a4f5d4.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.bfbe76f93ff87e72e8d5.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.bfbe76f93ff87e72e8d5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.bfbe76f93ff87e72e8d5.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.bfbe76f93ff87e72e8d5.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.c7e82623d55ff4a2402b.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.c7e82623d55ff4a2402b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.c7e82623d55ff4a2402b.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.c7e82623d55ff4a2402b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d0df2c2c41c52ce5e6bf.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d0df2c2c41c52ce5e6bf.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d0df2c2c41c52ce5e6bf.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d0df2c2c41c52ce5e6bf.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d1d9356b9fda6e7696e8.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d1d9356b9fda6e7696e8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d1d9356b9fda6e7696e8.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d1d9356b9fda6e7696e8.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d4e0dbdaa229184ab605.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d4e0dbdaa229184ab605.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d4e0dbdaa229184ab605.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d4e0dbdaa229184ab605.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d8d5eef5f577cf52ed2e.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d8d5eef5f577cf52ed2e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.d8d5eef5f577cf52ed2e.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.d8d5eef5f577cf52ed2e.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.dac0e43082d308e0e490.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.dac0e43082d308e0e490.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.dac0e43082d308e0e490.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.dac0e43082d308e0e490.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.deec7b1a19e037c57782.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.deec7b1a19e037c57782.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.deec7b1a19e037c57782.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.deec7b1a19e037c57782.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e1f82fcdb1df57164b69.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e1f82fcdb1df57164b69.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e1f82fcdb1df57164b69.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e1f82fcdb1df57164b69.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e2381d09a8797b4febd2.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e2381d09a8797b4febd2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e2381d09a8797b4febd2.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e2381d09a8797b4febd2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e2580aaee693c29e07cb.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e2580aaee693c29e07cb.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e2580aaee693c29e07cb.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e2580aaee693c29e07cb.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e8530757b556bf028152.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e8530757b556bf028152.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e8530757b556bf028152.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e8530757b556bf028152.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e9225fce3da73baaa974.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e9225fce3da73baaa974.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e9225fce3da73baaa974.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e9225fce3da73baaa974.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e9ea030b4a00ebbcf710.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e9ea030b4a00ebbcf710.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.e9ea030b4a00ebbcf710.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.e9ea030b4a00ebbcf710.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f23e1e8e2f15f4973b4d.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f23e1e8e2f15f4973b4d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f23e1e8e2f15f4973b4d.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f23e1e8e2f15f4973b4d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f8edc82fc51b7640b290.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f8edc82fc51b7640b290.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f8edc82fc51b7640b290.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f8edc82fc51b7640b290.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f94f1cfa271c209d2015.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f94f1cfa271c209d2015.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/lib_index_js.f94f1cfa271c209d2015.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/lib_index_js.f94f1cfa271c209d2015.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.059a5ab6fa0d40dc2ec5.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.059a5ab6fa0d40dc2ec5.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.05cdb0e2d59ddf299c2d.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.05cdb0e2d59ddf299c2d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.09954ab8aac77ff30097.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.09954ab8aac77ff30097.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.158e6dc4043218c5fd93.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.158e6dc4043218c5fd93.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.192da90950725b39b157.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.192da90950725b39b157.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.1a998993d84da7b0a455.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.1a998993d84da7b0a455.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.23e4fe60cdea9dc96d93.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.23e4fe60cdea9dc96d93.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.2e7b0d7b4fb0ed4dae07.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.2e7b0d7b4fb0ed4dae07.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.30a762e9c23bdc35e52e.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.30a762e9c23bdc35e52e.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.35249e44af8d1f7377c0.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.35249e44af8d1f7377c0.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.3842d1844bc92ce96c88.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.3842d1844bc92ce96c88.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.38bce3ca0ff07fde40d7.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.38bce3ca0ff07fde40d7.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.38bced12d1b42c4c1a31.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.38bced12d1b42c4c1a31.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.3c2b1e1171eb58df862a.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.3c2b1e1171eb58df862a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.3e26fc8afccac357e6be.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.3e26fc8afccac357e6be.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.3e5cc4a2b41e91b597ab.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.3e5cc4a2b41e91b597ab.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.3e9eac384c105b303e79.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.3e9eac384c105b303e79.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.4312b39770d43fd0d656.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.4312b39770d43fd0d656.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.431464fdcb2b990c3b1a.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.431464fdcb2b990c3b1a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.431464fdcb2b990c3b1a.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.431464fdcb2b990c3b1a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.4558ccb53085fe45df87.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.4558ccb53085fe45df87.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.53de14fff371a123d029.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.53de14fff371a123d029.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.5849cb718fc52ee6df46.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.5849cb718fc52ee6df46.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.5a10e773711543bda859.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.5a10e773711543bda859.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.5ac71cfa716a71c030d6.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.5ac71cfa716a71c030d6.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.5e9875f82a3ad5f97952.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.5e9875f82a3ad5f97952.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.5f57ce37214d4953598d.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.5f57ce37214d4953598d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.6042c480082a224a48b9.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.6042c480082a224a48b9.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.643577e67810f43714a8.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.643577e67810f43714a8.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.66304c18bf3697d2473c.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.66304c18bf3697d2473c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.66ffd46a03333ee56a42.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.66ffd46a03333ee56a42.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.69cb0d28c6d4f2854af1.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.69cb0d28c6d4f2854af1.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.75c1ff3819927bdbf902.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.75c1ff3819927bdbf902.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.766ed606d07a8b832abc.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.766ed606d07a8b832abc.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.7acd16813491fa0ff615.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.7acd16813491fa0ff615.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.7ba614e2875b1e9680ff.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.7ba614e2875b1e9680ff.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.800679a3fe495198cfd2.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.800679a3fe495198cfd2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.82d9bc0bc37152ea73c7.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.82d9bc0bc37152ea73c7.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.84ceea7b4267012e84c7.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.84ceea7b4267012e84c7.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.86707e8d7112b13cc3ad.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.86707e8d7112b13cc3ad.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.87cc3741e1b6de69aa89.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.87cc3741e1b6de69aa89.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.8ecf538fde2ccfcf33fb.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.8ecf538fde2ccfcf33fb.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.9f0a2eefe7aadb15ae41.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.9f0a2eefe7aadb15ae41.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.a98bc4ff5170118ea64a.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.a98bc4ff5170118ea64a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.ab1975ca0d1b9df1f91b.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.ab1975ca0d1b9df1f91b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.b084e69afb14892a975c.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.b084e69afb14892a975c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.b20eaff3587d6b3ac566.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.b20eaff3587d6b3ac566.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.b75b1ac5e362e0ae72d6.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.b75b1ac5e362e0ae72d6.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.bd557903020a2b46b920.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.bd557903020a2b46b920.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.bd670e7ca8849267ece7.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.bd670e7ca8849267ece7.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.c151b05f5da9fabb7410.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.c151b05f5da9fabb7410.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.c1f7ed49e666074234d9.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.c1f7ed49e666074234d9.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.c59ecde72df993d90563.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.c59ecde72df993d90563.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.c9fb1eac6c2c9fedd03a.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.c9fb1eac6c2c9fedd03a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.d2fd8a3c468010c8e1a1.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.d2fd8a3c468010c8e1a1.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.d80e408bab17a43c87c2.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.d80e408bab17a43c87c2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.dcc6b30986c6497bca3c.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.dcc6b30986c6497bca3c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.dda78c3c2459e905f54c.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.dda78c3c2459e905f54c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.de590b3308b7618cc4d7.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.de590b3308b7618cc4d7.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.e276b399887d08c35e71.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.e276b399887d08c35e71.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.e37bcd7c63c6418dfbb3.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.e37bcd7c63c6418dfbb3.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.eda5332dafec41590e5b.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.eda5332dafec41590e5b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.f5c4021326e0456459a2.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.f5c4021326e0456459a2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.f5e261b210e647b2d4ba.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.f5e261b210e647b2d4ba.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.f6f75a2ce44969d92c2c.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.f6f75a2ce44969d92c2c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.f7bdba3f4581ac7e4ce9.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.f7bdba3f4581ac7e4ce9.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.fb4a4b567bf481c1d484.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.fb4a4b567bf481c1d484.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/remoteEntry.fe2870f0697685b06781.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/remoteEntry.fe2870f0697685b06781.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/style_index_js.9cf61c47582680994e2f.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/style_index_js.9cf61c47582680994e2f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/style_index_js.9cf61c47582680994e2f.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/style_index_js.9cf61c47582680994e2f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.f87f93d906d92e4f7101.js` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.f87f93d906d92e4f7101.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/jupyterlab_local_browser/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.f87f93d906d92e4f7101.js.map` & `jupyterlab_local_browser-0.4.1/jupyterlab_local_browser/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.f87f93d906d92e4f7101.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/src/icon.ts` & `jupyterlab_local_browser-0.4.1/src/icon.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/src/index.ts` & `jupyterlab_local_browser-0.4.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/src/widget.tsx` & `jupyterlab_local_browser-0.4.1/src/widget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/ui-tests/README.md` & `jupyterlab_local_browser-0.4.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/ui-tests/tests/jupyterlab_local_browser.spec.ts` & `jupyterlab_local_browser-0.4.1/ui-tests/tests/jupyterlab_local_browser.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/.gitignore` & `jupyterlab_local_browser-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/LICENSE` & `jupyterlab_local_browser-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/README.md` & `jupyterlab_local_browser-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/pyproject.toml` & `jupyterlab_local_browser-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_local_browser-0.4.0/PKG-INFO` & `jupyterlab_local_browser-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_local_browser
-Version: 0.4.0
+Version: 0.4.1
 Summary: A JupyterLab local browser
 Project-URL: Homepage, https://github.com/scmmmh/jupyterlab-local-browser
 Project-URL: Bug Tracker, https://github.com/scmmmh/jupyterlab-local-browser/issues
 Project-URL: Repository, https://github.com/scmmmh/jupyterlab-local-browser.git
 Author-email: Mark Hall <mark.hall@open.ac.uk>
 License: BSD 3-Clause License
```

