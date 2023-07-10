# Comparing `tmp/nbtools-23.5.0.tar.gz` & `tmp/nbtools-23.7.0.tar.gz`

## Comparing `nbtools-23.5.0.tar` & `nbtools-23.7.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbtools-23.5.0/.coveragerc
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nbtools-23.5.0/.eslintignore
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 nbtools-23.5.0/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nbtools-23.5.0/.npmignore
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 nbtools-23.5.0/.prettierignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbtools-23.5.0/.prettierrc
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 nbtools-23.5.0/DEPLOY.md
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 nbtools-23.5.0/Dockerfile
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 nbtools-23.5.0/appveyor.yml
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 nbtools-23.5.0/codecov.yml
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbtools-23.5.0/dev.Dockerfile
--rwxr-xr-x   0        0        0      827 2020-02-02 00:00:00.000000 nbtools-23.5.0/docker_build.sh
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nbtools-23.5.0/install.json
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 nbtools-23.5.0/package.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nbtools-23.5.0/postBuild
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbtools-23.5.0/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nbtools-23.5.0/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 nbtools-23.5.0/setup.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nbtools-23.5.0/tsconfig.json
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 nbtools-23.5.0/webpack.config.js
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/.gitignore
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/compiler.xml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/modules.xml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/nbtools.iml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/rSettings.xml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/vcs.xml
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/workspace.xml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nbtools-23.5.0/config/overrides.json
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 nbtools-23.5.0/docs/toolmanager.md
--rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 nbtools-23.5.0/docs/uibuilder.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nbtools-23.5.0/docs/uioutput.md
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 nbtools-23.5.0/docs/wysiwyg.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nbtools-23.5.0/jupyter-config/nbtools.json
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/_frontend.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/_version.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/basewidget.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/event_manager.py
--rw-r--r--   0        0        0    19059 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/form.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/nbtools.json
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/parsing_manager.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/settings.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/tool_manager.py
--rw-r--r--   0        0        0    12833 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/uibuilder.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/uioutput.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/utils.py
--rw-r--r--   0        0        0    20298 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/build_log.json
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/package.json
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/schemas/@g2nb/nbtools/plugin.json
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js.map
--rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js
--rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js.map
--rw-r--r--   0        0        0   141481 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js
--rw-r--r--   0        0        0   139488 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js.map
--rw-r--r--   0        0        0    33507 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js
--rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js.map
--rw-r--r--   0        0        0    29361 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js
--rw-r--r--   0        0        0    28197 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js.map
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/style.js
--rw-r--r--   0        0        0    16904 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js
--rw-r--r--   0        0        0    14914 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js.map
--rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js
--rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js.map
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/nbextension/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/nbextension/static/extension.js
--rw-r--r--   0        0        0    21002 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/nbextension/static/notebook.css
--rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/nbextension/static/toolbox.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/tests/__init__.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/tests/conftest.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/tests/test_example.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nbtools-23.5.0/schema/plugin.json
--rw-r--r--   0        0        0    15823 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/basewidget.ts
--rw-r--r--   0        0        0    17444 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/context.ts
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/dataregistry.ts
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/extension.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/index.ts
--rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/plugin.ts
--rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/registry.ts
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/toolbox.ts
--rw-r--r--   0        0        0    31309 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/uibuilder.ts
--rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/uioutput.ts
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/utils.ts
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/version.ts
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/basewidget.css
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/g2nb_logo.png
--rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/icon.svg
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/index.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/index.js
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/toolbox.css
--rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/uibuilder.css
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/uioutput.css
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nbtools-23.5.0/tests/karma.conf.js
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nbtools-23.5.0/tests/tsconfig.json
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nbtools-23.5.0/tests/src/index.spec.ts
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 nbtools-23.5.0/tests/src/utils.spec.ts
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 nbtools-23.5.0/.gitignore
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 nbtools-23.5.0/LICENSE.txt
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 nbtools-23.5.0/README.md
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 nbtools-23.5.0/pyproject.toml
--rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 nbtools-23.5.0/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbtools-23.7.0/.coveragerc
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nbtools-23.7.0/.eslintignore
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 nbtools-23.7.0/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nbtools-23.7.0/.npmignore
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 nbtools-23.7.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbtools-23.7.0/.prettierrc
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 nbtools-23.7.0/DEPLOY.md
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 nbtools-23.7.0/Dockerfile
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 nbtools-23.7.0/appveyor.yml
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 nbtools-23.7.0/codecov.yml
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbtools-23.7.0/dev.Dockerfile
+-rwxr-xr-x   0        0        0      827 2020-02-02 00:00:00.000000 nbtools-23.7.0/docker_build.sh
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nbtools-23.7.0/install.json
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 nbtools-23.7.0/package.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nbtools-23.7.0/postBuild
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbtools-23.7.0/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nbtools-23.7.0/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 nbtools-23.7.0/setup.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nbtools-23.7.0/tsconfig.json
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 nbtools-23.7.0/webpack.config.js
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbtools-23.7.0/.idea/.gitignore
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 nbtools-23.7.0/.idea/compiler.xml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nbtools-23.7.0/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 nbtools-23.7.0/.idea/modules.xml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nbtools-23.7.0/.idea/nbtools.iml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nbtools-23.7.0/.idea/rSettings.xml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nbtools-23.7.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 nbtools-23.7.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nbtools-23.7.0/config/overrides.json
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 nbtools-23.7.0/docs/toolmanager.md
+-rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 nbtools-23.7.0/docs/uibuilder.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nbtools-23.7.0/docs/uioutput.md
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 nbtools-23.7.0/docs/wysiwyg.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nbtools-23.7.0/jupyter-config/nbtools.json
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/_frontend.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/_version.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/basewidget.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/event_manager.py
+-rw-r--r--   0        0        0    19059 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/form.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/nbtools.json
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/parsing_manager.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/settings.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/tool_manager.py
+-rw-r--r--   0        0        0    12833 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/uibuilder.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/uioutput.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/utils.py
+-rw-r--r--   0        0        0    20274 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/build_log.json
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/package.json
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/schemas/@g2nb/nbtools/plugin.json
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js.map
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/lib_plugin_js.6292de8fa547e3973251.js
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/lib_plugin_js.6292de8fa547e3973251.js.map
+-rw-r--r--   0        0        0   144063 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.cd289910d38270a1d73e.js
+-rw-r--r--   0        0        0   142446 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.cd289910d38270a1d73e.js.map
+-rw-r--r--   0        0        0    33507 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js
+-rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js.map
+-rw-r--r--   0        0        0    29600 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/remoteEntry.5f8f98422831593fa148.js
+-rw-r--r--   0        0        0    28437 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/remoteEntry.5f8f98422831593fa148.js.map
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/style.js
+-rw-r--r--   0        0        0    16904 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js
+-rw-r--r--   0        0        0    14914 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js.map
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js
+-rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js.map
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/nbextension/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/nbextension/static/extension.js
+-rw-r--r--   0        0        0    21002 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/nbextension/static/notebook.css
+-rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/nbextension/static/toolbox.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/tests/__init__.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/tests/conftest.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/tests/test_example.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 nbtools-23.7.0/nbtools/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nbtools-23.7.0/schema/plugin.json
+-rw-r--r--   0        0        0    16556 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/basewidget.ts
+-rw-r--r--   0        0        0    18810 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/context.ts
+-rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/dataregistry.ts
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/extension.ts
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/index.ts
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/plugin.ts
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/registry.ts
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/toolbox.ts
+-rw-r--r--   0        0        0    31309 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/uibuilder.ts
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/uioutput.ts
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/utils.ts
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nbtools-23.7.0/src/version.ts
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 nbtools-23.7.0/style/basewidget.css
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nbtools-23.7.0/style/g2nb_logo.png
+-rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 nbtools-23.7.0/style/icon.svg
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nbtools-23.7.0/style/index.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nbtools-23.7.0/style/index.js
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 nbtools-23.7.0/style/toolbox.css
+-rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 nbtools-23.7.0/style/uibuilder.css
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 nbtools-23.7.0/style/uioutput.css
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nbtools-23.7.0/tests/karma.conf.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nbtools-23.7.0/tests/tsconfig.json
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nbtools-23.7.0/tests/src/index.spec.ts
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 nbtools-23.7.0/tests/src/utils.spec.ts
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 nbtools-23.7.0/.gitignore
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 nbtools-23.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 nbtools-23.7.0/README.md
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 nbtools-23.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8910 2020-02-02 00:00:00.000000 nbtools-23.7.0/PKG-INFO
```

### Comparing `nbtools-23.5.0/.eslintrc.js` & `nbtools-23.7.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/DEPLOY.md` & `nbtools-23.7.0/DEPLOY.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/Dockerfile` & `nbtools-23.7.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/appveyor.yml` & `nbtools-23.7.0/appveyor.yml`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/dev.Dockerfile` & `nbtools-23.7.0/dev.Dockerfile`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/docker_build.sh` & `nbtools-23.7.0/docker_build.sh`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/package.json` & `nbtools-23.7.0/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/tsconfig.json` & `nbtools-23.7.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/webpack.config.js` & `nbtools-23.7.0/webpack.config.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/.idea/nbtools.iml` & `nbtools-23.7.0/.idea/nbtools.iml`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/.idea/workspace.xml` & `nbtools-23.7.0/.idea/workspace.xml`

 * *Files 12% similar despite different names*

#### Comparing `nbtools-23.5.0/.idea/workspace.xml` & `nbtools-23.7.0/.idea/workspace.xml`

```diff
@@ -1,84 +1,73 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="07938b4a-ab13-4e2d-9217-d9f9a634d868" name="Changes" comment="More property bug fixes">
-      <change beforePath="$PROJECT_DIR$/dev.Dockerfile" beforeDir="false" afterPath="$PROJECT_DIR$/dev.Dockerfile" afterDir="false"/>
+    <list default="true" id="46940df7-d665-48c0-8edf-b196002175c5" name="Changes" comment="Added the ability to toggle forced rendering on and off">
+      <change beforePath="$PROJECT_DIR$/.idea/misc.xml" beforeDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
-  <component name="Git.Merge.Settings">
-    <option name="BRANCH" value="hatch"/>
-  </component>
   <component name="Git.Settings">
-    <option name="RECENT_BRANCH_BY_REPOSITORY">
-      <map>
-        <entry key="$PROJECT_DIR$" value="master"/>
-      </map>
-    </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
-  <component name="ProjectId" id="2OyGrGnro2Gb5YAX78WLJyJ6sTc"/>
+  <component name="ProjectId" id="2R9iHKSwaH5w8G3P3vIBv1YtC0X"/>
   <component name="ProjectLevelVcsManager" settingsEditedManually="true"/>
   <component name="ProjectViewState">
     <option name="autoscrollFromSource" value="true"/>
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">
     <property name="RunOnceActivity.OpenProjectViewOnStart" value="true"/>
     <property name="RunOnceActivity.ShowReadmeOnStart" value="true"/>
     <property name="WebServerToolWindowFactoryState" value="false"/>
     <property name="node.js.detected.package.eslint" value="true"/>
+    <property name="node.js.detected.package.tslint" value="true"/>
     <property name="node.js.selected.package.eslint" value="(autodetect)"/>
     <property name="node.js.selected.package.tslint" value="(autodetect)"/>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
-    <task id="LOCAL-00001" summary="Updating files">
-      <created>1681758324874</created>
-      <option name="number" value="00001"/>
-      <option name="presentableId" value="LOCAL-00001"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1681758324874</updated>
-    </task>
     <task active="true" id="Default" summary="Default task">
-      <changelist id="07938b4a-ab13-4e2d-9217-d9f9a634d868" name="Changes" comment="Updating files"/>
-      <created>1682525606744</created>
+      <changelist id="46940df7-d665-48c0-8edf-b196002175c5" name="Changes" comment=""/>
+      <created>1686668612369</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
-      <updated>1682525606744</updated>
-      <workItem from="1682525608012" duration="292000"/>
-      <workItem from="1683645942319" duration="6492000"/>
-      <workItem from="1683658898540" duration="66000"/>
+      <updated>1686668612369</updated>
+      <workItem from="1686668615646" duration="1893000"/>
+      <workItem from="1686764637656" duration="7332000"/>
+      <workItem from="1687274187864" duration="7233000"/>
+      <workItem from="1687533644599" duration="4204000"/>
+      <workItem from="1687793960982" duration="359000"/>
+      <workItem from="1689005352994" duration="180000"/>
     </task>
-    <task id="LOCAL-00002" summary="Bug fix for property getters and setters no longer working on UIBuilder after ipywidgets 8 migration">
-      <created>1683649438114</created>
-      <option name="number" value="00002"/>
-      <option name="presentableId" value="LOCAL-00002"/>
+    <task id="LOCAL-00001" summary="Ensure rendering of widgets through execution, if necessary">
+      <created>1687467233902</created>
+      <option name="number" value="00001"/>
+      <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
-      <updated>1683649438114</updated>
+      <updated>1687467233902</updated>
     </task>
-    <task id="LOCAL-00003" summary="More property bug fixes">
-      <created>1683652389561</created>
-      <option name="number" value="00003"/>
-      <option name="presentableId" value="LOCAL-00003"/>
+    <task id="LOCAL-00002" summary="Added the ability to toggle forced rendering on and off">
+      <created>1687536884714</created>
+      <option name="number" value="00002"/>
+      <option name="presentableId" value="LOCAL-00002"/>
       <option name="project" value="LOCAL"/>
-      <updated>1683652389561</updated>
+      <updated>1687536884715</updated>
     </task>
-    <option name="localTasksCounter" value="4"/>
+    <option name="localTasksCounter" value="3"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -88,13 +77,12 @@
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Updating files"/>
-    <MESSAGE value="Bug fix for property getters and setters no longer working on UIBuilder after ipywidgets 8 migration"/>
-    <MESSAGE value="More property bug fixes"/>
-    <option name="LAST_COMMIT_MESSAGE" value="More property bug fixes"/>
+    <MESSAGE value="Ensure rendering of widgets through execution, if necessary"/>
+    <MESSAGE value="Added the ability to toggle forced rendering on and off"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Added the ability to toggle forced rendering on and off"/>
   </component>
 </project>
```

### Comparing `nbtools-23.5.0/docs/toolmanager.md` & `nbtools-23.7.0/docs/toolmanager.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/docs/uibuilder.md` & `nbtools-23.7.0/docs/uibuilder.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/docs/uioutput.md` & `nbtools-23.7.0/docs/uioutput.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/docs/wysiwyg.md` & `nbtools-23.7.0/docs/wysiwyg.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/__init__.py` & `nbtools-23.7.0/nbtools/__init__.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/_version.py` & `nbtools-23.7.0/nbtools/_version.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/basewidget.py` & `nbtools-23.7.0/nbtools/basewidget.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/event_manager.py` & `nbtools-23.7.0/nbtools/event_manager.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/form.py` & `nbtools-23.7.0/nbtools/form.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/parsing_manager.py` & `nbtools-23.7.0/nbtools/parsing_manager.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/settings.py` & `nbtools-23.7.0/nbtools/settings.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/tool_manager.py` & `nbtools-23.7.0/nbtools/tool_manager.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/uibuilder.py` & `nbtools-23.7.0/nbtools/uibuilder.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/uioutput.py` & `nbtools-23.7.0/nbtools/uioutput.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/utils.py` & `nbtools-23.7.0/nbtools/utils.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/labextension/build_log.json` & `nbtools-23.7.0/nbtools/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999909631854078%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@g2nb/nbtools': {'version': '23.5.0'}, delete: "*

 * *      "['yarn']}}}}}"}*

```diff
@@ -97,15 +97,15 @@
                         "type": "var"
                     },
                     "name": "@g2nb/nbtools",
                     "shared": {
                         "@g2nb/nbtools": {
                             "import": "/Users/tmtabor/workspace/nbtools/lib/index.js",
                             "singleton": true,
-                            "version": "23.3.2"
+                            "version": "23.5.0"
                         },
                         "@jupyter-widgets/base": {
                             "import": false,
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
@@ -580,15 +580,14 @@
                             "singleton": true
                         },
                         "react-dom": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
-                        "yarn": {},
                         "yjs": {
                             "import": false,
                             "requiredVersion": "^13.5.17",
                             "singleton": true
                         }
                     }
                 }
```

### Comparing `nbtools-23.5.0/nbtools/labextension/package.json` & `nbtools-23.7.0/nbtools/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9662808641975309%*

 * *Differences: {"'dependencies'": "{delete: ['yarn']}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.5f8f98422831593fa148.js'}}",*

 * * "'version'": "'23.5.0'"}*

```diff
@@ -6,16 +6,15 @@
     "bugs": {
         "url": "https://github.com/g2nb/nbtools/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^6",
         "@jupyterlab/application": "^3.0.4",
         "@jupyterlab/mainmenu": "^3.0.3",
-        "@jupyterlab/notebook": "^3.0.4",
-        "yarn": "^1.22.19"
+        "@jupyterlab/notebook": "^3.0.4"
     },
     "description": "Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike.",
     "devDependencies": {
         "@jupyterlab/apputils": "^3.0.3",
         "@jupyterlab/builder": "^3.0.0",
         "@jupyterlab/ui-components": "^3.0.3",
         "@lumino/application": "^1.13.1",
@@ -53,15 +52,15 @@
         "dist/*.{js,css}",
         "style/index.js"
     ],
     "homepage": "https://github.com/g2nb/nbtools",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ed7f531dbfb094c43618.js",
+            "load": "static/remoteEntry.5f8f98422831593fa148.js",
             "style": "./style"
         },
         "discovery": {
             "kernel": [
                 {
                     "base": {
                         "name": "nbtools"
@@ -126,9 +125,9 @@
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch",
         "watch:src": "tsc -w"
     },
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "./lib/index.d.ts",
-    "version": "23.3.2"
+    "version": "23.5.0"
 }
```

### Comparing `nbtools-23.5.0/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig` & `nbtools-23.7.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666666%*

 * *Differences: {"'dependencies'": "{delete: ['yarn']}", "'version'": "'23.7.0'"}*

```diff
@@ -6,16 +6,15 @@
     "bugs": {
         "url": "https://github.com/g2nb/nbtools/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^6",
         "@jupyterlab/application": "^3.0.4",
         "@jupyterlab/mainmenu": "^3.0.3",
-        "@jupyterlab/notebook": "^3.0.4",
-        "yarn": "^1.22.19"
+        "@jupyterlab/notebook": "^3.0.4"
     },
     "description": "Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike.",
     "devDependencies": {
         "@jupyterlab/apputils": "^3.0.3",
         "@jupyterlab/builder": "^3.0.0",
         "@jupyterlab/ui-components": "^3.0.3",
         "@lumino/application": "^1.13.1",
@@ -121,9 +120,9 @@
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch",
         "watch:src": "tsc -w"
     },
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "./lib/index.d.ts",
-    "version": "23.3.2"
+    "version": "23.7.0"
 }
```

### Comparing `nbtools-23.5.0/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png` & `nbtools-23.7.0/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js` & `nbtools-23.7.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js.map` & `nbtools-23.7.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js` & `nbtools-23.7.0/nbtools/labextension/static/lib_plugin_js.6292de8fa547e3973251.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -18,126 +18,144 @@
                     /* harmony export */
                 });
                 /* harmony import */
                 var _jupyter_widgets_base__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyter-widgets/base */ "webpack/sharing/consume/default/@jupyter-widgets/base");
                 /* harmony import */
                 var _jupyter_widgets_base__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyter_widgets_base__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
-                var _version__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! ./version */ "./lib/version.js");
+                var _jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! @jupyterlab/settingregistry */ "webpack/sharing/consume/default/@jupyterlab/settingregistry");
                 /* harmony import */
-                var _basewidget__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! ./basewidget */ "./lib/basewidget.js");
+                var _jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_1__);
                 /* harmony import */
-                var _uioutput__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! ./uioutput */ "./lib/uioutput.js");
+                var _version__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! ./version */ "./lib/version.js");
                 /* harmony import */
-                var _uibuilder__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__( /*! ./uibuilder */ "./lib/uibuilder.js");
+                var _basewidget__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! ./basewidget */ "./lib/basewidget.js");
                 /* harmony import */
-                var _jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__( /*! @jupyterlab/mainmenu */ "webpack/sharing/consume/default/@jupyterlab/mainmenu");
+                var _uioutput__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__( /*! ./uioutput */ "./lib/uioutput.js");
                 /* harmony import */
-                var _jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_5___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_5__);
+                var _uibuilder__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__( /*! ./uibuilder */ "./lib/uibuilder.js");
                 /* harmony import */
-                var _toolbox__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__( /*! ./toolbox */ "./lib/toolbox.js");
+                var _jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__( /*! @jupyterlab/mainmenu */ "webpack/sharing/consume/default/@jupyterlab/mainmenu");
                 /* harmony import */
-                var _registry__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__( /*! ./registry */ "./lib/registry.js");
+                var _jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_6___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_6__);
                 /* harmony import */
-                var _utils__WEBPACK_IMPORTED_MODULE_8__ = __webpack_require__( /*! ./utils */ "./lib/utils.js");
+                var _toolbox__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__( /*! ./toolbox */ "./lib/toolbox.js");
                 /* harmony import */
-                var _jupyterlab_application__WEBPACK_IMPORTED_MODULE_9__ = __webpack_require__( /*! @jupyterlab/application */ "webpack/sharing/consume/default/@jupyterlab/application");
+                var _registry__WEBPACK_IMPORTED_MODULE_8__ = __webpack_require__( /*! ./registry */ "./lib/registry.js");
                 /* harmony import */
-                var _jupyterlab_application__WEBPACK_IMPORTED_MODULE_9___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_application__WEBPACK_IMPORTED_MODULE_9__);
+                var _utils__WEBPACK_IMPORTED_MODULE_9__ = __webpack_require__( /*! ./utils */ "./lib/utils.js");
                 /* harmony import */
-                var _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_10__ = __webpack_require__( /*! @jupyterlab/notebook */ "webpack/sharing/consume/default/@jupyterlab/notebook");
+                var _jupyterlab_application__WEBPACK_IMPORTED_MODULE_10__ = __webpack_require__( /*! @jupyterlab/application */ "webpack/sharing/consume/default/@jupyterlab/application");
                 /* harmony import */
-                var _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_10___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_10__);
+                var _jupyterlab_application__WEBPACK_IMPORTED_MODULE_10___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_application__WEBPACK_IMPORTED_MODULE_10__);
                 /* harmony import */
-                var _context__WEBPACK_IMPORTED_MODULE_11__ = __webpack_require__( /*! ./context */ "./lib/context.js");
+                var _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_11__ = __webpack_require__( /*! @jupyterlab/notebook */ "webpack/sharing/consume/default/@jupyterlab/notebook");
                 /* harmony import */
-                var _dataregistry__WEBPACK_IMPORTED_MODULE_12__ = __webpack_require__( /*! ./dataregistry */ "./lib/dataregistry.js");
+                var _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_11___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_11__);
+                /* harmony import */
+                var _context__WEBPACK_IMPORTED_MODULE_12__ = __webpack_require__( /*! ./context */ "./lib/context.js");
+                /* harmony import */
+                var _dataregistry__WEBPACK_IMPORTED_MODULE_13__ = __webpack_require__( /*! ./dataregistry */ "./lib/dataregistry.js");
 
 
 
 
 
 
 
 
 
 
 
 
 
-                const module_exports = Object.assign(Object.assign(Object.assign({}, _basewidget__WEBPACK_IMPORTED_MODULE_2__), _uioutput__WEBPACK_IMPORTED_MODULE_3__), _uibuilder__WEBPACK_IMPORTED_MODULE_4__);
+
+                const module_exports = Object.assign(Object.assign(Object.assign({}, _basewidget__WEBPACK_IMPORTED_MODULE_3__), _uioutput__WEBPACK_IMPORTED_MODULE_4__), _uibuilder__WEBPACK_IMPORTED_MODULE_5__);
                 const EXTENSION_ID = '@g2nb/nbtools:plugin';
                 const NAMESPACE = 'nbtools';
                 /**
                  * The nbtools plugin.
                  */
                 const nbtools_plugin = {
                     id: EXTENSION_ID,
-                    provides: [_registry__WEBPACK_IMPORTED_MODULE_7__.IToolRegistry, _dataregistry__WEBPACK_IMPORTED_MODULE_12__.IDataRegistry],
-                    requires: [_jupyter_widgets_base__WEBPACK_IMPORTED_MODULE_0__.IJupyterWidgetRegistry],
-                    optional: [_jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_5__.IMainMenu, _jupyterlab_application__WEBPACK_IMPORTED_MODULE_9__.ILayoutRestorer, _jupyterlab_application__WEBPACK_IMPORTED_MODULE_9__.ILabShell, _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_10__.INotebookTracker],
+                    provides: [_registry__WEBPACK_IMPORTED_MODULE_8__.IToolRegistry, _dataregistry__WEBPACK_IMPORTED_MODULE_13__.IDataRegistry],
+                    requires: [_jupyter_widgets_base__WEBPACK_IMPORTED_MODULE_0__.IJupyterWidgetRegistry, _jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_1__.ISettingRegistry],
+                    optional: [_jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_6__.IMainMenu, _jupyterlab_application__WEBPACK_IMPORTED_MODULE_10__.ILayoutRestorer, _jupyterlab_application__WEBPACK_IMPORTED_MODULE_10__.ILabShell, _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_11__.INotebookTracker],
                     activate: activate_widget_extension,
                     autoStart: true
                 };
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (nbtools_plugin);
                 /**
                  * Activate the widget extension.
                  */
-                function activate_widget_extension(app, widget_registry, mainmenu, restorer, shell, notebook_tracker) {
+                async function activate_widget_extension(app, widget_registry, settings, mainmenu, restorer, shell, notebook_tracker) {
                     // Initialize the ContextManager
                     init_context(app, notebook_tracker);
+                    // Initialize settings
+                    const setting_dict = await init_settings(settings);
                     // Create the tool and data registries
-                    const tool_registry = new _registry__WEBPACK_IMPORTED_MODULE_7__.ToolRegistry();
-                    const data_registry = new _dataregistry__WEBPACK_IMPORTED_MODULE_12__.DataRegistry();
+                    const tool_registry = new _registry__WEBPACK_IMPORTED_MODULE_8__.ToolRegistry(setting_dict);
+                    const data_registry = new _dataregistry__WEBPACK_IMPORTED_MODULE_13__.DataRegistry();
                     // Add items to the help menu
                     add_help_links(app, mainmenu);
                     // Add keyboard shortcuts
                     add_keyboard_shortcuts(app, tool_registry);
                     // Add the toolbox
                     add_tool_browser(app, restorer);
                     // Register the nbtools widgets with the widget registry
                     widget_registry.registerWidget({
-                        name: _version__WEBPACK_IMPORTED_MODULE_1__.MODULE_NAME,
-                        version: _version__WEBPACK_IMPORTED_MODULE_1__.MODULE_VERSION,
+                        name: _version__WEBPACK_IMPORTED_MODULE_2__.MODULE_NAME,
+                        version: _version__WEBPACK_IMPORTED_MODULE_2__.MODULE_VERSION,
                         exports: module_exports,
                     });
                     // Register the plugin as loaded
-                    (0, _utils__WEBPACK_IMPORTED_MODULE_8__.usage_tracker)('labextension_load', location.protocol + '//' + location.host + location.pathname);
+                    (0, _utils__WEBPACK_IMPORTED_MODULE_9__.usage_tracker)('labextension_load', location.protocol + '//' + location.host + location.pathname);
                     // Return the tool registry so that it is provided to other extensions
                     return [tool_registry, data_registry];
                 }
+                async function init_settings(settings) {
+                    let setting = null;
+                    try {
+                        setting = await settings.load(EXTENSION_ID);
+                    } catch (_a) {
+                        console.log('Unable to load nbtools settings');
+                    }
+                    return {
+                        force_render: setting ? setting.get('force_render').composite : true
+                    };
+                }
 
                 function init_context(app, notebook_tracker) {
-                    _context__WEBPACK_IMPORTED_MODULE_11__.ContextManager.jupyter_app = app;
-                    _context__WEBPACK_IMPORTED_MODULE_11__.ContextManager.notebook_tracker = notebook_tracker;
-                    _context__WEBPACK_IMPORTED_MODULE_11__.ContextManager.context();
-                    window.ContextManager = _context__WEBPACK_IMPORTED_MODULE_11__.ContextManager; // Left in for development purposes
+                    _context__WEBPACK_IMPORTED_MODULE_12__.ContextManager.jupyter_app = app;
+                    _context__WEBPACK_IMPORTED_MODULE_12__.ContextManager.notebook_tracker = notebook_tracker;
+                    _context__WEBPACK_IMPORTED_MODULE_12__.ContextManager.context();
+                    window.ContextManager = _context__WEBPACK_IMPORTED_MODULE_12__.ContextManager; // Left in for development purposes
                 }
 
                 function add_keyboard_shortcuts(app, tool_registry) {
                     app.commands.addCommand("nbtools:insert-tool", {
                         label: 'Insert Notebook Tool',
                         execute: () => {
                             // Open the tool manager, if necessary
                             app.shell.activateById('nbtools-browser');
-                            (0, _utils__WEBPACK_IMPORTED_MODULE_8__.pulse_red)(document.getElementById('nbtools-browser'));
+                            (0, _utils__WEBPACK_IMPORTED_MODULE_9__.pulse_red)(document.getElementById('nbtools-browser'));
                             // If only one tool is available, add it
                             const tools = tool_registry.list();
                             if (tools.length === 1)
-                                _toolbox__WEBPACK_IMPORTED_MODULE_6__.Toolbox.add_tool_cell(tools[0]);
+                                _toolbox__WEBPACK_IMPORTED_MODULE_7__.Toolbox.add_tool_cell(tools[0]);
                             // Otherwise give the search box focus
                             else
                                 document.querySelector('.nbtools-search').focus();
                         },
                     });
                 }
 
                 function add_tool_browser(app, restorer) {
-                    const tool_browser = new _toolbox__WEBPACK_IMPORTED_MODULE_6__.ToolBrowser();
+                    const tool_browser = new _toolbox__WEBPACK_IMPORTED_MODULE_7__.ToolBrowser();
                     tool_browser.title.iconClass = 'nbtools-icon fa fa-th jp-SideBar-tabIcon';
                     tool_browser.title.caption = 'Toolbox';
                     tool_browser.id = 'nbtools-browser';
                     // Add the tool browser widget to the application restorer
                     if (restorer)
                         restorer.add(tool_browser, NAMESPACE);
                     app.shell.add(tool_browser, 'left', {
@@ -196,8 +214,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_plugin_js.9ee79910806137e493ce.js.map
+//# sourceMappingURL=lib_plugin_js.6292de8fa547e3973251.js.map
```

### Comparing `nbtools-23.5.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js.map` & `nbtools-23.7.0/nbtools/labextension/static/lib_plugin_js.6292de8fa547e3973251.js.map`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7857142857142857%*

 * *Differences: {"'file'": "'lib_plugin_js.6292de8fa547e3973251.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAA+D;AACA;AACP;AACX;AACE;AACE;AACA;AACA;AACQ;AACN;AACkB;AACb;AACb;AACkB;AAC7D,mEAAmE,EAAE,wCAAY,GAAG,sCAAgB,GAAG,uCAAiB;AACxH;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,oDAAa,EAAE,yDAAa;AAC3C,eAAe,yEAAsB,EAAE,yEAAgB;AACvD,eAAe,2DAAS,EAAE,qEAAe,EAAE,+DAAS,EAAE,mEAAgB;AACtE;AACA;AACA;AACA,iEAAe,cAAc,EAAC;AAC9B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8BAA8B,mDAAY;AAC1C,8BAA8B,wDAAY;AAC1C;AACA;AACA;AACA;AAC […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "file": "lib_plugin_js.9ee79910806137e493ce.js",
-    "mappings": ";;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAA+D;AACP;AACX;AACE;AACE;AACA;AACA;AACQ;AACN;AACkB;AACb;AACb;AACkB;AAC7D,mEAAmE,EAAE,wCAAY,GAAG,sCAAgB,GAAG,uCAAiB;AACxH;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,oDAAa,EAAE,yDAAa;AAC3C,eAAe,yEAAsB;AACrC,eAAe,2DAAS,EAAE,oEAAe,EAAE,8DAAS,EAAE,mEAAgB;AACtE;AACA;AACA;AACA,iEAAe,cAAc,EAAC;AAC9B;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8BAA8B,mDAAY;AAC1C,8BAA8B,wDAAY;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,cAAc,iDAAW;AACzB,iBAAiB,oDAAc;AAC/B;AACA,KAAK;AACL;AACA,IAAI,qDAAa;AACjB;AACA;AACA;AACA;AACA,IAAI,iEAA0B;AAC9B,IAAI,sEAA+B;AACnC,IAAI,6DAAsB;AAC1B,4BAA4B,qDAAc,CAAC;AAC3C;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,iDAAS;AACrB;AACA;AACA;AACA,gBAAgB,2DAAqB;AACrC;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA,6BAA6B,iDAAW;AACxC;AACA;AACA;AACA;AACA;AACA;AACA,yCAAyC,YAAY;AACrD;AACA;AACA;AACA;AACA,WAAW,oBAAoB;AAC/B,WAAW,UAAU;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA,qCAAqC,oBAAoB,GAAG,yBAAyB;AACrF",
+    "file": "lib_plugin_js.6292de8fa547e3973251.js",
+    "mappings": ";;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAA+D;AACA;AACP;AACX;AACE;AACE;AACA;AACA;AACQ;AACN;AACkB;AACb;AACb;AACkB;AAC7D,mEAAmE,EAAE,wCAAY,GAAG,sCAAgB,GAAG,uCAAiB;AACxH;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,oDAAa,EAAE,yDAAa;AAC3C,eAAe,yEAAsB,EAAE,yEAAgB;AACvD,eAAe,2DAAS,EAAE,qEAAe,EAAE,+DAAS,EAAE,mEAAgB;AACtE;AACA;AACA;AACA,iEAAe,cAAc,EAAC;AAC9B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8BAA8B,mDAAY;AAC1C,8BAA8B,wDAAY;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,cAAc,iDAAW;AACzB,iBAAiB,oDAAc;AAC/B;AACA,KAAK;AACL;AACA,IAAI,qDAAa;AACjB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY;AACZ;AACA;AACA,IAAI,iEAA0B;AAC9B,IAAI,sEAA+B;AACnC,IAAI,6DAAsB;AAC1B,4BAA4B,qDAAc,CAAC;AAC3C;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,iDAAS;AACrB;AACA;AACA;AACA,gBAAgB,2DAAqB;AACrC;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA,6BAA6B,iDAAW;AACxC;AACA;AACA;AACA;AACA;AACA;AACA,yCAAyC,YAAY;AACrD;AACA;AACA;AACA;AACA,WAAW,oBAAoB;AAC/B,WAAW,UAAU;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA,qCAAqC,oBAAoB,GAAG,yBAAyB;AACrF",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@g2nb/nbtools/./lib/plugin.js"
     ],
     "sourcesContent": [
-        "import { IJupyterWidgetRegistry } from '@jupyter-widgets/base';\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport * as base_exports from './basewidget';\nimport * as uioutput_exports from './uioutput';\nimport * as uibuilder_exports from './uibuilder';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { ToolBrowser, Toolbox } from \"./toolbox\";\nimport { IToolRegistry, ToolRegistry } from \"./registry\";\nimport { pulse_red, usage_tracker } from \"./utils\";\nimport { ILabShell, ILayoutRestorer } from \"@jupyterlab/application\";\nimport { INotebookTracker } from '@jupyterlab/notebook';\nimport { ContextManager } from \"./context\";\nimport { DataRegistry, IDataRegistry } from \"./dataregistry\";\nconst module_exports = Object.assign(Object.assign(Object.assign({}, base_exports), uioutput_exports), uibuilder_exports);\nconst EXTENSION_ID = '@g2nb/nbtools:plugin';\nconst NAMESPACE = 'nbtools';\n/**\n * The nbtools plugin.\n */\nconst nbtools_plugin = {\n    id: EXTENSION_ID,\n    provides: [IToolRegistry, IDataRegistry],\n    requires: [IJupyterWidgetRegistry],\n    optional: [IMainMenu, ILayoutRestorer, ILabShell, INotebookTracker],\n    activate: activate_widget_extension,\n    autoStart: true\n};\nexport default nbtools_plugin;\n/**\n * Activate the widget extension.\n */\nfunction activate_widget_extension(app, widget_registry, mainmenu, restorer, shell, notebook_tracker) {\n    // Initialize the ContextManager\n    init_context(app, notebook_tracker);\n    // Create the tool and data registries\n    const tool_registry = new ToolRegistry();\n    const data_registry = new DataRegistry();\n    // Add items to the help menu\n    add_help_links(app, mainmenu);\n    // Add keyboard shortcuts\n    add_keyboard_shortcuts(app, tool_registry);\n    // Add the toolbox\n    add_tool_browser(app, restorer);\n    // Register the nbtools widgets with the widget registry\n    widget_registry.registerWidget({\n        name: MODULE_NAME,\n        version: MODULE_VERSION,\n        exports: module_exports,\n    });\n    // Register the plugin as loaded\n    usage_tracker('labextension_load', location.protocol + '//' + location.host + location.pathname);\n    // Return the tool registry so that it is provided to other extensions\n    return [tool_registry, data_registry];\n}\nfunction init_context(app, notebook_tracker) {\n    ContextManager.jupyter_app = app;\n    ContextManager.notebook_tracker = notebook_tracker;\n    ContextManager.context();\n    window.ContextManager = ContextManager; // Left in for development purposes\n}\nfunction add_keyboard_shortcuts(app, tool_registry) {\n    app.commands.addCommand(\"nbtools:insert-tool\", {\n        label: 'Insert Notebook Tool',\n        execute: () => {\n            // Open the tool manager, if necessary\n            app.shell.activateById('nbtools-browser');\n            pulse_red(document.getElementById('nbtools-browser'));\n            // If only one tool is available, add it\n            const tools = tool_registry.list();\n            if (tools.length === 1)\n                Toolbox.add_tool_cell(tools[0]);\n            // Otherwise give the search box focus\n            else\n                document.querySelector('.nbtools-search').focus();\n        },\n    });\n}\nfunction add_tool_browser(app, restorer) {\n    const tool_browser = new ToolBrowser();\n    tool_browser.title.iconClass = 'nbtools-icon fa fa-th jp-SideBar-tabIcon';\n    tool_browser.title.caption = 'Toolbox';\n    tool_browser.id = 'nbtools-browser';\n    // Add the tool browser widget to the application restorer\n    if (restorer)\n        restorer.add(tool_browser, NAMESPACE);\n    app.shell.add(tool_browser, 'left', { rank: 102 });\n}\n/**\n * Add the nbtools documentation and feedback links to the help menu\n *\n * @param {Application<Widget>} app\n * @param {IMainMenu} mainmenu\n */\nfunction add_help_links(app, mainmenu) {\n    const feedback = 'nbtools:feedback';\n    const documentation = 'nbtools:documentation';\n    // Add feedback command to the command palette\n    app.commands.addCommand(feedback, {\n        label: 'g2nb Help Forum',\n        caption: 'Open the g2nb help forum',\n        isEnabled: () => !!app.shell,\n        execute: () => {\n            const url = 'https://community.mesirovlab.org/c/g2nb/';\n            let element = document.createElement('a');\n            element.href = url;\n            element.target = '_blank';\n            document.body.appendChild(element);\n            element.click();\n            document.body.removeChild(element);\n            return void 0;\n        }\n    });\n    // Add documentation command to the command palette\n    app.commands.addCommand(documentation, {\n        label: 'nbtools Documentation',\n        caption: 'Open documentation for nbtools',\n        isEnabled: () => !!app.shell,\n        execute: () => {\n            const url = 'https://github.com/g2nb/nbtools#nbtools';\n            let element = document.createElement('a');\n            element.href = url;\n            element.target = '_blank';\n            document.body.appendChild(element);\n            element.click();\n            document.body.removeChild(element);\n            return void 0;\n        }\n    });\n    // Add documentation link to the help menu\n    if (mainmenu)\n        mainmenu.helpMenu.addGroup([{ command: feedback }, { command: documentation }], 2);\n}\n"
+        "import { IJupyterWidgetRegistry } from '@jupyter-widgets/base';\nimport { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport * as base_exports from './basewidget';\nimport * as uioutput_exports from './uioutput';\nimport * as uibuilder_exports from './uibuilder';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { ToolBrowser, Toolbox } from \"./toolbox\";\nimport { IToolRegistry, ToolRegistry } from \"./registry\";\nimport { pulse_red, usage_tracker } from \"./utils\";\nimport { ILabShell, ILayoutRestorer } from \"@jupyterlab/application\";\nimport { INotebookTracker } from '@jupyterlab/notebook';\nimport { ContextManager } from \"./context\";\nimport { DataRegistry, IDataRegistry } from \"./dataregistry\";\nconst module_exports = Object.assign(Object.assign(Object.assign({}, base_exports), uioutput_exports), uibuilder_exports);\nconst EXTENSION_ID = '@g2nb/nbtools:plugin';\nconst NAMESPACE = 'nbtools';\n/**\n * The nbtools plugin.\n */\nconst nbtools_plugin = {\n    id: EXTENSION_ID,\n    provides: [IToolRegistry, IDataRegistry],\n    requires: [IJupyterWidgetRegistry, ISettingRegistry],\n    optional: [IMainMenu, ILayoutRestorer, ILabShell, INotebookTracker],\n    activate: activate_widget_extension,\n    autoStart: true\n};\nexport default nbtools_plugin;\n/**\n * Activate the widget extension.\n */\nasync function activate_widget_extension(app, widget_registry, settings, mainmenu, restorer, shell, notebook_tracker) {\n    // Initialize the ContextManager\n    init_context(app, notebook_tracker);\n    // Initialize settings\n    const setting_dict = await init_settings(settings);\n    // Create the tool and data registries\n    const tool_registry = new ToolRegistry(setting_dict);\n    const data_registry = new DataRegistry();\n    // Add items to the help menu\n    add_help_links(app, mainmenu);\n    // Add keyboard shortcuts\n    add_keyboard_shortcuts(app, tool_registry);\n    // Add the toolbox\n    add_tool_browser(app, restorer);\n    // Register the nbtools widgets with the widget registry\n    widget_registry.registerWidget({\n        name: MODULE_NAME,\n        version: MODULE_VERSION,\n        exports: module_exports,\n    });\n    // Register the plugin as loaded\n    usage_tracker('labextension_load', location.protocol + '//' + location.host + location.pathname);\n    // Return the tool registry so that it is provided to other extensions\n    return [tool_registry, data_registry];\n}\nasync function init_settings(settings) {\n    let setting = null;\n    try {\n        setting = await settings.load(EXTENSION_ID);\n    }\n    catch (_a) {\n        console.log('Unable to load nbtools settings');\n    }\n    return { force_render: setting ? setting.get('force_render').composite : true };\n}\nfunction init_context(app, notebook_tracker) {\n    ContextManager.jupyter_app = app;\n    ContextManager.notebook_tracker = notebook_tracker;\n    ContextManager.context();\n    window.ContextManager = ContextManager; // Left in for development purposes\n}\nfunction add_keyboard_shortcuts(app, tool_registry) {\n    app.commands.addCommand(\"nbtools:insert-tool\", {\n        label: 'Insert Notebook Tool',\n        execute: () => {\n            // Open the tool manager, if necessary\n            app.shell.activateById('nbtools-browser');\n            pulse_red(document.getElementById('nbtools-browser'));\n            // If only one tool is available, add it\n            const tools = tool_registry.list();\n            if (tools.length === 1)\n                Toolbox.add_tool_cell(tools[0]);\n            // Otherwise give the search box focus\n            else\n                document.querySelector('.nbtools-search').focus();\n        },\n    });\n}\nfunction add_tool_browser(app, restorer) {\n    const tool_browser = new ToolBrowser();\n    tool_browser.title.iconClass = 'nbtools-icon fa fa-th jp-SideBar-tabIcon';\n    tool_browser.title.caption = 'Toolbox';\n    tool_browser.id = 'nbtools-browser';\n    // Add the tool browser widget to the application restorer\n    if (restorer)\n        restorer.add(tool_browser, NAMESPACE);\n    app.shell.add(tool_browser, 'left', { rank: 102 });\n}\n/**\n * Add the nbtools documentation and feedback links to the help menu\n *\n * @param {Application<Widget>} app\n * @param {IMainMenu} mainmenu\n */\nfunction add_help_links(app, mainmenu) {\n    const feedback = 'nbtools:feedback';\n    const documentation = 'nbtools:documentation';\n    // Add feedback command to the command palette\n    app.commands.addCommand(feedback, {\n        label: 'g2nb Help Forum',\n        caption: 'Open the g2nb help forum',\n        isEnabled: () => !!app.shell,\n        execute: () => {\n            const url = 'https://community.mesirovlab.org/c/g2nb/';\n            let element = document.createElement('a');\n            element.href = url;\n            element.target = '_blank';\n            document.body.appendChild(element);\n            element.click();\n            document.body.removeChild(element);\n            return void 0;\n        }\n    });\n    // Add documentation command to the command palette\n    app.commands.addCommand(documentation, {\n        label: 'nbtools Documentation',\n        caption: 'Open documentation for nbtools',\n        isEnabled: () => !!app.shell,\n        execute: () => {\n            const url = 'https://github.com/g2nb/nbtools#nbtools';\n            let element = document.createElement('a');\n            element.href = url;\n            element.target = '_blank';\n            document.body.appendChild(element);\n            element.click();\n            document.body.removeChild(element);\n            return void 0;\n        }\n    });\n    // Add documentation link to the help menu\n    if (mainmenu)\n        mainmenu.helpMenu.addGroup([{ command: feedback }, { command: documentation }], 2);\n}\n"
     ],
     "version": 3
 }
```

### Comparing `nbtools-23.5.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js` & `nbtools-23.7.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.cd289910d38270a1d73e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -156,14 +156,16 @@
                         // Attach the gear event
                         const gear = this.element.querySelector("button.nbtools-gear");
                         gear.addEventListener("click", () => this.toggle_menu());
                         // Attach toggle code event
                         this.add_menu_item('Toggle Code View', () => this.toggle_code());
                         // Apply the body
                         this.element.querySelector('div.nbtools-body').innerHTML = this.body;
+                        // Add the metadata flag
+                        this.update_metadata();
                         // Attach the disconnected cover
                         this.element.appendChild(new DOMParser().parseFromString(this.disconnected, "text/html")
                             .querySelector('body > :first-child'));
                         this.attach_connect_event();
                         this.disconnected_sync_fix();
                         // Set the element
                         this.setElement(this.element);
@@ -209,14 +211,31 @@
                     attach_connect_event() {
                         const button = this.element.querySelector('button.nbtools-connect');
                         button.addEventListener("click", () => {
                             // Run all cells with disconnected nbtools widgets
                             _context__WEBPACK_IMPORTED_MODULE_1__.ContextManager.context().run_tool_cells();
                         });
                     }
+                    /**
+                     * Update the cell metadata with the nbtools flag
+                     */
+                    update_metadata() {
+                        if (!_context__WEBPACK_IMPORTED_MODULE_1__.ContextManager.notebook_tracker)
+                            return;
+                        if (!_context__WEBPACK_IMPORTED_MODULE_1__.ContextManager.notebook_tracker.currentWidget)
+                            return;
+                        const cells = _context__WEBPACK_IMPORTED_MODULE_1__.ContextManager.notebook_tracker.currentWidget.content.widgets;
+                        for (let i = 0; i < cells.length; i++) {
+                            const execution_area = cells[i].node.querySelector('.lm-Widget.p-Widget.jp-InputPrompt.jp-InputArea-prompt');
+                            if (execution_area.innerText.includes('[*]')) {
+                                _context__WEBPACK_IMPORTED_MODULE_1__.ContextManager.context().make_tool_cell(cells[i]);
+                                return;
+                            }
+                        }
+                    }
                     disconnected_sync_fix() {
                         // Fix a bug that can occur when a disconnected widget and a connected widget are somehow rendered in the same cell
                         setTimeout(() => {
                             const cell = this.element.closest('.jp-Cell, .cell');
                             if (!cell)
                                 return; // No cell found, bug cannot occur
                             // Do both connected and disconnected widgets appear in the cell?
@@ -545,14 +564,18 @@
                     /**
                      * Determines if the given cell contains a notebook tool widget
                      *
                      * @param cell
                      * @returns boolean
                      */
                     is_tool_cell(cell) {
+                        // Check for nbtools metadata
+                        if (cell.model.metadata.get('nbtools'))
+                            return true;
+                        // Check for an existing disconnected nbtools widget
                         const dom_node = cell.node || cell.element;
                         if (!!dom_node)
                             return !!dom_node.querySelector('.nbtools');
                         else
                             return false;
                     }
                     /**
@@ -644,14 +667,28 @@
                     create_comm(current, name, callback) {
                         const kernel = current.context.sessionContext.session.kernel;
                         const comm = kernel.createComm(name);
                         comm.onMsg = callback;
                         comm.open({}); // Open the comm
                         return comm;
                     }
+                    /**
+                     * Sets whether this is a nbtools widget cell
+                     *
+                     * @param cell
+                     * @param is_widget_cell
+                     */
+                    make_tool_cell(cell, is_widget_cell = true) {
+                        if (is_widget_cell)
+                            cell.model.metadata.set('nbtools', {
+                                'force_display': true
+                            });
+                        else
+                            cell.model.metadata.clear();
+                    }
                 }
                 /**
                  * Context handler for the classic Jupyter Notebook
                  */
                 class NotebookContext extends Context {
                     /**
                      * Toggle hiding or or showing the code for the specified cell
@@ -712,14 +749,29 @@
                         const dom_node = cell.node || cell.element;
                         if (!!dom_node)
                             return !!dom_node.find('.nbtools').length;
                         else
                             return false;
                     }
                     /**
+                     * Sets whether this is a nbtools widget cell
+                     *
+                     * @param cell
+                     * @param is_widget_cell
+                     */
+                    make_tool_cell(cell, is_widget_cell = true) {
+                        // TODO: Test in Jupyter Notebook
+                        if (is_widget_cell)
+                            cell.metadata.set('nbtools', {
+                                'force_display': true
+                            });
+                        else
+                            cell.metadata.clear();
+                    }
+                    /**
                      * Path to the default GenePattern logo
                      */
                     default_logo() {
                         return this.base_path() + __webpack_require__( /*! ../style/g2nb_logo.png */ "./style/g2nb_logo.png").default;
                     }
                     /**
                      * Path to the default GenePattern icon
@@ -823,14 +875,29 @@
                     base_path() {
                         const body = document.querySelector('body');
                         if (!body)
                             return ''; // If there is no body, unable to get path
                         return body.getAttribute('data-base-url') + 'nbextensions/nbtools/';
                     }
                     /**
+                     * Sets whether this is a nbtools widget cell
+                     *
+                     * @param cell
+                     * @param is_widget_cell
+                     */
+                    make_tool_cell(cell, is_widget_cell = true) {
+                        // TODO: Test in embedded context
+                        if (is_widget_cell)
+                            cell.metadata.set('nbtools', {
+                                'force_display': true
+                            });
+                        else
+                            cell.metadata.clear();
+                    }
+                    /**
                      * Determines if the given cell contains a notebook tool widget
                      *
                      * @param cell
                      * @returns boolean
                      */
                     is_tool_cell(cell) {
                         const dom_node = cell.node || cell.element;
@@ -1124,15 +1191,15 @@
 
 
                 const IToolRegistry = new _lumino_coreutils__WEBPACK_IMPORTED_MODULE_3__.Token("nbtools");
                 class ToolRegistry {
                     /**
                      * Initialize the ToolRegistry and connect event handlers
                      */
-                    constructor() {
+                    constructor(setting_dict) {
                         this.current = null; // Reference to the currently selected notebook or other widget
                         this._update_callbacks = []; // Functions to call when an update happens
                         this.kernel_tool_cache = {}; // Keep a cache of kernels to registered tools
                         this.kernel_import_cache = {}; // Keep a cache of whether nbtools has been imported
                         // Lazily assign the tool registry to the context
                         if (!_context__WEBPACK_IMPORTED_MODULE_2__.ContextManager.tool_registry)
                             _context__WEBPACK_IMPORTED_MODULE_2__.ContextManager.tool_registry = this;
@@ -1145,14 +1212,24 @@
                             // If the current selected widget isn't a notebook, no comm is needed
                             if (!(this.current instanceof _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0__.NotebookPanel) && _context__WEBPACK_IMPORTED_MODULE_2__.ContextManager.is_lab())
                                 return;
                             // Initialize the comm
                             this.init_comm();
                             // Load the default tools
                             this.import_default_tools();
+                            // Ensure rendering of tool cells
+                            if (setting_dict.force_render)
+                                this.ensure_rendering();
+                        });
+                    }
+                    ensure_rendering() {
+                        _context__WEBPACK_IMPORTED_MODULE_2__.ContextManager.context().kernel_ready(this.current, () => {
+                            if (!this.current)
+                                return; // Return if no notebook is selected
+                            _context__WEBPACK_IMPORTED_MODULE_2__.ContextManager.context().run_tool_cells();
                         });
                     }
                     import_default_tools() {
                         _context__WEBPACK_IMPORTED_MODULE_2__.ContextManager.context().kernel_changed(this.current, () => {
                             _context__WEBPACK_IMPORTED_MODULE_2__.ContextManager.context().execute_code(this.current, 'from nbtools import import_defaults\nimport_defaults()');
                         });
                     }
@@ -3084,15 +3161,15 @@
             /*!**********************!*\
               !*** ./package.json ***!
               \**********************/
             /***/
             ((module) => {
 
                 "use strict";
-                module.exports = JSON.parse("{\"name\":\"@g2nb/nbtools\",\"version\":\"23.3.2\",\"description\":\"Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike.\",\"keywords\":[\"jupyter\",\"jupyterlab\",\"jupyterlab-extension\",\"widgets\"],\"files\":[\"lib/**/*.{js,css}\",\"style/*.{js,css,png,svg}\",\"schema/**/*.json\",\"dist/*.{js,css}\",\"style/index.js\"],\"homepage\":\"https://github.com/g2nb/nbtools\",\"bugs\":{\"url\":\"https://github.com/g2nb/nbtools/issues\"},\"license\":\"BSD-3-Clause\",\"author\":{\"name\":\"Thorin Tabor\",\"email\":\"tmtabor@cloud.ucsd.edu\"},\"main\":\"lib/index.js\",\"types\":\"./lib/index.d.ts\",\"style\":\"style/index.css\",\"repository\":{\"type\":\"git\",\"url\":\"https://github.com/g2nb/nbtools\"},\"scripts\":{\"build\":\"jlpm run build:lib && jlpm run build:labextension:dev\",\"build:all\":\"jlpm run build:lib && jlpm run build:labextension && jlpm run build:nbextension\",\"build:labextension\":\"jupyter labextension build .\",\"build:labextension:dev\":\"jupyter labextension build --development True .\",\"build:lib\":\"tsc\",\"build:nbextension\":\"webpack --mode production\",\"clean\":\"jlpm run clean:lib\",\"clean:all\":\"jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension\",\"clean:labextension\":\"rimraf nbtools/labextension\",\"clean:lib\":\"rimraf lib tsconfig.tsbuildinfo\",\"clean:nbextension\":\"rimraf nbtools/nbextension/static/index.js\",\"eslint\":\"eslint . --ext .ts,.tsx --fix\",\"eslint:check\":\"eslint . --ext .ts,.tsx\",\"install:extension\":\"jlpm run build\",\"prepack\":\"jlpm run build:lib\",\"prepare\":\"jlpm run clean && jlpm run build:all\",\"test\":\"jlpm run test:firefox\",\"test:chrome\":\"karma start --browsers=Chrome tests/karma.conf.js\",\"test:debug\":\"karma start --browsers=Chrome --singleRun=false --debug=true tests/karma.conf.js\",\"test:firefox\":\"karma start --browsers=Firefox tests/karma.conf.js\",\"test:ie\":\"karma start --browsers=IE tests/karma.conf.js\",\"watch\":\"run-p watch:src watch:labextension\",\"watch:labextension\":\"jupyter labextension watch .\",\"watch:lib\":\"tsc -w\",\"watch:nbextension\":\"webpack --watch\",\"watch:src\":\"tsc -w\"},\"dependencies\":{\"@jupyter-widgets/base\":\"^6\",\"@jupyterlab/application\":\"^3.0.4\",\"@jupyterlab/mainmenu\":\"^3.0.3\",\"@jupyterlab/notebook\":\"^3.0.4\",\"yarn\":\"^1.22.19\"},\"devDependencies\":{\"@jupyterlab/apputils\":\"^3.0.3\",\"@jupyterlab/builder\":\"^3.0.0\",\"@jupyterlab/ui-components\":\"^3.0.3\",\"@lumino/application\":\"^1.13.1\",\"@lumino/widgets\":\"^1.16.1\",\"@types/backbone\":\"^1.4.4\",\"@types/node\":\"^14.14.27\",\"@typescript-eslint/eslint-plugin\":\"^4.8.1\",\"@typescript-eslint/parser\":\"^4.8.1\",\"backbone\":\"^1.2.3\",\"css-loader\":\"^5.2.7\",\"eslint\":\"^7.14.0\",\"eslint-config-prettier\":\"^6.15.0\",\"eslint-plugin-prettier\":\"^3.1.4\",\"expect.js\":\"^0.3.1\",\"file-loader\":\"^6.2.0\",\"fs-extra\":\"^9.1.0\",\"karma\":\"^6.1.1\",\"karma-typescript\":\"^5.3.0\",\"mkdirp\":\"^1.0.4\",\"mocha\":\"^8.3.0\",\"npm-run-all\":\"^4.1.5\",\"prettier\":\"^2.1.1\",\"rimraf\":\"^3.0.2\",\"source-map-loader\":\"^2.0.1\",\"style-loader\":\"^2.0.0\",\"ts-loader\":\"^8.0.17\",\"typescript\":\"~4.1.3\",\"webpack\":\"^5.21.2\",\"webpack-cli\":\"^4.5.0\"},\"jupyterlab\":{\"extension\":\"lib/plugin\",\"schemaDir\":\"schema\",\"sharedPackages\":{\"@jupyter-widgets/base\":{\"bundled\":false,\"singleton\":true}},\"discovery\":{\"kernel\":[{\"kernel_spec\":{\"language\":\"^python\"},\"base\":{\"name\":\"nbtools\"},\"managers\":[\"pip\",\"conda\"]}]},\"outputDir\":\"nbtools/labextension\"},\"styleModule\":\"style/index.js\"}");
+                module.exports = JSON.parse("{\"name\":\"@g2nb/nbtools\",\"version\":\"23.5.0\",\"description\":\"Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike.\",\"keywords\":[\"jupyter\",\"jupyterlab\",\"jupyterlab-extension\",\"widgets\"],\"files\":[\"lib/**/*.{js,css}\",\"style/*.{js,css,png,svg}\",\"schema/**/*.json\",\"dist/*.{js,css}\",\"style/index.js\"],\"homepage\":\"https://github.com/g2nb/nbtools\",\"bugs\":{\"url\":\"https://github.com/g2nb/nbtools/issues\"},\"license\":\"BSD-3-Clause\",\"author\":{\"name\":\"Thorin Tabor\",\"email\":\"tmtabor@cloud.ucsd.edu\"},\"main\":\"lib/index.js\",\"types\":\"./lib/index.d.ts\",\"style\":\"style/index.css\",\"repository\":{\"type\":\"git\",\"url\":\"https://github.com/g2nb/nbtools\"},\"scripts\":{\"build\":\"jlpm run build:lib && jlpm run build:labextension:dev\",\"build:all\":\"jlpm run build:lib && jlpm run build:labextension && jlpm run build:nbextension\",\"build:labextension\":\"jupyter labextension build .\",\"build:labextension:dev\":\"jupyter labextension build --development True .\",\"build:lib\":\"tsc\",\"build:nbextension\":\"webpack --mode production\",\"clean\":\"jlpm run clean:lib\",\"clean:all\":\"jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension\",\"clean:labextension\":\"rimraf nbtools/labextension\",\"clean:lib\":\"rimraf lib tsconfig.tsbuildinfo\",\"clean:nbextension\":\"rimraf nbtools/nbextension/static/index.js\",\"eslint\":\"eslint . --ext .ts,.tsx --fix\",\"eslint:check\":\"eslint . --ext .ts,.tsx\",\"install:extension\":\"jlpm run build\",\"prepack\":\"jlpm run build:lib\",\"prepare\":\"jlpm run clean && jlpm run build:all\",\"test\":\"jlpm run test:firefox\",\"test:chrome\":\"karma start --browsers=Chrome tests/karma.conf.js\",\"test:debug\":\"karma start --browsers=Chrome --singleRun=false --debug=true tests/karma.conf.js\",\"test:firefox\":\"karma start --browsers=Firefox tests/karma.conf.js\",\"test:ie\":\"karma start --browsers=IE tests/karma.conf.js\",\"watch\":\"run-p watch:src watch:labextension\",\"watch:labextension\":\"jupyter labextension watch .\",\"watch:lib\":\"tsc -w\",\"watch:nbextension\":\"webpack --watch\",\"watch:src\":\"tsc -w\"},\"dependencies\":{\"@jupyter-widgets/base\":\"^6\",\"@jupyterlab/application\":\"^3.0.4\",\"@jupyterlab/mainmenu\":\"^3.0.3\",\"@jupyterlab/notebook\":\"^3.0.4\"},\"devDependencies\":{\"@jupyterlab/apputils\":\"^3.0.3\",\"@jupyterlab/builder\":\"^3.0.0\",\"@jupyterlab/ui-components\":\"^3.0.3\",\"@lumino/application\":\"^1.13.1\",\"@lumino/widgets\":\"^1.16.1\",\"@types/backbone\":\"^1.4.4\",\"@types/node\":\"^14.14.27\",\"@typescript-eslint/eslint-plugin\":\"^4.8.1\",\"@typescript-eslint/parser\":\"^4.8.1\",\"backbone\":\"^1.2.3\",\"css-loader\":\"^5.2.7\",\"eslint\":\"^7.14.0\",\"eslint-config-prettier\":\"^6.15.0\",\"eslint-plugin-prettier\":\"^3.1.4\",\"expect.js\":\"^0.3.1\",\"file-loader\":\"^6.2.0\",\"fs-extra\":\"^9.1.0\",\"karma\":\"^6.1.1\",\"karma-typescript\":\"^5.3.0\",\"mkdirp\":\"^1.0.4\",\"mocha\":\"^8.3.0\",\"npm-run-all\":\"^4.1.5\",\"prettier\":\"^2.1.1\",\"rimraf\":\"^3.0.2\",\"source-map-loader\":\"^2.0.1\",\"style-loader\":\"^2.0.0\",\"ts-loader\":\"^8.0.17\",\"typescript\":\"~4.1.3\",\"webpack\":\"^5.21.2\",\"webpack-cli\":\"^4.5.0\"},\"jupyterlab\":{\"extension\":\"lib/plugin\",\"schemaDir\":\"schema\",\"sharedPackages\":{\"@jupyter-widgets/base\":{\"bundled\":false,\"singleton\":true}},\"discovery\":{\"kernel\":[{\"kernel_spec\":{\"language\":\"^python\"},\"base\":{\"name\":\"nbtools\"},\"managers\":[\"pip\",\"conda\"]}]},\"outputDir\":\"nbtools/labextension\"},\"styleModule\":\"style/index.js\"}");
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js.map
+//# sourceMappingURL=lib_registry_js-lib_uibuilder_js-lib_uioutput_js.cd289910d38270a1d73e.js.map
```

### Comparing `nbtools-23.5.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js.map` & `nbtools-23.7.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.cd289910d38270a1d73e.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8319327731092436%*

 * *Differences: {"'file'": "'lib_registry_js-lib_uibuilder_js-lib_uioutput_js.cd289910d38270a1d73e.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;;;;AAAiC;AACU;AACQ;AAC2B;AACtB;AACpB;AACpC;AACO,8BAA8B,iEAAc;AACnD;AACA,6CAA6C,sBAAsB,yHAAyH,4DAAsB,4DAA4D,EAAE;AAChR;AACA;AACA;AACA,+BAA+B,iDAAW;AAC1C,uCAAuC,oDAAc;AACrD;AACA,8BAA8B,iDAAW;AACzC,sCAAsC,oDAAc;AACpD,8CAA8C,EAAE,6EAA0B;AAC1E;AACO,6BAA6B,gEAAa;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA, […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js",
-    "mappings": ";;;;;;;;;;;;;;;;;;;;;AAAiC;AACU;AACQ;AAC2B;AACtB;AACpB;AACpC;AACO,8BAA8B,iEAAc;AACnD;AACA,6CAA6C,sBAAsB,yHAAyH,4DAAsB,4DAA4D,EAAE;AAChR;AACA;AACA;AACA,+BAA+B,iDAAW;AAC1C,uCAAuC,oDAAc;AACrD;AACA,8BAA8B,iDAAW;AACzC,sCAAsC,oDAAc;AACpD,8CAA8C,EAAE,6EAA0B;AAC1E;AACO,6BAA6B,gEAAa;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uEAAuE;AACvE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mEAAmE,SAAS;AAC5E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,yBAAyB,YAAY,EAAE;AACvC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB,4DAAsB;AACzC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,4DAAsB;AAClC,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA,SAAS;AACT;AACA;AACA;AACA,4DAA4D,MAAM;AAClE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,yEAAyE,KAAK;AAC9E;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA,QAAQ,4DAAsB;AAC9B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,8CAAM;AACd;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iDAAiD;AACjD;AACA;AACA,gCAAgC,wDAAgB;AAChD;AACA;AACA,8BAA8B,wDAAgB;AAC9C;AACA;AACA,yBAAyB,2DAAqB,CAAC,wDAAgB;AAC/D;AACA;AACA;AACA;AACA,+BAA+B,0BAA0B,wDAAgB,+BAA+B;AACxG;AACA,+BAA+B,0BAA0B,wDAAgB,uCAAuC,wDAAgB,iCAAiC;AACjK;AACA;AACA;AACA,gCAAgC,wDAAgB;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,qDAAqD,aAAa;AAClE;AACA;AACA;AACA;AACA,eAAe,eAAe;AAC9B,eAAe,oBAAoB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb;AACA;AACA;AACA;AACA;AACA,eAAe,OAAO;AACtB,eAAe,OAAO;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS,QAAQ,6DAAM,kBAAkB,WAAW,MAAM,iBAAiB;AAC3E;AACA,cAAc,uBAAuB,EAAE;AACvC,mBAAmB,EAAE;AACrB;;;;;;;;;;;;;;;;;;;;;AChV6C;AACQ;AACR;AACtC;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB;AAClB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,YAAY;AAC3B,eAAe,QAAQ;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,4CAAI;AACpB;AACA,gBAAgB,4CAAI;AACpB;AACA,gBAAgB,8CAAM;AACtB,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA,4BAA4B,uDAAQ;AACpC;AACA;AACA,gBAAgB,+DAAgB;AAChC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB;AACtB;AACA,sBAAsB;AACtB;AACA,sBAAsB;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kFAAyC;AACxD;AACA;AACA;AACA;AACA;AACA,eAAe,wEAAoC;AACnD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,+DAAa;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC,+DAAa;AAC9C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA,sEAAsE,aAAa;AACnF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,EAAE;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,YAAY;AAC3B,eAAe,QAAQ;AACvB;AACA;AACA;AACA;AACA;AACA,uBAAuB;AACvB;AACA;AACA;AACA,gBAAgB,4CAAI;AACpB;AACA,gBAAgB,4CAAI;AACpB;AACA,gBAAgB,8CAAM;AACtB,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,kFAAyC;AAC3E;AACA;AACA;AACA;AACA;AACA,kCAAkC,wEAAoC;AACtE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,YAAY;AAC3B,eAAe,QAAQ;AACvB;AACA,mCAAmC;AACnC;AACA;AACA;AACA;AACA,oBAAoB;AACpB;AACA;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA,qBAAqB,WAAW;AAChC;AACA;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,kFAAyC;AAC3E;AACA;AACA;AACA;AACA;AACA,eAAe,wEAAoC;AACnD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8BAA8B;AAC9B;AACA;AACA;AACA;AACA;AACA;AACA,qCAAqC;AACrC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;AC/d2C;AACD;AACqB;AACxD,0BAA0B,oDAAK;AAC/B;AACP,QAAQ,eAAe,YAAY,qBAAqB,EAAE;AAC1D;AACA;AACA;AACA;AACA,4BAA4B;AAC5B,oCAAoC;AACpC;AACA,aAAa,kEAA4B;AACzC,YAAY,kEAA4B;AACxC,QAAQ,4DAAsB;AAC9B;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,cAAc,sDAAsD;AACpE;AACA;AACA;AACA;AACA;AACA,yBAAyB;AACzB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,sDAAsD;AACtE;AACA;AACA;AACA;AACA;AACA,wBAAwB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,cAAc,+BAA+B;AAC7C;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,4DAAsB;AACrC;AACA;AACO;AACP;AACA;AACA;AACA,uCAAuC,yDAAiB;AACxD,oCAAoC,yDAAiB;AACrD;AACA;;;;;;;;;;;;;;;;;;;;;;;ACjIqD;AACT;AACD;AACD;AACnC,0BAA0B,oDAAK;AAC/B;AACP;AACA;AACA;AACA;AACA,4BAA4B;AAC5B,oCAAoC;AACpC,oCAAoC;AACpC,sCAAsC;AACtC;AACA,aAAa,kEAA4B;AACzC,YAAY,kEAA4B;AACxC,QAAQ,4DAAsB;AAC9B;AACA;AACA;AACA;AACA;AACA;AACA,0CAA0C,+DAAa,KAAK,2DAAqB;AACjF;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA,QAAQ,4DAAsB;AAC9B,YAAY,4DAAsB;AAClC,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,QAAQ,4DAAsB;AAC9B;AACA;AACA;AACA,6BAA6B,4DAAsB;AACnD;AACA;AACA;AACA;AACA;AACA,wBAAwB,yDAAiB,4CAA4C,4DAAsB;AAC3G;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA,YAAY,4DAAsB;AAClC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB,2BAA2B;AAC9C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,4DAAsB;AACrC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wBAAwB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB,MAAM;AACvB;AACA;AACA;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACzKsD;AACrB;AACU;AAC2B;AAC/D,0BAA0B,mDAAM;AACvC;AACA;AACA;AACA;AACA;AACA,0BAA0B,wDAAW;AACrC;AACA;AACA;AACA;AACA;AACA;AACO,sBAAsB,mDAAM;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,4EAAsC;AAC9C;AACA;AACA;AACA;AACA,oCAAoC;AACpC,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oCAAoC;AACpC,4CAA4C;AAC5C,aAAa,wDAAwD;AACrE,uCAAuC;AACvC;AACA;AACA;AACA;AACA,4BAA4B,+EAAyC;AACrE;AACA,gEAAgE,QAAQ,aAAa,YAAY;AACjG;AACA;AACA,aAAa,qEAA+B;AAC5C,mBAAmB;AACnB,wBAAwB,0EAAoC;AAC5D,6CAA6C,+DAAa;AAC1D,mBAAmB;AACnB,mBAAmB,gFAA0C;AAC7D;AACA,mBAAmB;AACnB;AACA;AACA;AACA,YAAY,6EAA2B;AACvC;AACA,eAAe,gFAA0C,CAAC;AAC1D;AACA;AACA;AACA,eAAe,qEAAmB;AAClC;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB,uEAAiC;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kDAAkD;AAClD;AACA,gDAAgD;AAChD,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oDAAoD,KAAK;AACzD;AACA,kBAAkB;AAClB;AACA,gDAAgD,KAAK;AACrD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0CAA0C,UAAU;AACpD,+CAA+C,iBAAiB;AAChE;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,8CAAM;AACd;AACA;AACO,wBAAwB,mDAAM;AACrC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;;;;;;;;AC5MA;AACA;AACA;AACA;AACA;AACA;AACA;AACgC;AACwB;AACF;AACS;AACZ;AACR;AAC3C;AACO,6BAA6B,wDAAe;AACnD;AACA,6CAA6C,sBAAsB,ocAAoc,aAAa,aAAa,iHAAiH;AAClpB;AACA;AACA;AACA,8BAA8B,iDAAW;AACzC,sCAAsC,oDAAc;AACpD;AACA,6BAA6B,iDAAW;AACxC,qCAAqC,oDAAc;AACnD,2DAA2D,EAAE,oEAA2B,IAAI,QAAQ,cAAc,gEAAa,EAAE,EAAE;AACnI;AACO,4BAA4B,uDAAc;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,wDAAgB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kDAAkD;AAClD;AACA,mBAAmB;AACnB,4BAA4B;AAC5B;AACA;AACA;AACA;AACA,2CAA2C;AAC3C;AACA;AACA,aAAa,EAAE;AACf;AACA;AACA;AACA;AACA;AACA,0EAA0E,MAAM;AAChF;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB;AACvB;AACA,4CAA4C;AAC5C,+CAA+C;AAC/C,8BAA8B;AAC9B;AACA;AACA,kDAAkD;AAClD,SAAS;AACT;AACA;AACA,mBAAmB,8DAA8D;AACjF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA,6CAA6C;AAC7C,iDAAiD;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2BAA2B;AAC3B;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,8CAAM;AACd;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oEAAoE,KAAK;AACzE;AACA,yBAAyB;AACzB;AACA;AACA;AACA,wBAAwB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB,4BAA4B;AACnD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mCAAmC,2EAAqC,EAAE,iCAAiC;AAC3G;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC;AACjC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2BAA2B;AAC3B;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA,SAAS;AACT;AACA;AACA,yCAAyC;AACzC;AACA;AACA,gDAAgD;AAChD,4EAA4E;AAC5E,qDAAqD;AACrD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iDAAiD,EAAE;AACnD;AACA;AACA;AACA;AACA,8DAA8D,kBAAkB;AAChF,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,eAAe,YAAY;AAC3B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,2BAA2B,mBAAmB;AAC9C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,cAAc;AACd;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA,uBAAuB,mBAAmB;AAC1C;AACA;AACA,4EAA4E,KAAK;AACjF,iCAAiC;AACjC;AACA,iDAAiD,KAAK;AACtD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;AC9rBA;AACA;AACA;AACA;AACA;AACA;AACA;AAC+B;AACuB;AACE;AACO;AAC4C;AAChE;AACL;AACtC;AACO,4BAA4B,wDAAe;AAClD;AACA,6CAA6C,sBAAsB,gaAAga,EAAE;AACre;AACA;AACA;AACA,6BAA6B,iDAAW;AACxC,qCAAqC,oDAAc;AACnD;AACA,4BAA4B,iDAAW;AACvC,oCAAoC,oDAAc;AAClD,0DAA0D,EAAE,oEAA2B,IAAI,YAAY,cAAc,gEAAa,EAAE,EAAE;AACtI;AACO,2BAA2B,uDAAc;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,6EAAuC,EAAE,UAAU;AAC/D;AACA;AACA;AACA;AACA,YAAY,6EAAuC,EAAE,UAAU;AAC/D;AACA;AACA;AACA;AACA,qCAAqC,+CAAI;AACzC;AACA;AACA,YAAY,2EAAqC,EAAE,UAAU;AAC7D;AACA;AACA;AACA;AACA;AACA;AACA,yBAAyB,yDAAiB;AAC1C,yBAAyB,yDAAiB;AAC1C;AACA,0DAA0D,YAAY,EAAE,KAAK,eAAe,KAAK,wBAAwB,IAAI,KAAK;AAClI,0FAA0F;AAC1F,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,8CAAM;AAClB,wEAAwE,cAAc;AACtF;AACA;AACA;AACA;AACA;AACA;AACA;AACA,yEAAyE,KAAK;AAC9E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA,YAAY,8CAAM;AAClB,sBAAsB;AACtB,iBAAiB,wDAAgB;AACjC,sBAAsB;AACtB;AACA,8BAA8B,4DAAsB,mBAAmB;AACvE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8DAA8D,gBAAgB;AAC9E;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA,oDAAoD,EAAE;AACtD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,4EAA4E,wDAAgB;AAC5F;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B;AAC5B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACzQA;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACO;AACP;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,WAAW,OAAO;AAClB,aAAa;AACb;AACO;AACP;AACA;AACA;AACA;AACA;AACA,WAAW,YAAY;AACvB;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA;AACA;AACA,WAAW,YAAY;AACvB;AACO;AACP;AACA,eAAe;AACf;AACA;AACA,qCAAqC;AACrC,gDAAgD;AAChD,gCAAgC;AAChC;AACA;AACA,+BAA+B;AAC/B,4CAA4C;AAC5C,+BAA+B;AAC/B;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACP;AACA,eAAe;AACf;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACP;AACA,kDAAkD,EAAE,UAAU;AAC9D,KAAK;AACL;AACA;AACO;AACP;AACA,kDAAkD,WAAW,UAAU,qBAAqB;AAC5F;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA,oEAAoE;AACpE;AACA;AACA;AACA;AACA;AACA;AACO;AACP,aAAa,SAAS,EAAE,YAAY;AACpC;AACA;AACA,KAAK,+DAA+D,EAAE;AACtE;;;;;;;;;;;;;;;;;AC3LA,aAAa,mBAAO,CAAC,uCAAiB;AACtC;AACA;AACA;AACA;AACO;AACP;AACA;AACA;AACO;;;;;;;;;;;;;;;;ACTP,iEAAe,qBAAuB,yCAAyC,E;;;;;;;;;;;;;;;ACA/E,iEAAe,0IAA0I,mBAAmB,OAAO,eAAe,qBAAqB,oBAAoB,4BAA4B,OAAO,cAAc,OAAO,iBAAiB,OAAO,aAAa,yBAAyB,OAAO,cAAc,OAAO,cAAc,OAAO,mBAAmB,OAAO,mBAAmB,QAAQ,mBAAmB,QAAQ,mBAAmB,QAAQ,mBAAmB,QAAQ,mBAAmB,QAAQ,mBAAmB,QAAQ,mBAAmB,QAAQ,gCAAgC,g2BAAg2B,66CAA66C,k7CAAk7C,q7CAAq7C,qtDAAqtD,0sDAA0sD,khDAAkhD,0kDAA0kD,ulDAAulD,ouIAAouI,E;;;;;;;;;;;;;;;;;;ACA19jB;AACzF,YAA4F;;AAE5F;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,wFAAO;;;;AAIxB,iEAAe,+FAAc,MAAM,E;;;;;;;;;;;;;;;;;;ACZsD;AACzF,YAA2F;;AAE3F;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,uFAAO;;;;AAIxB,iEAAe,8FAAc,MAAM,E;;;;;;;;;;;;;;;;;;ACZsD;AACzF,YAA0F;;AAE1F;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,sFAAO;;;;AAIxB,iEAAe,6FAAc,MAAM,E",
+    "file": "lib_registry_js-lib_uibuilder_js-lib_uioutput_js.cd289910d38270a1d73e.js",
+    "mappings": ";;;;;;;;;;;;;;;;;;;;;AAAiC;AACU;AACQ;AAC2B;AACtB;AACpB;AACpC;AACO,8BAA8B,iEAAc;AACnD;AACA,6CAA6C,sBAAsB,yHAAyH,4DAAsB,4DAA4D,EAAE;AAChR;AACA;AACA;AACA,+BAA+B,iDAAW;AAC1C,uCAAuC,oDAAc;AACrD;AACA,8BAA8B,iDAAW;AACzC,sCAAsC,oDAAc;AACpD,8CAA8C,EAAE,6EAA0B;AAC1E;AACO,6BAA6B,gEAAa;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uEAAuE;AACvE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mEAAmE,SAAS;AAC5E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,yBAAyB,YAAY,EAAE;AACvC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB,4DAAsB;AACzC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,4DAAsB;AAClC,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,aAAa,qEAA+B;AAC5C;AACA,aAAa,mFAA6C;AAC1D;AACA,sBAAsB,mGAA6D;AACnF,uBAAuB,kBAAkB;AACzC;AACA;AACA,gBAAgB,4DAAsB;AACtC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA,SAAS;AACT;AACA;AACA;AACA,4DAA4D,MAAM;AAClE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,yEAAyE,KAAK;AAC9E;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA,QAAQ,4DAAsB;AAC9B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,8CAAM;AACd;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iDAAiD;AACjD;AACA;AACA,gCAAgC,wDAAgB;AAChD;AACA;AACA,8BAA8B,wDAAgB;AAC9C;AACA;AACA,yBAAyB,2DAAqB,CAAC,wDAAgB;AAC/D;AACA;AACA;AACA;AACA,+BAA+B,0BAA0B,wDAAgB,+BAA+B;AACxG;AACA,+BAA+B,0BAA0B,wDAAgB,uCAAuC,wDAAgB,iCAAiC;AACjK;AACA;AACA;AACA,gCAAgC,wDAAgB;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,qDAAqD,aAAa;AAClE;AACA;AACA;AACA;AACA,eAAe,eAAe;AAC9B,eAAe,oBAAoB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb;AACA;AACA;AACA;AACA;AACA,eAAe,OAAO;AACtB,eAAe,OAAO;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS,QAAQ,6DAAM,kBAAkB,WAAW,MAAM,iBAAiB;AAC3E;AACA,cAAc,uBAAuB,EAAE;AACvC,mBAAmB,EAAE;AACrB;;;;;;;;;;;;;;;;;;;;;ACnW6C;AACQ;AACR;AACtC;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB;AAClB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,YAAY;AAC3B,eAAe,QAAQ;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,4CAAI;AACpB;AACA,gBAAgB,4CAAI;AACpB;AACA,gBAAgB,8CAAM;AACtB,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA,4BAA4B,uDAAQ;AACpC;AACA;AACA,gBAAgB,+DAAgB;AAChC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB;AACtB;AACA,sBAAsB;AACtB;AACA,sBAAsB;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kFAAyC;AACxD;AACA;AACA;AACA;AACA;AACA,eAAe,wEAAoC;AACnD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,+DAAa;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC,+DAAa;AAC9C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA,sEAAsE,aAAa;AACnF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,EAAE;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gDAAgD,wBAAwB;AACxE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,YAAY;AAC3B,eAAe,QAAQ;AACvB;AACA;AACA;AACA;AACA;AACA,uBAAuB;AACvB;AACA;AACA;AACA,gBAAgB,4CAAI;AACpB;AACA,gBAAgB,4CAAI;AACpB;AACA,gBAAgB,8CAAM;AACtB,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0CAA0C,wBAAwB;AAClE;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,kFAAyC;AAC3E;AACA;AACA;AACA;AACA;AACA,kCAAkC,wEAAoC;AACtE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,YAAY;AAC3B,eAAe,QAAQ;AACvB;AACA,mCAAmC;AACnC;AACA;AACA;AACA;AACA,oBAAoB;AACpB;AACA;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA,qBAAqB,WAAW;AAChC;AACA;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0CAA0C,wBAAwB;AAClE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,kFAAyC;AAC3E;AACA;AACA;AACA;AACA;AACA,eAAe,wEAAoC;AACnD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8BAA8B;AAC9B;AACA;AACA;AACA;AACA;AACA;AACA,qCAAqC;AACrC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;ACzgB2C;AACD;AACqB;AACxD,0BAA0B,oDAAK;AAC/B;AACP,QAAQ,eAAe,YAAY,qBAAqB,EAAE;AAC1D;AACA;AACA;AACA;AACA,4BAA4B;AAC5B,oCAAoC;AACpC;AACA,aAAa,kEAA4B;AACzC,YAAY,kEAA4B;AACxC,QAAQ,4DAAsB;AAC9B;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,cAAc,sDAAsD;AACpE;AACA;AACA;AACA;AACA;AACA,yBAAyB;AACzB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,sDAAsD;AACtE;AACA;AACA;AACA;AACA;AACA,wBAAwB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,cAAc,+BAA+B;AAC7C;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,4DAAsB;AACrC;AACA;AACO;AACP;AACA;AACA;AACA,uCAAuC,yDAAiB;AACxD,oCAAoC,yDAAiB;AACrD;AACA;;;;;;;;;;;;;;;;;;;;;;;ACjIqD;AACT;AACD;AACD;AACnC,0BAA0B,oDAAK;AAC/B;AACP;AACA;AACA;AACA;AACA,4BAA4B;AAC5B,oCAAoC;AACpC,oCAAoC;AACpC,sCAAsC;AACtC;AACA,aAAa,kEAA4B;AACzC,YAAY,kEAA4B;AACxC,QAAQ,4DAAsB;AAC9B;AACA;AACA;AACA;AACA;AACA;AACA,0CAA0C,+DAAa,KAAK,2DAAqB;AACjF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA,QAAQ,4DAAsB;AAC9B;AACA,uBAAuB;AACvB,YAAY,4DAAsB;AAClC,SAAS;AACT;AACA;AACA,QAAQ,4DAAsB;AAC9B,YAAY,4DAAsB;AAClC,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,QAAQ,4DAAsB;AAC9B;AACA;AACA;AACA,6BAA6B,4DAAsB;AACnD;AACA;AACA;AACA;AACA;AACA,wBAAwB,yDAAiB,4CAA4C,4DAAsB;AAC3G;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA,YAAY,4DAAsB;AAClC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB,2BAA2B;AAC9C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,4DAAsB;AACrC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wBAAwB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB,MAAM;AACvB;AACA;AACA;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACnLsD;AACrB;AACU;AAC2B;AAC/D,0BAA0B,mDAAM;AACvC;AACA;AACA;AACA;AACA;AACA,0BAA0B,wDAAW;AACrC;AACA;AACA;AACA;AACA;AACA;AACO,sBAAsB,mDAAM;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,4EAAsC;AAC9C;AACA;AACA;AACA;AACA,oCAAoC;AACpC,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oCAAoC;AACpC,4CAA4C;AAC5C,aAAa,wDAAwD;AACrE,uCAAuC;AACvC;AACA;AACA;AACA;AACA,4BAA4B,+EAAyC;AACrE;AACA,gEAAgE,QAAQ,aAAa,YAAY;AACjG;AACA;AACA,aAAa,qEAA+B;AAC5C,mBAAmB;AACnB,wBAAwB,0EAAoC;AAC5D,6CAA6C,+DAAa;AAC1D,mBAAmB;AACnB,mBAAmB,gFAA0C;AAC7D;AACA,mBAAmB;AACnB;AACA;AACA;AACA,YAAY,6EAA2B;AACvC;AACA,eAAe,gFAA0C,CAAC;AAC1D;AACA;AACA;AACA,eAAe,qEAAmB;AAClC;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB,uEAAiC;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kDAAkD;AAClD;AACA,gDAAgD;AAChD,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oDAAoD,KAAK;AACzD;AACA,kBAAkB;AAClB;AACA,gDAAgD,KAAK;AACrD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0CAA0C,UAAU;AACpD,+CAA+C,iBAAiB;AAChE;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,8CAAM;AACd;AACA;AACO,wBAAwB,mDAAM;AACrC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;;;;;;;;AC5MA;AACA;AACA;AACA;AACA;AACA;AACA;AACgC;AACwB;AACF;AACS;AACZ;AACR;AAC3C;AACO,6BAA6B,wDAAe;AACnD;AACA,6CAA6C,sBAAsB,ocAAoc,aAAa,aAAa,iHAAiH;AAClpB;AACA;AACA;AACA,8BAA8B,iDAAW;AACzC,sCAAsC,oDAAc;AACpD;AACA,6BAA6B,iDAAW;AACxC,qCAAqC,oDAAc;AACnD,2DAA2D,EAAE,oEAA2B,IAAI,QAAQ,cAAc,gEAAa,EAAE,EAAE;AACnI;AACO,4BAA4B,uDAAc;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,wDAAgB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kDAAkD;AAClD;AACA,mBAAmB;AACnB,4BAA4B;AAC5B;AACA;AACA;AACA;AACA,2CAA2C;AAC3C;AACA;AACA,aAAa,EAAE;AACf;AACA;AACA;AACA;AACA;AACA,0EAA0E,MAAM;AAChF;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB;AACvB;AACA,4CAA4C;AAC5C,+CAA+C;AAC/C,8BAA8B;AAC9B;AACA;AACA,kDAAkD;AAClD,SAAS;AACT;AACA;AACA,mBAAmB,8DAA8D;AACjF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA,6CAA6C;AAC7C,iDAAiD;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2BAA2B;AAC3B;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,8CAAM;AACd;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oEAAoE,KAAK;AACzE;AACA,yBAAyB;AACzB;AACA;AACA;AACA,wBAAwB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB,4BAA4B;AACnD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mCAAmC,2EAAqC,EAAE,iCAAiC;AAC3G;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC;AACjC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2BAA2B;AAC3B;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA,SAAS;AACT;AACA;AACA,yCAAyC;AACzC;AACA;AACA,gDAAgD;AAChD,4EAA4E;AAC5E,qDAAqD;AACrD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iDAAiD,EAAE;AACnD;AACA;AACA;AACA;AACA,8DAA8D,kBAAkB;AAChF,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,eAAe,YAAY;AAC3B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,2BAA2B,mBAAmB;AAC9C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,cAAc;AACd;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA,uBAAuB,mBAAmB;AAC1C;AACA;AACA,4EAA4E,KAAK;AACjF,iCAAiC;AACjC;AACA,iDAAiD,KAAK;AACtD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;AC9rBA;AACA;AACA;AACA;AACA;AACA;AACA;AAC+B;AACuB;AACE;AACO;AAC4C;AAChE;AACL;AACtC;AACO,4BAA4B,wDAAe;AAClD;AACA,6CAA6C,sBAAsB,gaAAga,EAAE;AACre;AACA;AACA;AACA,6BAA6B,iDAAW;AACxC,qCAAqC,oDAAc;AACnD;AACA,4BAA4B,iDAAW;AACvC,oCAAoC,oDAAc;AAClD,0DAA0D,EAAE,oEAA2B,IAAI,YAAY,cAAc,gEAAa,EAAE,EAAE;AACtI;AACO,2BAA2B,uDAAc;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,6EAAuC,EAAE,UAAU;AAC/D;AACA;AACA;AACA;AACA,YAAY,6EAAuC,EAAE,UAAU;AAC/D;AACA;AACA;AACA;AACA,qCAAqC,+CAAI;AACzC;AACA;AACA,YAAY,2EAAqC,EAAE,UAAU;AAC7D;AACA;AACA;AACA;AACA;AACA;AACA,yBAAyB,yDAAiB;AAC1C,yBAAyB,yDAAiB;AAC1C;AACA,0DAA0D,YAAY,EAAE,KAAK,eAAe,KAAK,wBAAwB,IAAI,KAAK;AAClI,0FAA0F;AAC1F,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,8CAAM;AAClB,wEAAwE,cAAc;AACtF;AACA;AACA;AACA;AACA;AACA;AACA;AACA,yEAAyE,KAAK;AAC9E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA,YAAY,8CAAM;AAClB,sBAAsB;AACtB,iBAAiB,wDAAgB;AACjC,sBAAsB;AACtB;AACA,8BAA8B,4DAAsB,mBAAmB;AACvE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8DAA8D,gBAAgB;AAC9E;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA,oDAAoD,EAAE;AACtD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,4EAA4E,wDAAgB;AAC5F;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B;AAC5B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACzQA;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACO;AACP;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,WAAW,OAAO;AAClB,aAAa;AACb;AACO;AACP;AACA;AACA;AACA;AACA;AACA,WAAW,YAAY;AACvB;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA;AACA;AACA,WAAW,YAAY;AACvB;AACO;AACP;AACA,eAAe;AACf;AACA;AACA,qCAAqC;AACrC,gDAAgD;AAChD,gCAAgC;AAChC;AACA;AACA,+BAA+B;AAC/B,4CAA4C;AAC5C,+BAA+B;AAC/B;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACP;AACA,eAAe;AACf;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACP;AACA,kDAAkD,EAAE,UAAU;AAC9D,KAAK;AACL;AACA;AACO;AACP;AACA,kDAAkD,WAAW,UAAU,qBAAqB;AAC5F;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA,oEAAoE;AACpE;AACA;AACA;AACA;AACA;AACA;AACO;AACP,aAAa,SAAS,EAAE,YAAY;AACpC;AACA;AACA,KAAK,+DAA+D,EAAE;AACtE;;;;;;;;;;;;;;;;;AC3LA,aAAa,mBAAO,CAAC,uCAAiB;AACtC;AACA;AACA;AACA;AACO;AACP;AACA;AACA;AACO;;;;;;;;;;;;;;;;ACTP,iEAAe,qBAAuB,yCAAyC,E;;;;;;;;;;;;;;;ACA/E,iEAAe,0IAA0I,mBAAmB,OAAO,eAAe,qBAAqB,oBAAoB,4BAA4B,OAAO,cAAc,OAAO,iBAAiB,OAAO,aAAa,yBAAyB,OAAO,cAAc,OAAO,cAAc,OAAO,mBAAmB,OAAO,mBAAmB,QAAQ,mBAAmB,QAAQ,mBAAmB,QAAQ,mBAAmB,QAAQ,mBAAmB,QAAQ,mBAAmB,QAAQ,mBAAmB,QAAQ,gCAAgC,g2BAAg2B,66CAA66C,k7CAAk7C,q7CAAq7C,qtDAAqtD,0sDAA0sD,khDAAkhD,0kDAA0kD,ulDAAulD,ouIAAouI,E;;;;;;;;;;;;;;;;;;ACA19jB;AACzF,YAA4F;;AAE5F;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,wFAAO;;;;AAIxB,iEAAe,+FAAc,MAAM,E;;;;;;;;;;;;;;;;;;ACZsD;AACzF,YAA2F;;AAE3F;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,uFAAO;;;;AAIxB,iEAAe,8FAAc,MAAM,E;;;;;;;;;;;;;;;;;;ACZsD;AACzF,YAA0F;;AAE1F;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,sFAAO;;;;AAIxB,iEAAe,6FAAc,MAAM,E",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@g2nb/nbtools/./lib/basewidget.js",
         "webpack://@g2nb/nbtools/./lib/context.js",
         "webpack://@g2nb/nbtools/./lib/dataregistry.js",
         "webpack://@g2nb/nbtools/./lib/registry.js",
@@ -16,18 +16,18 @@
         "webpack://@g2nb/nbtools/./style/g2nb_logo.png",
         "webpack://@g2nb/nbtools/./style/icon.svg",
         "webpack://@g2nb/nbtools/./style/basewidget.css?23c0",
         "webpack://@g2nb/nbtools/./style/uibuilder.css?043a",
         "webpack://@g2nb/nbtools/./style/uioutput.css?93d6"
     ],
     "sourcesContent": [
-        "import '../style/basewidget.css';\nimport { ContextManager } from \"./context\";\nimport { process_template, toggle } from \"./utils\";\nimport { DOMWidgetModel, DOMWidgetView, reject } from \"@jupyter-widgets/base\";\nimport { MODULE_NAME, MODULE_VERSION } from \"./version\";\nimport { Toolbox } from \"./toolbox\";\n// noinspection JSAnnotator\nexport class BaseWidgetModel extends DOMWidgetModel {\n    defaults() {\n        return Object.assign(Object.assign({}, super.defaults()), { _id: '', origin: '', name: '', subtitle: '', description: '', collapsed: false, color: 'var(--jp-layout-color4)', logo: ContextManager.context().default_logo(), info: '', error: '', extra_menu_items: {} });\n    }\n}\nBaseWidgetModel.model_name = 'BaseWidgetModel';\nBaseWidgetModel.model_module = MODULE_NAME;\nBaseWidgetModel.model_module_version = MODULE_VERSION;\nBaseWidgetModel.view_name = 'BaseWidgetView';\nBaseWidgetModel.view_module = MODULE_NAME;\nBaseWidgetModel.view_module_version = MODULE_VERSION;\nBaseWidgetModel.serializers = Object.assign({}, DOMWidgetModel.serializers);\n// noinspection JSAnnotator\nexport class BaseWidgetView extends DOMWidgetView {\n    constructor() {\n        super(...arguments);\n        this.dom_class = '';\n        this.element = document.createElement('div');\n        this.traitlets = ['name', 'subtitle', 'description', 'info', 'error'];\n        this.renderers = {\n            \"description\": this.render_description,\n            \"error\": this.render_error,\n            \"info\": this.render_info\n        };\n        this.template = `<div class=\"nbtools\">\n                           <div class=\"nbtools-header\"></div>\n                           <div class=\"nbtools-body\"></div>\n                       </div>`;\n        this.header = `<img class=\"nbtools-logo\" src=\"\" />\n                     <label class=\"nbtools-title\" data-traitlet=\"name\"></label>\n                     <label class=\"nbtools-subtitle\" data-traitlet=\"subtitle\"></label>\n                     <div class=\"nbtools-controls\">\n                         <button class=\"nbtools-collapse\">\n                             <span class=\"fa fa-minus\"></span>\n                         </button>\n                         <button class=\"nbtools-gear\">\n                             <span class=\"fa fa-cog\"></span>\n                             <span class=\"fa fa-caret-down\"></span>\n                         </button>\n                         <ul class=\"nbtools-menu\" style=\"display: none;\"></ul>\n                     </div>`;\n        this.body = `<div class=\"nbtools-description\" data-traitlet=\"description\"></div>\n                   <div class=\"nbtools-error\" data-traitlet=\"error\"></div>\n                   <div class=\"nbtools-info\" data-traitlet=\"info\"></div>`;\n        this.disconnected = `<div class=\"nbtools-disconnected\">\n                               <div class=\"nbtools-panel\">\n                                   <div class=\"nbtools-header\">Widget Disconnected From Kernel</div>\n                                   <div class=\"nbtools-body\">\n                                       <p>You need to run this cell before it can connect to the notebook kernel. Please click the Connect to Kernel button below.</p>\n                                       <div class=\"nbtools-connect nbtools-panel-button\"><button class=\"nbtools-connect nbtools-panel-button\">Connect to Kernel</button></div>\n                                   </div>\n                               </div>\n                           </div>`;\n    }\n    render() {\n        super.render();\n        // Build the widget\n        this.build();\n        // Apply the color\n        this.set_color();\n        this.model.on('change:color', this.set_color, this);\n        // Apply the logo\n        this.set_logo();\n        this.model.on('change:logo', this.set_logo, this);\n        // Set the traitlet values\n        this.traitlets.forEach(traitlet => this.traitlet_changed(traitlet));\n        // Hook in the traitlet change events\n        this.traitlets.forEach(traitlet => this.model.on(`change:${traitlet}`, this.traitlet_changed, this));\n        // Hook in the expand / collapse events\n        this.model.on('change:collapsed', this.toggle_collapse, this);\n        if (this.model.get('collapsed'))\n            this.toggle_collapse();\n        // Hide the code\n        this.toggle_code(false);\n        // Attach the extra menu options\n        this.attach_menu_options();\n        this.model.on('change:extra_menu_items', this.attach_menu_options, this);\n        // Allow menus to overflow the container\n        this.float_menus();\n        // Initialize the widget\n        this.initialize({ options: {} });\n        // Call any post render events\n        this.post_render();\n    }\n    build() {\n        // Parse the template\n        this.element = new DOMParser().parseFromString(this.template, \"text/html\")\n            .querySelector('div.nbtools');\n        // Apply the DOM class\n        if (this.dom_class)\n            this.element.classList.add(this.dom_class);\n        // Apply the header\n        this.element.querySelector('div.nbtools-header').innerHTML = this.header;\n        // Attach collapse event\n        const collapse = this.element.querySelector(\"button.nbtools-collapse\");\n        collapse.addEventListener(\"click\", () => {\n            this.model.set('collapsed', !this.model.get('collapsed'));\n            this.model.save_changes();\n        });\n        // Attach the gear event\n        const gear = this.element.querySelector(\"button.nbtools-gear\");\n        gear.addEventListener(\"click\", () => this.toggle_menu());\n        // Attach toggle code event\n        this.add_menu_item('Toggle Code View', () => this.toggle_code());\n        // Apply the body\n        this.element.querySelector('div.nbtools-body').innerHTML = this.body;\n        // Attach the disconnected cover\n        this.element.appendChild(new DOMParser().parseFromString(this.disconnected, \"text/html\")\n            .querySelector('body > :first-child'));\n        this.attach_connect_event();\n        this.disconnected_sync_fix();\n        // Set the element\n        this.setElement(this.element);\n    }\n    set_logo() {\n        // Get custom logo\n        let logo = this.model.get('logo');\n        const logo_element = this.element.querySelector(\"img.nbtools-logo\");\n        // Fall back to default logo if no custom logo is set\n        if (!logo) {\n            logo = ContextManager.context().default_logo();\n            this.model.set('logo', logo);\n            this.model.save();\n        }\n        // Special case for \"None\" logo\n        if (logo.toLowerCase() === \"none\")\n            logo_element.classList.add('nbtools-logo-hidden');\n        else\n            logo_element.classList.remove('nbtools-logo-hidden');\n        // Set the logo\n        logo_element.src = logo;\n    }\n    set_color() {\n        const color = this.model.get('color').trim();\n        this.element.style.borderColor = color;\n        this.element.querySelectorAll('.nbtools-body button, .nbtools-header').forEach((e) => {\n            e.style.backgroundColor = color;\n        });\n    }\n    render_description(description, widget) {\n        return widget._render_or_hide('.nbtools-description', description, widget);\n    }\n    render_error(message, widget) {\n        return widget._render_or_hide('.nbtools-error', message, widget);\n    }\n    render_info(message, widget) {\n        return widget._render_or_hide('.nbtools-info', message, widget);\n    }\n    _render_or_hide(selector, message, widget) {\n        widget.element.querySelector(selector).style.display = message.trim() ? 'block' : 'none';\n        return message;\n    }\n    attach_connect_event() {\n        const button = this.element.querySelector('button.nbtools-connect');\n        button.addEventListener(\"click\", () => {\n            // Run all cells with disconnected nbtools widgets\n            ContextManager.context().run_tool_cells();\n        });\n    }\n    disconnected_sync_fix() {\n        // Fix a bug that can occur when a disconnected widget and a connected widget are somehow rendered in the same cell\n        setTimeout(() => {\n            const cell = this.element.closest('.jp-Cell, .cell');\n            if (!cell)\n                return; // No cell found, bug cannot occur\n            // Do both connected and disconnected widgets appear in the cell?\n            const contains_disconnected = !!cell.querySelectorAll('.nbtools.jupyter-widgets-disconnected').length;\n            const contains_connected = !!cell.querySelectorAll('.nbtools:not(.jupyter-widgets-disconnected)').length;\n            // If they do, hide the irrelevant disconnected widgets\n            if (contains_disconnected && contains_connected) {\n                cell.querySelectorAll('.nbtools.jupyter-widgets-disconnected').forEach((e) => {\n                    e.style.display = 'none';\n                });\n            }\n        }, 100);\n    }\n    add_menu_item(label, callback, dom_class = null, menu = null, prepend = true) {\n        // Create the menu item\n        const item = new DOMParser().parseFromString(`<li>${label}</li>`, \"text/html\")\n            .querySelector('li');\n        // Apply the class if one is specified\n        if (dom_class)\n            item.classList.add(dom_class);\n        // Attach the menu item\n        if (!menu)\n            menu = this.element.querySelector('.nbtools-menu');\n        if (prepend)\n            menu.prepend(item);\n        else\n            menu.append(item);\n        // Attach the click event\n        item.addEventListener('click', () => callback());\n        return item;\n    }\n    traitlet_changed(event) {\n        const widget = this;\n        const name = typeof event === \"string\" ? event : Object.keys(event.changed)[0];\n        const elements = this.element.querySelectorAll(`[data-traitlet=${name}]`);\n        elements.forEach(element => {\n            if (name in this.renderers)\n                element.innerHTML = this.renderers[name](this.model.get(name), widget);\n            else\n                element.innerHTML = this.model.get(name);\n        });\n    }\n    toggle_code(display) {\n        const element = this.element;\n        ContextManager.context().toggle_code(element, display);\n    }\n    toggle_collapse() {\n        const body = this.element.querySelector(\".nbtools-body\");\n        const collapsed = body.style.display === \"none\" || body.style.height == \"0px\";\n        // Toggle the collapse button\n        const button = this.element.querySelector(\".nbtools-collapse > span\");\n        if (collapsed) {\n            button.classList.add('fa-minus');\n            button.classList.remove('fa-plus');\n        }\n        else {\n            button.classList.remove('fa-minus');\n            button.classList.add('fa-plus');\n        }\n        // Hide or show widget body\n        toggle(body);\n    }\n    toggle_menu() {\n        const gear = this.element.querySelector(\"button.nbtools-gear\");\n        const menu = this.element.querySelector(\".nbtools-menu\");\n        const collapsed = menu.style.display === \"none\";\n        // Hide or show the menu\n        if (collapsed)\n            menu.style.display = \"block\";\n        else\n            menu.style.display = \"none\";\n        // Hide the menu with the next click\n        const hide_next_click = function (event) {\n            if (gear.contains(event.target))\n                return;\n            menu.style.display = \"none\";\n            document.removeEventListener('click', hide_next_click);\n        };\n        document.addEventListener('click', hide_next_click);\n    }\n    create_menu_callback(item, template_vars = {}) {\n        // Create callback for string literal\n        if (typeof item === 'string')\n            return new Function(process_template(item, template_vars));\n        // Create callback for javascript event type\n        else if (item['action'] === 'javascript')\n            return () => eval(process_template(item['code'], template_vars));\n        // Create callback for cell event type\n        else if (item['action'] === 'cell')\n            return () => Toolbox.add_code_cell(process_template(item['code'], template_vars));\n        // Create callback for method event type\n        else if (item['action'] === 'method')\n            return () => {\n                if (!item['params'])\n                    this.send({ event: 'method', method: process_template(item['code'], template_vars) });\n                else\n                    this.send({ event: 'method', method: process_template(item['code'], template_vars), params: process_template(item['params'], template_vars) });\n            };\n        // Create callback for custom event type\n        else\n            return new Function(process_template(item['code'], template_vars));\n    }\n    attach_menu_options() {\n        // Clear any existing menu\n        const menu = this.element.querySelector('.nbtools-menu');\n        menu.querySelectorAll('.nbtools-menu-extra').forEach((e) => e.remove());\n        const menu_items = this.model.get('extra_menu_items');\n        Object.keys(menu_items).forEach((name) => {\n            const item = menu_items[name];\n            const callback = this.create_menu_callback(item);\n            this.add_menu_item(name, callback, 'nbtools-menu-extra');\n        });\n    }\n    float_menus() {\n        const fix_cell = () => {\n            const elements = [\n                this.el.closest('.lm-Widget.jp-OutputPrompt.jp-OutputArea-prompt'),\n                this.el.closest('.lm-Widget.lm-Panel.jp-OutputArea'),\n                this.el.closest('.lm-Widget.lm-Panel.jp-OutputArea-child'),\n                this.el.closest('.lm-Widget.lm-Panel.jp-OutputArea-output'),\n                this.el.closest('.lm-Widget.jp-OutputArea.jp-Cell-outputArea')\n            ];\n            elements.forEach((e) => {\n                if (e)\n                    e.style.overflow = 'visible';\n            });\n        };\n        this.el.addEventListener('click', fix_cell, { once: true });\n    }\n    /**\n     * Recursively trigger the 'displayed' event for all child widgets\n     *\n     * @param {DOMWidgetModel} model\n     * @param {DOMWidgetView | any} view\n     * @private\n     */\n    static _initialize_display(model, view) {\n        // Trigger the display for this widget\n        view.trigger('displayed');\n        // Recursively trigger the display for all child widgets\n        if ('children_views' in view) {\n            view.children_views.update(model.get('children')).then((children) => {\n                children.forEach((child) => {\n                    BaseWidgetView._initialize_display(child.model, child);\n                    child.el.widget = child;\n                });\n            });\n        }\n    }\n    /**\n     * Add the specified child widget to the view and initialize\n     *\n     * @param {string} element_selector\n     * @param {string} model_name\n     */\n    attach_child_widget(element_selector, model_name) {\n        const element = this.element.querySelector(element_selector);\n        const model = this.model.get(model_name);\n        this.create_child_view(model).then((view) => {\n            element.appendChild(view.el);\n            BaseWidgetView._initialize_display(model, view);\n            return view;\n        }).catch(reject(`Could not add ${model_name} to ${element_selector}`, true));\n    }\n    basics() { return this.traitlets; } // Return the list of basic traitlets\n    post_render() { } // Empty function, can be overridden in subclasses\n}\n",
-        "import { hide, show, toggle } from \"./utils\";\nimport { NotebookPanel } from \"@jupyterlab/notebook\";\nimport { CodeCell } from \"@jupyterlab/cells\";\nexport class ContextManager {\n    static context() {\n        if (!ContextManager._context) {\n            if (ContextManager.is_lab())\n                ContextManager._context = new LabContext();\n            else if (ContextManager.is_notebook())\n                ContextManager._context = new NotebookContext();\n            else\n                ContextManager._context = new EmbedContext();\n        }\n        return ContextManager._context;\n    }\n    /**\n     * Determine is this is running in JupyterLab\n     *\n      * @returns {boolean}\n     */\n    static is_lab() {\n        // The assumption is that only JupyterLab will provide an initialized NotebookTracker object\n        // If a better way to detect the environment becomes available, use that instead\n        return !!ContextManager.notebook_tracker;\n        // A previous implementation replied on checking the DOM\n        // return !!document.querySelector(\"#main.jp-LabShell\")\n    }\n    /**\n     * Determine if this is running in the classic Jupyter Notebook\n     *\n     * @returns {boolean}\n     */\n    static is_notebook() {\n        // Check if the Jupyter global variable has been defined\n        return !!(window['Jupyter']);\n    }\n}\n/**\n * Abstract base class representing the context in which the widgets are running.\n * Contexts include: JupyterLab, Jupyter Notebook and Embedded.\n */\nclass Context {\n}\n/**\n * Context handler for JupyterLab\n */\nclass LabContext extends Context {\n    /**\n     * Toggle hiding or or showing the code for the specified cell\n     *\n     * @param {HTMLElement} element\n     * @param {boolean} display\n     */\n    toggle_code(element, display) {\n        setTimeout(() => {\n            let input_block = element.closest('.jp-Cell');\n            if (input_block)\n                input_block = input_block.querySelector('.jp-Cell-inputWrapper');\n            // Set display to toggle if not specified\n            if (!!display)\n                show(input_block);\n            else if (display === false)\n                hide(input_block, '30px');\n            else\n                toggle(input_block, '30px');\n        }, 100);\n    }\n    /**\n     * Execute the indicated cell in the notebook\n     *\n     * @param cell\n     */\n    run_cell(cell = null) {\n        if (!ContextManager.notebook_tracker)\n            return; // If no notebook_tracker, do nothing\n        // If cell is falsy, default to the active cell\n        if (!cell)\n            cell = ContextManager.notebook_tracker.activeCell;\n        // If this is a code cell\n        if (cell instanceof CodeCell) {\n            const current = ContextManager.notebook_tracker.currentWidget;\n            if (current) {\n                CodeCell.execute(cell, current.context.sessionContext);\n            }\n        }\n        // If this is a markdown cell\n        // if (ContextManager.notebook_tracker.activeCell instanceof MarkdownCell)\n        //     MarkdownCell.renderInput(ContextManager.notebook_tracker.activeCell)\n    }\n    /**\n     * Execute all cells with nbtools widgets in the current notebook\n     */\n    run_tool_cells() {\n        if (!ContextManager.notebook_tracker)\n            return; // If no notebook_tracker, do nothing\n        if (!ContextManager.notebook_tracker.currentWidget)\n            return; // If no notebook selected, do nothing\n        const cell_widgets = ContextManager.notebook_tracker.currentWidget.content.widgets;\n        cell_widgets.forEach((widget) => {\n            if (this.is_tool_cell(widget))\n                this.run_cell(widget);\n        });\n    }\n    /**\n     * Get the relative path to the current notebook\n     */\n    notebook_path() {\n        if (!ContextManager.notebook_tracker)\n            return ''; // If no notebook_tracker, do nothing\n        if (!ContextManager.notebook_tracker.currentWidget)\n            return ''; // If no active notebook, do nothing\n        if (!ContextManager.notebook_tracker.currentWidget.context)\n            return ''; // If no context, do nothing\n        const notebook_context = ContextManager.notebook_tracker.currentWidget.context;\n        const notebook_path = notebook_context.path;\n        const directory_path = notebook_path.substring(0, notebook_path.lastIndexOf(\"/\") + 1);\n        return directory_path;\n    }\n    /**\n     * Determines if the given cell contains a notebook tool widget\n     *\n     * @param cell\n     * @returns boolean\n     */\n    is_tool_cell(cell) {\n        const dom_node = cell.node || cell.element;\n        if (!!dom_node)\n            return !!dom_node.querySelector('.nbtools');\n        else\n            return false;\n    }\n    /**\n     * Path to the default GenePattern logo\n     */\n    default_logo() {\n        return require(\"../style/g2nb_logo.png\").default;\n    }\n    /**\n     * Path to the default GenePattern icon\n     */\n    default_icon() {\n        return require(\"../style/icon.svg\").default;\n    }\n    /**\n     * Return the id of the current notebook's kernel\n     *\n     * @param notebook\n     */\n    kernel_id(notebook) {\n        // If the current widget isn't a notebook, there is no kernel\n        if (!(notebook instanceof NotebookPanel))\n            return null;\n        // Protect against null\n        if (!notebook ||\n            !notebook.context ||\n            !notebook.context.sessionContext ||\n            !notebook.context.sessionContext.session ||\n            !notebook.context.sessionContext.session.kernel)\n            return null;\n        return notebook.context.sessionContext.session.kernel.id;\n    }\n    /**\n     * Function to execute when the notebook is opened and selected\n     *\n     * @param callback\n     */\n    notebook_focus(callback) {\n        const notebook_tracker = ContextManager.notebook_tracker;\n        notebook_tracker && notebook_tracker.activeCellChanged.connect(() => {\n            const current_widget = notebook_tracker.currentWidget;\n            callback(current_widget);\n        });\n    }\n    /**\n     * Execute the callback when the current kernel is ready\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_ready(current, callback) {\n        // If the current widget isn't a notebook, there is no kernel\n        if (!(current instanceof NotebookPanel))\n            return;\n        current.context.sessionContext.ready.then(() => callback());\n    }\n    /**\n     * Execute the callback every time the kernel is changed or restarts\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_changed(current, callback) {\n        current.context.sessionContext.kernelChanged.connect(() => callback());\n    }\n    /**\n     * Send the provided code to the kernel\n     *\n     * @param notebook\n     * @param code\n     */\n    execute_code(notebook, code) {\n        const current = notebook;\n        if (!current.context.sessionContext.session ||\n            !current.context.sessionContext.session.kernel)\n            return; // Protect against null kernels\n        // Import the default tools\n        current.context.sessionContext.session.kernel.requestExecute({ code: code });\n    }\n    /**\n     * Create a new comm\n     *\n     * @param current\n     * @param name\n     * @param callback\n     */\n    create_comm(current, name, callback) {\n        const kernel = current.context.sessionContext.session.kernel;\n        const comm = kernel.createComm(name);\n        comm.onMsg = callback;\n        comm.open({}); // Open the comm\n        return comm;\n    }\n}\n/**\n * Context handler for the classic Jupyter Notebook\n */\nclass NotebookContext extends Context {\n    /**\n     * Toggle hiding or or showing the code for the specified cell\n     *\n     * @param {HTMLElement} element\n     * @param {boolean} display\n     */\n    toggle_code(element, display) {\n        setTimeout(() => {\n            const cell_element = element.closest(\".cell\");\n            if (!cell_element)\n                return; // Widget has not yet been added to the DOM\n            const code = cell_element.querySelector(\".input\");\n            // Set display to toggle if not specified\n            if (!!display)\n                show(code);\n            else if (display === false)\n                hide(code);\n            else\n                toggle(code);\n        }, 10);\n    }\n    /**\n     * Execute the indicated cell in the notebook\n     *\n     * @param cell\n     */\n    run_cell(cell) {\n        window.Jupyter.notebook.execute_cell(cell);\n    }\n    /**\n     * Execute all cells with nbtools widgets in the current notebook\n     */\n    run_tool_cells() {\n        const cells_to_run = [];\n        window.Jupyter.notebook.get_cells().forEach((cell, index) => {\n            if (this.is_tool_cell(cell))\n                cells_to_run.push(index);\n        });\n        window.Jupyter.notebook.execute_cells(cells_to_run);\n    }\n    notebook_path() {\n        return window.Jupyter.notebook.path;\n    }\n    base_path() {\n        const body = document.querySelector('body');\n        if (!body)\n            return ''; // If there is no body, unable to get path\n        return body.getAttribute('data-base-url') + 'nbextensions/nbtools/';\n    }\n    /**\n     * Determines if the given cell contains a notebook tool widget\n     *\n     * @param cell\n     * @returns boolean\n     */\n    is_tool_cell(cell) {\n        const dom_node = cell.node || cell.element;\n        if (!!dom_node)\n            return !!dom_node.find('.nbtools').length;\n        else\n            return false;\n    }\n    /**\n     * Path to the default GenePattern logo\n     */\n    default_logo() {\n        return this.base_path() + require(\"../style/g2nb_logo.png\").default;\n    }\n    /**\n     * Path to the default GenePattern icon\n     */\n    default_icon() {\n        return this.base_path() + require(\"../style/icon.svg\").default;\n    }\n    /**\n     * Return the id of the current notebook's kernel\n     *\n     * @param notebook\n     */\n    kernel_id(notebook) {\n        return window.Jupyter.notebook.kernel.id;\n    }\n    /**\n     * Function to execute when the notebook is opened and selected\n     *\n     * @param callback\n     */\n    notebook_focus(callback) {\n        window.Jupyter.notebook.events.ready(() => {\n            callback(window.Jupyter.notebook);\n        });\n    }\n    /**\n     * Execute the callback when the current kernel is ready\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_ready(current, callback) {\n        setTimeout(() => {\n            if (window.Jupyter.notebook.kernel.is_connected())\n                callback(window.Jupyter.notebook);\n            else\n                window.Jupyter.notebook.events.one('kernel_ready.Kernel', () => {\n                    callback(window.Jupyter.notebook);\n                });\n        }, 100);\n    }\n    /**\n     * Execute the callback every time the kernel is changed or restarts\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_changed(current, callback) {\n        window.Jupyter.notebook.events.on('kernel_ready.Kernel', () => {\n            callback(window.Jupyter.notebook);\n        });\n    }\n    /**\n     * Send the provided code to the kernel\n     *\n     * @param notebook\n     * @param code\n     */\n    execute_code(notebook, code) {\n        window.Jupyter.notebook.kernel.execute(code);\n    }\n    /**\n     * Create a new comm\n     *\n     * @param current\n     * @param name\n     * @param callback\n     */\n    create_comm(current, name, callback) {\n        let comm = window.Jupyter.notebook.kernel.comm_manager.new_comm(name);\n        comm.on_msg(callback);\n        return comm;\n    }\n}\n/**\n * Context handler for embedded widgets\n */\nclass EmbedContext extends Context {\n    /**\n     * No cells in this context, so do nothing\n     *\n     * @param {HTMLElement} element\n     * @param {boolean} display\n     */\n    toggle_code(element, display) { }\n    /**\n     * No cells in this context, so do nothing\n     * @param cell\n     */\n    run_cell(cell) { }\n    /**\n     * No cells in this context, so do nothing\n     */\n    run_tool_cells() { }\n    /**\n     * No notebook in this context\n     */\n    notebook_path() { return ''; }\n    base_path() {\n        const body = document.querySelector('body');\n        if (!body)\n            return ''; // If there is no body, unable to get path\n        return body.getAttribute('data-base-url') + 'nbextensions/nbtools/';\n    }\n    /**\n     * Determines if the given cell contains a notebook tool widget\n     *\n     * @param cell\n     * @returns boolean\n     */\n    is_tool_cell(cell) {\n        const dom_node = cell.node || cell.element;\n        if (!!dom_node)\n            return !!dom_node.querySelector('.nbtools');\n        else\n            return false;\n    }\n    /**\n     * Path to the default GenePattern logo\n     */\n    default_logo() {\n        return this.base_path() + require(\"../style/g2nb_logo.png\").default;\n    }\n    /**\n     * Path to the default GenePattern icon\n     */\n    default_icon() {\n        return require(\"../style/icon.svg\").default;\n    }\n    /**\n     * Return the id of the current notebook's kernel\n     *\n     * @param notebook\n     */\n    kernel_id(notebook) {\n        return null;\n    }\n    /**\n     * Function to execute when the notebook is opened and selected\n     *\n     * @param callback\n     */\n    notebook_focus(callback) { }\n    /**\n     * Execute the callback when the current kernel is ready\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_ready(current, callback) { }\n    /**\n     * Execute the callback every time the kernel is changed or restarts\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_changed(current, callback) {\n        // FIXME: Global Jupyter variable may not be accessible in newer version of voila\n        window.Jupyter.notebook.events.on('kernel_ready.Kernel', () => {\n            callback(window.Jupyter.notebook);\n        });\n    }\n    /**\n     * Send the provided code to the kernel\n     *\n     * @param notebook\n     * @param code\n     */\n    execute_code(notebook, code) {\n        // FIXME: Global Jupyter variable may not be accessible in newer version of voila\n        window.Jupyter.notebook.kernel.execute(code);\n    }\n    /**\n     * Create a new comm\n     *\n     * @param current\n     * @param name\n     * @param callback\n     */\n    create_comm(current, name, callback) {\n        // FIXME: Global Jupyter variable may not be accessible in newer version of voila\n        let comm = window.Jupyter.notebook.kernel.comm_manager.new_comm(name);\n        comm.on_msg(callback);\n        return comm;\n    }\n}\n",
+        "import '../style/basewidget.css';\nimport { ContextManager } from \"./context\";\nimport { process_template, toggle } from \"./utils\";\nimport { DOMWidgetModel, DOMWidgetView, reject } from \"@jupyter-widgets/base\";\nimport { MODULE_NAME, MODULE_VERSION } from \"./version\";\nimport { Toolbox } from \"./toolbox\";\n// noinspection JSAnnotator\nexport class BaseWidgetModel extends DOMWidgetModel {\n    defaults() {\n        return Object.assign(Object.assign({}, super.defaults()), { _id: '', origin: '', name: '', subtitle: '', description: '', collapsed: false, color: 'var(--jp-layout-color4)', logo: ContextManager.context().default_logo(), info: '', error: '', extra_menu_items: {} });\n    }\n}\nBaseWidgetModel.model_name = 'BaseWidgetModel';\nBaseWidgetModel.model_module = MODULE_NAME;\nBaseWidgetModel.model_module_version = MODULE_VERSION;\nBaseWidgetModel.view_name = 'BaseWidgetView';\nBaseWidgetModel.view_module = MODULE_NAME;\nBaseWidgetModel.view_module_version = MODULE_VERSION;\nBaseWidgetModel.serializers = Object.assign({}, DOMWidgetModel.serializers);\n// noinspection JSAnnotator\nexport class BaseWidgetView extends DOMWidgetView {\n    constructor() {\n        super(...arguments);\n        this.dom_class = '';\n        this.element = document.createElement('div');\n        this.traitlets = ['name', 'subtitle', 'description', 'info', 'error'];\n        this.renderers = {\n            \"description\": this.render_description,\n            \"error\": this.render_error,\n            \"info\": this.render_info\n        };\n        this.template = `<div class=\"nbtools\">\n                           <div class=\"nbtools-header\"></div>\n                           <div class=\"nbtools-body\"></div>\n                       </div>`;\n        this.header = `<img class=\"nbtools-logo\" src=\"\" />\n                     <label class=\"nbtools-title\" data-traitlet=\"name\"></label>\n                     <label class=\"nbtools-subtitle\" data-traitlet=\"subtitle\"></label>\n                     <div class=\"nbtools-controls\">\n                         <button class=\"nbtools-collapse\">\n                             <span class=\"fa fa-minus\"></span>\n                         </button>\n                         <button class=\"nbtools-gear\">\n                             <span class=\"fa fa-cog\"></span>\n                             <span class=\"fa fa-caret-down\"></span>\n                         </button>\n                         <ul class=\"nbtools-menu\" style=\"display: none;\"></ul>\n                     </div>`;\n        this.body = `<div class=\"nbtools-description\" data-traitlet=\"description\"></div>\n                   <div class=\"nbtools-error\" data-traitlet=\"error\"></div>\n                   <div class=\"nbtools-info\" data-traitlet=\"info\"></div>`;\n        this.disconnected = `<div class=\"nbtools-disconnected\">\n                               <div class=\"nbtools-panel\">\n                                   <div class=\"nbtools-header\">Widget Disconnected From Kernel</div>\n                                   <div class=\"nbtools-body\">\n                                       <p>You need to run this cell before it can connect to the notebook kernel. Please click the Connect to Kernel button below.</p>\n                                       <div class=\"nbtools-connect nbtools-panel-button\"><button class=\"nbtools-connect nbtools-panel-button\">Connect to Kernel</button></div>\n                                   </div>\n                               </div>\n                           </div>`;\n    }\n    render() {\n        super.render();\n        // Build the widget\n        this.build();\n        // Apply the color\n        this.set_color();\n        this.model.on('change:color', this.set_color, this);\n        // Apply the logo\n        this.set_logo();\n        this.model.on('change:logo', this.set_logo, this);\n        // Set the traitlet values\n        this.traitlets.forEach(traitlet => this.traitlet_changed(traitlet));\n        // Hook in the traitlet change events\n        this.traitlets.forEach(traitlet => this.model.on(`change:${traitlet}`, this.traitlet_changed, this));\n        // Hook in the expand / collapse events\n        this.model.on('change:collapsed', this.toggle_collapse, this);\n        if (this.model.get('collapsed'))\n            this.toggle_collapse();\n        // Hide the code\n        this.toggle_code(false);\n        // Attach the extra menu options\n        this.attach_menu_options();\n        this.model.on('change:extra_menu_items', this.attach_menu_options, this);\n        // Allow menus to overflow the container\n        this.float_menus();\n        // Initialize the widget\n        this.initialize({ options: {} });\n        // Call any post render events\n        this.post_render();\n    }\n    build() {\n        // Parse the template\n        this.element = new DOMParser().parseFromString(this.template, \"text/html\")\n            .querySelector('div.nbtools');\n        // Apply the DOM class\n        if (this.dom_class)\n            this.element.classList.add(this.dom_class);\n        // Apply the header\n        this.element.querySelector('div.nbtools-header').innerHTML = this.header;\n        // Attach collapse event\n        const collapse = this.element.querySelector(\"button.nbtools-collapse\");\n        collapse.addEventListener(\"click\", () => {\n            this.model.set('collapsed', !this.model.get('collapsed'));\n            this.model.save_changes();\n        });\n        // Attach the gear event\n        const gear = this.element.querySelector(\"button.nbtools-gear\");\n        gear.addEventListener(\"click\", () => this.toggle_menu());\n        // Attach toggle code event\n        this.add_menu_item('Toggle Code View', () => this.toggle_code());\n        // Apply the body\n        this.element.querySelector('div.nbtools-body').innerHTML = this.body;\n        // Add the metadata flag\n        this.update_metadata();\n        // Attach the disconnected cover\n        this.element.appendChild(new DOMParser().parseFromString(this.disconnected, \"text/html\")\n            .querySelector('body > :first-child'));\n        this.attach_connect_event();\n        this.disconnected_sync_fix();\n        // Set the element\n        this.setElement(this.element);\n    }\n    set_logo() {\n        // Get custom logo\n        let logo = this.model.get('logo');\n        const logo_element = this.element.querySelector(\"img.nbtools-logo\");\n        // Fall back to default logo if no custom logo is set\n        if (!logo) {\n            logo = ContextManager.context().default_logo();\n            this.model.set('logo', logo);\n            this.model.save();\n        }\n        // Special case for \"None\" logo\n        if (logo.toLowerCase() === \"none\")\n            logo_element.classList.add('nbtools-logo-hidden');\n        else\n            logo_element.classList.remove('nbtools-logo-hidden');\n        // Set the logo\n        logo_element.src = logo;\n    }\n    set_color() {\n        const color = this.model.get('color').trim();\n        this.element.style.borderColor = color;\n        this.element.querySelectorAll('.nbtools-body button, .nbtools-header').forEach((e) => {\n            e.style.backgroundColor = color;\n        });\n    }\n    render_description(description, widget) {\n        return widget._render_or_hide('.nbtools-description', description, widget);\n    }\n    render_error(message, widget) {\n        return widget._render_or_hide('.nbtools-error', message, widget);\n    }\n    render_info(message, widget) {\n        return widget._render_or_hide('.nbtools-info', message, widget);\n    }\n    _render_or_hide(selector, message, widget) {\n        widget.element.querySelector(selector).style.display = message.trim() ? 'block' : 'none';\n        return message;\n    }\n    attach_connect_event() {\n        const button = this.element.querySelector('button.nbtools-connect');\n        button.addEventListener(\"click\", () => {\n            // Run all cells with disconnected nbtools widgets\n            ContextManager.context().run_tool_cells();\n        });\n    }\n    /**\n     * Update the cell metadata with the nbtools flag\n     */\n    update_metadata() {\n        if (!ContextManager.notebook_tracker)\n            return;\n        if (!ContextManager.notebook_tracker.currentWidget)\n            return;\n        const cells = ContextManager.notebook_tracker.currentWidget.content.widgets;\n        for (let i = 0; i < cells.length; i++) {\n            const execution_area = cells[i].node.querySelector('.lm-Widget.p-Widget.jp-InputPrompt.jp-InputArea-prompt');\n            if (execution_area.innerText.includes('[*]')) {\n                ContextManager.context().make_tool_cell(cells[i]);\n                return;\n            }\n        }\n    }\n    disconnected_sync_fix() {\n        // Fix a bug that can occur when a disconnected widget and a connected widget are somehow rendered in the same cell\n        setTimeout(() => {\n            const cell = this.element.closest('.jp-Cell, .cell');\n            if (!cell)\n                return; // No cell found, bug cannot occur\n            // Do both connected and disconnected widgets appear in the cell?\n            const contains_disconnected = !!cell.querySelectorAll('.nbtools.jupyter-widgets-disconnected').length;\n            const contains_connected = !!cell.querySelectorAll('.nbtools:not(.jupyter-widgets-disconnected)').length;\n            // If they do, hide the irrelevant disconnected widgets\n            if (contains_disconnected && contains_connected) {\n                cell.querySelectorAll('.nbtools.jupyter-widgets-disconnected').forEach((e) => {\n                    e.style.display = 'none';\n                });\n            }\n        }, 100);\n    }\n    add_menu_item(label, callback, dom_class = null, menu = null, prepend = true) {\n        // Create the menu item\n        const item = new DOMParser().parseFromString(`<li>${label}</li>`, \"text/html\")\n            .querySelector('li');\n        // Apply the class if one is specified\n        if (dom_class)\n            item.classList.add(dom_class);\n        // Attach the menu item\n        if (!menu)\n            menu = this.element.querySelector('.nbtools-menu');\n        if (prepend)\n            menu.prepend(item);\n        else\n            menu.append(item);\n        // Attach the click event\n        item.addEventListener('click', () => callback());\n        return item;\n    }\n    traitlet_changed(event) {\n        const widget = this;\n        const name = typeof event === \"string\" ? event : Object.keys(event.changed)[0];\n        const elements = this.element.querySelectorAll(`[data-traitlet=${name}]`);\n        elements.forEach(element => {\n            if (name in this.renderers)\n                element.innerHTML = this.renderers[name](this.model.get(name), widget);\n            else\n                element.innerHTML = this.model.get(name);\n        });\n    }\n    toggle_code(display) {\n        const element = this.element;\n        ContextManager.context().toggle_code(element, display);\n    }\n    toggle_collapse() {\n        const body = this.element.querySelector(\".nbtools-body\");\n        const collapsed = body.style.display === \"none\" || body.style.height == \"0px\";\n        // Toggle the collapse button\n        const button = this.element.querySelector(\".nbtools-collapse > span\");\n        if (collapsed) {\n            button.classList.add('fa-minus');\n            button.classList.remove('fa-plus');\n        }\n        else {\n            button.classList.remove('fa-minus');\n            button.classList.add('fa-plus');\n        }\n        // Hide or show widget body\n        toggle(body);\n    }\n    toggle_menu() {\n        const gear = this.element.querySelector(\"button.nbtools-gear\");\n        const menu = this.element.querySelector(\".nbtools-menu\");\n        const collapsed = menu.style.display === \"none\";\n        // Hide or show the menu\n        if (collapsed)\n            menu.style.display = \"block\";\n        else\n            menu.style.display = \"none\";\n        // Hide the menu with the next click\n        const hide_next_click = function (event) {\n            if (gear.contains(event.target))\n                return;\n            menu.style.display = \"none\";\n            document.removeEventListener('click', hide_next_click);\n        };\n        document.addEventListener('click', hide_next_click);\n    }\n    create_menu_callback(item, template_vars = {}) {\n        // Create callback for string literal\n        if (typeof item === 'string')\n            return new Function(process_template(item, template_vars));\n        // Create callback for javascript event type\n        else if (item['action'] === 'javascript')\n            return () => eval(process_template(item['code'], template_vars));\n        // Create callback for cell event type\n        else if (item['action'] === 'cell')\n            return () => Toolbox.add_code_cell(process_template(item['code'], template_vars));\n        // Create callback for method event type\n        else if (item['action'] === 'method')\n            return () => {\n                if (!item['params'])\n                    this.send({ event: 'method', method: process_template(item['code'], template_vars) });\n                else\n                    this.send({ event: 'method', method: process_template(item['code'], template_vars), params: process_template(item['params'], template_vars) });\n            };\n        // Create callback for custom event type\n        else\n            return new Function(process_template(item['code'], template_vars));\n    }\n    attach_menu_options() {\n        // Clear any existing menu\n        const menu = this.element.querySelector('.nbtools-menu');\n        menu.querySelectorAll('.nbtools-menu-extra').forEach((e) => e.remove());\n        const menu_items = this.model.get('extra_menu_items');\n        Object.keys(menu_items).forEach((name) => {\n            const item = menu_items[name];\n            const callback = this.create_menu_callback(item);\n            this.add_menu_item(name, callback, 'nbtools-menu-extra');\n        });\n    }\n    float_menus() {\n        const fix_cell = () => {\n            const elements = [\n                this.el.closest('.lm-Widget.jp-OutputPrompt.jp-OutputArea-prompt'),\n                this.el.closest('.lm-Widget.lm-Panel.jp-OutputArea'),\n                this.el.closest('.lm-Widget.lm-Panel.jp-OutputArea-child'),\n                this.el.closest('.lm-Widget.lm-Panel.jp-OutputArea-output'),\n                this.el.closest('.lm-Widget.jp-OutputArea.jp-Cell-outputArea')\n            ];\n            elements.forEach((e) => {\n                if (e)\n                    e.style.overflow = 'visible';\n            });\n        };\n        this.el.addEventListener('click', fix_cell, { once: true });\n    }\n    /**\n     * Recursively trigger the 'displayed' event for all child widgets\n     *\n     * @param {DOMWidgetModel} model\n     * @param {DOMWidgetView | any} view\n     * @private\n     */\n    static _initialize_display(model, view) {\n        // Trigger the display for this widget\n        view.trigger('displayed');\n        // Recursively trigger the display for all child widgets\n        if ('children_views' in view) {\n            view.children_views.update(model.get('children')).then((children) => {\n                children.forEach((child) => {\n                    BaseWidgetView._initialize_display(child.model, child);\n                    child.el.widget = child;\n                });\n            });\n        }\n    }\n    /**\n     * Add the specified child widget to the view and initialize\n     *\n     * @param {string} element_selector\n     * @param {string} model_name\n     */\n    attach_child_widget(element_selector, model_name) {\n        const element = this.element.querySelector(element_selector);\n        const model = this.model.get(model_name);\n        this.create_child_view(model).then((view) => {\n            element.appendChild(view.el);\n            BaseWidgetView._initialize_display(model, view);\n            return view;\n        }).catch(reject(`Could not add ${model_name} to ${element_selector}`, true));\n    }\n    basics() { return this.traitlets; } // Return the list of basic traitlets\n    post_render() { } // Empty function, can be overridden in subclasses\n}\n",
+        "import { hide, show, toggle } from \"./utils\";\nimport { NotebookPanel } from \"@jupyterlab/notebook\";\nimport { CodeCell } from \"@jupyterlab/cells\";\nexport class ContextManager {\n    static context() {\n        if (!ContextManager._context) {\n            if (ContextManager.is_lab())\n                ContextManager._context = new LabContext();\n            else if (ContextManager.is_notebook())\n                ContextManager._context = new NotebookContext();\n            else\n                ContextManager._context = new EmbedContext();\n        }\n        return ContextManager._context;\n    }\n    /**\n     * Determine is this is running in JupyterLab\n     *\n      * @returns {boolean}\n     */\n    static is_lab() {\n        // The assumption is that only JupyterLab will provide an initialized NotebookTracker object\n        // If a better way to detect the environment becomes available, use that instead\n        return !!ContextManager.notebook_tracker;\n        // A previous implementation replied on checking the DOM\n        // return !!document.querySelector(\"#main.jp-LabShell\")\n    }\n    /**\n     * Determine if this is running in the classic Jupyter Notebook\n     *\n     * @returns {boolean}\n     */\n    static is_notebook() {\n        // Check if the Jupyter global variable has been defined\n        return !!(window['Jupyter']);\n    }\n}\n/**\n * Abstract base class representing the context in which the widgets are running.\n * Contexts include: JupyterLab, Jupyter Notebook and Embedded.\n */\nclass Context {\n}\n/**\n * Context handler for JupyterLab\n */\nclass LabContext extends Context {\n    /**\n     * Toggle hiding or or showing the code for the specified cell\n     *\n     * @param {HTMLElement} element\n     * @param {boolean} display\n     */\n    toggle_code(element, display) {\n        setTimeout(() => {\n            let input_block = element.closest('.jp-Cell');\n            if (input_block)\n                input_block = input_block.querySelector('.jp-Cell-inputWrapper');\n            // Set display to toggle if not specified\n            if (!!display)\n                show(input_block);\n            else if (display === false)\n                hide(input_block, '30px');\n            else\n                toggle(input_block, '30px');\n        }, 100);\n    }\n    /**\n     * Execute the indicated cell in the notebook\n     *\n     * @param cell\n     */\n    run_cell(cell = null) {\n        if (!ContextManager.notebook_tracker)\n            return; // If no notebook_tracker, do nothing\n        // If cell is falsy, default to the active cell\n        if (!cell)\n            cell = ContextManager.notebook_tracker.activeCell;\n        // If this is a code cell\n        if (cell instanceof CodeCell) {\n            const current = ContextManager.notebook_tracker.currentWidget;\n            if (current) {\n                CodeCell.execute(cell, current.context.sessionContext);\n            }\n        }\n        // If this is a markdown cell\n        // if (ContextManager.notebook_tracker.activeCell instanceof MarkdownCell)\n        //     MarkdownCell.renderInput(ContextManager.notebook_tracker.activeCell)\n    }\n    /**\n     * Execute all cells with nbtools widgets in the current notebook\n     */\n    run_tool_cells() {\n        if (!ContextManager.notebook_tracker)\n            return; // If no notebook_tracker, do nothing\n        if (!ContextManager.notebook_tracker.currentWidget)\n            return; // If no notebook selected, do nothing\n        const cell_widgets = ContextManager.notebook_tracker.currentWidget.content.widgets;\n        cell_widgets.forEach((widget) => {\n            if (this.is_tool_cell(widget))\n                this.run_cell(widget);\n        });\n    }\n    /**\n     * Get the relative path to the current notebook\n     */\n    notebook_path() {\n        if (!ContextManager.notebook_tracker)\n            return ''; // If no notebook_tracker, do nothing\n        if (!ContextManager.notebook_tracker.currentWidget)\n            return ''; // If no active notebook, do nothing\n        if (!ContextManager.notebook_tracker.currentWidget.context)\n            return ''; // If no context, do nothing\n        const notebook_context = ContextManager.notebook_tracker.currentWidget.context;\n        const notebook_path = notebook_context.path;\n        const directory_path = notebook_path.substring(0, notebook_path.lastIndexOf(\"/\") + 1);\n        return directory_path;\n    }\n    /**\n     * Determines if the given cell contains a notebook tool widget\n     *\n     * @param cell\n     * @returns boolean\n     */\n    is_tool_cell(cell) {\n        // Check for nbtools metadata\n        if (cell.model.metadata.get('nbtools'))\n            return true;\n        // Check for an existing disconnected nbtools widget\n        const dom_node = cell.node || cell.element;\n        if (!!dom_node)\n            return !!dom_node.querySelector('.nbtools');\n        else\n            return false;\n    }\n    /**\n     * Path to the default GenePattern logo\n     */\n    default_logo() {\n        return require(\"../style/g2nb_logo.png\").default;\n    }\n    /**\n     * Path to the default GenePattern icon\n     */\n    default_icon() {\n        return require(\"../style/icon.svg\").default;\n    }\n    /**\n     * Return the id of the current notebook's kernel\n     *\n     * @param notebook\n     */\n    kernel_id(notebook) {\n        // If the current widget isn't a notebook, there is no kernel\n        if (!(notebook instanceof NotebookPanel))\n            return null;\n        // Protect against null\n        if (!notebook ||\n            !notebook.context ||\n            !notebook.context.sessionContext ||\n            !notebook.context.sessionContext.session ||\n            !notebook.context.sessionContext.session.kernel)\n            return null;\n        return notebook.context.sessionContext.session.kernel.id;\n    }\n    /**\n     * Function to execute when the notebook is opened and selected\n     *\n     * @param callback\n     */\n    notebook_focus(callback) {\n        const notebook_tracker = ContextManager.notebook_tracker;\n        notebook_tracker && notebook_tracker.activeCellChanged.connect(() => {\n            const current_widget = notebook_tracker.currentWidget;\n            callback(current_widget);\n        });\n    }\n    /**\n     * Execute the callback when the current kernel is ready\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_ready(current, callback) {\n        // If the current widget isn't a notebook, there is no kernel\n        if (!(current instanceof NotebookPanel))\n            return;\n        current.context.sessionContext.ready.then(() => callback());\n    }\n    /**\n     * Execute the callback every time the kernel is changed or restarts\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_changed(current, callback) {\n        current.context.sessionContext.kernelChanged.connect(() => callback());\n    }\n    /**\n     * Send the provided code to the kernel\n     *\n     * @param notebook\n     * @param code\n     */\n    execute_code(notebook, code) {\n        const current = notebook;\n        if (!current.context.sessionContext.session ||\n            !current.context.sessionContext.session.kernel)\n            return; // Protect against null kernels\n        // Import the default tools\n        current.context.sessionContext.session.kernel.requestExecute({ code: code });\n    }\n    /**\n     * Create a new comm\n     *\n     * @param current\n     * @param name\n     * @param callback\n     */\n    create_comm(current, name, callback) {\n        const kernel = current.context.sessionContext.session.kernel;\n        const comm = kernel.createComm(name);\n        comm.onMsg = callback;\n        comm.open({}); // Open the comm\n        return comm;\n    }\n    /**\n     * Sets whether this is a nbtools widget cell\n     *\n     * @param cell\n     * @param is_widget_cell\n     */\n    make_tool_cell(cell, is_widget_cell = true) {\n        if (is_widget_cell)\n            cell.model.metadata.set('nbtools', { 'force_display': true });\n        else\n            cell.model.metadata.clear();\n    }\n}\n/**\n * Context handler for the classic Jupyter Notebook\n */\nclass NotebookContext extends Context {\n    /**\n     * Toggle hiding or or showing the code for the specified cell\n     *\n     * @param {HTMLElement} element\n     * @param {boolean} display\n     */\n    toggle_code(element, display) {\n        setTimeout(() => {\n            const cell_element = element.closest(\".cell\");\n            if (!cell_element)\n                return; // Widget has not yet been added to the DOM\n            const code = cell_element.querySelector(\".input\");\n            // Set display to toggle if not specified\n            if (!!display)\n                show(code);\n            else if (display === false)\n                hide(code);\n            else\n                toggle(code);\n        }, 10);\n    }\n    /**\n     * Execute the indicated cell in the notebook\n     *\n     * @param cell\n     */\n    run_cell(cell) {\n        window.Jupyter.notebook.execute_cell(cell);\n    }\n    /**\n     * Execute all cells with nbtools widgets in the current notebook\n     */\n    run_tool_cells() {\n        const cells_to_run = [];\n        window.Jupyter.notebook.get_cells().forEach((cell, index) => {\n            if (this.is_tool_cell(cell))\n                cells_to_run.push(index);\n        });\n        window.Jupyter.notebook.execute_cells(cells_to_run);\n    }\n    notebook_path() {\n        return window.Jupyter.notebook.path;\n    }\n    base_path() {\n        const body = document.querySelector('body');\n        if (!body)\n            return ''; // If there is no body, unable to get path\n        return body.getAttribute('data-base-url') + 'nbextensions/nbtools/';\n    }\n    /**\n     * Determines if the given cell contains a notebook tool widget\n     *\n     * @param cell\n     * @returns boolean\n     */\n    is_tool_cell(cell) {\n        const dom_node = cell.node || cell.element;\n        if (!!dom_node)\n            return !!dom_node.find('.nbtools').length;\n        else\n            return false;\n    }\n    /**\n     * Sets whether this is a nbtools widget cell\n     *\n     * @param cell\n     * @param is_widget_cell\n     */\n    make_tool_cell(cell, is_widget_cell = true) {\n        // TODO: Test in Jupyter Notebook\n        if (is_widget_cell)\n            cell.metadata.set('nbtools', { 'force_display': true });\n        else\n            cell.metadata.clear();\n    }\n    /**\n     * Path to the default GenePattern logo\n     */\n    default_logo() {\n        return this.base_path() + require(\"../style/g2nb_logo.png\").default;\n    }\n    /**\n     * Path to the default GenePattern icon\n     */\n    default_icon() {\n        return this.base_path() + require(\"../style/icon.svg\").default;\n    }\n    /**\n     * Return the id of the current notebook's kernel\n     *\n     * @param notebook\n     */\n    kernel_id(notebook) {\n        return window.Jupyter.notebook.kernel.id;\n    }\n    /**\n     * Function to execute when the notebook is opened and selected\n     *\n     * @param callback\n     */\n    notebook_focus(callback) {\n        window.Jupyter.notebook.events.ready(() => {\n            callback(window.Jupyter.notebook);\n        });\n    }\n    /**\n     * Execute the callback when the current kernel is ready\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_ready(current, callback) {\n        setTimeout(() => {\n            if (window.Jupyter.notebook.kernel.is_connected())\n                callback(window.Jupyter.notebook);\n            else\n                window.Jupyter.notebook.events.one('kernel_ready.Kernel', () => {\n                    callback(window.Jupyter.notebook);\n                });\n        }, 100);\n    }\n    /**\n     * Execute the callback every time the kernel is changed or restarts\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_changed(current, callback) {\n        window.Jupyter.notebook.events.on('kernel_ready.Kernel', () => {\n            callback(window.Jupyter.notebook);\n        });\n    }\n    /**\n     * Send the provided code to the kernel\n     *\n     * @param notebook\n     * @param code\n     */\n    execute_code(notebook, code) {\n        window.Jupyter.notebook.kernel.execute(code);\n    }\n    /**\n     * Create a new comm\n     *\n     * @param current\n     * @param name\n     * @param callback\n     */\n    create_comm(current, name, callback) {\n        let comm = window.Jupyter.notebook.kernel.comm_manager.new_comm(name);\n        comm.on_msg(callback);\n        return comm;\n    }\n}\n/**\n * Context handler for embedded widgets\n */\nclass EmbedContext extends Context {\n    /**\n     * No cells in this context, so do nothing\n     *\n     * @param {HTMLElement} element\n     * @param {boolean} display\n     */\n    toggle_code(element, display) { }\n    /**\n     * No cells in this context, so do nothing\n     * @param cell\n     */\n    run_cell(cell) { }\n    /**\n     * No cells in this context, so do nothing\n     */\n    run_tool_cells() { }\n    /**\n     * No notebook in this context\n     */\n    notebook_path() { return ''; }\n    base_path() {\n        const body = document.querySelector('body');\n        if (!body)\n            return ''; // If there is no body, unable to get path\n        return body.getAttribute('data-base-url') + 'nbextensions/nbtools/';\n    }\n    /**\n     * Sets whether this is a nbtools widget cell\n     *\n     * @param cell\n     * @param is_widget_cell\n     */\n    make_tool_cell(cell, is_widget_cell = true) {\n        // TODO: Test in embedded context\n        if (is_widget_cell)\n            cell.metadata.set('nbtools', { 'force_display': true });\n        else\n            cell.metadata.clear();\n    }\n    /**\n     * Determines if the given cell contains a notebook tool widget\n     *\n     * @param cell\n     * @returns boolean\n     */\n    is_tool_cell(cell) {\n        const dom_node = cell.node || cell.element;\n        if (!!dom_node)\n            return !!dom_node.querySelector('.nbtools');\n        else\n            return false;\n    }\n    /**\n     * Path to the default GenePattern logo\n     */\n    default_logo() {\n        return this.base_path() + require(\"../style/g2nb_logo.png\").default;\n    }\n    /**\n     * Path to the default GenePattern icon\n     */\n    default_icon() {\n        return require(\"../style/icon.svg\").default;\n    }\n    /**\n     * Return the id of the current notebook's kernel\n     *\n     * @param notebook\n     */\n    kernel_id(notebook) {\n        return null;\n    }\n    /**\n     * Function to execute when the notebook is opened and selected\n     *\n     * @param callback\n     */\n    notebook_focus(callback) { }\n    /**\n     * Execute the callback when the current kernel is ready\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_ready(current, callback) { }\n    /**\n     * Execute the callback every time the kernel is changed or restarts\n     *\n     * @param current\n     * @param callback\n     */\n    kernel_changed(current, callback) {\n        // FIXME: Global Jupyter variable may not be accessible in newer version of voila\n        window.Jupyter.notebook.events.on('kernel_ready.Kernel', () => {\n            callback(window.Jupyter.notebook);\n        });\n    }\n    /**\n     * Send the provided code to the kernel\n     *\n     * @param notebook\n     * @param code\n     */\n    execute_code(notebook, code) {\n        // FIXME: Global Jupyter variable may not be accessible in newer version of voila\n        window.Jupyter.notebook.kernel.execute(code);\n    }\n    /**\n     * Create a new comm\n     *\n     * @param current\n     * @param name\n     * @param callback\n     */\n    create_comm(current, name, callback) {\n        // FIXME: Global Jupyter variable may not be accessible in newer version of voila\n        let comm = window.Jupyter.notebook.kernel.comm_manager.new_comm(name);\n        comm.on_msg(callback);\n        return comm;\n    }\n}\n",
         "import { ContextManager } from \"./context\";\nimport { Token } from \"@lumino/coreutils\";\nimport { extract_file_name, extract_file_type } from \"./utils\";\nexport const IDataRegistry = new Token(\"nbtools.data\");\nexport class DataRegistry {\n    // { 'kernel_id': { 'origin': { 'identifier': data } } }\n    /**\n     * Initialize the DataRegistry and connect event handlers\n     */\n    constructor() {\n        this.current = null; // Reference to the currently selected notebook or other widget\n        this.kernel_data_cache = {}; // Keep a cache of kernels to registered data\n        // Lazily assign the data registry to the context\n        if (!ContextManager.data_registry)\n            ContextManager.data_registry = this;\n        ContextManager.context().notebook_focus((current_widget) => {\n            // Current notebook hasn't changed, no need to do anything, return\n            if (this.current === current_widget)\n                return;\n            // Otherwise, update the current notebook reference\n            this.current = current_widget;\n        });\n    }\n    /**\n     * Register data for the sent to/come from menus\n     * Return whether registration was successful or not\n     *\n     * @param origin\n     * @param identifier\n     * @param kind\n     * @param data\n     */\n    register({ origin = null, uri = null, kind = null, data = null }) {\n        // Use origin, identifier and kind to initialize data, if needed\n        if (!data)\n            data = new Data(origin, uri, kind);\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return false; // If no kernel, do nothing\n        // Lazily initialize dict for kernel cache\n        let cache = this.kernel_data_cache[kernel_id];\n        if (!cache)\n            cache = this.kernel_data_cache[kernel_id] = {};\n        // Lazily initialize dict for origin\n        let origin_data = cache[data.origin];\n        if (!origin_data)\n            origin_data = cache[data.origin] = {};\n        // Add to cache and return\n        origin_data[data.uri] = data;\n        return true;\n    }\n    /**\n     * Unregister data with the given origin and identifier\n     * Return the unregistered data object\n     * Return null if un-registration was unsuccessful\n     *\n     * @param origin\n     * @param identifier\n     * @param kind\n     * @param data\n     */\n    unregister({ origin = null, uri = null, kind = null, data = null }) {\n        // Use origin, identifier and kind to initialize data, if needed\n        if (!data)\n            data = new Data(origin, uri, kind);\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return null; // If no kernel, do nothing\n        // If unable to retrieve cache, return null\n        const cache = this.kernel_data_cache[kernel_id];\n        if (!cache)\n            return null;\n        // If unable to retrieve origin, return null\n        const origin_data = cache[data.origin];\n        if (!origin_data)\n            return null;\n        // If unable to find identifier, return null;\n        const found = origin_data[data.uri];\n        if (!found)\n            return null;\n        // Remove from the registry and return\n        delete origin_data[data.uri];\n        return found;\n    }\n    /**\n     * Get all data that matches one of the specified kinds or origins\n     * If kinds or origins is null or empty, accept all kinds or origins, respectively\n     *\n     * @param kinds\n     * @param origins\n     */\n    get_data({ kinds = null, origins = null }) {\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return {}; // If no kernel, return empty\n        // If unable to retrieve cache, return empty\n        const cache = this.kernel_data_cache[kernel_id];\n        if (!cache)\n            return {};\n        // Compile map of data with a matching origin and kind\n        const matching = {};\n        for (let origin of Object.keys(cache)) {\n            if (origins === null || origins.length === 0 || origins.includes(origin)) {\n                const hits = {};\n                for (let data of Object.values(cache[origin])) {\n                    if (kinds === null || kinds.length === 0 || kinds.includes(data.kind))\n                        hits[data.label] = data.uri;\n                }\n                if (Object.keys(hits).length > 0)\n                    matching[origin] = hits;\n            }\n        }\n        return matching;\n    }\n    /**\n     * Retrieve the kernel ID from the currently selected notebook\n     * Return null if no kernel or no notebook selected\n     */\n    current_kernel_id() {\n        return ContextManager.context().kernel_id(this.current);\n    }\n}\nexport class Data {\n    constructor(origin, uri, label = null, kind = null) {\n        this.origin = origin;\n        this.uri = uri;\n        this.label = !!label ? label : extract_file_name(uri);\n        this.kind = !!kind ? kind : extract_file_type(uri);\n    }\n}\n",
-        "import { NotebookPanel } from \"@jupyterlab/notebook\";\nimport { send_notification } from \"./utils\";\nimport { ContextManager } from \"./context\";\nimport { Token } from \"@lumino/coreutils\";\nexport const IToolRegistry = new Token(\"nbtools\");\nexport class ToolRegistry {\n    /**\n     * Initialize the ToolRegistry and connect event handlers\n     */\n    constructor() {\n        this.current = null; // Reference to the currently selected notebook or other widget\n        this._update_callbacks = []; // Functions to call when an update happens\n        this.kernel_tool_cache = {}; // Keep a cache of kernels to registered tools\n        this.kernel_import_cache = {}; // Keep a cache of whether nbtools has been imported\n        // Lazily assign the tool registry to the context\n        if (!ContextManager.tool_registry)\n            ContextManager.tool_registry = this;\n        ContextManager.context().notebook_focus((current_widget) => {\n            // Current notebook hasn't changed, no need to do anything, return\n            if (this.current === current_widget)\n                return;\n            // Otherwise, update the current notebook reference\n            this.current = current_widget;\n            // If the current selected widget isn't a notebook, no comm is needed\n            if (!(this.current instanceof NotebookPanel) && ContextManager.is_lab())\n                return;\n            // Initialize the comm\n            this.init_comm();\n            // Load the default tools\n            this.import_default_tools();\n        });\n    }\n    import_default_tools() {\n        ContextManager.context().kernel_changed(this.current, () => {\n            ContextManager.context().execute_code(this.current, 'from nbtools import import_defaults\\nimport_defaults()');\n        });\n    }\n    /**\n     * Initialize the comm between the notebook widget kernel and the ToolManager\n     */\n    init_comm() {\n        ContextManager.context().kernel_ready(this.current, () => {\n            const current = this.current;\n            // Create a new comm that connects to the nbtools_comm target\n            const connect_comm = () => {\n                const comm = ContextManager.context().create_comm(current, 'nbtools_comm', (msg) => {\n                    // Handle message sent by the kernel\n                    const data = msg.content.data;\n                    if (data.func === 'update')\n                        this.update_tools(data.payload);\n                    else if (data.func === 'notification')\n                        send_notification(data.payload.message, data.payload.sender, ContextManager.context().default_logo());\n                    else\n                        console.error('ToolRegistry received unknown message: ' + data);\n                });\n                window.comm = comm;\n                // Request the current tool list\n                comm.send({\n                    'func': 'request_update'\n                });\n            };\n            // When the kernel restarts or is changed, reconnect the comm\n            ContextManager.context().kernel_changed(current, () => connect_comm());\n            // Connect to the comm upon initial startup\n            connect_comm();\n            // Update tools from the cache\n            this.update_from_cache();\n        });\n    }\n    /**\n     * Get tools from the cache and make registered callbacks\n     */\n    update_from_cache() {\n        // Get the kernel ID\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return; // Do nothing if null\n        // Get tools from the cache\n        const tool_list = this.kernel_tool_cache[kernel_id];\n        // Make registered callbacks for when tools are updated\n        this._update_callbacks.forEach((callback) => {\n            callback(tool_list);\n        });\n    }\n    /**\n     * Message the kernel, requesting an update to the tools cache\n     *\n     * @param comm\n     */\n    request_update(comm) {\n        comm.send({ 'func': 'request_update' });\n    }\n    /**\n     * Register an update callback with the ToolRegistry\n     *\n     * @param callback\n     */\n    on_update(callback) {\n        this._update_callbacks.push(callback);\n    }\n    /**\n     * Retrieve the kernel ID from the currently selected notebook\n     * Return null if no kernel or no notebook selected\n     */\n    current_kernel_id() {\n        return ContextManager.context().kernel_id(this.current);\n    }\n    /**\n     * Update the tools cache for the current kernel\n     *\n     * @param message\n     */\n    update_tools(message) {\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return; // Do nothing if no kernel\n        // Parse the message\n        const tool_list = message['tools'];\n        const needs_import = !!message['import'];\n        // Update the cache\n        this.kernel_tool_cache[kernel_id] = tool_list;\n        this.kernel_import_cache[kernel_id] = needs_import;\n        // Make registered callbacks when tools are updated\n        this._update_callbacks.forEach((callback) => {\n            callback(tool_list);\n        });\n    }\n    /**\n     * Query whether nbtools has been imported in this kernel\n     */\n    needs_import() {\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return true; // Assume true if no kernel\n        // Get import status from the cache and protect against undefined\n        return !this.kernel_import_cache[kernel_id];\n    }\n    /**\n     * Returns a list of all currently registered tools\n     *\n     * @returns {Array} - A list of registered tools\n     */\n    list() {\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return []; // Empty list if no kernel\n        // Get tools from the cache and protect against undefined\n        const tools = this.kernel_tool_cache[kernel_id];\n        if (!tools)\n            return [];\n        return Object.keys(tools).map(function (key) {\n            return tools[key];\n        });\n    }\n    /**\n     * Has this tool already been registered?\n     *\n     * @param origin\n     * @param id\n     * @returns {boolean}\n     */\n    has_tool(origin, id) {\n        let found_tool = false;\n        this.list().forEach(tool => {\n            if (tool.id === id && tool.origin === origin)\n                found_tool = true;\n        });\n        return found_tool;\n    }\n}\n",
+        "import { NotebookPanel } from \"@jupyterlab/notebook\";\nimport { send_notification } from \"./utils\";\nimport { ContextManager } from \"./context\";\nimport { Token } from \"@lumino/coreutils\";\nexport const IToolRegistry = new Token(\"nbtools\");\nexport class ToolRegistry {\n    /**\n     * Initialize the ToolRegistry and connect event handlers\n     */\n    constructor(setting_dict) {\n        this.current = null; // Reference to the currently selected notebook or other widget\n        this._update_callbacks = []; // Functions to call when an update happens\n        this.kernel_tool_cache = {}; // Keep a cache of kernels to registered tools\n        this.kernel_import_cache = {}; // Keep a cache of whether nbtools has been imported\n        // Lazily assign the tool registry to the context\n        if (!ContextManager.tool_registry)\n            ContextManager.tool_registry = this;\n        ContextManager.context().notebook_focus((current_widget) => {\n            // Current notebook hasn't changed, no need to do anything, return\n            if (this.current === current_widget)\n                return;\n            // Otherwise, update the current notebook reference\n            this.current = current_widget;\n            // If the current selected widget isn't a notebook, no comm is needed\n            if (!(this.current instanceof NotebookPanel) && ContextManager.is_lab())\n                return;\n            // Initialize the comm\n            this.init_comm();\n            // Load the default tools\n            this.import_default_tools();\n            // Ensure rendering of tool cells\n            if (setting_dict.force_render)\n                this.ensure_rendering();\n        });\n    }\n    ensure_rendering() {\n        ContextManager.context().kernel_ready(this.current, () => {\n            if (!this.current)\n                return; // Return if no notebook is selected\n            ContextManager.context().run_tool_cells();\n        });\n    }\n    import_default_tools() {\n        ContextManager.context().kernel_changed(this.current, () => {\n            ContextManager.context().execute_code(this.current, 'from nbtools import import_defaults\\nimport_defaults()');\n        });\n    }\n    /**\n     * Initialize the comm between the notebook widget kernel and the ToolManager\n     */\n    init_comm() {\n        ContextManager.context().kernel_ready(this.current, () => {\n            const current = this.current;\n            // Create a new comm that connects to the nbtools_comm target\n            const connect_comm = () => {\n                const comm = ContextManager.context().create_comm(current, 'nbtools_comm', (msg) => {\n                    // Handle message sent by the kernel\n                    const data = msg.content.data;\n                    if (data.func === 'update')\n                        this.update_tools(data.payload);\n                    else if (data.func === 'notification')\n                        send_notification(data.payload.message, data.payload.sender, ContextManager.context().default_logo());\n                    else\n                        console.error('ToolRegistry received unknown message: ' + data);\n                });\n                window.comm = comm;\n                // Request the current tool list\n                comm.send({\n                    'func': 'request_update'\n                });\n            };\n            // When the kernel restarts or is changed, reconnect the comm\n            ContextManager.context().kernel_changed(current, () => connect_comm());\n            // Connect to the comm upon initial startup\n            connect_comm();\n            // Update tools from the cache\n            this.update_from_cache();\n        });\n    }\n    /**\n     * Get tools from the cache and make registered callbacks\n     */\n    update_from_cache() {\n        // Get the kernel ID\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return; // Do nothing if null\n        // Get tools from the cache\n        const tool_list = this.kernel_tool_cache[kernel_id];\n        // Make registered callbacks for when tools are updated\n        this._update_callbacks.forEach((callback) => {\n            callback(tool_list);\n        });\n    }\n    /**\n     * Message the kernel, requesting an update to the tools cache\n     *\n     * @param comm\n     */\n    request_update(comm) {\n        comm.send({ 'func': 'request_update' });\n    }\n    /**\n     * Register an update callback with the ToolRegistry\n     *\n     * @param callback\n     */\n    on_update(callback) {\n        this._update_callbacks.push(callback);\n    }\n    /**\n     * Retrieve the kernel ID from the currently selected notebook\n     * Return null if no kernel or no notebook selected\n     */\n    current_kernel_id() {\n        return ContextManager.context().kernel_id(this.current);\n    }\n    /**\n     * Update the tools cache for the current kernel\n     *\n     * @param message\n     */\n    update_tools(message) {\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return; // Do nothing if no kernel\n        // Parse the message\n        const tool_list = message['tools'];\n        const needs_import = !!message['import'];\n        // Update the cache\n        this.kernel_tool_cache[kernel_id] = tool_list;\n        this.kernel_import_cache[kernel_id] = needs_import;\n        // Make registered callbacks when tools are updated\n        this._update_callbacks.forEach((callback) => {\n            callback(tool_list);\n        });\n    }\n    /**\n     * Query whether nbtools has been imported in this kernel\n     */\n    needs_import() {\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return true; // Assume true if no kernel\n        // Get import status from the cache and protect against undefined\n        return !this.kernel_import_cache[kernel_id];\n    }\n    /**\n     * Returns a list of all currently registered tools\n     *\n     * @returns {Array} - A list of registered tools\n     */\n    list() {\n        const kernel_id = this.current_kernel_id();\n        if (!kernel_id)\n            return []; // Empty list if no kernel\n        // Get tools from the cache and protect against undefined\n        const tools = this.kernel_tool_cache[kernel_id];\n        if (!tools)\n            return [];\n        return Object.keys(tools).map(function (key) {\n            return tools[key];\n        });\n    }\n    /**\n     * Has this tool already been registered?\n     *\n     * @param origin\n     * @param id\n     * @returns {boolean}\n     */\n    has_tool(origin, id) {\n        let found_tool = false;\n        this.list().forEach(tool => {\n            if (tool.id === id && tool.origin === origin)\n                found_tool = true;\n        });\n        return found_tool;\n    }\n}\n",
         "import { PanelLayout, Widget } from '@lumino/widgets';\nimport { toggle } from \"./utils\";\nimport { ContextManager } from \"./context\";\nimport { NotebookActions, NotebookPanel } from \"@jupyterlab/notebook\";\nexport class ToolBrowser extends Widget {\n    constructor() {\n        super();\n        this.search = null;\n        this.toolbox = null;\n        this.addClass('nbtools-browser');\n        this.layout = new PanelLayout();\n        this.search = new SearchBox();\n        this.toolbox = new Toolbox(this.search);\n        this.layout.addWidget(this.search);\n        this.layout.addWidget(this.toolbox);\n    }\n}\nexport class Toolbox extends Widget {\n    constructor(associated_search) {\n        super();\n        this.last_update = 0;\n        this.update_waiting = false;\n        this.search = associated_search;\n        this.addClass('nbtools-toolbox');\n        this.addClass('nbtools-wrapper');\n        // Update the toolbox when the tool registry changes\n        ContextManager.tool_registry.on_update(() => {\n            // If the last update was more than 10 seconds ago, update the toolbox\n            if (this.update_stale())\n                this.fill_toolbox();\n            else\n                this.queue_update(); // Otherwise, queue an update if not already waiting for one\n        });\n        // Fill the toolbox with the registered tools\n        this.fill_toolbox();\n    }\n    update_stale() {\n        return this.last_update + (3 * 1000) < Date.now();\n    }\n    queue_update() {\n        // If no update is waiting, queue an update\n        if (!this.update_waiting) {\n            setTimeout(() => {\n                this.fill_toolbox(); // Fill the toolbox\n                this.update_waiting = false; // And mark as no update queued\n            }, Math.abs(this.last_update + (3 * 1000) - Date.now())); // Queue for 3 seconds since last update\n            this.update_waiting = true; // And mark as queued\n        }\n    }\n    static add_tool_cell(tool) {\n        // Check to see if nbtools needs to be imported\n        const import_line = ContextManager.tool_registry.needs_import() ? 'import nbtools\\n\\n' : '';\n        // Add and run a code cell with the generated tool code\n        Toolbox.add_code_cell(import_line + `nbtools.tool(id='${tool.id}', origin='${tool.origin}')`);\n    }\n    static add_code_cell(code) {\n        if (!ContextManager.notebook_tracker)\n            return; // If no NotebookTracker, do nothing\n        const current = ContextManager.tool_registry.current;\n        if (!current || !(current instanceof NotebookPanel))\n            return; // If no notebook is currently selected, return\n        let cell = ContextManager.notebook_tracker.activeCell;\n        if (!cell)\n            return; // If no cell is selected, do nothing\n        // If the currently selected cell isn't empty, insert a new one below and select it\n        const current_cell_code = cell.model.value.text.trim();\n        if (!!current_cell_code)\n            NotebookActions.insertBelow(current.content);\n        // Fill the cell with the tool's code\n        cell = ContextManager.notebook_tracker.activeCell; // The active cell may just have been updated\n        if (cell)\n            cell.model.value.text = code;\n        // Run the cell\n        return NotebookActions.run(current.content, current.context.sessionContext);\n    }\n    fill_toolbox() {\n        this.last_update = Date.now();\n        // First empty the toolbox\n        this.empty_toolbox();\n        // Get the list of tools\n        const tools = ContextManager.tool_registry.list();\n        // Organize by origin and sort\n        const organized_tools = this.organize_tools(tools);\n        const origins = Object.keys(organized_tools);\n        origins.sort((a, b) => {\n            const a_name = a.toLowerCase();\n            const b_name = b.toLowerCase();\n            return (a_name < b_name) ? -1 : (a_name > b_name) ? 1 : 0;\n        });\n        // Add each origin\n        origins.forEach((origin) => {\n            const origin_box = this.add_origin(origin);\n            organized_tools[origin].forEach((tool) => {\n                this.add_tool(origin_box, tool);\n            });\n        });\n        // Apply search filter after refresh\n        this.search.filter(this.search.node.querySelector('input.nbtools-search'));\n    }\n    organize_tools(tool_list) {\n        const organized = {};\n        // Group tools by origin\n        tool_list.forEach((tool) => {\n            if (tool.origin in organized)\n                organized[tool.origin].push(tool); // Add tool to origin\n            else\n                organized[tool.origin] = [tool]; // Lazily create origin\n        });\n        // Sort the tools in each origin\n        Object.keys(organized).forEach((origin) => {\n            organized[origin].sort((a, b) => {\n                const a_name = a.name.toLowerCase();\n                const b_name = b.name.toLowerCase();\n                return (a_name < b_name) ? -1 : (a_name > b_name) ? 1 : 0;\n            });\n        });\n        // Return the organized set of notebooks\n        return organized;\n    }\n    empty_toolbox() {\n        this.node.innerHTML = '';\n    }\n    add_origin(name) {\n        // Create the HTML DOM element\n        const origin_wrapper = document.createElement('div');\n        origin_wrapper.innerHTML = `\n            <header class=\"nbtools-origin\" title=\"${name}\">\n                <span class=\"nbtools-expanded nbtools-collapse jp-Icon jp-Icon-16 jp-ToolbarButtonComponent-icon\"></span>\n                ${name}\n            </header>\n            <ul class=\"nbtools-origin\" title=\"${name}\"></ul>`;\n        // Attach the expand / collapse functionality\n        const collapse = origin_wrapper.querySelector('span.nbtools-collapse');\n        collapse.addEventListener(\"click\", () => this.toggle_collapse(origin_wrapper));\n        // Add to the toolbox\n        this.node.append(origin_wrapper);\n        return origin_wrapper;\n    }\n    add_tool(origin, tool) {\n        const list = origin.querySelector('ul');\n        const tool_wrapper = document.createElement('li');\n        tool_wrapper.classList.add('nbtools-tool');\n        tool_wrapper.setAttribute('title', 'Click to add to notebook');\n        tool_wrapper.innerHTML = `\n            <div class=\"nbtools-add\">+</div>\n            <div class=\"nbtools-header\">${tool.name}</div>\n            <div class=\"nbtools-description\">${tool.description}</div>`;\n        if (list)\n            list.append(tool_wrapper);\n        // Add the click event\n        tool_wrapper.addEventListener(\"click\", () => {\n            Toolbox.add_tool_cell(tool);\n        });\n    }\n    toggle_collapse(origin_wrapper) {\n        const list = origin_wrapper.querySelector(\"ul.nbtools-origin\");\n        const collapsed = list.classList.contains('nbtools-hidden');\n        // Toggle the collapse button\n        const collapse = origin_wrapper.querySelector('span.nbtools-collapse');\n        if (collapsed) {\n            collapse.classList.add('nbtools-expanded');\n            collapse.classList.remove('nbtools-collapsed');\n        }\n        else {\n            collapse.classList.remove('nbtools-expanded');\n            collapse.classList.add('nbtools-collapsed');\n        }\n        // Hide or show widget body\n        toggle(list);\n    }\n}\nexport class SearchBox extends Widget {\n    constructor() {\n        super();\n        this.value = '';\n        this.node.innerHTML = `\n            <div class=\"nbtools-wrapper\">\n                <div class=\"nbtools-outline\">\n                    <input type=\"search\" class=\"nbtools-search\" spellcheck=\"false\" placeholder=\"SEARCH\" />\n                </div>\n            </div>\n        `;\n        this.attach_events();\n    }\n    attach_events() {\n        // Attach the change event to the search box\n        const search_box = this.node.querySelector('input.nbtools-search');\n        search_box.addEventListener(\"keyup\", () => this.filter(search_box));\n    }\n    filter(search_box) {\n        // Update the value state\n        this.value = search_box.value.toLowerCase().replace(/[^a-z0-9]/g, '');\n        // Get the toolbox\n        const toolbox = document.querySelector('#nbtools-browser > .nbtools-toolbox');\n        if (!toolbox)\n            return; // Do nothing if the toolbox is null\n        // Show any tool that matches and hide anything else\n        toolbox.querySelectorAll('li.nbtools-tool').forEach((tool) => {\n            if (tool.textContent.toLowerCase().replace(/[^a-z0-9]/g, '').includes(this.value))\n                tool.style.display = 'block';\n            else\n                tool.style.display = 'none';\n        });\n    }\n}\n",
         "/**\n * Define the UI Builder widget for Jupyter Notebook\n *\n * @author Thorin Tabor\n *\n * Copyright 2020 Regents of the University of California and the Broad Institute\n */\nimport '../style/uibuilder.css';\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport { unpack_models } from \"@jupyter-widgets/base\";\nimport { BaseWidgetModel, BaseWidgetView } from \"./basewidget\";\nimport { element_rendered, toggle } from \"./utils\";\nimport { ContextManager } from \"./context\";\n// noinspection JSAnnotator\nexport class UIBuilderModel extends BaseWidgetModel {\n    defaults() {\n        return Object.assign(Object.assign({}, super.defaults()), { _model_name: UIBuilderModel.model_name, _model_module: UIBuilderModel.model_module, _model_module_version: UIBuilderModel.model_module_version, _view_name: UIBuilderModel.view_name, _view_module: UIBuilderModel.view_module, _view_module_version: UIBuilderModel.view_module_version, name: 'Python Function', description: '', _parameters: [], parameter_groups: [], accept_origins: [], function_import: '', register_tool: true, collapse: true, events: {}, buttons: {}, license: {}, display_header: true, display_footer: true, busy: false, run_label: 'Run', form: undefined, output: undefined });\n    }\n}\nUIBuilderModel.model_name = 'UIBuilderModel';\nUIBuilderModel.model_module = MODULE_NAME;\nUIBuilderModel.model_module_version = MODULE_VERSION;\nUIBuilderModel.view_name = 'UIBuilderView';\nUIBuilderModel.view_module = MODULE_NAME;\nUIBuilderModel.view_module_version = MODULE_VERSION;\nUIBuilderModel.serializers = Object.assign(Object.assign({}, BaseWidgetModel.serializers), { form: { deserialize: unpack_models } });\n// noinspection JSAnnotator\nexport class UIBuilderView extends BaseWidgetView {\n    constructor() {\n        super(...arguments);\n        this.dom_class = 'nbtools-uibuilder';\n        this.traitlets = [...super.basics(), 'origin', '_parameters', 'function_import', 'register_tool', 'collapse',\n            'events', 'run_label', 'form', 'output'];\n        this.renderers = {\n            \"error\": this.render_error,\n            \"info\": this.render_info\n        };\n        this.body = `\n        <div class=\"nbtools-buttons\">\n            <button class=\"nbtools-run\" data-traitlet=\"run_label\"></button>\n        </div>\n        <div class=\"nbtools-description\" data-traitlet=\"description\"></div>\n        <div class=\"nbtools-busy\">\n            <div>\n                <i class=\"fas fa-circle-notch fa-spin\"></i>\n            </div>\n        </div>\n        <div class=\"nbtools-error\" data-traitlet=\"error\"></div>\n        <div class=\"nbtools-info\" data-traitlet=\"info\"></div>\n        <div class=\"nbtools-form\"></div>\n        <div class=\"nbtools-footer\"></div>\n        <div class=\"nbtools-buttons\">\n            <button class=\"nbtools-run\" data-traitlet=\"run_label\"></button>\n        </div>`;\n        this.dialog = `<div class=\"nbtools-dialog\">\n                           <div class=\"nbtools-panel\">\n                               <div class=\"nbtools-header\"></div>\n                               <div class=\"nbtools-body\">\n                                   <p></p>\n                                   <div class=\"nbtools-panel-button\">\n                                       <button class=\"nbtools-panel-cancel\">Cancel</button>\n                                       <button class=\"nbtools-panel-button\"></button>\n                                   </div>\n                               </div>\n                           </div>\n                       </div>`;\n    }\n    render() {\n        super.render();\n        // Hide the header or footer, if necessary\n        this.display_header_changed();\n        this.display_footer_changed();\n        this.model.on(`change:display_header`, this.display_header_changed, this);\n        this.model.on(`change:display_footer`, this.display_footer_changed, this);\n        // Show or hide the \"busy\" UI\n        this.busy_changed();\n        this.model.on(`change:busy`, this.busy_changed, this);\n        // Attach the Reset Parameters gear option\n        this.add_menu_item('Reset Parameters', () => this.reset_parameters());\n        // Attach the Run button callbacks\n        this.activate_run_buttons();\n        // Attach custom buttons\n        this.activate_custom_buttons();\n        // Display the license, if any\n        this.display_license();\n        // Add the interactive form widget\n        this.attach_child_widget('.nbtools-form', 'form');\n        // After the view is rendered\n        element_rendered(this.el).then(() => {\n            // Attach ID and event callbacks\n            this._attach_callbacks();\n            // Create parameter groups\n            this._init_parameter_groups();\n            // Attach the Advanced Options gear option, if necessary\n            if (this.has_advanced())\n                this.add_menu_item('Advanced Options', () => this.toggle_advanced());\n        });\n    }\n    busy_changed() {\n        const display = this.model.get('busy') ? 'block' : 'none';\n        this.element.querySelector('.nbtools-busy').style.display = display;\n    }\n    display_header_changed() {\n        const display = this.model.get('display_header') ? 'block' : 'none';\n        this.element.querySelector('.nbtools-buttons:first-of-type').style.display = display;\n        this.element.querySelector('.nbtools-description').style.display = display;\n    }\n    display_footer_changed() {\n        const display = this.model.get('display_footer') ? 'block' : 'none';\n        this.element.querySelector('.nbtools-buttons:last-of-type').style.display = display;\n        this.element.querySelector('.nbtools-footer').style.display = display;\n        // If there is an output_var element, hide or show it as necessary\n        if (!this.output_var_displayed())\n            return;\n        this.element.querySelector('.nbtools-input:last-of-type').style.display = display;\n    }\n    output_var_displayed() {\n        const output_var = this.model.get('_parameters')['output_var'];\n        return !!(output_var && output_var['hide'] == false);\n    }\n    /**\n     * Displays a EULA to the user, who must agree before continuing.\n     *\n     * License should be a dict with the following keys:\n     *      text: The text of the license\n     *      title: The name of the license (optional)\n     *      callback: Whether the license has been agreed to (boolean)\n     */\n    display_license() {\n        const license = this.model.get('license'); // Get the license model\n        if (!license || !license['text'])\n            return; // If there is no license, skip\n        this.widget_dialog({ title: license['title'] ||\n                'You must agree below to the following end-user license agreement',\n            body: license['text'],\n            button_label: 'Agree',\n            callback: () => {\n                license['callback'] = true; // Set to true to trigger callback function\n                this.model.set('license', license);\n                this.model.save();\n            } });\n    }\n    activate_custom_buttons() {\n        this.el.querySelectorAll('.nbtools-buttons').forEach((box) => {\n            const buttons = this.model.get('buttons');\n            Object.keys(buttons).forEach((label) => {\n                const button = new DOMParser().parseFromString(`<button>${label}</button>`, \"text/html\")\n                    .querySelector('button');\n                const button_event = new Function(buttons[label]);\n                button.addEventListener('click', button_event);\n                box.prepend(button);\n            });\n        });\n    }\n    /**\n     * Attach the click event to each Run button\n     */\n    activate_run_buttons() {\n        this.el.querySelectorAll('.nbtools-run').forEach((button) => button.addEventListener('click', () => {\n            // Validate required parameters and return if not valid\n            if (!this.validate())\n                return;\n            // Execute the interact instance\n            this.el.querySelector('.widget-interact > .jupyter-button').click();\n            // Collapse the widget, if collapse=True\n            if (this.model.get('collapse'))\n                this.el.querySelector('.nbtools-collapse').click();\n        }));\n    }\n    /**\n     * Check to make sure required parameters are checked out.\n     * Highlight missing parameters. Return whether valid.\n     */\n    validate() {\n        let valid = true;\n        const form = this.el.querySelector('.nbtools-form');\n        form.querySelectorAll('.nbtools-input').forEach((param) => {\n            if (!param.classList.contains('required'))\n                return; // Ignore optional parameters\n            const input = param.querySelector('input, select');\n            if (input.value.trim() === '') { // If empty\n                param.classList.add('missing'); // Add missing style\n                valid = false; // Not all params are valid\n            }\n            else\n                param.classList.remove('missing'); // Remove missing style\n        });\n        return valid;\n    }\n    widget_dialog({ title = '', body = '', button_label = 'OK', callback = null }) {\n        this.element.appendChild(new DOMParser().parseFromString(this.dialog, \"text/html\")\n            .querySelector('body > :first-child'));\n        const dialog = this.element.querySelector('.nbtools-dialog');\n        const header = dialog.querySelector('.nbtools-header');\n        const button = dialog.querySelector('button.nbtools-panel-button');\n        header.style.backgroundColor = this.model.get('color');\n        header.textContent = title;\n        dialog.querySelector('.nbtools-body > p').textContent = body;\n        dialog.querySelector('.nbtools-panel-cancel').addEventListener('click', () => dialog.remove());\n        button.textContent = button_label;\n        button.style.backgroundColor = this.model.get('color');\n        button.addEventListener('click', () => {\n            dialog.remove();\n            callback();\n        });\n    }\n    /**\n     * Create group headers and reorder the form widget according to the group spec\n     *\n     * @private\n     */\n    _init_parameter_groups() {\n        // Get the parameter groups\n        const groups = this.model.get('parameter_groups');\n        if (!groups || !groups.length)\n            return; // No groups are defined, skip this step\n        // Get the UI Builder form container\n        const form = this.el.querySelector('.nbtools-form > .widget-interact');\n        if (!form)\n            return; // If no container is found, skip this step\n        // Iterate over each group, create headers and add parameters\n        groups.reverse().forEach((group) => {\n            const hidden = !!group['hidden']; // Is the group collapsed by default?\n            const advanced = !!group['advanced']; // Toggle on with advanced options call?\n            // Create and add the header\n            const header = this._create_group_header(group['name'], hidden, advanced);\n            const body = this._create_group_body(header, group['description'], hidden, advanced);\n            form.prepend(body);\n            form.prepend(header);\n            // Add the parameters\n            group['parameters'] && group['parameters'].forEach((param_name) => {\n                const param = this._param_dom_by_name(form, param_name);\n                if (!param)\n                    return; // If the parameter is not found, skip\n                body.append(param);\n            });\n        });\n    }\n    _create_group_header(name, hidden, advanced) {\n        // Create the expand / collapse button\n        const controls = document.createElement('controls');\n        const button = document.createElement('button');\n        const icon = document.createElement('span');\n        controls.classList.add('nbtools-controls');\n        button.classList.add('nbtools-collapse');\n        icon.classList.add('fa', 'fa-minus');\n        button.append(icon);\n        controls.append(button);\n        // Create the header\n        const header = document.createElement('div');\n        header.classList.add('nbtools-header', 'nbtools-group-header');\n        if (advanced)\n            header.classList.add('nbtools-advanced');\n        header.append(name || '');\n        header.append(controls);\n        // Apply the color\n        header.style.backgroundColor = this.model.get('color');\n        // Hide the header if no name is given and not collapsed\n        if (!name && !hidden)\n            header.style.display = 'none';\n        // Return the container\n        return header;\n    }\n    _create_group_body(header, description, hidden, advanced) {\n        // Create the container\n        const box = document.createElement('div');\n        box.classList.add('nbtools-group');\n        if (advanced)\n            box.classList.add('nbtools-advanced');\n        // Create the description\n        if (description) {\n            const desc = document.createElement('div');\n            desc.classList.add('nbtools-description');\n            desc.append(description || '');\n            box.append(desc);\n        }\n        // Add controls to the expand / collapse button\n        const button = header.querySelector('button');\n        const icon = button.querySelector('span');\n        button.addEventListener('click', () => {\n            this._group_toggle_collapse(box, icon);\n        });\n        // Collapse if hidden\n        if (hidden)\n            this._group_toggle_collapse(box, icon);\n        return box;\n    }\n    _group_toggle_collapse(group_box, button) {\n        const collapsed = group_box.style.display === \"none\";\n        // Hide or show widget body\n        toggle(group_box);\n        // Toggle the collapse button\n        if (collapsed) {\n            button.classList.add('fa-minus');\n            button.classList.remove('fa-plus');\n        }\n        else {\n            button.classList.remove('fa-minus');\n            button.classList.add('fa-plus');\n        }\n    }\n    _param_dom_by_name(form, name) {\n        // First attempt: Try to get parameter by data-name attribute (created by attach_callbacks() method)\n        let param = form.querySelector(`.nbtools-input[data-name='${name}']`);\n        if (param)\n            return param; // Found it! Return the parameter\n        // Second attempt: Try to locate by parameter name label\n        const label = form.querySelector(`.nbtools-input > .widget-label:first-child`);\n        if (!label)\n            return null; // No matching label found, return null\n        const match = name.toLowerCase().replace(/[^a-zA-Z]/g, '') ===\n            label.textContent.toLowerCase().replace(/[^a-zA-Z]/g, '');\n        if (match)\n            return label.closest('.nbtools-input');\n        // Match not found, return null\n        return null;\n    }\n    /**\n     * Attach ID and event callbacks to the UI Builder\n     *\n     * @private\n     */\n    _attach_callbacks() {\n        // Handle widget events\n        const widget_events = this.model.get('events');\n        this._attach_all_events(this.el, widget_events);\n        // Handle parameter IDs and parameter events\n        const json_parameters = this.model.get('_parameters');\n        const dom_parameters = this.el.querySelectorAll('.nbtools-input');\n        for (let i = 0; i < json_parameters.length; i++) {\n            const param_spec = json_parameters[i];\n            const param_el = dom_parameters[i];\n            // Attach the data-name attribute\n            param_el.setAttribute('data-name', param_spec.name);\n            // Attach specified ID as a data-id attribute\n            if (!!param_spec.id)\n                param_el.setAttribute('data-id', param_spec.id);\n            // Attach parameter events\n            if (!!param_spec.events) {\n                this._attach_all_events(param_el, param_spec.events);\n            }\n            // Resize footer, if necessary\n            if (param_spec.name === 'output_var' && param_spec.description) {\n                // noinspection JSConstantReassignment\n                this.el.querySelector('.nbtools-footer').style.height = '50px';\n            }\n        }\n        // Attach send to / come from menus\n        this._attach_menus();\n        // Attach enter key submit event\n        this._submit_keypress();\n    }\n    _submit_keypress() {\n        this.el.querySelectorAll('.nbtools-form input, .nbtools-form select').forEach((element) => {\n            element.addEventListener(\"keydown\", (event) => {\n                if (event.keyCode === 13) {\n                    this.el.querySelector('.nbtools-run').click();\n                }\n            });\n        });\n    }\n    /**\n     * Add default choices defined in with UI Builder choice parameter to the label -> value map\n     *\n     * @param display_value_map\n     * @param model\n     * @private\n     */\n    _add_default_choices(display_value_map, model) {\n        const choices = model.get('choices');\n        if (choices && Object.keys(choices).length)\n            display_value_map['Default Choices'] = model.get('choices');\n    }\n    /**\n     * Add all files matching a specific selector to the label -> value map under the specified name\n     *\n     * @param display_value_map\n     * @param target\n     * @param kinds\n     * @param selector\n     * @param group_name\n     * @private\n     */\n    _add_notebook_files(display_value_map, target, kinds, selector, group_name) {\n        // Get the notebook's parent node\n        const notebook = target.closest('.jp-Notebook');\n        // Get all possible outputs\n        const markdown_outputs = [...notebook.querySelectorAll(selector)];\n        // Build list of compatible outputs\n        const compatible_outputs = {};\n        markdown_outputs.forEach((output) => {\n            let href, label, kind;\n            // Handle getting the kind and label from a link\n            if (output.tagName.toLowerCase() === 'a') {\n                href = output.getAttribute('href');\n                label = (output.textContent || href).trim();\n                kind = UIBuilderView.get_kind(href);\n            }\n            // Handle getting the kind and label from text\n            else {\n                label = (output.textContent || 'Blank Text Option').trim();\n                href = (output.textContent || '').trim();\n                kind = 'text';\n            }\n            // Special case for text \"send to\"\n            if (group_name === \"Text Options\") {\n                if (kinds.includes('text'))\n                    compatible_outputs[label] = href;\n                kind = 'text';\n            }\n            // Include if matching kind\n            if (UIBuilderView.matching_kind(kinds, kind))\n                compatible_outputs[label] = href;\n            // Include if kinds blank and not text\n            else if (kinds.length === 0 && kind !== 'text')\n                compatible_outputs[label] = href;\n        });\n        // Add to the label -> value map\n        if (Object.keys(compatible_outputs).length > 0)\n            display_value_map[group_name] = compatible_outputs;\n    }\n    /**\n     * Add markdown input files to the label -> value map\n     *\n     * @param display_value_map\n     * @param target\n     * @param kinds\n     * @private\n     */\n    _add_markdown_files(display_value_map, target, kinds) {\n        this._add_notebook_files(display_value_map, target, kinds, '.nbtools-markdown-file', 'Notebook Instructions');\n    }\n    /**\n     * Add markdown text options to the label -> value map\n     *\n     * @param display_value_map\n     * @param target\n     * @param kinds\n     * @private\n     */\n    _add_markdown_text(display_value_map, target, kinds) {\n        this._add_notebook_files(display_value_map, target, kinds, '.nbtools-text-option', 'Text Options');\n    }\n    /**\n     * Add UIOutput files to the label -> value map\n     *\n     * @param display_value_map\n     * @param target\n     * @param kinds\n     * @private\n     */\n    _add_output_files(display_value_map, target, kinds) {\n        const origins = this.supported_origins();\n        const compatible_outputs = ContextManager.data_registry.get_data({ kinds: kinds, origins: origins });\n        if (Object.keys(compatible_outputs).length > 0) {\n            for (let origin of Object.keys(compatible_outputs))\n                display_value_map[origin] = compatible_outputs[origin];\n        }\n    }\n    supported_origins() {\n        // Get the list of supported origins for data\n        let this_origin = this.model.get('origin');\n        let accept_origins = this.model.get('accept_origins');\n        // If supported origins is empty or undefined, accept same origins and \"Notebook\" by default\n        if (accept_origins === null || accept_origins.length < 1) {\n            accept_origins = [this_origin];\n            if (this_origin !== 'Notebook')\n                accept_origins.push('Notebook');\n        }\n        // Unless... if this origin is empty or undefined, accept all origins\n        if (this_origin === null || this_origin.length < 1)\n            accept_origins = [];\n        // Otherwise, return the list\n        return accept_origins;\n    }\n    _attach_kinds(attach_point) {\n        const view = attach_point.widget;\n        const model = view.model; // Get the model from the view\n        const kinds = model.get('kinds') || ['text'];\n        attach_point.setAttribute('data-type', kinds.join(', '));\n    }\n    _attach_name(attach_point) {\n        let name = '';\n        let param_element = null;\n        let name_element = null;\n        param_element = attach_point.closest('.nbtools-input');\n        if (param_element)\n            name_element = param_element.querySelector('div:first-child');\n        if (name_element)\n            name = name_element.textContent.replace(/\\*/g, '');\n        attach_point.setAttribute('data-name', name);\n    }\n    _attach_accept_origins(attach_point) {\n        const origins = this.supported_origins();\n        attach_point.setAttribute('data-origins', origins.join(', '));\n    }\n    /**\n     * Attach sent to / come from menu support to the UI Builder widget\n     *\n     * @private\n     */\n    _attach_menus() {\n        this.el.querySelectorAll('.nbtools-menu-attached').forEach((attach_point) => {\n            this._attach_kinds(attach_point);\n            this._attach_name(attach_point);\n            this._attach_accept_origins(attach_point);\n            attach_point.addEventListener(\"click\", (event) => {\n                // Get all compatible outputs and build display -> value map\n                const display_value_map = this.build_display_map(attach_point);\n                if (display_value_map === null)\n                    return; // No view found, return\n                // Update and attach the menu\n                const target = attach_point.querySelector('input, select');\n                this.attach_combobox_menu(target, display_value_map);\n                // Attach the chevron to the input... or not\n                this.update_chevron(attach_point, display_value_map);\n            });\n            // Initial menu attachment\n            this.update_chevron(attach_point);\n        });\n    }\n    build_display_map(attach_point) {\n        const view = attach_point.widget; // Get widget view or abort\n        if (!view)\n            return null;\n        const model = attach_point.widget.model; // Get the model from the view\n        const sendto = !attach_point.classList.contains('nbtools-nosendto'); // Send if sendto enabled\n        const kinds = model.get('kinds') || ['text']; // Get the list of compatible kinds\n        // Build the map\n        const display_value_map = {};\n        this._add_default_choices(display_value_map, model);\n        if (sendto)\n            this._add_output_files(display_value_map, attach_point, kinds);\n        if (sendto)\n            this._add_markdown_files(display_value_map, attach_point, kinds);\n        if (sendto)\n            this._add_markdown_text(display_value_map, attach_point, kinds);\n        return display_value_map;\n    }\n    update_chevron(attach_point, display_value_map = null) {\n        if (!display_value_map)\n            display_value_map = this.build_display_map(attach_point);\n        if (Object.keys(display_value_map).length > 0)\n            attach_point.classList.add('nbtools-dropdown');\n        else\n            attach_point.classList.remove('nbtools-dropdown');\n    }\n    toggle_file_menu(link, display_value_map) {\n        const menu = link.nextElementSibling;\n        const collapsed = menu.style.display === \"none\";\n        // If the menu is empty, don't show it\n        if (menu.childElementCount === 0)\n            return;\n        // Hide or show the menu\n        if (collapsed)\n            menu.style.display = \"block\";\n        else\n            menu.style.display = \"none\";\n        // Hide the menu with the next click\n        const hide_next_click = function (event) {\n            if (link.contains(event.target))\n                return;\n            menu.style.display = \"none\";\n            document.removeEventListener('click', hide_next_click);\n        };\n        document.addEventListener('click', hide_next_click);\n    }\n    /**\n     * Create or update the menu based on the label -> value map\n     *\n     * @param target\n     * @param display_value_map\n     */\n    attach_combobox_menu(target, display_value_map) {\n        // Get the menu and empty it, if it exists.\n        let menu = target.nextSibling;\n        const menu_exists = menu && menu.classList.contains('nbtools-menu');\n        if (menu_exists)\n            menu.innerHTML = '';\n        // Create and insert the menu, if necessary\n        else {\n            menu = document.createElement('ul');\n            menu.classList.add('nbtools-menu', 'nbtools-file-menu');\n            menu.style.display = 'none';\n            target.parentNode ? target.parentNode.insertBefore(menu, target.nextSibling) : null;\n        }\n        // Iterate over display -> value map and insert menu items\n        Object.keys(display_value_map).forEach((group) => {\n            // Add the group label\n            if (group !== 'Default Choices')\n                this.add_menu_item(group, () => { }, 'nbtools-menu-header', menu, false);\n            // Loop over all files in the group\n            Object.keys(display_value_map[group]).forEach((display_name) => {\n                this.add_menu_item(display_name, () => {\n                    target.value = display_value_map[group][display_name];\n                    target.dispatchEvent(new Event('change', { 'bubbles': true }));\n                }, 'nbtools-menu-subitem', menu, false);\n            });\n        });\n        this.toggle_file_menu(target, display_value_map);\n    }\n    /**\n     * Get the kind based on a given URL\n     *\n     * @param url\n     */\n    static get_kind(url) {\n        return url.split(/\\#|\\?/)[0].split('.').pop().trim();\n    }\n    static matching_kind(kinds, kind) {\n        let match = false;\n        kinds.forEach((k) => {\n            if (k.trim().endsWith(kind.trim()))\n                match = true;\n        });\n        return match;\n    }\n    /**\n     * Attach a map of events to the given DOM element (widget or parameter)\n     *\n     * @param {HTMLElement} element\n     * @param event_map\n     * @private\n     */\n    _attach_all_events(element, event_map) {\n        Object.keys(event_map).forEach((key) => {\n            const str_func = event_map[key];\n            const func = new Function(str_func);\n            // Handle the load event as a special case (run now)\n            if (key === 'load')\n                func.call(this, new CustomEvent('load'));\n            // Handle the run event as a special case (bind as click to the Run button)\n            else if (key === 'run') {\n                const run_button = element.querySelector('.jupyter-button');\n                if (!!run_button)\n                    run_button.addEventListener('click', func);\n            }\n            // Special case to handle focus events, which are swallowed by the Jupyter UI\n            else if (key === 'focus')\n                element.addEventListener('focusin', func);\n            // Otherwise, attach the event\n            else\n                element.addEventListener(key, func);\n        });\n    }\n    set_input_model(model, spec) {\n        // Special case for DropdownModel\n        if (model.name === 'DropdownModel') {\n            const labels = Object.keys(spec['choices']);\n            for (let i = 0; i < labels.length; i++) {\n                const label = labels[i];\n                const value = spec['choices'][label];\n                if (value === spec['default']) {\n                    model.set('index', i);\n                    break;\n                }\n            }\n        }\n        else { // Otherwise just set the value traitlet\n            model.set('value', spec['default']);\n        }\n        // Save the model\n        model.save_changes();\n    }\n    has_advanced() {\n        return !!this.element.querySelector('.nbtools-advanced');\n    }\n    toggle_advanced() {\n        this.element.querySelectorAll('.nbtools-advanced').forEach((e) => {\n            const hidden = !e.classList.contains('nbtools-advanced-show');\n            if (hidden)\n                e.classList.add('nbtools-advanced-show');\n            else\n                e.classList.remove('nbtools-advanced-show');\n        });\n    }\n    reset_parameters() {\n        const params = this.model.get('_parameters');\n        for (let i = 0; i < params.length; i++) {\n            const spec = params[i];\n            const name = spec['name'];\n            const param_element = this.element.querySelector(`[data-name='${name}']:not(.nbtools-input)`);\n            if (!param_element) { // Protect against nulls\n                if (name !== 'output_var')\n                    console.log(`Error finding ${name} in reset_parameters()`);\n                return;\n            }\n            const view = param_element.widget;\n            this.set_input_model(view.model, spec);\n            // Special case for file lists\n            const all_inputs = param_element.parentNode ? param_element.parentNode.querySelectorAll('input') : [];\n            if (all_inputs.length > 1) {\n                let first = true;\n                all_inputs.forEach((input) => {\n                    if (first)\n                        first = false;\n                    else\n                        input.value = '';\n                });\n            }\n        }\n    }\n}\n",
         "/**\n * Widget for representing Python output as an interactive interface\n *\n * @author Thorin Tabor\n *\n * Copyright 2020 Regents of the University of California and the Broad Institute\n */\nimport '../style/uioutput.css';\nimport { unpack_models } from '@jupyter-widgets/base';\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport { BaseWidgetModel, BaseWidgetView } from \"./basewidget\";\nimport { extract_file_name, extract_file_type, get_absolute_url, is_absolute_path, is_url } from './utils';\nimport { ContextManager } from \"./context\";\nimport { Data } from \"./dataregistry\";\n// noinspection JSAnnotator\nexport class UIOutputModel extends BaseWidgetModel {\n    defaults() {\n        return Object.assign(Object.assign({}, super.defaults()), { _model_name: UIOutputModel.model_name, _model_module: UIOutputModel.model_module, _model_module_version: UIOutputModel.model_module_version, _view_name: UIOutputModel.view_name, _view_module: UIOutputModel.view_module, _view_module_version: UIOutputModel.view_module_version, name: 'Python Results', description: '', status: '', files: [], text: '', visualization: '', appendix: undefined, extra_file_menu_items: {} });\n    }\n}\nUIOutputModel.model_name = 'UIOutputModel';\nUIOutputModel.model_module = MODULE_NAME;\nUIOutputModel.model_module_version = MODULE_VERSION;\nUIOutputModel.view_name = 'UIOutputView';\nUIOutputModel.view_module = MODULE_NAME;\nUIOutputModel.view_module_version = MODULE_VERSION;\nUIOutputModel.serializers = Object.assign(Object.assign({}, BaseWidgetModel.serializers), { appendix: { deserialize: unpack_models } });\n// noinspection JSAnnotator\nexport class UIOutputView extends BaseWidgetView {\n    constructor() {\n        super(...arguments);\n        this.dom_class = 'nbtools-uioutput';\n        this.traitlets = [...super.basics(), 'status', 'files', 'text', 'visualization'];\n        this.renderers = {\n            \"description\": this.render_description,\n            \"error\": this.render_error,\n            \"info\": this.render_info,\n            \"files\": this.render_files,\n            \"visualization\": this.render_visualization\n        };\n        this.body = `\n        <div class=\"nbtools-description\" data-traitlet=\"description\"></div>\n        <div class=\"nbtools-error\" data-traitlet=\"error\"></div>\n        <div class=\"nbtools-info\" data-traitlet=\"info\"></div>\n        <div class=\"nbtools-status\" data-traitlet=\"status\"></div>\n        <div class=\"nbtools-files\" data-traitlet=\"files\"></div>\n        <pre class=\"nbtools-text\" data-traitlet=\"text\"></pre>\n        <div class=\"nbtools-visualization\" data-traitlet=\"visualization\"></div>\n        <div class=\"nbtools-appendix\"></div>`;\n        this.file_cache = [];\n    }\n    render() {\n        super.render();\n        // Add the child widgets\n        this.attach_child_widget('.nbtools-appendix', 'appendix');\n    }\n    remove() {\n        super.remove();\n        // Clean up data files from the cache\n        for (let f of this.file_cache)\n            ContextManager.data_registry.unregister({ data: f });\n    }\n    sync_file_cache() {\n        // Unregister old files associated with this widget\n        for (let f of this.file_cache)\n            ContextManager.data_registry.unregister({ data: f });\n        // Create the data objects and add them to the file cache\n        this.file_cache = [];\n        const origin = this.model.get('origin');\n        for (let f of this.model.get('files'))\n            this.file_cache.push(new Data(origin, f));\n        // Register the files currently associated with this widget\n        for (let f of this.file_cache)\n            ContextManager.data_registry.register({ data: f });\n    }\n    render_files(files, widget) {\n        // Sync the file cache with what is displayed\n        widget.sync_file_cache();\n        let to_return = '';\n        files.forEach(path => {\n            const name = extract_file_name(path);\n            const type = extract_file_type(path);\n            const path_prefix = UIOutputView.pick_path_prefix(path);\n            to_return += `<a class=\"nbtools-file\" href=\"${path_prefix}${path}\" data-type=\"${type}\" onclick=\"return false;\">${name} <i class=\"fa fa-info-circle\"></i></a>`;\n            to_return += `<ul class=\"nbtools-menu nbtools-file-menu\" style=\"display: none;\"></ul>`;\n        });\n        setTimeout(() => widget.initialize_file_menus(widget), 100);\n        return to_return;\n    }\n    render_visualization(visualization, widget) {\n        // Function for toggling pop out menu item on or off\n        function toggle_open_visualizer(hide) {\n            const controls = widget.element.querySelector('.nbtools-controls');\n            if (!controls)\n                return; // Get the gear menu buttons at the top and protect against null\n            // Toggle or set the Pop Out Visualizer menu option's visibility\n            controls.querySelectorAll('.nbtools-menu > li').forEach((item) => {\n                if (item.textContent.includes('Pop Out Visualizer')) {\n                    if (hide)\n                        item.style.display = 'none';\n                    else\n                        item.style.display = 'block';\n                }\n            });\n        }\n        // Hide or show the open visualizer menu option, depending on whether there is a visualization\n        if (!visualization.trim())\n            toggle_open_visualizer(true);\n        else\n            toggle_open_visualizer(false);\n        // If URL, display an iframe\n        if (is_url(visualization))\n            return `<iframe class=\"nbtools-visualization-iframe\" src=\"${visualization}\"></iframe>`;\n        // Otherwise, embed visualization as HTML\n        else\n            return visualization;\n    }\n    traitlet_changed(event) {\n        const widget = this;\n        const name = typeof event === \"string\" ? event : Object.keys(event.changed)[0];\n        const elements = this.element.querySelectorAll(`[data-traitlet=${name}]`);\n        elements.forEach(element => {\n            // Ignore traitlets in the appendix, unless this is a subwidget in the appendix\n            if (!this.element.closest('.nbtools-appendix') && element.closest('.nbtools-appendix'))\n                return;\n            if (name in this.renderers)\n                element.innerHTML = this.renderers[name](this.model.get(name), widget);\n            else\n                element.innerHTML = this.model.get(name);\n        });\n    }\n    static pick_path_prefix(path) {\n        if (is_url(path))\n            return ''; // is a URL\n        else if (is_absolute_path(path))\n            return ''; // is an absolute\n        else\n            return 'files/' + ContextManager.context().notebook_path(); // is relative path\n    }\n    attach_menu_options() {\n        // Determine if \"Pop Out\" has already been attached\n        const menu_exists = !!this.element.querySelector('.nbtools-menu-popout');\n        // Attach the Pop Out Visualizer gear option if needed\n        if (!menu_exists) {\n            const visualizer_option = this.add_menu_item('Pop Out Visualizer', () => this.open_visualizer(), 'nbtools-menu-popout');\n            visualizer_option.style.display = this.model.get('visualization').trim() ? 'block' : 'none';\n        }\n        // Call the base widget's attach_menu_options()\n        super.attach_menu_options();\n    }\n    open_visualizer() {\n        window.open(this.model.get('visualization'));\n    }\n    initialize_file_menus(widget) {\n        const files = widget.el.querySelectorAll('.nbtools-file');\n        files.forEach((link) => {\n            link.addEventListener(\"click\", function () {\n                widget.toggle_file_menu(link);\n            });\n        });\n    }\n    initialize_menu_items(link) {\n        const menu = link.nextElementSibling;\n        if (!menu)\n            return; // Protect against null\n        const type = link.getAttribute('data-type');\n        const href = link.getAttribute('href');\n        const file_name = link.textContent ? link.textContent.trim() : href;\n        const widget_name = this.model.get('name');\n        const origin = this.model.get('origin') || '';\n        // Add the send to options\n        let send_to_empty = true;\n        this.get_input_list(type, origin).forEach(input => {\n            send_to_empty = false;\n            this.add_menu_item(input['name'] + ' -> ' + input['param'], () => {\n                const form_input = input['element'].querySelector('input');\n                form_input.value = href;\n                form_input.dispatchEvent(new Event('change', { bubbles: true }));\n                const widget = form_input.closest('.nbtools');\n                widget.scrollIntoView();\n            }, 'nbtools-menu-subitem', menu);\n        });\n        // Add send to header\n        if (!send_to_empty)\n            this.add_menu_item('Send to...', () => { }, 'nbtools-menu-header', menu);\n        // Add the extra menu items\n        const menu_items = this.model.get('extra_file_menu_items');\n        const template_vars = {\n            'widget_name': widget_name,\n            'file_name': file_name,\n            'href': href,\n            'type': type\n        };\n        Object.keys(menu_items).forEach((name) => {\n            const item = menu_items[name];\n            // Skip if this file doesn't match any type restrictions\n            if (item['kinds'] && Array.isArray(item['kinds']) && !item['kinds'].includes(type))\n                return;\n            // Create the callback and attach the menu item\n            const callback = this.create_menu_callback(item, template_vars);\n            this.add_menu_item(name, callback, 'nbtools-menu-subitem', menu);\n        });\n        // Add download and new tab options\n        this.add_menu_item('Copy Link', () => navigator.clipboard.writeText(get_absolute_url(link.getAttribute('href'))), '', menu);\n        this.add_menu_item('Download', () => window.open(link.getAttribute('href') + '?download=1'), '', menu);\n        this.add_menu_item('Open in New Tab', () => window.open(link.getAttribute('href')), '', menu);\n    }\n    toggle_file_menu(link) {\n        const menu = link.nextElementSibling;\n        const collapsed = menu.style.display === \"none\";\n        // Build the menu lazily\n        menu.innerHTML = ''; // Clear all existing children\n        this.initialize_menu_items(link);\n        // Hide or show the menu\n        if (collapsed)\n            menu.style.display = \"block\";\n        else\n            menu.style.display = \"none\";\n        // Hide the menu with the next click\n        const hide_next_click = function (event) {\n            if (link.contains(event.target))\n                return;\n            menu.style.display = \"none\";\n            document.removeEventListener('click', hide_next_click);\n        };\n        document.addEventListener('click', hide_next_click);\n    }\n    get_input_list(type, origin) {\n        // Get the notebook's parent node\n        const notebook = this.el.closest('.jp-Notebook');\n        // Get all possible outputs\n        const parameters = [...notebook.querySelectorAll('.nbtools-menu-attached')];\n        // Build list of compatible inputs\n        const compatible_inputs = [];\n        parameters.forEach((input) => {\n            // Ignore hidden parameters\n            if (input.offsetWidth === 0 && input.offsetHeight === 0)\n                return;\n            // Ignore parameters with sendto=False\n            if (input.classList.contains('nbtools-nosendto'))\n                return;\n            // Ignore if this origin does not match the supported origins\n            const origins_str = input.getAttribute('data-origins') || '';\n            const origins_list = origins_str.split(', ');\n            if (!origins_list.includes(origin) && origins_str !== '')\n                return;\n            // Ignore incompatible inputs\n            const kinds = input.getAttribute('data-type') || '';\n            const param_name = input.getAttribute('data-name') || '';\n            const kinds_list = kinds.split(', ');\n            if (!kinds_list.includes(type) && kinds !== '')\n                return;\n            // Add the input to the compatible list\n            const widget_element = input.closest('.nbtools');\n            let name = widget_element.querySelector('.nbtools-title').textContent;\n            if (!name)\n                name = \"Untitled Widget\";\n            compatible_inputs.push({\n                'name': name,\n                'param': param_name,\n                'element': input\n            });\n        });\n        return compatible_inputs;\n    }\n}\n",
         "/**\n * Send a browser notification\n *\n * @param message\n * @param sender\n * @param icon\n */\nexport function send_notification(message, sender = 'nbtools', icon = '') {\n    // Internal function to display the notification\n    function notification() {\n        new Notification(sender, {\n            body: message,\n            badge: icon,\n            icon: icon,\n            silent: true\n        });\n    }\n    // Browser supports notifications and permission is granted\n    if (\"Notification\" in window && Notification.permission === \"granted\") {\n        notification();\n    }\n    // Otherwise, we need to ask the user for permission\n    else if (\"Notification\" in window && Notification.permission !== \"denied\") {\n        Notification.requestPermission(function (permission) {\n            // If the user accepts, let's create a notification\n            if (permission === \"granted\") {\n                notification();\n            }\n        });\n    }\n}\n/**\n * Determines ia a given string is an absolute file path\n *\n * @param path_or_url\n * @returns {boolean}\n */\nexport function is_absolute_path(path_or_url) {\n    let path_exp = new RegExp('^/');\n    return path_exp.test(path_or_url);\n}\n/**\n * Decides if a string represents a valid URL or not\n *\n * @param path_or_url\n * @returns {boolean}\n */\nexport function is_url(path_or_url) {\n    const url_exp = new RegExp('^(?:http|ftp)s?://');\n    return url_exp.test(path_or_url);\n}\nexport function get_absolute_url(url) {\n    try {\n        return new URL(url).href;\n    }\n    catch (e) {\n        return new URL(url, document.baseURI).href;\n    }\n}\n/**\n * Extracts a file name from a URL\n *\n * @param path\n * @returns {*}\n */\nexport function extract_file_name(path) {\n    if (is_url(path))\n        return path.split('/').pop();\n    else\n        return path;\n}\n/**\n * Extracts a file type from a path or URL\n *\n * @param {string} path\n * @returns {any}\n */\nexport function extract_file_type(path) {\n    return path.split('.').pop().trim();\n}\n/**\n * Wait until the specified element is found in the DOM and then execute a promise\n *\n * @param {HTMLElement} el\n */\nexport function element_rendered(el) {\n    return new Promise((resolve, reject) => {\n        (function element_in_dom() {\n            if (document.body.contains(el))\n                return resolve(el);\n            else\n                setTimeout(element_in_dom, 200);\n        })();\n    });\n}\n/**\n * Show an element\n *\n * @param {HTMLElement} elem\n */\nexport function show(elem) {\n    if (!elem)\n        return; // Protect against null elements\n    // Get the natural height of the element\n    const getHeight = function () {\n        elem.style.display = 'block'; // Make it visible\n        const height = elem.scrollHeight + 'px'; // Get it's height\n        elem.style.display = ''; //  Hide it again\n        return height;\n    };\n    const height = getHeight(); // Get the natural height\n    elem.classList.remove('nbtools-hidden'); // Make the element visible\n    elem.style.height = height; // Update the height\n    // Once the transition is complete, remove the inline height so the content can scale responsively\n    setTimeout(function () {\n        elem.style.height = '';\n        elem.classList.remove('nbtools-toggle');\n    }, 350);\n}\n/**\n * Hide an element\n *\n * @param elem\n * @param min_height\n */\nexport function hide(elem, min_height = '0') {\n    if (!elem)\n        return; // Protect against null elements\n    elem.classList.add('nbtools-toggle');\n    // Give the element a height to change from\n    elem.style.height = elem.scrollHeight + 'px';\n    // Set the height back to 0\n    setTimeout(function () {\n        elem.style.height = min_height;\n    }, 10);\n    // When the transition is complete, hide it\n    setTimeout(function () {\n        elem.classList.add('nbtools-hidden');\n    }, 350);\n}\n/**\n * Toggle element visibility\n *\n * @param elem\n * @param min_height\n */\nexport function toggle(elem, min_height = '0') {\n    // If the element is visible, hide it\n    if (!elem.classList.contains('nbtools-hidden')) {\n        hide(elem, min_height);\n        return;\n    }\n    // Otherwise, show it\n    show(elem);\n}\nexport function process_template(template, template_vars) {\n    Object.keys(template_vars).forEach((key_var) => {\n        template = template.replace(new RegExp(`{{${key_var}}}`, 'g'), template_vars[key_var]);\n    });\n    return template;\n}\nexport function pulse_red(element, count = 0, count_up = true) {\n    setTimeout(() => {\n        element.style.border = `rgba(255, 0, 0, ${count / 10}) solid ${Math.ceil(count / 2)}px`;\n        if (count_up && count < 10)\n            pulse_red(element, count + 1, count_up);\n        else if (count_up)\n            pulse_red(element, count, false);\n        else if (count > 0)\n            pulse_red(element, count - 1, count_up);\n        else\n            element.style.border = `none`;\n    }, 25);\n}\n/**\n * We maintain a basic counter of how many times our tools are used; this helps us secure funding.\n * No identifying information is sent.\n *\n * @param event_token\n * @param description\n * @param endpoint\n */\nexport function usage_tracker(event_token, description = '', endpoint = 'https://workspace.g2nb.org/services/usage/') {\n    fetch(`${endpoint}${event_token}/`, {\n        method: \"POST\",\n        body: description\n    }).then(r => r.text()).then(b => console.log(`usage response: ${b}`));\n}\n",
         "const data = require('../package.json');\n/**\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
         "export default __webpack_public_path__ + \"6b8c90c7eb68fb0a698ade6fa7df2e33.png\";",
         "export default \"<svg xmlns=\\\"http://www.w3.org/2000/svg\\\" xmlns:xlink=\\\"http://www.w3.org/1999/xlink\\\" viewBox=\\\"0 0 166.53 166.53\\\"><defs><style>.cls-1{isolation:isolate;}.cls-2{stroke:#dbdcdd;stroke-miterlimit:10;stroke-width:2.43px;fill:url(#linear-gradient);}.cls-3{fill:#534f97;}.cls-4{mask:url(#mask);}.cls-5{opacity:0.25;mix-blend-mode:multiply;}.cls-6{fill:#020202;}.cls-7{fill:#ec1c24;}.cls-8{mask:url(#mask-2);}.cls-9{mask:url(#mask-3);}.cls-10{mask:url(#mask-4);}.cls-11{mask:url(#mask-5);}.cls-12{mask:url(#mask-6);}.cls-13{mask:url(#mask-7);}.cls-14{mask:url(#mask-8);}.cls-15{mask:url(#mask-9);}.cls-16{filter:url(#luminosity-invert);}</style><linearGradient id=\\\"linear-gradient\\\" x1=\\\"582.21\\\" y1=\\\"458.05\\\" x2=\\\"582.21\\\" y2=\\\"622.15\\\" gradientTransform=\\\"matrix(-1, 0, 0, 1, 665.48, -456.63)\\\" gradientUnits=\\\"userSpaceOnUse\\\"><stop offset=\\\"0\\\" stop-color=\\\"#ededee\\\"/><stop offset=\\\"0.18\\\" stop-color=\\\"#fff\\\"/><stop offset=\\\"0.63\\\" stop-color=\\\"#fff\\\"/><stop offset=\\\"0.63\\\" stop-color=\\\"#fff\\\"/><stop offset=\\\"1\\\" stop-color=\\\"#dbdcdd\\\"/></linearGradient><filter id=\\\"luminosity-invert\\\" filterUnits=\\\"userSpaceOnUse\\\" color-interpolation-filters=\\\"sRGB\\\"><feColorMatrix values=\\\"-1 0 0 0 1 0 -1 0 0 1 0 0 -1 0 1 0 0 0 1 0\\\"/></filter><mask id=\\\"mask\\\" x=\\\"11.57\\\" y=\\\"11.37\\\" width=\\\"43\\\" height=\\\"43\\\" maskUnits=\\\"userSpaceOnUse\\\"><g class=\\\"cls-16\\\"><g transform=\\\"translate(-876.43 -456.63)\\\"><image width=\\\"43\\\" height=\\\"43\\\" transform=\\\"translate(888 468)\\\" xlink:href=\\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAArCAYAAADhXXHAAAAACXBIWXMAAAsSAAALEgHS3X78AAADHElEQVRYR+3Z70vyXBzH8feOc83csJImPREkoSfW//+HRNCDSirRTHDq5tL9uh/cnHPNOa4Lo5xBHxio5zhenB+DfY8GpPyQiH91OKTo+R+63S6tVgvbtjEMg2q1ihACTdPQNK3oHp9Omv4/qUmSEMcxURSxWq2Yz+eMx2MeHx83+m9gb25u6PV6tNttms0mlmVhGAaVSgUhhELL7IqXuOz3PNTzPN7f33l9feX4+Jjb21vVX2G73S69Xo/r62s6nQ6O42DbNqZpbmBldoXKZMFpmpKmKXEcE4YhQRAwn895e3vj9PSUNE0JgoCHhwcgg221WrTbbTqdDpeXlziOszWy8HlkUbLYOI7VErAsCyEEruvy8vKyjbVtm2azieM4OI7D+fk5pml+Ke5fSZIE0zQB8H2fs7MzbNtW7WpeDcPAsixs28ayrL1DAYQQ1Ot1ZZAzq9rlh2q1imEYmKaJYRh7h8oIITg6OlIOXf/zDFBYIQSVSkVdZUYIga7r6Lq+YVFYTdPUjs/u+jKSfUxmZ7gQW3YkNP9c35DJhrLWazZFlvKHcYdsYQ9hVGXylsJlcAgpsvzsZXDI+cV+V36x35Vf7HflF/td+bnY/Ht9mSmybI3sIYHzOehlkB+4g8bCJlhhZXVEXmUmSZJCxwY2jmPVsczIgl0erLCymievMpMkifIUYqMoIgxD1us1URQV3mRfieNYObIWhV2v1wRBgO/7BEFQGliWPoMg4OPjoxi7XC5xXZfpdMpsNsPzvL2DwzBksVjgui6u6+J5HqvVSrWrqtdoNGIwGNBqtajX66RpSqPRwDRNdF1XlZqvrNjITZQkCVEUEQQBs9mM4XDIaDRiMpngeZ7qr7D39/dcXFxg2zaapuH7PicnJ9RqNVVQzteedn11/1uZfr1es1wumU6njEYjnp6eeH5+Zjweq/4bZwr9fh+AxWLBYDCg0WhQq9WoVqtb2F2hMvkyffZMYblcMp/PGQ6H9Pt9+v3+xiGIRsE52NXVlVoOEiqx8HloNhKdLdOHYYjv+0wmE+7u7rb+U4g91HzdbtlD/gNw/7gOVEqcSgAAAABJRU5ErkJggg==\\\"/></g></g></mask><mask id=\\\"mask-2\\\" x=\\\"61.57\\\" y=\\\"11.37\\\" width=\\\"43\\\" height=\\\"43\\\" maskUnits=\\\"userSpaceOnUse\\\"><g class=\\\"cls-16\\\"><g transform=\\\"translate(-876.43 -456.63)\\\"><image width=\\\"43\\\" height=\\\"43\\\" transform=\\\"translate(938 468)\\\" xlink:href=\\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAArCAYAAADhXXHAAAAACXBIWXMAAAsSAAALEgHS3X78AAADIElEQVRYR+3Z7UvyUBjH8e+O0023NYtIfRX26Mv+/78jgqBCqIGpkK3pdO7hfhHntJlxc3eXLugHB9Rdjo9nZwe8pgEZPyTibwVlir76Qbfbpd1uY9s2pmmi6zqVSgUhXn+XpmnvTvLZZNnrRU3TlCRJiOOYxWKB7/sMh0Pu7u4K9QXsyckJFxcXHB4esr+/j+M4GIZBtVpFCIEQooD9V7jE5d+vQoMgYDQa8fDwQKPR4PLyUtUXsN1ul16vx+npKZ1Oh52dHer1usJqmqaA/wqVyYOzLCPLMpIkYblcEoYhvu/z+PjI7u4uWZYRhiG3t7dADtvr9Tg7O+Po6Ijj42Pa7Tau62IYBrquK+hnkeuSxyZJopaAbdsIIZhMJtzf37/HttttNVqtFgcHB1iWpdbqJpKmKaZpAjCdTtnb28NxHHVcSSzLwnVdms0mrutuHAoghMCyLBzHwbZtbNumVqu9HZcvqtUqpmnSaDQwDGPjUBkhBIZhYJomtVoNXX+7rZRI13Wq1aoa24wQAl3X1bapPs8XVCoVKpXKl95En0l+m8xbCtd6XcE2Ih2r+7rC5rembWPhbR//cGbLnnfYMsyqzKqlgC0zFH76MihzfrHflV/sd+UX+135xX5Xfi529X992fJuZssCXuco9TJYBZcaC0WwwsruiBzbTJqmax0FbJIkqnCb+WjiFFZ28+TYZvKWtdg4jlkul0RRRBzHa0+yqSRJQhRFqhUqo7BRFBGGIdPplDAMtwaO45j5fM58PicMw8JVVtjZbMZkMuHp6Ynn52eCINg4OI5jgiDA931832c2m7FYLNRx1fUaDAZ4nker1cKyLLIsw3Vd1aqXjbqvbNjJm1mu0fl8ju/7DAYDhsMh4/GYIAhUvcJeX1/T6XRwHAdN05hOpzSbTer1OrVaTfXA/qdNDx93vqMoUtjhcEi/38fzPEajkaovtOn7/T4ALy8veJ6H67qqTb+K/QxURoJXO99hGDKbzRiPx3iex9XVFTc3N+p7Gmueg52fn6vlIKH57uL/QGVWwXEcq1a9fAiSh8IH2LLm6+6WDeQP81+8EyzgnHEAAAAASUVORK5CYII=\\\"/></g></g></mask><mask id=\\\"mask-3\\\" x=\\\"111.57\\\" y=\\\"11.37\\\" width=\\\"43\\\" height=\\\"43\\\" maskUnits=\\\"userSpaceOnUse\\\"><g class=\\\"cls-16\\\"><g transform=\\\"translate(-876.43 -456.63)\\\"><image width=\\\"43\\\" height=\\\"43\\\" transform=\\\"translate(988 468)\\\" xlink:href=\\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAArCAYAAADhXXHAAAAACXBIWXMAAAsSAAALEgHS3X78AAADJElEQVRYR+3ZS0/qQByH4Zeh0NKLFUMQVwYVw9Lv/yXcGDdeolEiAkbSlN5o6VmYjqViTo5HoCb+kibQGZqHYWYS/lMBUn5IxN86lClK8Ua326XT6WCaJpqmoSgK1WoVId6+V6VS+fCQryZN337UxWJBkiTEcUwYhjiOw2g04vb2dqn/Evbk5ISzszMODw9ptVpYloWqqtRqNYQQCCGWsP8Kz3D590Wo67qMx2MeHx/RdZ2LiwvZfwnb7Xbp9/v0ej0ODg7Y2dmh0WhIbKVSkcB/hWbJg9M0JU1TkiRhPp/j+z6O4/D8/Eyz2SRNU3zf5+bmBshh+/0+p6enHB0dcXx8TKfTwbZtVFVFURQJ/SpyVfLYJEnkFDBNEyEE0+mUh4eHj9hOpyOv/f192u02hmHIubqJLBYLNE0DYDabsbe3h2VZsl1KDMPAtm12d3exbXvjUAAhBIZhYFkWpmlimib1ev29PXtRq9XQNA1d11FVdePQLEIIVFVF0zTq9TqK8r6spEhRFGq1mry2GSEEiqLIbVPez3eoVqtUq9VvXURfSX6bzFuWfutVHbaRzFHc1yU2vzVtGwvv+/inI1v2fMCWYVSzFC1L2DJD4adPgzLnF7uu/GLXlV/suvKLXVd+Lrb4v75s+TCyZQGvcpR6GhTBpZ8GeZPEZnWnrEqyzXzmWMLmwdtMZimCJTZfzYvjeOVDNpXMkiTJamwcx0RRRBRFW8cmSUIURXLwskhsGIbMZjNc18X3/a2B4zgmCAKCIMD3fZIkkW0S63ke0+mUl5cXXl9fcRyH+Xy+8oHrShzHuK6L4zg4joPneYRhKNtl1evp6Yn7+3tarRaGYZCmKUEQyFJ9vkryXckWczZHgyDAcRyGwyGj0YjJZILrurK/xF5dXWGaJo1GA3ivj+q6Tr1el+cK/1Omh88r31EUSexoNOLu7o7BYMB4PJb9l8r05+fnsjQ+HA5pNpsSWzxT+Ao0SwYuVr5938fzPCaTCYPBgMvLS66vr+XnKqw4B+v1erTbbSzLkqOary7+DzRLERzHsSzVZ4cgeSh8gi1rvm+1bCB/AOUnxFb7yBLGAAAAAElFTkSuQmCC\\\"/></g></g></mask><mask id=\\\"mask-4\\\" x=\\\"11.57\\\" y=\\\"61.37\\\" width=\\\"43\\\" height=\\\"44\\\" maskUnits=\\\"userSpaceOnUse\\\"><g class=\\\"cls-16\\\"><g transform=\\\"translate(-876.43 -456.63)\\\"><image width=\\\"43\\\" height=\\\"44\\\" transform=\\\"translate(888 518)\\\" xlink:href=\\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAAsCAYAAAD8WEF4AAAACXBIWXMAAAsSAAALEgHS3X78AAAD/ElEQVRYR+2Z60/yPADFT9l9QwbjEkXMo1/w//9/jEExTHSMwZizu5T3w5M2Gwx8NC+giSdpGFm7/XLWS3pKAKzxQ1T7qMJ3krzv5s3NDdrtNkzThCzLkCQJhBAQQgBA/P6r1ut16ZoxBsYYkiQBpRSz2Qz39/c72xNsdIPBYIButwvHcTAYDOA4Dur1OjRNgyzLqNVqqNX+fpAi7C7wIiD/z0ue58iyDJRSRFEEz/Pgui5838fLywuenp5KbUvOXl9f4/b2FldXV7i4uECv10Or1RKwiqJAkiTUarVPu8uhOShjDHmeI01TUEoRhiGCIMDr6ytc18V4PIYsyxiNRuIZArbf72M4HGI4HOL6+hqXl5fodrtoNBqo1+tQVRWKoghn/8VVrs3PX3SWw0ZRhMVigW63C9u2oes6GGOglMJ1XQAFWMdxcH5+jsFggD9//qDf76PT6YiGXwUtquguADDGkGUZsixDHMewbRumaUKSJKRpiiAI4LruNqxlWXAcB51OB71eD71eD+12G5ZlQZblT0F9RpqmYb1ewzAMqKoKQgiSJEEQBGg2mzAMQ9QVsJqmwbIsNBoN2LYN27ZhWRYURal8yf8pQghUVUW9XkeapgjDEI1GA6ZpQlVVUU/Ms5IkQdM0GIYBwzDEgDqmFEWBruswDAO6rovux1WCVRRFQB4bFPjrsCzL4v18quQSV3zwSJK0VemYkiSpxFAJSwgRNzdH/DFFCBFz+SZHyT6+lBaX1GNrH8NO2FOriqXUDTYrn0q73r01ir6Ts5va6gan1j6G08xPX9Qv7KH0C3so/cIeSj8XdnPb/N1U6ewpoTc3lUVtwe6rfGoJ2O8Et4tlq8/ycmpVcZSc3Syn0D6OkrM81WOMnRQ2z/P9sDwo43EOY6zyYYdWnuciVto0rQSbZRmSJEGapkjTtPJhhxYP66pME7A8J43jGHEcg1KKLMsqH3gocbMopaCUIkkS5Hku7gtYHjuGYYjlcokwDPH29nY04DzPEccxVquVKHEcI0kSUUcEc1EUYT6fYzabodVqQdd1AECapiJS4qED3yd9dc9WXHj4WHl/f8dqtUIQBPB9H/P5HIvFAnEci3YC1vd9TKdTcYZACAGlFKvVSgR1xdT7q8BVoPzTL5dLeJ6H5+dnTKdTeJ4H3/dFWwE7mUxgmiYURcF6vUYcxwiCAGdnZyI75flTVQDxEXRxVPMpqRjV8y7g+z4mkwlGoxEeHx8xHo9Fu9KZwt3dHRhjSNMUi8UCzWazdPhRzKCAjwF3iYPywgdWFEUIggDT6RQPDw8i8ebaOq0BIE5pLMsqOfqVg48qFbsCXwTyPBezked5Wyc1wA7Y76oftVP4D/nsfMMRIRpaAAAAAElFTkSuQmCC\\\"/></g></g></mask><mask id=\\\"mask-5\\\" x=\\\"61.57\\\" y=\\\"61.37\\\" width=\\\"43\\\" height=\\\"44\\\" maskUnits=\\\"userSpaceOnUse\\\"><g class=\\\"cls-16\\\"><g transform=\\\"translate(-876.43 -456.63)\\\"><image width=\\\"43\\\" height=\\\"44\\\" transform=\\\"translate(938 518)\\\" xlink:href=\\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAAsCAYAAAD8WEF4AAAACXBIWXMAAAsSAAALEgHS3X78AAAD8UlEQVRYR+2Z626qQBSF1wgoN294SWttav/Y93+fJk1tarEpIMqdAc6PZiao1HNsjqVN+iVEExnmy5LZhD0EQIEfQuNvJ3wnxGM/3t7eYjAYQFVViKIIQRBACAEhBAD45ykURcE/i6JAnufIsgxJkiAIAti2jcViUTn2QHY6nWI0GsEwDEynUxiGAV3X0Wq1IIoiGo0GGo33P6Qse0ycCbLvVaJhGGKz2cC2bUwmEyyXywPpHdnZbIa7uztcX1/j8vIS4/EY/X6fy0qSBEEQ0Gg0Tk53P9GiKJBlGdI05am6rgvLsjAcDmEYBgRBwMPDA78Gl51MJpjP55jP55jNZri6usJoNEKn04Gu62g2m5AkiSf7r6kCx5NlsmEYwnVdvL29Qdd1iKIISimiKMLLywuAkqxhGLi4uMB0OsXNzQ0mkwmGwyG63S5kWf60aJl96TzPuXAURWi321AUBYQQRFEEx3GwXC4PZTVNg2EYGA6HGI/HGI/HGAwG0DQNoiieJHUqsixDURRIkgRCCOI4xnq9Rq/Xg6qq/Dwu22q1oGkaOp0Out0uut0uNE2DJEmVE/xPCCGQJAm6riNNU7TbbbTbbaiqimazyc/jdVYQBLRaLSiKAkVR+IL6SkRRhCzL/GAViLEjK0kSl/xqUeA9YeYhiiKv7QwuyxaPIAi8ntaBIAjcgT2EGNyIEMKF91f8V8LSZQ6VsuzE8lEHxxw+lK2bKped22D/5Lr4aO6DVfSdkt3n4Daom2MO9dSnT/Irey5+Zc/Fr+y5+Lmy5Xek70hlsnVKH5v7QLb8fl8nVfNz2brlynzkcnDPsqNuqjx2kt0/6uCYx06yrEOS53mtsmz+D2VZR49SCkop8jyvvNi5KYqCe+yHtiNLKUWSJEjTFGmaVl7s3LCwKKXIsqxallKKOI4RhiHCMEQcx6CUVl7wXLCw4jjmoWVZxn/nsnEcw/d9bLdbbDYbbLdbBEHwZcJZliEMQwRBAN/3EQQBoija+Yd5I8n3fTiOA8uy0O/3IcsyACBNU95S2m88fPadrfzgYWsliiL4vg/btuE4DlzXhed5SJKEj+Oytm1jtVrxPQRC3luPnufxRl1Vp+RU4X3RPM+RJAmiKMJ2u4VlWTBNE6+vr3AcB57n8bFcdrlcQlVVSJKEoigQhiHW6zVv8DabTd4Dq2pA/E26vFBYSWKpsmay53lwHAemaeLx8RHPz89Yr9d83M6ewv39Pe9Eu66LXq+3s/nBkq3aADmFci1lZSpJEvi+j81mg9VqhcViAdM0YZomH0dQsWnHdmk0TdtJ9DMbHx9RLvpZliHLMl6NLMvC09PTwZhK2e/Kj3pT+AOtZ3ePHu+txgAAAABJRU5ErkJggg==\\\"/></g></g></mask><mask id=\\\"mask-6\\\" x=\\\"111.57\\\" y=\\\"61.37\\\" width=\\\"43\\\" height=\\\"44\\\" maskUnits=\\\"userSpaceOnUse\\\"><g class=\\\"cls-16\\\"><g transform=\\\"translate(-876.43 -456.63)\\\"><image width=\\\"43\\\" height=\\\"44\\\" transform=\\\"translate(988 518)\\\" xlink:href=\\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAAsCAYAAAD8WEF4AAAACXBIWXMAAAsSAAALEgHS3X78AAADaUlEQVRYR+2Z207qWhRAR0tLuRUFKUjUuNWowcQH//8jTHwwJiImJhKwQcDQQu/nqWsXqR73ORutiSNZCem6dDA7VwNzSUDEN0H+twFZQnmv8/z8nGazSalUQlEUFEVBkiQkSXpv2oeIokg03/fxPI/ZbMZwOOTm5iZ1jsSrNDg+PmZnZwfDMDg4OKDRaKDrOvl8nlwuhyzLyLK8JPwR+ShazrYoigiCgDAM8TyPxWLBZDLBNE16vR739/dcX18vzVmK7MnJCRcXF0K43W5Tr9cpl8vk83kRWVn+nT0fEY1JCkdRRBiGBEGA7/vYts1sNsM0TdrtNoZhoCgKV1dXYs6S7OHhIZ1Oh06nw+7uLs1mE13XKRQKKIpCLpf762kQBAFBEOB5HpZlYRiGeJLxl+h2u0BC9uzsjKOjI379+sX+/j57e3tsbGxQLBaXIrlOdF0X93McB9M0abVaq7KtVot2u0273abValGr1SgWi28uvA7y+Tybm5s4jsPW1hb1ep1KpSL6RchKpRLVapVqtUqlUqFQKKQuuG5UVaVUKlEul8VeiRGyqqpSKBQoFotomvZX8vK/oigKmqahqiqK8ntbCVlFUVBVdWXAVyDLMrlcTjRxPf4gSZLo/MqoAuL1+Pp9viQbd3617FseS7LJlhVSI/sdyKzsu2nw1oAskdnIpvEjuy5+ZNfFj+y6+JFdF99X9vV/+6yxEtksC2c2DdKClllZWBVeydm4ZYWki5CNa09ZEI093oxsLBu3ryT5hFMjm6zoBUGQushnkSyHpsp6nofjOCwWC1zXTV3ks/B9XxSYk4ETsq7rYlkWlmUxn8/xPC91oXXj+z6O42DbNq7rLnkI2ZeXF0ajEaPRiOfnZ15eXj49wkEQYFkW0+mU6XS64iCKWk9PTzw+PrK9vU25XEaSJBzHoVQqoaqqKNHDn1W73yPeQGEY4vs+8/mc6XTKYDBgOByKoMUI2W63i67raJpGGIbYtk2j0aBSqaBp2tJ5Avx/4eRuT1a+x+Mx/X6fu7s7er0epmmKOUvlwsvLS8IwxHVdxuMxtVpN1EiTRbs/PfxIknauEG+m+XzOZDKh3+9ze3vLw8MDvV5PjF85rQE4PT3FMAyq1aoog66jaPc6DVzXxbZtBoNB6vFSqmxWyfQPmdf8A6NKyy8g/AoLAAAAAElFTkSuQmCC\\\"/></g></g></mask><mask id=\\\"mask-7\\\" x=\\\"11.57\\\" y=\\\"112.37\\\" width=\\\"43\\\" height=\\\"43\\\" maskUnits=\\\"userSpaceOnUse\\\"><g class=\\\"cls-16\\\"><g transform=\\\"translate(-876.43 -456.63)\\\"><image width=\\\"43\\\" height=\\\"43\\\" transform=\\\"translate(888 569)\\\" xlink:href=\\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAArCAYAAADhXXHAAAAACXBIWXMAAAsSAAALEgHS3X78AAADkUlEQVRYR+2Za2vqShRAV4xmjAY1FRGlQvvB//+PCgVp00iNtXl08ryfZoivHm971B7oAjHoTGa5ndk6ewyg4h+h8acGP4nm7gvT6ZThcEin00EIQbPZpNFo0Gg0MAwDQD9/laqq9HNVVZRlSVEUZFlGmqa8v7+zXq/xPG+r35bs3d0d8/mcyWSC67o4joMQglarhWmaGIahH4pTxZWgut4VTdOUJEmIoojVaoXneQgheHx81P207HQ6ZT6fM5/Pmc1mjEYj+v0+tm0jhMA0TR3dXeFT2Y1oVVU6olJK4jhmvV6zXC5xHAcAKaWOsJYdDodMJhNmsxn39/eMx2Nc18W2bSzL0tOhLvp/hQ/JlmVJmqZIKQnDkPV6TafTASAMQ15eXvZlO50OrusyGo0Yj8dMJhMGg4GW/a6ooi4MUJYleZ6TpilRFNFutynLkjiO8TxPi0NNVgiB4zj0+31c12UwGDAYDLAs68tipyKEoN1u02q1AIjjmF6vR7fbxbIs3U7LNptNhBDYtq0flxBVmKaJbdukaYrjONi2vfUBoJZnG40GrVYLIQSWZV1UVGGaph7bsiydhRRbsqZpYpqmXkzXQI3fbDZ1BlLoK7V4dn8ALo0av54q9Xv1hvUcei3ZzwK2F9lriiqOpci9ifndPPo3ORrZzxpdmmPj783Za/PZN3ud/PRFfmXPxa/sufiVPRe/sudiS7a+Xb4Wu3u0OnuRVbvOn8jRaXBN4WNja9n6Xv6aoopDHntz9trCuw51j73IlmV5NVFAl5T+KFsUhS6UlWV58GbnRo2d5/le4LRsURS6mpemKXmeH7zZOVEBy7KMPM+1sGJLNk1TPj4+kFIipaQoioM3PRd5nuuxpZTHZaWURFFEGIZsNhvCMCSKootEuKoqsiwjjmPCMNRjJ0lClmW6na51JUnC29sbQRCwWq2wbRuALMv2Sp51Tt237S5atXjU9FMlzyAICIKAzWZDFEVIKXUfLfv6+orv+zw9PWHbti47qup3vZzzne26kq4vaFVMVrKe57FcLgmCgCRJdF8tu1gs9FmCYRjEccxqtaLb7WrZQ9E9Vbge2XpaUgtJTcPNZsNyuWSxWOD7PkEQ6H5bZwrPz88ARFGE7/v0er2jle9TJQ9Rl1VpKs9zfaYQBAG+7/Pw8KCdAAzYPwe7vb3l5ubmr54n7LIrXJ8OSZIQBMGWKByR/an8U3++/wN2T3nxpLkmlwAAAABJRU5ErkJggg==\\\"/></g></g></mask><mask id=\\\"mask-8\\\" x=\\\"61.57\\\" y=\\\"112.37\\\" width=\\\"43\\\" height=\\\"43\\\" maskUnits=\\\"userSpaceOnUse\\\"><g class=\\\"cls-16\\\"><g transform=\\\"translate(-876.43 -456.63)\\\"><image width=\\\"43\\\" height=\\\"43\\\" transform=\\\"translate(938 569)\\\" xlink:href=\\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAArCAYAAADhXXHAAAAACXBIWXMAAAsSAAALEgHS3X78AAADnElEQVRYR+2Za2+qShSGH0BAkBgvaYymafVD//8/atLEtBRTsZZLh+v5NBPwsndzjKU76ZsQiM4wj69rFswaDaj5R6T/rcFPUu/wg9lsxnQ6xXVdbNvGsix0XUfXdTRNQ9M0AHX+P6rrWp3ruqaqKsqyJM9zsizj4+OD3W6H7/utfi3YxWLBw8MDi8WC6XSK53k4joNpmhiGcQQMX4eWgPL6EDTLMtI0JY5jttstvu9j2zZPT0+qXwt2Pp+zWq1YrVbMZjNGo5FyuNfrYRjGRe4eOlrXtXJUCEGSJOx2OzabDZ7nASCEUA4r2Lu7O5bLJff39yyXSxaLBZPJRMGapnlxKJyCraqKLMsQQhBFEbvdDtd1AYiiiNfX12PY6XTKzc0Ns9mM+XzOfD5XsJZlXeyqVBMYoKoqiqIgyzLiOKbf71NVFUmS4Pu+AocGrOM4DIdDxuMx4/GYyWTCaDTCtm10/bpJw7Zt+v0+pmkCkCQJw+GQwWCAZVmqnYK1LAvXdXFdF8/z1N9/bVApwzBwHIcsy9TEbv4AaORZwzAwTZN+v99KWd8pwzCwLEsdMgtJKRpd1+n1eupoNvpOGYbRYmgapq40TUPXdQzDUJOpC8kHUDOvq+/khZzpzaMLSdMOQeHg3aBrUKlzKbLl7GGHrvVHZ2WDrkHPjX8UBl3rT0/I702kF+oX9lr6hb2WfmGvpV/Ya6kF21wud6XDNVpTR87KVedP1Nkw6BL43NgKtrmW7xJU6hTHUcx2DXzI0OQ4craqqs5AAVVS+itsWZaqUFZV1cmbXVty7KIojoxTsGVZqmpelmUURXHyZteUNCzPc4qiUMBSLdgsy/j8/EQIgRCCsixP3vRaKopCjS2EOA8rhCCOY6IoYr/fE0URcRx/i8N1XZPnOUmSEEWRGjtNU/I8V+1UrStNU97f3wnDkO12i+M4AOR5jmVZ9Hq9k2v5r67bDietnDwy/GTJMwxDwjBkv98TxzFCCNVHwb69vREEAc/PzziOo8qOnue1islN4K+CNiWhmxNaFpMlrO/7bDYbwjAkTVPVV8Gu12u1l6BpGkmSsN1uGQwGCvaUu18FbjrbTEtyIskw3O/3bDYb1us1QRAQhqHq1yrTv7y8ABDHMUEQMBwOcRznKAwurS00YWWaKopC7SmEYUgQBDw+PiomAA2O98Fub2+ZTCY4joNt20ebH5eASh0CN8MhTVPCMGyBwhnYn6p/6uX7P4W9eoGB8TNYAAAAAElFTkSuQmCC\\\"/></g></g></mask><mask id=\\\"mask-9\\\" x=\\\"111.57\\\" y=\\\"112.37\\\" width=\\\"43\\\" height=\\\"43\\\" maskUnits=\\\"userSpaceOnUse\\\"><g class=\\\"cls-16\\\"><g transform=\\\"translate(-876.43 -456.63)\\\"><image width=\\\"43\\\" height=\\\"43\\\" transform=\\\"translate(988 569)\\\" xlink:href=\\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAArCAYAAADhXXHAAAAACXBIWXMAAAsSAAALEgHS3X78AAADoUlEQVRYR+2ZW2+qTBiFH0COpY2HNEYvWr3o//9FbdKkB6pRiHKQ83exMxNE7W6+1tKddCUTiDLwuJx5YRYKUPOPSP3bAT9JvfYH4/GY0WiE4ziYpolhGKiqiqqqKIqCoigAcvt/VNe13NZ1TVVVlGVJnudkWcZ2uyUIAjzP2+u3BzudTrm7u2M6nTIajXBdF9u20XUdTdMOgOHj0AJQ7LdBsywjSRKiKGK9XuN5HqZp8vj4KPvtwU4mE+bzOfP5nPF4TL/flw73ej00TfuUu21H67qWjqZpShzHBEHAcrnEdV0A0jSVDkvYm5sbZrMZt7e3zGYzptMpw+FQwuq6/umhcAy2qiqyLCNNU8IwJAgCHMcBIAxD3t7eDmFHoxHX19eMx2MmkwmTyUTCGobxaVeFmsAAVVVRFAVZlhFFEZZlUVUVcRzjeZ4EhwasbdtcXV0xGAwYDAYMh0P6/T6maaKq5y0apmliWRa6rgMQxzFXV1dcXFxgGIY8TsIahoHjODiOg+u68u8/N6iQpmnYtk2WZXJiN38ANOqspmnouo5lWXsl6zulaRqGYcgmqpCQpFFVlV6vJ1vzoO+Upml7DE3D5J6iKKiqiqZpcjJ1IXEDatZ1+Z3YETO92bqQMK0NCq1ng65BhU6VyD1n2x261rvOigO6Bj11/YNh0LXeu0N+byH9pH5hz6Vf2HPpF/Zc+oU9l/Zgm8vlrtReozV14KxYdf5EnRwGXQKfuraEba7luwQVOsZxMGa7Bm4zNDkOnK2qiqqqOoUty/J9WBGQlWXZKay4flEUBxx7sCLGybKMPM+PnuycEq7meU5RFBJYSMKK2HG327Hb7UjTlLIsj570XCqKgjRNZTsJu9vtiKKI7XbLZrNhu90SRRFFURw98VeqrmvyPCeOY8IwJAxDoigiSZK9f1hmXUmSEAQBq9WKwWCAZVkAZFkm81mRjjTXRx9dt7XngJg8Yp6IyNP3fXzfZ7PZEEURaZrKPhJ2tVrx8vJCv9/Htm3quiaOYy4vL2U+205JPgralIAWoFVVyTBZwHqex3K5xPd9kiSRfSXs8/OzDOXgT+y4Xq9xXVfC9nq9gyDko8BNZ5tlSUykNE2JoojNZsNyueTp6YnFYoHv+7LfXkx/f38P/InGV6uVdLk5DL4itWnCiipUFIV8p+D7PovFgoeHB15fX2U/hSPvwcQLENu2ZfT4VaBCbeDmcEiSBN/390DhBOxP1T/18P0fQcp4ILYL4HQAAAAASUVORK5CYII=\\\"/></g></g></mask></defs><title>genepattern-logo</title><g class=\\\"cls-1\\\"><g id=\\\"Layer_1\\\" data-name=\\\"Layer 1\\\"><rect class=\\\"cls-2\\\" x=\\\"1.22\\\" y=\\\"1.22\\\" width=\\\"164.1\\\" height=\\\"164.1\\\"/><path class=\\\"cls-3\\\" d=\\\"M928.78,503.56a5,5,0,0,1-5,5H895.44a5,5,0,0,1-5-5V475.21a5,5,0,0,1,5-5h28.34a5,5,0,0,1,5,5Z\\\" transform=\\\"translate(-876.43 -456.63)\\\"/><g class=\\\"cls-4\\\"><g class=\\\"cls-5\\\"><path class=\\\"cls-6\\\" d=\\\"M928.78,503.56a5,5,0,0,1-5,5H895.44a5,5,0,0,1-5-5V475.21a5,5,0,0,1,5-5h28.34a5,5,0,0,1,5,5Z\\\" transform=\\\"translate(-876.43 -456.63)\\\"/></g></g><path class=\\\"cls-7\\\" d=\\\"M978.86,503.56a5,5,0,0,1-5,5H945.53a5,5,0,0,1-5-5V475.21a5,5,0,0,1,5-5h28.34a5,5,0,0,1,5,5Z\\\" transform=\\\"translate(-876.43 -456.63)\\\"/><g class=\\\"cls-8\\\"><g class=\\\"cls-5\\\"><path d=\\\"M978.86,503.56a5,5,0,0,1-5,5H945.53a5,5,0,0,1-5-5V475.21a5,5,0,0,1,5-5h28.34a5,5,0,0,1,5,5Z\\\" transform=\\\"translate(-876.43 -456.63)\\\"/></g></g><path class=\\\"cls-7\\\" d=\\\"M1029,503.56a5,5,0,0,1-5,5H995.61a5,5,0,0,1-5-5V475.21a5,5,0,0,1,5-5H1024a5,5,0,0,1,5,5Z\\\" transform=\\\"translate(-876.43 -456.63)\\\"/><g class=\\\"cls-9\\\"><g class=\\\"cls-5\\\"><path d=\\\"M1029,503.56a5,5,0,0,1-5,5H995.61a5,5,0,0,1-5-5V475.21a5,5,0,0,1,5-5H1024a5,5,0,0,1,5,5Z\\\" transform=\\\"translate(-876.43 -456.63)\\\"/></g></g><path class=\\\"cls-3\\\" d=\\\"M19,64.35H47.35a5,5,0,0,1,5,5V97.69a5,5,0,0,1-5,5H19a5,5,0,0,1-5-5V69.34A5,5,0,0,1,19,64.35Z\\\"/><g class=\\\"cls-10\\\"><g class=\\\"cls-5\\\"><path d=\\\"M19,64.35H47.35a5,5,0,0,1,5,5V97.69a5,5,0,0,1-5,5H19a5,5,0,0,1-5-5V69.34A5,5,0,0,1,19,64.35Z\\\"/></g></g><rect class=\\\"cls-3\\\" x=\\\"64.1\\\" y=\\\"64.35\\\" width=\\\"38.33\\\" height=\\\"38.33\\\" rx=\\\"5\\\"/><g class=\\\"cls-11\\\"><g class=\\\"cls-5\\\"><rect x=\\\"64.1\\\" y=\\\"64.35\\\" width=\\\"38.33\\\" height=\\\"38.33\\\" rx=\\\"5\\\"/></g></g><path class=\\\"cls-7\\\" d=\\\"M119.18,64.35h28.34a5,5,0,0,1,5,5V97.69a5,5,0,0,1-5,5H119.18a5,5,0,0,1-5-5V69.34A5,5,0,0,1,119.18,64.35Z\\\"/><g class=\\\"cls-12\\\"><g class=\\\"cls-5\\\"><path d=\\\"M119.18,64.35h28.34a5,5,0,0,1,5,5V97.69a5,5,0,0,1-5,5H119.18a5,5,0,0,1-5-5V69.34A5,5,0,0,1,119.18,64.35Z\\\"/></g></g><path class=\\\"cls-3\\\" d=\\\"M19,114.6H47.35a5,5,0,0,1,5,5v28.35a5,5,0,0,1-5,5H19a5,5,0,0,1-5-5V119.59a5,5,0,0,1,5-5Z\\\"/><g class=\\\"cls-13\\\"><g class=\\\"cls-5\\\"><path d=\\\"M19,114.6H47.35a5,5,0,0,1,5,5v28.35a5,5,0,0,1-5,5H19a5,5,0,0,1-5-5V119.59a5,5,0,0,1,5-5Z\\\"/></g></g><path class=\\\"cls-7\\\" d=\\\"M69.09,114.6H97.44a5,5,0,0,1,5,5v28.35a5,5,0,0,1-5,5H69.09a5,5,0,0,1-5-5V119.59A5,5,0,0,1,69.09,114.6Z\\\"/><g class=\\\"cls-14\\\"><g class=\\\"cls-5\\\"><path d=\\\"M69.09,114.6H97.44a5,5,0,0,1,5,5v28.35a5,5,0,0,1-5,5H69.09a5,5,0,0,1-5-5V119.59A5,5,0,0,1,69.09,114.6Z\\\"/></g></g><path class=\\\"cls-3\\\" d=\\\"M1029,604.57a5,5,0,0,1-5,5H995.61a5,5,0,0,1-5-5V576.22a5,5,0,0,1,5-5H1024a5,5,0,0,1,5,5Z\\\" transform=\\\"translate(-876.43 -456.63)\\\"/><g class=\\\"cls-15\\\"><g class=\\\"cls-5\\\"><path d=\\\"M1029,604.57a5,5,0,0,1-5,5H995.61a5,5,0,0,1-5-5V576.22a5,5,0,0,1,5-5H1024a5,5,0,0,1,5,5Z\\\" transform=\\\"translate(-876.43 -456.63)\\\"/></g></g></g></g></svg>\";",
```

### Comparing `nbtools-23.5.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js` & `nbtools-23.7.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js.map` & `nbtools-23.7.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js` & `nbtools-23.7.0/nbtools/labextension/static/remoteEntry.5f8f98422831593fa148.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -179,17 +179,17 @@
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
                 "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9": "05e08e7398a87350659a",
                 "node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759": "0a0e1ed7766bfba46905",
-                "lib_registry_js-lib_uibuilder_js-lib_uioutput_js": "62f16408cce9e2f6ea27",
+                "lib_registry_js-lib_uibuilder_js-lib_uioutput_js": "cd289910d38270a1d73e",
                 "lib_index_js": "7be7e51ff21fbbccb028",
-                "lib_plugin_js": "9ee79910806137e493ce",
+                "lib_plugin_js": "6292de8fa547e3973251",
                 "style_index_js": "1f214e1107ae935d92bb"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
@@ -423,15 +423,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("@g2nb/nbtools", "23.3.2", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9"), __webpack_require__.e("node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759"), __webpack_require__.e("lib_registry_js-lib_uibuilder_js-lib_uioutput_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("@g2nb/nbtools", "23.5.0", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9"), __webpack_require__.e("node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759"), __webpack_require__.e("lib_registry_js-lib_uibuilder_js-lib_uioutput_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -794,17 +794,19 @@
             /******/
             "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 5, 3])),
             /******/
             "webpack/sharing/consume/default/@jupyter-widgets/base": () => (loadSingletonVersionCheck("default", "@jupyter-widgets/base", [1, 6])),
             /******/
             "webpack/sharing/consume/default/@jupyterlab/cells": () => (loadVersionCheck("default", "@jupyterlab/cells", [1, 3, 5, 3])),
             /******/
+            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 1, 33, 0])),
+            /******/
             "webpack/sharing/consume/default/@lumino/coreutils": () => (loadSingletonVersionCheck("default", "@lumino/coreutils", [1, 1, 11, 0])),
             /******/
-            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 1, 33, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 3, 5, 3])),
             /******/
             "webpack/sharing/consume/default/@jupyterlab/mainmenu": () => (loadSingletonVersionCheck("default", "@jupyterlab/mainmenu", [1, 3, 5, 3])),
             /******/
             "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 3, 5, 3]))
             /******/
         };
         /******/ // no consumes in initial chunks
@@ -815,22 +817,24 @@
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/notebook",
                 /******/
                 "webpack/sharing/consume/default/@jupyter-widgets/base",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/cells",
                 /******/
-                "webpack/sharing/consume/default/@lumino/coreutils",
+                "webpack/sharing/consume/default/@lumino/widgets",
                 /******/
-                "webpack/sharing/consume/default/@lumino/widgets"
+                "webpack/sharing/consume/default/@lumino/coreutils"
                 /******/
             ],
             /******/
             "lib_plugin_js": [
                 /******/
+                "webpack/sharing/consume/default/@jupyterlab/settingregistry",
+                /******/
                 "webpack/sharing/consume/default/@jupyterlab/mainmenu",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/application"
                 /******/
             ]
             /******/
         };
@@ -1057,8 +1061,8 @@
     /******/ // module exports must be returned from runtime so entry inlining is disabled
     /******/ // startup
     /******/ // Load entry module and return exports
     /******/
     return __webpack_require__("webpack/container/entry/@g2nb/nbtools");
     /******/
 })();
-//# sourceMappingURL=remoteEntry.ed7f531dbfb094c43618.js.map
+//# sourceMappingURL=remoteEntry.5f8f98422831593fa148.js.map
```

### Comparing `nbtools-23.5.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js.map` & `nbtools-23.7.0/nbtools/labextension/static/remoteEntry.5f8f98422831593fa148.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333333%*

 * *Differences: {"'file'": "'remoteEntry.5f8f98422831593fa148.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC,E;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;;;;WCxBA;WACA;WACA;WACA;WACA;WACA,gCAAgC,YAAY;WAC5C;WACA,E;;;;;WCPA;WACA;WACA;WACA;WACA,wCAAwC,yCAAyC;WACjF;WACA; […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.ed7f531dbfb094c43618.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC,E;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;;;;WCxBA;WACA;WACA;WACA;WACA;WACA,gCAAgC,YAAY;WAC5C;WACA,E;;;;;WCPA;WACA;WACA;WACA;WACA,wCAAwC,yCAAyC;WACjF;WACA;WACA,E;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF,E;;;;;WCRA;WACA;WACA;WACA,8BAA8B,2bAA2b;WACzd,E;;;;;WCJA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA,CAAC,I;;;;;WCPD,wF;;;;;WCAA;WACA;WACA;WACA;WACA,sBAAsB,4BAA4B,QAAQ;WAC1D;WACA;WACA;WACA,gBAAgB,oBAAoB;WACpC;WACA,kGAAkG,YAAY,OAAO;WACrH;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,kEAAkE,kCAAkC;WACpG;WACA;WACA;WACA,E;;;;;WCzCA;WACA;WACA;WACA,sDAAsD,kBAAkB;WACxE;WACA,+CAA+C,cAAc;WAC7D,E;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mJAAmJ;WACnJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,GAAG,aAAa,kBAAkB;WAClC;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,E;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,kC;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,+BAA+B,eAAe,oBAAoB,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WACnZ;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,KAAK;WACL,IAAI,WAAW,YAAY;WAC3B,GAAG;WACH;WACA,C;;;;;WCzKA;;WAEA;WACA;WACA;WACA;WACA;WACA;;;WAGA;WACA;WACA;WACA,gCAAgC;;WAEhC;WACA;WACA;WACA,IAAI;WACJ,cAAc;WACd;WACA;WACA;WACA,MAAM;WACN;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,oBAAoB;WAC1B;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;WAEA,sB;;;;UC3FA;UACA;UACA;UACA",
+    "file": "remoteEntry.5f8f98422831593fa148.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC,E;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;;;;WCxBA;WACA;WACA;WACA;WACA;WACA,gCAAgC,YAAY;WAC5C;WACA,E;;;;;WCPA;WACA;WACA;WACA;WACA,wCAAwC,yCAAyC;WACjF;WACA;WACA,E;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF,E;;;;;WCRA;WACA;WACA;WACA,8BAA8B,2bAA2b;WACzd,E;;;;;WCJA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA,CAAC,I;;;;;WCPD,wF;;;;;WCAA;WACA;WACA;WACA;WACA,sBAAsB,4BAA4B,QAAQ;WAC1D;WACA;WACA;WACA,gBAAgB,oBAAoB;WACpC;WACA,kGAAkG,YAAY,OAAO;WACrH;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,kEAAkE,kCAAkC;WACpG;WACA;WACA;WACA,E;;;;;WCzCA;WACA;WACA;WACA,sDAAsD,kBAAkB;WACxE;WACA,+CAA+C,cAAc;WAC7D,E;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mJAAmJ;WACnJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,GAAG,aAAa,kBAAkB;WAClC;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,E;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,kC;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,+BAA+B,eAAe,oBAAoB,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WACnZ;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,KAAK;WACL,IAAI,WAAW,YAAY;WAC3B,GAAG;WACH;WACA,C;;;;;WC3KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;;WAGA;WACA;WACA;WACA,gCAAgC;;WAEhC;WACA;WACA;WACA,IAAI;WACJ,cAAc;WACd;WACA;WACA;WACA,MAAM;WACN;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,oBAAoB;WAC1B;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;WAEA,sB;;;;UC3FA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@g2nb/nbtools/webpack/container-entry",
         "webpack://@g2nb/nbtools/webpack/bootstrap",
         "webpack://@g2nb/nbtools/webpack/runtime/compat get default export",
         "webpack://@g2nb/nbtools/webpack/runtime/define property getters",
@@ -22,20 +22,20 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9\"), __webpack_require__.e(\"node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759\"), __webpack_require__.e(\"lib_registry_js-lib_uibuilder_js-lib_uioutput_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9\"), __webpack_require__.e(\"node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759\"), __webpack_require__.e(\"lib_registry_js-lib_uibuilder_js-lib_uioutput_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9\"), __webpack_require__.e(\"node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar oldScope = __webpack_require__.S[\"default\"];\n\tvar name = \"default\"\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tif(__webpack_module_cache__[moduleId]) {\n\t\treturn __webpack_module_cache__[moduleId].exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9\":\"05e08e7398a87350659a\",\"node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759\":\"0a0e1ed7766bfba46905\",\"lib_registry_js-lib_uibuilder_js-lib_uioutput_js\":\"62f16408cce9e2f6ea27\",\"lib_index_js\":\"7be7e51ff21fbbccb028\",\"lib_plugin_js\":\"9ee79910806137e493ce\",\"style_index_js\":\"1f214e1107ae935d92bb\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9\":\"05e08e7398a87350659a\",\"node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759\":\"0a0e1ed7766bfba46905\",\"lib_registry_js-lib_uibuilder_js-lib_uioutput_js\":\"cd289910d38270a1d73e\",\"lib_index_js\":\"7be7e51ff21fbbccb028\",\"lib_plugin_js\":\"6292de8fa547e3973251\",\"style_index_js\":\"1f214e1107ae935d92bb\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"@g2nb/nbtools:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"@g2nb/nbtools\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult.catch(handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@g2nb/nbtools\", \"23.3.2\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9\"), __webpack_require__.e(\"node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759\"), __webpack_require__.e(\"lib_registry_js-lib_uibuilder_js-lib_uioutput_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"@g2nb/nbtools\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult.catch(handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@g2nb/nbtools\", \"23.5.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9\"), __webpack_require__.e(\"node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759\"), __webpack_require__.e(\"lib_registry_js-lib_uibuilder_js-lib_uioutput_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(1===range.length)return\"*\";if(0 in range){var r=\"\",n=range[0];r+=0==n?\">=\":-1==n?\"<\":1==n?\"^\":2==n?\"~\":n>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,r+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return r}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/cells\": () => (loadVersionCheck(\"default\", \"@jupyterlab/cells\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,33,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/mainmenu\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,5,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_registry_js-lib_uibuilder_js-lib_uioutput_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/cells\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\"\n\t],\n\t\"lib_plugin_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_modules__[id] = (module) => {\n\t\t\t\t\tdelete __webpack_module_cache__[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_modules__[id] = (module) => {\n\t\t\t\t\tdelete __webpack_module_cache__[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory).catch(onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(1===range.length)return\"*\";if(0 in range){var r=\"\",n=range[0];r+=0==n?\">=\":-1==n?\"<\":1==n?\"^\":2==n?\"~\":n>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,r+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return r}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/cells\": () => (loadVersionCheck(\"default\", \"@jupyterlab/cells\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,33,0])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/mainmenu\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,5,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_registry_js-lib_uibuilder_js-lib_uioutput_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/cells\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\"\n\t],\n\t\"lib_plugin_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_modules__[id] = (module) => {\n\t\t\t\t\tdelete __webpack_module_cache__[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_modules__[id] = (module) => {\n\t\t\t\t\tdelete __webpack_module_cache__[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory).catch(onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// Promise = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"@g2nb/nbtools\": 0\n};\n\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => {\n\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId] = [resolve, reject];\n\t\t\t\t\t});\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no deferred startup\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0, resolves = [];\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tresolves.push(installedChunks[chunkId][0]);\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\tfor(moduleId in moreModules) {\n\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t}\n\t}\n\tif(runtime) runtime(__webpack_require__);\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\twhile(resolves.length) {\n\t\tresolves.shift()();\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_g2nb_nbtools\"] = self[\"webpackChunk_g2nb_nbtools\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));\n\n// no deferred startup",
         "// module exports must be returned from runtime so entry inlining is disabled\n// startup\n// Load entry module and return exports\nreturn __webpack_require__(\"webpack/container/entry/@g2nb/nbtools\");\n"
     ],
     "version": 3
 }
```

### Comparing `nbtools-23.5.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js` & `nbtools-23.7.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js.map` & `nbtools-23.7.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js` & `nbtools-23.7.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js.map` & `nbtools-23.7.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/nbextension/static/extension.js` & `nbtools-23.7.0/nbtools/nbextension/static/extension.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/nbextension/static/notebook.css` & `nbtools-23.7.0/nbtools/nbextension/static/notebook.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/nbextension/static/toolbox.js` & `nbtools-23.7.0/nbtools/nbextension/static/toolbox.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/nbtools/tests/conftest.py` & `nbtools-23.7.0/nbtools/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/src/basewidget.ts` & `nbtools-23.7.0/src/basewidget.ts`

 * *Files 6% similar despite different names*

```diff
@@ -140,14 +140,17 @@
 
         // Attach toggle code event
         this.add_menu_item('Toggle Code View', () => this.toggle_code());
 
         // Apply the body
         (this.element.querySelector('div.nbtools-body') as HTMLElement).innerHTML = this.body;
 
+        // Add the metadata flag
+        this.update_metadata();
+
         // Attach the disconnected cover
         this.element.appendChild(new DOMParser().parseFromString(this.disconnected, "text/html")
             .querySelector('body > :first-child') as HTMLElement);
         this.attach_connect_event();
         this.disconnected_sync_fix();
 
         // Set the element
@@ -203,14 +206,31 @@
         const button = this.element.querySelector('button.nbtools-connect') as HTMLElement;
         button.addEventListener("click", () => {
             // Run all cells with disconnected nbtools widgets
             ContextManager.context().run_tool_cells();
         });
     }
 
+    /**
+     * Update the cell metadata with the nbtools flag
+     */
+    update_metadata() {
+        if (!ContextManager.notebook_tracker) return;
+        if (!ContextManager.notebook_tracker.currentWidget) return;
+
+        const cells = ContextManager.notebook_tracker.currentWidget.content.widgets;
+        for (let i = 0; i < cells.length; i++) {
+            const execution_area:HTMLElement = cells[i].node.querySelector('.lm-Widget.p-Widget.jp-InputPrompt.jp-InputArea-prompt');
+            if (execution_area.innerText.includes('[*]')) {
+                ContextManager.context().make_tool_cell(cells[i]);
+                return;
+            }
+        }
+    }
+
     disconnected_sync_fix() {
         // Fix a bug that can occur when a disconnected widget and a connected widget are somehow rendered in the same cell
         setTimeout(() => {
             const cell = this.element.closest('.jp-Cell, .cell');
             if (!cell) return;  // No cell found, bug cannot occur
 
             // Do both connected and disconnected widgets appear in the cell?
```

### Comparing `nbtools-23.5.0/src/context.ts` & `nbtools-23.7.0/src/context.ts`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,22 @@
 
     /**
      * Execute all cells with nbtools widgets in the current notebook
      */
     abstract run_tool_cells():void;
 
     /**
+     * Sets whether this is a nbtools widget cell
+     *
+     * @param cell
+     * @param is_widget_cell
+     */
+    abstract make_tool_cell(cell: any, is_widget_cell?:boolean):void
+
+    /**
      * Returns a path to the active notebook, relative to the top directory
      */
     abstract notebook_path():string
 
     /**
      * Determines if the given cell contains a notebook tool widget
      *
@@ -219,14 +227,18 @@
     /**
      * Determines if the given cell contains a notebook tool widget
      *
      * @param cell
      * @returns boolean
      */
     is_tool_cell(cell:any):boolean {
+        // Check for nbtools metadata
+        if (cell.model.metadata.get('nbtools')) return true;
+
+        // Check for an existing disconnected nbtools widget
         const dom_node = cell.node || cell.element;
         if (!!dom_node) return !!dom_node.querySelector('.nbtools');
         else return false;
     }
 
     /**
      * Path to the default GenePattern logo
@@ -322,14 +334,25 @@
     create_comm(current:any, name:string, callback:Function):any {
         const kernel = current.context.sessionContext.session.kernel;
         const comm = kernel.createComm(name);
         comm.onMsg = callback;
         comm.open({});  // Open the comm
         return comm
     }
+
+    /**
+     * Sets whether this is a nbtools widget cell
+     *
+     * @param cell
+     * @param is_widget_cell
+     */
+    make_tool_cell(cell: any, is_widget_cell=true): void {
+        if (is_widget_cell) cell.model.metadata.set('nbtools', {'force_display': true});
+        else cell.model.metadata.clear();
+    }
 }
 
 /**
  * Context handler for the classic Jupyter Notebook
  */
 class NotebookContext extends Context {
     /**
@@ -391,14 +414,26 @@
     is_tool_cell(cell:any):boolean {
         const dom_node = cell.node || cell.element;
         if (!!dom_node) return !!dom_node.find('.nbtools').length;
         else return false;
     }
 
     /**
+     * Sets whether this is a nbtools widget cell
+     *
+     * @param cell
+     * @param is_widget_cell
+     */
+    make_tool_cell(cell: any, is_widget_cell=true): void {
+        // TODO: Test in Jupyter Notebook
+        if (is_widget_cell) cell.metadata.set('nbtools', {'force_display': true});
+        else cell.metadata.clear();
+    }
+
+    /**
      * Path to the default GenePattern logo
      */
     default_logo():string {
         return  this.base_path() + require("../style/g2nb_logo.png").default;
     }
 
     /**
@@ -510,14 +545,26 @@
     base_path():string {
         const body = document.querySelector('body');
         if (!body) return ''; // If there is no body, unable to get path
         return body.getAttribute('data-base-url') + 'nbextensions/nbtools/';
     }
 
     /**
+     * Sets whether this is a nbtools widget cell
+     *
+     * @param cell
+     * @param is_widget_cell
+     */
+    make_tool_cell(cell: any, is_widget_cell=true): void {
+        // TODO: Test in embedded context
+        if (is_widget_cell) cell.metadata.set('nbtools', {'force_display': true});
+        else cell.metadata.clear();
+    }
+
+    /**
      * Determines if the given cell contains a notebook tool widget
      *
      * @param cell
      * @returns boolean
      */
     is_tool_cell(cell:any):boolean {
         const dom_node = cell.node || cell.element;
```

### Comparing `nbtools-23.5.0/src/dataregistry.ts` & `nbtools-23.7.0/src/dataregistry.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/src/extension.ts` & `nbtools-23.7.0/src/extension.ts`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,11 @@
 // Entry point for the notebook bundle containing custom model definitions.
 //
 // Setup notebook base URL
 //
 // Some static assets may be required by the custom widget javascript. The base
 // url for the notebook is not known at build time and is therefore computed
 // dynamically.
-import { ToolRegistry } from "./registry";
 
 (window as any).__webpack_public_path__ = document.querySelector('body')!.getAttribute('data-base-url') + 'nbextensions/nbtools';
 
-export * from './index';
-
-(window as any).NBToolManager = new ToolRegistry();
+export * from './index';
```

### Comparing `nbtools-23.5.0/src/plugin.ts` & `nbtools-23.7.0/src/plugin.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import { Application, IPlugin } from '@lumino/application';
 import { Widget } from '@lumino/widgets';
 import { IJupyterWidgetRegistry } from '@jupyter-widgets/base';
+import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { MODULE_NAME, MODULE_VERSION } from './version';
 import * as base_exports from './basewidget';
 import * as uioutput_exports from './uioutput';
 import * as uibuilder_exports from './uibuilder';
 import { IMainMenu } from '@jupyterlab/mainmenu';
 import { ToolBrowser, Toolbox } from "./toolbox";
 import { IToolRegistry, ToolRegistry } from "./registry";
@@ -21,38 +22,42 @@
 
 /**
  * The nbtools plugin.
  */
 const nbtools_plugin: IPlugin<Application<Widget>, [IToolRegistry, IDataRegistry]> = ({
     id: EXTENSION_ID,
     provides: [IToolRegistry, IDataRegistry],
-    requires: [IJupyterWidgetRegistry],
+    requires: [IJupyterWidgetRegistry, ISettingRegistry],
     optional: [IMainMenu, ILayoutRestorer, ILabShell, INotebookTracker],
     activate: activate_widget_extension,
     autoStart: true
 } as unknown) as IPlugin<Application<Widget>, [IToolRegistry, IDataRegistry]>;
 
 export default nbtools_plugin;
 
 
 /**
  * Activate the widget extension.
  */
-function activate_widget_extension(app: Application<Widget>,
+async function activate_widget_extension(app: Application<Widget>,
                                    widget_registry: IJupyterWidgetRegistry,
+                                   settings: ISettingRegistry,
                                    mainmenu: IMainMenu|null,
                                    restorer: ILayoutRestorer|null,
                                    shell: ILabShell|null,
-                                   notebook_tracker: INotebookTracker|null): [IToolRegistry, IDataRegistry] {
+                                   notebook_tracker: INotebookTracker|null): Promise<[IToolRegistry, IDataRegistry]> {
 
     // Initialize the ContextManager
     init_context(app as JupyterFrontEnd, notebook_tracker);
 
+    // Initialize settings
+    const setting_dict = await init_settings(settings);
+
     // Create the tool and data registries
-    const tool_registry = new ToolRegistry();
+    const tool_registry = new ToolRegistry(setting_dict);
     const data_registry = new DataRegistry();
 
     // Add items to the help menu
     add_help_links(app as JupyterFrontEnd, mainmenu);
 
     // Add keyboard shortcuts
     add_keyboard_shortcuts(app as JupyterFrontEnd, tool_registry);
@@ -70,14 +75,21 @@
     // Register the plugin as loaded
     usage_tracker('labextension_load', location.protocol + '//' + location.host + location.pathname);
 
     // Return the tool registry so that it is provided to other extensions
     return [tool_registry, data_registry];
 }
 
+async function init_settings(settings:ISettingRegistry) {
+    let setting = null;
+    try { setting = await settings.load(EXTENSION_ID); }
+    catch { console.log('Unable to load nbtools settings'); }
+    return { force_render: setting ? setting.get('force_render').composite as boolean : true };
+}
+
 function init_context(app:JupyterFrontEnd, notebook_tracker: INotebookTracker|null) {
     ContextManager.jupyter_app = app;
     ContextManager.notebook_tracker = notebook_tracker;
     ContextManager.context();
     (window as any).ContextManager = ContextManager;  // Left in for development purposes
 }
```

### Comparing `nbtools-23.5.0/src/registry.ts` & `nbtools-23.7.0/src/registry.ts`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     private _update_callbacks:Array<Function> = []; // Functions to call when an update happens
     kernel_tool_cache:any = {};                     // Keep a cache of kernels to registered tools
     kernel_import_cache:any = {};                   // Keep a cache of whether nbtools has been imported
 
     /**
      * Initialize the ToolRegistry and connect event handlers
      */
-    constructor() {
+    constructor(setting_dict:any) {
         // Lazily assign the tool registry to the context
         if (!ContextManager.tool_registry) ContextManager.tool_registry = this;
 
         ContextManager.context().notebook_focus((current_widget:any) => {
             // Current notebook hasn't changed, no need to do anything, return
             if (this.current === current_widget) return;
 
@@ -32,14 +32,24 @@
             if (!(this.current instanceof NotebookPanel) && ContextManager.is_lab()) return;
 
             // Initialize the comm
             this.init_comm();
 
             // Load the default tools
             this.import_default_tools();
+
+            // Ensure rendering of tool cells
+            if (setting_dict.force_render) this.ensure_rendering();
+        });
+    }
+
+    ensure_rendering() {
+        ContextManager.context().kernel_ready(this.current, () => {
+            if (!this.current) return;                              // Return if no notebook is selected
+            ContextManager.context().run_tool_cells();
         });
     }
 
     import_default_tools() {
         ContextManager.context().kernel_changed(this.current, () => {
             ContextManager.context().execute_code(this.current, 'from nbtools import import_defaults\nimport_defaults()');
         });
```

### Comparing `nbtools-23.5.0/src/toolbox.ts` & `nbtools-23.7.0/src/toolbox.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/src/uibuilder.ts` & `nbtools-23.7.0/src/uibuilder.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/src/uioutput.ts` & `nbtools-23.7.0/src/uioutput.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/src/utils.ts` & `nbtools-23.7.0/src/utils.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/style/basewidget.css` & `nbtools-23.7.0/style/basewidget.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/style/g2nb_logo.png` & `nbtools-23.7.0/style/g2nb_logo.png`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/style/icon.svg` & `nbtools-23.7.0/style/icon.svg`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/style/toolbox.css` & `nbtools-23.7.0/style/toolbox.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/style/uibuilder.css` & `nbtools-23.7.0/style/uibuilder.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/style/uioutput.css` & `nbtools-23.7.0/style/uioutput.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/tests/karma.conf.js` & `nbtools-23.7.0/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/tests/src/index.spec.ts` & `nbtools-23.7.0/tests/src/index.spec.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/tests/src/utils.spec.ts` & `nbtools-23.7.0/tests/src/utils.spec.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/.gitignore` & `nbtools-23.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/LICENSE.txt` & `nbtools-23.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/README.md` & `nbtools-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.5.0/pyproject.toml` & `nbtools-23.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
     "hatchling",
     "ipywidgets>7,<9",
-    "jupyterlab>=3.4",
+    "jupyterlab>=3.4,<4",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "nbtools"
 description = "Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike."
 readme = "README.md"
@@ -30,17 +30,17 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
     "ipyuploads",
     "ipywidgets>7,<9",
-    "jupyterlab>=3.4",
+    "jupyterlab>=3.4,<4",
 ]
-version = "23.5.0"
+version = "23.7.0"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.urls]
 Homepage = "https://github.com/g2nb/nbtools"
 
@@ -91,15 +91,15 @@
     "jlpm",
 ]
 
 [tool.tbump]
 github_url = "https://github.com/g2nb/nbtools"
 
 [tool.tbump.version]
-current = "23.5.0"
+current = "23.7.0"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?P<pre>((a|b|rc)\d+))?
```

### Comparing `nbtools-23.5.0/PKG-INFO` & `nbtools-23.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbtools
-Version: 23.5.0
+Version: 23.7.0
 Summary: Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike.
 Project-URL: Homepage, https://github.com/g2nb/nbtools
 Author-email: Thorin Tabor <tmtabor@cloud.ucsd.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Regents of the University of California & Broad Institute
         All rights reserved.
@@ -44,15 +44,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Requires-Dist: ipyuploads
 Requires-Dist: ipywidgets<9,>7
-Requires-Dist: jupyterlab>=3.4
+Requires-Dist: jupyterlab<4,>=3.4
 Description-Content-Type: text/markdown
 
 # nbtools for JupyterLab
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/g2nb/nbtools/lab?urlpath=lab)
 [![Build Status](https://travis-ci.org/g2nb/nbtools.svg?branch=lab)](https://travis-ci.org/genepattern/nbtools)
 [![Documentation Status](https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat)](https://gpnotebook-website-docs.readthedocs.io/en/latest/)
```

