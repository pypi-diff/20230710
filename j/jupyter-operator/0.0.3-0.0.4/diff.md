# Comparing `tmp/jupyter_operator-0.0.3.tar.gz` & `tmp/jupyter_operator-0.0.4.tar.gz`

## Comparing `jupyter_operator-0.0.3.tar` & `jupyter_operator-0.0.4.tar`

### file list

```diff
@@ -1,156 +1,156 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.dockerignore
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.eslintrc.js
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/CHANGELOG.md
--rwxr-xr-x   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/Dockerfile
--rwxr-xr-x   0        0        0     2440 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/Makefile
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/babel.config.js
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/conftest.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/install.json
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jest-playwright.config.js
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jest.config.js
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/setup.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/tsconfig copy.json
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/tsconfig.json
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/webpack.config.js
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.github/workflows/update-integration-tests.yml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.yarn/cache/.gitignore
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/README.md
--rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/config/README.md
--rwxr-xr-x   0        0        0     2371 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/config/jupyter_server_config.py
--rwxr-xr-x   0        0        0      303 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/README.md
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/ping.ipynb
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/test.ipynb
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/tmp.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/untitled.txt
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/subfolder-1/README.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/subfolder-1/test-1.ipynb
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/subfolder-1/subfolder-1-1/README.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/subfolder-2/README.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/subfolder-2/test-2.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/notebooks/subfolder-2/untitled.txt
--rwxr-xr-x   0        0        0      299 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/sh/README.md
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/sh/kill.sh
--rwxr-xr-x   0        0        0      619 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/dev/sh/start-jupyter-server.sh
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/LICENSE
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/Makefile
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/README.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/babel.config.js
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/docusaurus.config.js
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/environment.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/package.json
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/sidebars.js
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/docs/index.mdx
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/docs/setup/_category_.yml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/docs/setup/example_1.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/docs/setup/example_2.md
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/docs/setup/index.mdx
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/src/components/HomepageFeatures.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/src/components/HomepageFeatures.module.css
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/src/components/HomepageProducts.js
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/src/components/HomepageProducts.module.css
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/src/css/custom.css
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/src/pages/index.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/src/pages/markdown-page.md
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/src/pages/testimonials.tsx
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/static/img/favicon.ico
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/static/img/feature_1.svg
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/static/img/feature_2.svg
--rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/static/img/feature_3.svg
--rw-r--r--   0        0        0    15652 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/static/img/product_1.svg
--rw-r--r--   0        0        0    38790 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/static/img/product_2.svg
--rw-r--r--   0        0        0   103421 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/static/img/product_3.svg
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/static/img/datalayer/logo.png
--rwxr-xr-x   0        0        0     4924 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/docs/static/img/datalayer/logo.svg
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter-config/nb-config/jupyter_operator.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter-config/server-config/jupyter_operator.json
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/__main__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/_version.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/handlers.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/serverapplication.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/echo/__init__.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/echo/handler.py
--rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/build_log.json
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/package.json
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/schemas/@datalayer/jupyter-operator/package.json.orig
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/schemas/@datalayer/jupyter-operator/plugin.json
--rw-r--r--   0        0        0   906895 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/icons_react_index_esm_js.65493c25dd332aaf6b10.js
--rw-r--r--   0        0        0   845273 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/icons_react_index_esm_js.65493c25dd332aaf6b10.js.map
--rw-r--r--   0        0        0    55466 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/lib_index_js.f1f1be6235af06d15eb7.js
--rw-r--r--   0        0        0    25404 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/lib_index_js.f1f1be6235af06d15eb7.js.map
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/node_modules_hoist-non-react-statics_node_modules_react-is_index_js.7dd2af76c437d73cf272.js
--rw-r--r--   0        0        0     8961 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/node_modules_hoist-non-react-statics_node_modules_react-is_index_js.7dd2af76c437d73cf272.js.map
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/node_modules_react-is_index_js.8b062d16b8062ce2fe10.js
--rw-r--r--   0        0        0     9469 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/node_modules_react-is_index_js.8b062d16b8062ce2fe10.js.map
--rw-r--r--   0        0        0    38566 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/remoteEntry.3f20dfa3004465e59e7c.js
--rw-r--r--   0        0        0    37628 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/remoteEntry.3f20dfa3004465e59e7c.js.map
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/style.js
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/style_index_js.dd18ecca1126e33640ca.js
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/style_index_js.dd18ecca1126e33640ca.js.map
--rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f9144d1e6376fc430401.js
--rw-r--r--   0        0        0    13765 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f9144d1e6376fc430401.js.map
--rw-r--r--   0        0        0   474438 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_octicons-react_dist_index_esm_js.d49632050843d4efdeb6.js
--rw-r--r--   0        0        0   474037 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_octicons-react_dist_index_esm_js.d49632050843d4efdeb6.js.map
--rw-r--r--   0        0        0   666736 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc.9b3033f129d542a8c633.js
--rw-r--r--   0        0        0   624890 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc.9b3033f129d542a8c633.js.map
--rw-r--r--   0        0        0   686741 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_index_js.51541663eab422a16e66.js
--rw-r--r--   0        0        0   545333 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_index_js.51541663eab422a16e66.js.map
--rw-r--r--   0        0        0    42895 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_react_jsx-runtime_js.3bdd7b655f56f956a0aa.js
--rw-r--r--   0        0        0    50279 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_react_jsx-runtime_js.3bdd7b655f56f956a0aa.js.map
--rw-r--r--   0        0        0    65900 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.7ff043caf94499075eba.js
--rw-r--r--   0        0        0   152979 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.7ff043caf94499075eba.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/pong/__init__.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/pong/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/proxy/__init__.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/proxy/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/relay/__init__.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/relay/handler.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/static/README.md
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/templates/index.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/tests/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/jupyter_operator/tests/test_handlers.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/node_modules/@eslint/eslintrc/node_modules/ajv/scripts/.eslintrc.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/node_modules/eslint/node_modules/ajv/scripts/.eslintrc.yml
--rwxr-xr-x   0        0        0      764 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/public/index.html
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/schema/plugin.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/Example.tsx
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/emptyshim.js
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/handler.ts
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/index.ts
--rwxr-xr-x   0        0        0      334 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/typings.d.ts
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/widget.tsx
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/ws.ts
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/__tests__/browser.spec.ts
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/__tests__/datalayer.spec.ts
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/component/MockComponent.tsx
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/component/MockTab1.tsx
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/component/MockTab2.tsx
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/component/MockTab3.tsx
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/component/MockTab4.tsx
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/src/component/MockTab5.tsx
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/style/index.js
--rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/style/svg/icon.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/ui-tests/tests/datalayer.spec.ts
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/LICENSE
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/README.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/hatch_build.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 jupyter_operator-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.dockerignore
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.eslintrc.js
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/CHANGELOG.md
+-rwxr-xr-x   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/Dockerfile
+-rwxr-xr-x   0        0        0     2440 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/Makefile
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/babel.config.js
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/conftest.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/install.json
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jest-playwright.config.js
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jest.config.js
+-rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/setup.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/tsconfig copy.json
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/tsconfig.json
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/webpack.config.js
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.github/workflows/update-integration-tests.yml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.yarn/cache/.gitignore
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/README.md
+-rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/config/README.md
+-rwxr-xr-x   0        0        0     2371 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/config/jupyter_server_config.py
+-rwxr-xr-x   0        0        0      303 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/README.md
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/ping.ipynb
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/test.ipynb
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/tmp.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/untitled.txt
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/subfolder-1/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/subfolder-1/test-1.ipynb
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/subfolder-1/subfolder-1-1/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/subfolder-2/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/subfolder-2/test-2.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/notebooks/subfolder-2/untitled.txt
+-rwxr-xr-x   0        0        0      299 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/sh/README.md
+-rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/sh/kill.sh
+-rwxr-xr-x   0        0        0      619 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/dev/sh/start-jupyter-server.sh
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/LICENSE
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/Makefile
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/README.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/babel.config.js
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/docusaurus.config.js
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/environment.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/package.json
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/sidebars.js
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/docs/index.mdx
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/docs/setup/_category_.yml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/docs/setup/example_1.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/docs/setup/example_2.md
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/docs/setup/index.mdx
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/src/components/HomepageFeatures.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/src/components/HomepageFeatures.module.css
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/src/components/HomepageProducts.js
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/src/components/HomepageProducts.module.css
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/src/css/custom.css
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/src/pages/index.js
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/src/pages/markdown-page.md
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/src/pages/testimonials.tsx
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/static/img/feature_1.svg
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/static/img/feature_2.svg
+-rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/static/img/feature_3.svg
+-rw-r--r--   0        0        0    15652 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/static/img/product_1.svg
+-rw-r--r--   0        0        0    38790 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/static/img/product_2.svg
+-rw-r--r--   0        0        0   103421 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/static/img/product_3.svg
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/static/img/datalayer/logo.png
+-rwxr-xr-x   0        0        0     4924 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/docs/static/img/datalayer/logo.svg
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter-config/nb-config/jupyter_operator.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter-config/server-config/jupyter_operator.json
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/__init__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/__main__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/_version.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/handlers.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/serverapplication.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/echo/__init__.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/echo/handler.py
+-rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/build_log.json
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/package.json
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/schemas/@datalayer/jupyter-operator/package.json.orig
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/schemas/@datalayer/jupyter-operator/plugin.json
+-rw-r--r--   0        0        0   906895 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/icons_react_index_esm_js.65493c25dd332aaf6b10.js
+-rw-r--r--   0        0        0   845273 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/icons_react_index_esm_js.65493c25dd332aaf6b10.js.map
+-rw-r--r--   0        0        0    55466 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/lib_index_js.f1f1be6235af06d15eb7.js
+-rw-r--r--   0        0        0    25404 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/lib_index_js.f1f1be6235af06d15eb7.js.map
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/node_modules_hoist-non-react-statics_node_modules_react-is_index_js.7dd2af76c437d73cf272.js
+-rw-r--r--   0        0        0     8961 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/node_modules_hoist-non-react-statics_node_modules_react-is_index_js.7dd2af76c437d73cf272.js.map
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/node_modules_react-is_index_js.8b062d16b8062ce2fe10.js
+-rw-r--r--   0        0        0     9469 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/node_modules_react-is_index_js.8b062d16b8062ce2fe10.js.map
+-rw-r--r--   0        0        0    38566 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/remoteEntry.3f20dfa3004465e59e7c.js
+-rw-r--r--   0        0        0    37628 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/remoteEntry.3f20dfa3004465e59e7c.js.map
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/style.js
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/style_index_js.dd18ecca1126e33640ca.js
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/style_index_js.dd18ecca1126e33640ca.js.map
+-rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f9144d1e6376fc430401.js
+-rw-r--r--   0        0        0    13765 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f9144d1e6376fc430401.js.map
+-rw-r--r--   0        0        0   474438 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_octicons-react_dist_index_esm_js.d49632050843d4efdeb6.js
+-rw-r--r--   0        0        0   474037 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_octicons-react_dist_index_esm_js.d49632050843d4efdeb6.js.map
+-rw-r--r--   0        0        0   666736 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc.9b3033f129d542a8c633.js
+-rw-r--r--   0        0        0   624890 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc.9b3033f129d542a8c633.js.map
+-rw-r--r--   0        0        0   686741 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_index_js.51541663eab422a16e66.js
+-rw-r--r--   0        0        0   545333 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_index_js.51541663eab422a16e66.js.map
+-rw-r--r--   0        0        0    42895 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_react_jsx-runtime_js.3bdd7b655f56f956a0aa.js
+-rw-r--r--   0        0        0    50279 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_react_jsx-runtime_js.3bdd7b655f56f956a0aa.js.map
+-rw-r--r--   0        0        0    65900 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.7ff043caf94499075eba.js
+-rw-r--r--   0        0        0   152979 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.7ff043caf94499075eba.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/pong/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/pong/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/proxy/__init__.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/proxy/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/relay/__init__.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/relay/handler.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/static/README.md
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/templates/index.html
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/tests/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/jupyter_operator/tests/test_handlers.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/node_modules/@eslint/eslintrc/node_modules/ajv/scripts/.eslintrc.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/node_modules/eslint/node_modules/ajv/scripts/.eslintrc.yml
+-rwxr-xr-x   0        0        0      764 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/public/index.html
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/schema/plugin.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/Example.tsx
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/emptyshim.js
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/handler.ts
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/index.ts
+-rwxr-xr-x   0        0        0      334 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/typings.d.ts
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/widget.tsx
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/ws.ts
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/__tests__/browser.spec.ts
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/__tests__/datalayer.spec.ts
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/component/MockComponent.tsx
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/component/MockTab1.tsx
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/component/MockTab2.tsx
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/component/MockTab3.tsx
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/component/MockTab4.tsx
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/src/component/MockTab5.tsx
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/style/index.js
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/style/svg/icon.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/ui-tests/tests/datalayer.spec.ts
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/LICENSE
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/README.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/hatch_build.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 jupyter_operator-0.0.4/PKG-INFO
```

### Comparing `jupyter_operator-0.0.3/.eslintrc.js` & `jupyter_operator-0.0.4/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/Makefile` & `jupyter_operator-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/RELEASE.md` & `jupyter_operator-0.0.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jest.config.js` & `jupyter_operator-0.0.4/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/package.json` & `jupyter_operator-0.0.4/jupyter_operator/labextension/schemas/@datalayer/jupyter-operator/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/tsconfig copy.json` & `jupyter_operator-0.0.4/tsconfig copy.json`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/tsconfig.json` & `jupyter_operator-0.0.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/webpack.config.js` & `jupyter_operator-0.0.4/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/.github/workflows/build.yml` & `jupyter_operator-0.0.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/.github/workflows/check-release.yml` & `jupyter_operator-0.0.4/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/.github/workflows/update-integration-tests.yml` & `jupyter_operator-0.0.4/.github/workflows/update-integration-tests.yml`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/dev/config/jupyter_server_config.py` & `jupyter_operator-0.0.4/dev/config/jupyter_server_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/dev/notebooks/test.ipynb` & `jupyter_operator-0.0.4/dev/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/dev/notebooks/tmp.ipynb` & `jupyter_operator-0.0.4/dev/notebooks/tmp.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/dev/notebooks/subfolder-1/test-1.ipynb` & `jupyter_operator-0.0.4/dev/notebooks/subfolder-1/test-1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb` & `jupyter_operator-0.0.4/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/dev/notebooks/subfolder-2/test-2.ipynb` & `jupyter_operator-0.0.4/dev/notebooks/subfolder-2/test-2.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/dev/sh/start-jupyter-server.sh` & `jupyter_operator-0.0.4/dev/sh/start-jupyter-server.sh`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/LICENSE` & `jupyter_operator-0.0.4/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/Makefile` & `jupyter_operator-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/README.md` & `jupyter_operator-0.0.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/docusaurus.config.js` & `jupyter_operator-0.0.4/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/package.json` & `jupyter_operator-0.0.4/docs/package.json`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/sidebars.js` & `jupyter_operator-0.0.4/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/src/components/HomepageFeatures.js` & `jupyter_operator-0.0.4/docs/src/components/HomepageFeatures.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/src/components/HomepageProducts.js` & `jupyter_operator-0.0.4/docs/src/components/HomepageProducts.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/src/css/custom.css` & `jupyter_operator-0.0.4/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/src/pages/index.js` & `jupyter_operator-0.0.4/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/src/pages/index.module.css` & `jupyter_operator-0.0.4/docs/src/pages/index.module.css`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/static/img/favicon.ico` & `jupyter_operator-0.0.4/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/static/img/feature_1.svg` & `jupyter_operator-0.0.4/docs/static/img/feature_1.svg`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/static/img/feature_2.svg` & `jupyter_operator-0.0.4/docs/static/img/feature_2.svg`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/static/img/feature_3.svg` & `jupyter_operator-0.0.4/docs/static/img/feature_3.svg`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/static/img/product_1.svg` & `jupyter_operator-0.0.4/docs/static/img/product_1.svg`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/static/img/product_2.svg` & `jupyter_operator-0.0.4/docs/static/img/product_2.svg`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/static/img/product_3.svg` & `jupyter_operator-0.0.4/docs/static/img/product_3.svg`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/docs/static/img/datalayer/logo.svg` & `jupyter_operator-0.0.4/docs/static/img/datalayer/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/handlers.py` & `jupyter_operator-0.0.4/jupyter_operator/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/serverapplication.py` & `jupyter_operator-0.0.4/jupyter_operator/serverapplication.py`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/echo/handler.py` & `jupyter_operator-0.0.4/jupyter_operator/echo/handler.py`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/build_log.json` & `jupyter_operator-0.0.4/jupyter_operator/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/package.json` & `jupyter_operator-0.0.4/jupyter_operator/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/schemas/@datalayer/jupyter-operator/package.json.orig` & `jupyter_operator-0.0.4/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809523%*

 * *Differences: {"'description'": "'🪐 🥷 Jupyter Operator.'", "'version'": "'0.0.4'"}*

```diff
@@ -17,15 +17,15 @@
         "@primer/react": "36.0.0-rc.8ab77098",
         "@primer/react-brand": "0.20.0",
         "react": "18.2.0",
         "react-dom": "18.2.0",
         "react-is": "18.2.0",
         "styled-components": "5.3.10"
     },
-    "description": "\u039e Jupyter Operator.",
+    "description": "\ud83e\ude90 \ud83e\udd77 Jupyter Operator.",
     "devDependencies": {
         "@babel/core": "7.21.0",
         "@babel/plugin-proposal-class-properties": "7.18.6",
         "@babel/preset-env": "7.20.2",
         "@babel/preset-react": "7.18.6",
         "@babel/preset-typescript": "7.21.0",
         "@jupyterlab/builder": "4.0.0",
@@ -150,9 +150,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/icons_react_index_esm_js.65493c25dd332aaf6b10.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/icons_react_index_esm_js.65493c25dd332aaf6b10.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/icons_react_index_esm_js.65493c25dd332aaf6b10.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/icons_react_index_esm_js.65493c25dd332aaf6b10.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/lib_index_js.f1f1be6235af06d15eb7.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/lib_index_js.f1f1be6235af06d15eb7.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/lib_index_js.f1f1be6235af06d15eb7.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/lib_index_js.f1f1be6235af06d15eb7.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/node_modules_hoist-non-react-statics_node_modules_react-is_index_js.7dd2af76c437d73cf272.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/node_modules_hoist-non-react-statics_node_modules_react-is_index_js.7dd2af76c437d73cf272.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/node_modules_hoist-non-react-statics_node_modules_react-is_index_js.7dd2af76c437d73cf272.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/node_modules_hoist-non-react-statics_node_modules_react-is_index_js.7dd2af76c437d73cf272.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/node_modules_react-is_index_js.8b062d16b8062ce2fe10.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/node_modules_react-is_index_js.8b062d16b8062ce2fe10.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/node_modules_react-is_index_js.8b062d16b8062ce2fe10.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/node_modules_react-is_index_js.8b062d16b8062ce2fe10.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/remoteEntry.3f20dfa3004465e59e7c.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/remoteEntry.3f20dfa3004465e59e7c.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/remoteEntry.3f20dfa3004465e59e7c.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/remoteEntry.3f20dfa3004465e59e7c.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/style_index_js.dd18ecca1126e33640ca.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/style_index_js.dd18ecca1126e33640ca.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/style_index_js.dd18ecca1126e33640ca.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/style_index_js.dd18ecca1126e33640ca.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f9144d1e6376fc430401.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f9144d1e6376fc430401.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f9144d1e6376fc430401.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f9144d1e6376fc430401.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_octicons-react_dist_index_esm_js.d49632050843d4efdeb6.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_octicons-react_dist_index_esm_js.d49632050843d4efdeb6.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_octicons-react_dist_index_esm_js.d49632050843d4efdeb6.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_octicons-react_dist_index_esm_js.d49632050843d4efdeb6.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc.9b3033f129d542a8c633.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc.9b3033f129d542a8c633.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc.9b3033f129d542a8c633.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_TreeView_TreeView_js-node_modules_primer_react_lib--75b6cc.9b3033f129d542a8c633.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_index_js.51541663eab422a16e66.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_index_js.51541663eab422a16e66.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_index_js.51541663eab422a16e66.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_primer_react_lib-esm_index_js.51541663eab422a16e66.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_react_jsx-runtime_js.3bdd7b655f56f956a0aa.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_react_jsx-runtime_js.3bdd7b655f56f956a0aa.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_react_jsx-runtime_js.3bdd7b655f56f956a0aa.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_react_jsx-runtime_js.3bdd7b655f56f956a0aa.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.7ff043caf94499075eba.js` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.7ff043caf94499075eba.js`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.7ff043caf94499075eba.js.map` & `jupyter_operator-0.0.4/jupyter_operator/labextension/static/vendors-node_modules_styled-components_dist_styled-components_browser_esm_js.7ff043caf94499075eba.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/pong/handler.py` & `jupyter_operator-0.0.4/jupyter_operator/pong/handler.py`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/proxy/handler.py` & `jupyter_operator-0.0.4/jupyter_operator/proxy/handler.py`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/relay/handler.py` & `jupyter_operator-0.0.4/jupyter_operator/relay/handler.py`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/jupyter_operator/templates/index.html` & `jupyter_operator-0.0.4/jupyter_operator/templates/index.html`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/public/index.html` & `jupyter_operator-0.0.4/public/index.html`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/src/handler.ts` & `jupyter_operator-0.0.4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/src/index.ts` & `jupyter_operator-0.0.4/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/src/__tests__/browser.spec.ts` & `jupyter_operator-0.0.4/src/__tests__/browser.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/src/component/MockComponent.tsx` & `jupyter_operator-0.0.4/src/component/MockComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/src/component/MockTab1.tsx` & `jupyter_operator-0.0.4/src/component/MockTab1.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/src/component/MockTab2.tsx` & `jupyter_operator-0.0.4/src/component/MockTab2.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/src/component/MockTab3.tsx` & `jupyter_operator-0.0.4/src/component/MockTab3.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/src/component/MockTab4.tsx` & `jupyter_operator-0.0.4/src/component/MockTab4.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/src/component/MockTab5.tsx` & `jupyter_operator-0.0.4/src/component/MockTab5.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/style/svg/icon.svg` & `jupyter_operator-0.0.4/style/svg/icon.svg`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/ui-tests/README.md` & `jupyter_operator-0.0.4/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/ui-tests/jupyter_server_test_config.py` & `jupyter_operator-0.0.4/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/ui-tests/tests/datalayer.spec.ts` & `jupyter_operator-0.0.4/ui-tests/tests/datalayer.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/.gitignore` & `jupyter_operator-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/LICENSE` & `jupyter_operator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/hatch_build.py` & `jupyter_operator-0.0.4/hatch_build.py`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/pyproject.toml` & `jupyter_operator-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_operator-0.0.3/PKG-INFO` & `jupyter_operator-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jupyter_operator
-Version: 0.0.3
-Summary: Ξ Jupyter Operator.
+Version: 0.0.4
+Summary: 🪐 🥷 Jupyter Operator.
 Project-URL: Homepage, https://github.com/datalayer/jupyter-operator
 Project-URL: Bug Tracker, https://github.com/datalayer/jupyter-operator/issues
 Project-URL: Repository, https://github.com/datalayer/jupyter-operator.git
 Author-email: Datalayer <info@datalayer.io>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Datalayer
```

