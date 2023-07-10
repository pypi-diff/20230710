# Comparing `tmp/glue_jupyterlab-0.2.0.tar.gz` & `tmp/glue_jupyterlab-0.3.0.tar.gz`

## Comparing `glue_jupyterlab-0.2.0.tar` & `glue_jupyterlab-0.3.0.tar`

### file list

```diff
@@ -1,117 +1,125 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/.eslintignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/.eslintrc.js
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/.prettierrc
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/babel.config.js
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/conftest.py
--rw-r--r--   0        0        0   234868 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue-jupyterlab.png
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/install.json
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/jest.config.js
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/setup.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/tsconfig.test.json
--rw-r--r--   0        0        0   396413 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/yarn.lock
--rw-r--r--   0        0        0    39007 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/examples/session.glu
--rw-r--r--   0        0        0    28233 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/examples/session2.glu
--rw-r--r--   0        0        0    29798 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/examples/session3.glu
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/_version.py
--rw-r--r--   0        0        0    18115 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/glue_session.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/glue_utils.py
--rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/glue_ydoc.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/handlers.py
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/package.json
--rw-r--r--   0        0        0    25504 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/185.0cff412fc25ed146b7c1.js
--rw-r--r--   0        0        0    19398 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/398.bd2742885fb1b39ca17d.js
--rw-r--r--   0        0        0    54485 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/797.6a3ff8bb4f69a7056ffc.js
--rw-r--r--   0        0        0    73234 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/929.a029633e30c80e22d788.js
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/929.a029633e30c80e22d788.js.LICENSE.txt
--rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/remoteEntry.7851783ebd012eb24a52.js
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/style.js
--rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/tests/__init__.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/tests/conftest.py
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/tests/test_glue_session.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/tests/test_handlers.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/glue_jupyterlab/tests/test_ydoc.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/jupyter-config/nb-config/glue_jupyterlab.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/jupyter-config/server-config/glue_jupyterlab.json
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/commands.ts
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/index.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/svg.d.ts
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/token.ts
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/tools.ts
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/types.ts
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/yWidget.ts
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/__tests__/glue_lab.spec.ts
--rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/common/tabPanel.ts
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/document/default.json
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/document/docModel.ts
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/document/modelFactory.ts
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/document/plugin.ts
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/document/sharedModel.ts
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/document/tracker.ts
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/document/widgetFactory.ts
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/leftPanel/header.tsx
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/leftPanel/model.ts
--rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/leftPanel/plugin.ts
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/leftPanel/widget.ts
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/leftPanel/config/configPanel.ts
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/leftPanel/config/configWidget.ts
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/leftPanel/config/configWidgetModel.ts
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/leftPanel/data/dataPanel.ts
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/leftPanel/data/datasetsWidget.tsx
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/leftPanel/data/subsetsWidget.ts
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/linkPanel/linkEditor.ts
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/linkPanel/linkEditorWidget.ts
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/linkPanel/model.ts
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/linkPanel/types.ts
--rw-r--r--   0        0        0    22739 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/linkPanel/widgets/linking.tsx
--rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/linkPanel/widgets/summary.tsx
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/schemas/glue.schema.json
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/schemas/link.schema.json
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/schemas/data/attributes.schema.json
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/schemas/data/dataset.schema.json
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/schemas/viewers/1dprofile.schema.json
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/schemas/viewers/2dscatter.schema.json
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/schemas/viewers/3dscatter.schema.json
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/schemas/viewers/histogram.schema.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/schemas/viewers/image.schema.json
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/viewPanel/glueDocumentWidget.ts
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/viewPanel/gridStackItem.ts
--rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/viewPanel/sessionWidget.ts
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/viewPanel/tabLayout.ts
--rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/src/viewPanel/tabView.ts
--rw-r--r--   0        0        0    10313 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/style/base.css
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/style/index.css
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/style/index.js
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/style/icons/glue-icon.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/README.md
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/package.json
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148428 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts
--rw-r--r--   0        0        0    91016 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/add-data-data-added-linux.png
--rw-r--r--   0        0        0   112084 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/add-data-file-browser-linux.png
--rw-r--r--   0        0        0    62625 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/add-data-viewer-created-linux.png
--rw-r--r--   0        0        0    54384 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/add-data-viewer-selection-linux.png
--rw-r--r--   0        0        0   103662 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/control-panel-linux.png
--rw-r--r--   0        0        0    48352 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/control-panel-switch-tab-linux.png
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/histogram-linked-selection-linux.png
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/histogram-no-selection-linux.png
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/histogram-selection-linux.png
--rw-r--r--   0        0        0    80938 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/link-editor-linux.png
--rw-r--r--   0        0        0    79767 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/session-tab1-linux.png
--rw-r--r--   0        0        0    39876 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/session-tab2-linux.png
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/LICENSE
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/README.md
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 glue_jupyterlab-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/.eslintignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/.eslintrc.js
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/.prettierrc
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/.yarnrc.yml
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/babel.config.js
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/conftest.py
+-rw-r--r--   0        0        0   234868 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue-jupyterlab.png
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/install.json
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/jest.config.js
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/setup.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/tsconfig.test.json
+-rw-r--r--   0        0        0   387687 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/yarn.lock
+-rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/docs/Makefile
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/docs/doc-requirements.txt
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/docs/environment.yml
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0   741801 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/docs/source/glue-jupyterlab.gif
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0    39007 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/examples/session.glu
+-rw-r--r--   0        0        0    28233 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/examples/session2.glu
+-rw-r--r--   0        0        0    29798 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/examples/session3.glu
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/_version.py
+-rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/glue_session.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/glue_utils.py
+-rw-r--r--   0        0        0     9871 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/glue_ydoc.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/handlers.py
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/package.json
+-rw-r--r--   0        0        0    25504 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/185.0cff412fc25ed146b7c1.js
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/722.e912ef3d95501737406e.js
+-rw-r--r--   0        0        0    56068 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/797.6775a9c675159fcc67ec.js
+-rw-r--r--   0        0        0    73234 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/929.a029633e30c80e22d788.js
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/929.a029633e30c80e22d788.js.LICENSE.txt
+-rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/remoteEntry.5c208e7340414ff77977.js
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/style.js
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/tests/__init__.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/tests/conftest.py
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/tests/test_glue_session.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/tests/test_handlers.py
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/glue_jupyterlab/tests/test_ydoc.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/jupyter-config/nb-config/glue_jupyterlab.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/jupyter-config/server-config/glue_jupyterlab.json
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/commands.ts
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/index.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/svg.d.ts
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/token.ts
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/tools.ts
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/types.ts
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/yWidget.ts
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/__tests__/glue_lab.spec.ts
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/common/tabPanel.ts
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/document/default.json
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/document/docModel.ts
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/document/modelFactory.ts
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/document/plugin.ts
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/document/sharedModel.ts
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/document/tracker.ts
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/document/widgetFactory.ts
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/leftPanel/header.tsx
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/leftPanel/model.ts
+-rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/leftPanel/plugin.ts
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/leftPanel/widget.ts
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/leftPanel/config/configPanel.ts
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/leftPanel/config/configWidget.ts
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/leftPanel/config/configWidgetModel.ts
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/leftPanel/data/dataPanel.ts
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/leftPanel/data/datasetsWidget.tsx
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/leftPanel/data/subsetsWidget.ts
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/linkPanel/linkEditor.ts
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/linkPanel/linkEditorWidget.ts
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/linkPanel/model.ts
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/linkPanel/types.ts
+-rw-r--r--   0        0        0    22739 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/linkPanel/widgets/linking.tsx
+-rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/linkPanel/widgets/summary.tsx
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/schemas/glue.schema.json
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/schemas/link.schema.json
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/schemas/data/attributes.schema.json
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/schemas/data/dataset.schema.json
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/schemas/viewers/1dprofile.schema.json
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/schemas/viewers/2dscatter.schema.json
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/schemas/viewers/3dscatter.schema.json
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/schemas/viewers/histogram.schema.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/schemas/viewers/image.schema.json
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/viewPanel/glueDocumentWidget.ts
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/viewPanel/gridStackItem.ts
+-rw-r--r--   0        0        0     8206 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/viewPanel/sessionWidget.ts
+-rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/viewPanel/tabLayout.ts
+-rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/src/viewPanel/tabView.ts
+-rw-r--r--   0        0        0    10313 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/style/base.css
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/style/index.css
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/style/index.js
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/style/icons/glue-icon.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/README.md
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/package.json
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148428 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts
+-rw-r--r--   0        0        0    91016 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/add-data-data-added-linux.png
+-rw-r--r--   0        0        0   112084 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/add-data-file-browser-linux.png
+-rw-r--r--   0        0        0    62625 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/add-data-viewer-created-linux.png
+-rw-r--r--   0        0        0    54384 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/add-data-viewer-selection-linux.png
+-rw-r--r--   0        0        0   103662 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/control-panel-linux.png
+-rw-r--r--   0        0        0    48352 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/control-panel-switch-tab-linux.png
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/histogram-linked-selection-linux.png
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/histogram-no-selection-linux.png
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/histogram-selection-linux.png
+-rw-r--r--   0        0        0    80938 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/link-editor-linux.png
+-rw-r--r--   0        0        0    79767 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/session-tab1-linux.png
+-rw-r--r--   0        0        0    39876 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/session-tab2-linux.png
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/README.md
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 glue_jupyterlab-0.3.0/PKG-INFO
```

### Comparing `glue_jupyterlab-0.2.0/.eslintrc.js` & `glue_jupyterlab-0.3.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/.pre-commit-config.yaml` & `glue_jupyterlab-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/RELEASE.md` & `glue_jupyterlab-0.3.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/glue-jupyterlab.png` & `glue_jupyterlab-0.3.0/glue-jupyterlab.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/jest.config.js` & `glue_jupyterlab-0.3.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/package.json` & `glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.97%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.5c208e7340414ff77977.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -55,14 +55,19 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/QuantStack/glue-jupyterlab",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.5c208e7340414ff77977.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "glue-jupyterlab"
                 },
                 "managers": [
                     "pip"
@@ -128,9 +133,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `glue_jupyterlab-0.2.0/tsconfig.json` & `glue_jupyterlab-0.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/yarn.lock` & `glue_jupyterlab-0.3.0/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # This file is generated by running "yarn install" inside your project.
 # Manual changes might be lost - proceed with caution!
 
 __metadata:
   version: 6
   cacheKey: 8
 
+"@aashutoshrathi/word-wrap@npm:^1.2.3":
+  version: 1.2.6
+  resolution: "@aashutoshrathi/word-wrap@npm:1.2.6"
+  checksum: ada901b9e7c680d190f1d012c84217ce0063d8f5c5a7725bb91ec3c5ed99bb7572680eb2d2938a531ccbaec39a95422fcd8a6b4a13110c7d98dd75402f66a0cd
+  languageName: node
+  linkType: hard
+
 "@ampproject/remapping@npm:^2.2.0":
   version: 2.2.1
   resolution: "@ampproject/remapping@npm:2.2.1"
   dependencies:
     "@jridgewell/gen-mapping": ^0.3.0
     "@jridgewell/trace-mapping": ^0.3.9
   checksum: 03c04fd526acc64a1f4df22651186f3e5ef0a9d6d6530ce4482ec9841269cf7a11dbb8af79237c282d721c5312024ff17529cd72cc4768c11e999b58e2302079
@@ -41,53 +48,53 @@
   resolution: "@babel/code-frame@npm:7.22.5"
   dependencies:
     "@babel/highlight": ^7.22.5
   checksum: cfe804f518f53faaf9a1d3e0f9f74127ab9a004912c3a16fda07fb6a633393ecb9918a053cb71804204c1b7ec3d49e1699604715e2cfb0c9f7bc4933d324ebb6
   languageName: node
   linkType: hard
 
-"@babel/compat-data@npm:^7.17.7, @babel/compat-data@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/compat-data@npm:7.22.5"
-  checksum: eb1a47ebf79ae268b4a16903e977be52629339806e248455eb9973897c503a04b701f36a9de64e19750d6e081d0561e77a514c8dc470babbeba59ae94298ed18
+"@babel/compat-data@npm:^7.22.5, @babel/compat-data@npm:^7.22.6":
+  version: 7.22.6
+  resolution: "@babel/compat-data@npm:7.22.6"
+  checksum: b88631143a2ebdb75e5bac47984e950983294f1739c2133f32569c6f2fcee85f83634bb6cf4378afb44fa8eb7877d11e48811d1e6a52afa161f82276ffdc3fb4
   languageName: node
   linkType: hard
 
 "@babel/core@npm:^7.10.2, @babel/core@npm:^7.11.6, @babel/core@npm:^7.12.3":
-  version: 7.22.5
-  resolution: "@babel/core@npm:7.22.5"
+  version: 7.22.8
+  resolution: "@babel/core@npm:7.22.8"
   dependencies:
     "@ampproject/remapping": ^2.2.0
     "@babel/code-frame": ^7.22.5
-    "@babel/generator": ^7.22.5
-    "@babel/helper-compilation-targets": ^7.22.5
+    "@babel/generator": ^7.22.7
+    "@babel/helper-compilation-targets": ^7.22.6
     "@babel/helper-module-transforms": ^7.22.5
-    "@babel/helpers": ^7.22.5
-    "@babel/parser": ^7.22.5
+    "@babel/helpers": ^7.22.6
+    "@babel/parser": ^7.22.7
     "@babel/template": ^7.22.5
-    "@babel/traverse": ^7.22.5
+    "@babel/traverse": ^7.22.8
     "@babel/types": ^7.22.5
+    "@nicolo-ribaudo/semver-v6": ^6.3.3
     convert-source-map: ^1.7.0
     debug: ^4.1.0
     gensync: ^1.0.0-beta.2
     json5: ^2.2.2
-    semver: ^6.3.0
-  checksum: 173ae426958c90c7bbd7de622c6f13fcab8aef0fac3f138e2d47bc466d1cd1f86f71ca82ae0acb9032fd8794abed8efb56fea55c031396337eaec0d673b69d56
+  checksum: 75ed701c14ad17070382ae1dd166f7534b31f2c71e00995a5f261ee2398ee96335b0736573b8ff24ab6e3e6f5814ee2a48fa11ab90fabcd3dfc70ea87c5f30a6
   languageName: node
   linkType: hard
 
-"@babel/generator@npm:^7.22.5, @babel/generator@npm:^7.7.2":
-  version: 7.22.5
-  resolution: "@babel/generator@npm:7.22.5"
+"@babel/generator@npm:^7.22.7, @babel/generator@npm:^7.7.2":
+  version: 7.22.7
+  resolution: "@babel/generator@npm:7.22.7"
   dependencies:
     "@babel/types": ^7.22.5
     "@jridgewell/gen-mapping": ^0.3.2
     "@jridgewell/trace-mapping": ^0.3.17
     jsesc: ^2.5.1
-  checksum: efa64da70ca88fe69f05520cf5feed6eba6d30a85d32237671488cc355fdc379fe2c3246382a861d49574c4c2f82a317584f8811e95eb024e365faff3232b49d
+  checksum: cee15558888bdf5564e19cfaf95101b2910fa425f30cc1a25ac9b8621bd62b63544eb1b36ad89c80b5e41915699219f78712cab128d1f7e3da6a21fbf4143927
   languageName: node
   linkType: hard
 
 "@babel/helper-annotate-as-pure@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-annotate-as-pure@npm:7.22.5"
   dependencies:
@@ -101,74 +108,73 @@
   resolution: "@babel/helper-builder-binary-assignment-operator-visitor@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: d753acac62399fc6dd354cf1b9441bde0c331c2fe792a4c14904c5e5eafc3cac79478f6aa038e8a51c1148b0af6710a2e619855e4b5d54497ac972eaffed5884
   languageName: node
   linkType: hard
 
-"@babel/helper-compilation-targets@npm:^7.17.7, @babel/helper-compilation-targets@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-compilation-targets@npm:7.22.5"
+"@babel/helper-compilation-targets@npm:^7.22.5, @babel/helper-compilation-targets@npm:^7.22.6":
+  version: 7.22.6
+  resolution: "@babel/helper-compilation-targets@npm:7.22.6"
   dependencies:
-    "@babel/compat-data": ^7.22.5
+    "@babel/compat-data": ^7.22.6
     "@babel/helper-validator-option": ^7.22.5
-    browserslist: ^4.21.3
+    "@nicolo-ribaudo/semver-v6": ^6.3.3
+    browserslist: ^4.21.9
     lru-cache: ^5.1.1
-    semver: ^6.3.0
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: a479460615acffa0f4fd0a29b740eafb53a93694265207d23a6038ccd18d183a382cacca515e77b7c9b042c3ba80b0aca0da5f1f62215140e81660d2cf721b68
+  checksum: c7788c48099c4f0edf2adeb367a941a930d39ed7453140ceb10d7114c4091922adf56d3cdd832050fd4501f25e872886390629042ddd365d3bce2ecad69ed394
   languageName: node
   linkType: hard
 
 "@babel/helper-create-class-features-plugin@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-create-class-features-plugin@npm:7.22.5"
+  version: 7.22.6
+  resolution: "@babel/helper-create-class-features-plugin@npm:7.22.6"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
     "@babel/helper-environment-visitor": ^7.22.5
     "@babel/helper-function-name": ^7.22.5
     "@babel/helper-member-expression-to-functions": ^7.22.5
     "@babel/helper-optimise-call-expression": ^7.22.5
     "@babel/helper-replace-supers": ^7.22.5
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
-    "@babel/helper-split-export-declaration": ^7.22.5
-    semver: ^6.3.0
+    "@babel/helper-split-export-declaration": ^7.22.6
+    "@nicolo-ribaudo/semver-v6": ^6.3.3
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: f1e91deae06dbee6dd956c0346bca600adfbc7955427795d9d8825f0439a3c3290c789ba2b4a02a1cdf6c1a1bd163dfa16d3d5e96b02a8efb639d2a774e88ed9
+  checksum: 10412e8a509a607cde6137288d3f12b1f91acd374e29e6dd6a277b67217e9f4c932a0acd89eeda837c8432916df775a8af6321aeb8d8b131ccdbf7688208dda1
   languageName: node
   linkType: hard
 
 "@babel/helper-create-regexp-features-plugin@npm:^7.18.6, @babel/helper-create-regexp-features-plugin@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-create-regexp-features-plugin@npm:7.22.5"
+  version: 7.22.6
+  resolution: "@babel/helper-create-regexp-features-plugin@npm:7.22.6"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
+    "@nicolo-ribaudo/semver-v6": ^6.3.3
     regexpu-core: ^5.3.1
-    semver: ^6.3.0
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 94932145beeb1f91856be25fea8de30b4b81b63fbc7c5a207ed97a5ddc34cd1e9b04041ed28bd24ec09cdcfbb62e8d66f820e4fe864672afe0aa2f357c784e11
+  checksum: a26df33a08bc603177cc4a59d067740bd7156c05d6b519bf28cdd2f07f653be2a7f37d8dd93b85e620f20ad90da1b8dbe4d7c6cf5262e67f713904e811b7ffd2
   languageName: node
   linkType: hard
 
-"@babel/helper-define-polyfill-provider@npm:^0.4.0":
-  version: 0.4.0
-  resolution: "@babel/helper-define-polyfill-provider@npm:0.4.0"
+"@babel/helper-define-polyfill-provider@npm:^0.4.1":
+  version: 0.4.1
+  resolution: "@babel/helper-define-polyfill-provider@npm:0.4.1"
   dependencies:
-    "@babel/helper-compilation-targets": ^7.17.7
-    "@babel/helper-plugin-utils": ^7.16.7
+    "@babel/helper-compilation-targets": ^7.22.6
+    "@babel/helper-plugin-utils": ^7.22.5
     debug: ^4.1.1
     lodash.debounce: ^4.0.8
     resolve: ^1.14.2
-    semver: ^6.1.2
   peerDependencies:
     "@babel/core": ^7.4.0-0
-  checksum: 5dca4c5e78457c5ced366bea601efa4e8c69bf5d53b0fe540283897575c49b1b88191c8ef062110de9046e886703ed3270fcda3a87f0886cdbb549204d3ff63f
+  checksum: 712b440cdd343ac7c4617225f91b0a9db5a7b1c96356b720e011af64ad6c4da9c66889f8d2962a0a2ae2e4ccb6a9b4a210c4a3c8c8ff103846b3d93b61bc6634
   languageName: node
   linkType: hard
 
 "@babel/helper-environment-visitor@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-environment-visitor@npm:7.22.5"
   checksum: 248532077d732a34cd0844eb7b078ff917c3a8ec81a7f133593f71a860a582f05b60f818dc5049c2212e5baa12289c27889a4b81d56ef409b4863db49646c4b1
@@ -233,15 +239,15 @@
   resolution: "@babel/helper-optimise-call-expression@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: c70ef6cc6b6ed32eeeec4482127e8be5451d0e5282d5495d5d569d39eb04d7f1d66ec99b327f45d1d5842a9ad8c22d48567e93fc502003a47de78d122e355f7c
   languageName: node
   linkType: hard
 
-"@babel/helper-plugin-utils@npm:^7.0.0, @babel/helper-plugin-utils@npm:^7.10.4, @babel/helper-plugin-utils@npm:^7.12.13, @babel/helper-plugin-utils@npm:^7.14.5, @babel/helper-plugin-utils@npm:^7.16.7, @babel/helper-plugin-utils@npm:^7.18.6, @babel/helper-plugin-utils@npm:^7.22.5, @babel/helper-plugin-utils@npm:^7.8.0, @babel/helper-plugin-utils@npm:^7.8.3":
+"@babel/helper-plugin-utils@npm:^7.0.0, @babel/helper-plugin-utils@npm:^7.10.4, @babel/helper-plugin-utils@npm:^7.12.13, @babel/helper-plugin-utils@npm:^7.14.5, @babel/helper-plugin-utils@npm:^7.18.6, @babel/helper-plugin-utils@npm:^7.22.5, @babel/helper-plugin-utils@npm:^7.8.0, @babel/helper-plugin-utils@npm:^7.8.3":
   version: 7.22.5
   resolution: "@babel/helper-plugin-utils@npm:7.22.5"
   checksum: c0fc7227076b6041acd2f0e818145d2e8c41968cc52fb5ca70eed48e21b8fe6dd88a0a91cbddf4951e33647336eb5ae184747ca706817ca3bef5e9e905151ff5
   languageName: node
   linkType: hard
 
 "@babel/helper-remap-async-to-generator@npm:^7.22.5":
@@ -286,20 +292,20 @@
   resolution: "@babel/helper-skip-transparent-expression-wrappers@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: 1012ef2295eb12dc073f2b9edf3425661e9b8432a3387e62a8bc27c42963f1f216ab3124228015c748770b2257b4f1fda882ca8fa34c0bf485e929ae5bc45244
   languageName: node
   linkType: hard
 
-"@babel/helper-split-export-declaration@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-split-export-declaration@npm:7.22.5"
+"@babel/helper-split-export-declaration@npm:^7.22.5, @babel/helper-split-export-declaration@npm:^7.22.6":
+  version: 7.22.6
+  resolution: "@babel/helper-split-export-declaration@npm:7.22.6"
   dependencies:
     "@babel/types": ^7.22.5
-  checksum: d10e05a02f49c1f7c578cea63d2ac55356501bbf58856d97ac9bfde4957faee21ae97c7f566aa309e38a256eef58b58e5b670a7f568b362c00e93dfffe072650
+  checksum: e141cace583b19d9195f9c2b8e17a3ae913b7ee9b8120246d0f9ca349ca6f03cb2c001fd5ec57488c544347c0bb584afec66c936511e447fd20a360e591ac921
   languageName: node
   linkType: hard
 
 "@babel/helper-string-parser@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-string-parser@npm:7.22.5"
   checksum: 836851ca5ec813077bbb303acc992d75a360267aa3b5de7134d220411c852a6f17de7c0d0b8c8dcc0f567f67874c00f4528672b2a4f1bc978a3ada64c8c78467
@@ -328,42 +334,42 @@
     "@babel/template": ^7.22.5
     "@babel/traverse": ^7.22.5
     "@babel/types": ^7.22.5
   checksum: a4ba2d7577ad3ce92fadaa341ffce3b0e4b389808099b07c80847f9be0852f4b42344612bc1b3d1b796ffb75be56d5957c5c56a1734f6aee5ccbb7cd9ab12691
   languageName: node
   linkType: hard
 
-"@babel/helpers@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helpers@npm:7.22.5"
+"@babel/helpers@npm:^7.22.6":
+  version: 7.22.6
+  resolution: "@babel/helpers@npm:7.22.6"
   dependencies:
     "@babel/template": ^7.22.5
-    "@babel/traverse": ^7.22.5
+    "@babel/traverse": ^7.22.6
     "@babel/types": ^7.22.5
-  checksum: a96e785029dff72f171190943df895ab0f76e17bf3881efd630bc5fae91215042d1c2e9ed730e8e4adf4da6f28b24bd1f54ed93b90ffbca34c197351872a084e
+  checksum: 5c1f33241fe7bf7709868c2105134a0a86dca26a0fbd508af10a89312b1f77ca38ebae43e50be3b208613c5eacca1559618af4ca236f0abc55d294800faeff30
   languageName: node
   linkType: hard
 
 "@babel/highlight@npm:^7.10.4, @babel/highlight@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/highlight@npm:7.22.5"
   dependencies:
     "@babel/helper-validator-identifier": ^7.22.5
     chalk: ^2.0.0
     js-tokens: ^4.0.0
   checksum: f61ae6de6ee0ea8d9b5bcf2a532faec5ab0a1dc0f7c640e5047fc61630a0edb88b18d8c92eb06566d30da7a27db841aca11820ecd3ebe9ce514c9350fbed39c4
   languageName: node
   linkType: hard
 
-"@babel/parser@npm:^7.1.0, @babel/parser@npm:^7.14.7, @babel/parser@npm:^7.20.7, @babel/parser@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/parser@npm:7.22.5"
+"@babel/parser@npm:^7.1.0, @babel/parser@npm:^7.14.7, @babel/parser@npm:^7.20.7, @babel/parser@npm:^7.22.5, @babel/parser@npm:^7.22.7":
+  version: 7.22.7
+  resolution: "@babel/parser@npm:7.22.7"
   bin:
     parser: ./bin/babel-parser.js
-  checksum: 470ebba516417ce8683b36e2eddd56dcfecb32c54b9bb507e28eb76b30d1c3e618fd0cfeee1f64d8357c2254514e1a19e32885cfb4e73149f4ae875436a6d59c
+  checksum: 02209ddbd445831ee8bf966fdf7c29d189ed4b14343a68eb2479d940e7e3846340d7cc6bd654a5f3d87d19dc84f49f50a58cf9363bee249dc5409ff3ba3dab54
   languageName: node
   linkType: hard
 
 "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:7.22.5"
   dependencies:
@@ -647,25 +653,25 @@
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 35abb6c57062802c7ce8bd96b2ef2883e3124370c688bbd67609f7d2453802fb73944df8808f893b6c67de978eb2bcf87bbfe325e46d6f39b5fcb09ece11d01a
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-async-generator-functions@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-async-generator-functions@npm:7.22.5"
+"@babel/plugin-transform-async-generator-functions@npm:^7.22.7":
+  version: 7.22.7
+  resolution: "@babel/plugin-transform-async-generator-functions@npm:7.22.7"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.5
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-remap-async-to-generator": ^7.22.5
     "@babel/plugin-syntax-async-generators": ^7.8.4
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 32890b69ec5627eb46ee8e084bddc6b98d85b66cae5e015f3a23924611a759789d2ff836406605f5293b5c2bad306b20cb1f5b7a46ed549b07bfec634bcd31f9
+  checksum: 57cd2cce3fb696dadf00e88f168683df69e900b92dadeae07429243c43bc21d5ccdc0c2db61cf5c37bd0fbd893fc455466bef6babe4aa5b79d9cb8ba89f40ae7
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-async-to-generator@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/plugin-transform-async-to-generator@npm:7.22.5"
   dependencies:
@@ -721,30 +727,30 @@
     "@babel/plugin-syntax-class-static-block": ^7.14.5
   peerDependencies:
     "@babel/core": ^7.12.0
   checksum: bc48b92dbaf625a14f2bf62382384eef01e0515802426841636ae9146e27395d068c7a8a45e9e15699491b0a01d990f38f179cbc9dc89274a393f85648772f12
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-classes@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-classes@npm:7.22.5"
+"@babel/plugin-transform-classes@npm:^7.22.6":
+  version: 7.22.6
+  resolution: "@babel/plugin-transform-classes@npm:7.22.6"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
-    "@babel/helper-compilation-targets": ^7.22.5
+    "@babel/helper-compilation-targets": ^7.22.6
     "@babel/helper-environment-visitor": ^7.22.5
     "@babel/helper-function-name": ^7.22.5
     "@babel/helper-optimise-call-expression": ^7.22.5
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-replace-supers": ^7.22.5
-    "@babel/helper-split-export-declaration": ^7.22.5
+    "@babel/helper-split-export-declaration": ^7.22.6
     globals: ^11.1.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 124b1b79180524cc9d08155cecde92c7f2ab0db02cbe0f8befa187ef3c7320909ce1a6d6daf5ce73e8330f9b40cf9991f424c6e572b8dddc1f14e2758fa80d20
+  checksum: 8380e855c01033dbc7460d9acfbc1fc37c880350fa798c2de8c594ef818ade0e4c96173ec72f05f2a4549d8d37135e18cb62548352d51557b45a0fb4388d2f3f
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-computed-properties@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/plugin-transform-computed-properties@npm:7.22.5"
   dependencies:
@@ -1029,24 +1035,24 @@
     "@babel/plugin-syntax-optional-catch-binding": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: b0e8b4233ff06b5c9d285257f49c5bd441f883189b24282e6200f9ebdf5db29aeeebbffae57fbbcd5df9f4387b3e66e5d322aaae5652a78e89685ddbae46bbd1
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-optional-chaining@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-optional-chaining@npm:7.22.5"
+"@babel/plugin-transform-optional-chaining@npm:^7.22.5, @babel/plugin-transform-optional-chaining@npm:^7.22.6":
+  version: 7.22.6
+  resolution: "@babel/plugin-transform-optional-chaining@npm:7.22.6"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
     "@babel/plugin-syntax-optional-chaining": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 57b9c05fb22ae881b8a334b184fc6ee966661ed5d1eb4eed8c2fb9a12e68150d90b229efcb1aa777e246999830844fee06d7365f8bb4bb262fdcd23876ff3ea2
+  checksum: 9713f7920ed04090c149fc5ec024dd1638e8b97aa4ae3753b93072d84103b8de380afb96d6cf03e53b285420db4f705f3ac13149c6fd54f322b61dc19e33c54f
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-parameters@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/plugin-transform-parameters@npm:7.22.5"
   dependencies:
@@ -1217,19 +1223,19 @@
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: c042070f980b139547f8b0179efbc049ac5930abec7fc26ed7a41d89a048d8ab17d362200e204b6f71c3c20d6991a0e74415e1a412a49adc8131c2a40c04822e
   languageName: node
   linkType: hard
 
 "@babel/preset-env@npm:^7.10.2":
-  version: 7.22.5
-  resolution: "@babel/preset-env@npm:7.22.5"
+  version: 7.22.7
+  resolution: "@babel/preset-env@npm:7.22.7"
   dependencies:
-    "@babel/compat-data": ^7.22.5
-    "@babel/helper-compilation-targets": ^7.22.5
+    "@babel/compat-data": ^7.22.6
+    "@babel/helper-compilation-targets": ^7.22.6
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-validator-option": ^7.22.5
     "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression": ^7.22.5
     "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining": ^7.22.5
     "@babel/plugin-proposal-private-property-in-object": 7.21.0-placeholder-for-preset-env.2
     "@babel/plugin-syntax-async-generators": ^7.8.4
     "@babel/plugin-syntax-class-properties": ^7.12.13
@@ -1246,21 +1252,21 @@
     "@babel/plugin-syntax-object-rest-spread": ^7.8.3
     "@babel/plugin-syntax-optional-catch-binding": ^7.8.3
     "@babel/plugin-syntax-optional-chaining": ^7.8.3
     "@babel/plugin-syntax-private-property-in-object": ^7.14.5
     "@babel/plugin-syntax-top-level-await": ^7.14.5
     "@babel/plugin-syntax-unicode-sets-regex": ^7.18.6
     "@babel/plugin-transform-arrow-functions": ^7.22.5
-    "@babel/plugin-transform-async-generator-functions": ^7.22.5
+    "@babel/plugin-transform-async-generator-functions": ^7.22.7
     "@babel/plugin-transform-async-to-generator": ^7.22.5
     "@babel/plugin-transform-block-scoped-functions": ^7.22.5
     "@babel/plugin-transform-block-scoping": ^7.22.5
     "@babel/plugin-transform-class-properties": ^7.22.5
     "@babel/plugin-transform-class-static-block": ^7.22.5
-    "@babel/plugin-transform-classes": ^7.22.5
+    "@babel/plugin-transform-classes": ^7.22.6
     "@babel/plugin-transform-computed-properties": ^7.22.5
     "@babel/plugin-transform-destructuring": ^7.22.5
     "@babel/plugin-transform-dotall-regex": ^7.22.5
     "@babel/plugin-transform-duplicate-keys": ^7.22.5
     "@babel/plugin-transform-dynamic-import": ^7.22.5
     "@babel/plugin-transform-exponentiation-operator": ^7.22.5
     "@babel/plugin-transform-export-namespace-from": ^7.22.5
@@ -1277,15 +1283,15 @@
     "@babel/plugin-transform-named-capturing-groups-regex": ^7.22.5
     "@babel/plugin-transform-new-target": ^7.22.5
     "@babel/plugin-transform-nullish-coalescing-operator": ^7.22.5
     "@babel/plugin-transform-numeric-separator": ^7.22.5
     "@babel/plugin-transform-object-rest-spread": ^7.22.5
     "@babel/plugin-transform-object-super": ^7.22.5
     "@babel/plugin-transform-optional-catch-binding": ^7.22.5
-    "@babel/plugin-transform-optional-chaining": ^7.22.5
+    "@babel/plugin-transform-optional-chaining": ^7.22.6
     "@babel/plugin-transform-parameters": ^7.22.5
     "@babel/plugin-transform-private-methods": ^7.22.5
     "@babel/plugin-transform-private-property-in-object": ^7.22.5
     "@babel/plugin-transform-property-literals": ^7.22.5
     "@babel/plugin-transform-regenerator": ^7.22.5
     "@babel/plugin-transform-reserved-words": ^7.22.5
     "@babel/plugin-transform-shorthand-properties": ^7.22.5
@@ -1295,22 +1301,22 @@
     "@babel/plugin-transform-typeof-symbol": ^7.22.5
     "@babel/plugin-transform-unicode-escapes": ^7.22.5
     "@babel/plugin-transform-unicode-property-regex": ^7.22.5
     "@babel/plugin-transform-unicode-regex": ^7.22.5
     "@babel/plugin-transform-unicode-sets-regex": ^7.22.5
     "@babel/preset-modules": ^0.1.5
     "@babel/types": ^7.22.5
-    babel-plugin-polyfill-corejs2: ^0.4.3
-    babel-plugin-polyfill-corejs3: ^0.8.1
-    babel-plugin-polyfill-regenerator: ^0.5.0
-    core-js-compat: ^3.30.2
-    semver: ^6.3.0
+    "@nicolo-ribaudo/semver-v6": ^6.3.3
+    babel-plugin-polyfill-corejs2: ^0.4.4
+    babel-plugin-polyfill-corejs3: ^0.8.2
+    babel-plugin-polyfill-regenerator: ^0.5.1
+    core-js-compat: ^3.31.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 6d9d09010ababef2ab48c8830770b2a8f45d6cce51db0924a98b0d95a5b1248a99ee07ee61cb5446d8b05b562db99a8af30b3ed194546419fb9b2889b8fd1ed3
+  checksum: eabde70e450dd54f57997b0f92317f69f268e9a1f85b13f5ef5540d2a38cfae5620bd8e48ddffb547c55fbd2f17673276e6eb9411d6b5fb82e3422faf44cb6cf
   languageName: node
   linkType: hard
 
 "@babel/preset-modules@npm:^0.1.5":
   version: 0.1.5
   resolution: "@babel/preset-modules@npm:0.1.5"
   dependencies:
@@ -1329,48 +1335,48 @@
   version: 0.8.0
   resolution: "@babel/regjsgen@npm:0.8.0"
   checksum: 89c338fee774770e5a487382170711014d49a68eb281e74f2b5eac88f38300a4ad545516a7786a8dd5702e9cf009c94c2f582d200f077ac5decd74c56b973730
   languageName: node
   linkType: hard
 
 "@babel/runtime@npm:^7.8.4":
-  version: 7.22.5
-  resolution: "@babel/runtime@npm:7.22.5"
+  version: 7.22.6
+  resolution: "@babel/runtime@npm:7.22.6"
   dependencies:
     regenerator-runtime: ^0.13.11
-  checksum: 12a50b7de2531beef38840d17af50c55a094253697600cee255311222390c68eed704829308d4fd305e1b3dfbce113272e428e9d9d45b1730e0fede997eaceb1
+  checksum: e585338287c4514a713babf4fdb8fc2a67adcebab3e7723a739fc62c79cfda875b314c90fd25f827afb150d781af97bc16c85bfdbfa2889f06053879a1ddb597
   languageName: node
   linkType: hard
 
 "@babel/template@npm:^7.22.5, @babel/template@npm:^7.3.3":
   version: 7.22.5
   resolution: "@babel/template@npm:7.22.5"
   dependencies:
     "@babel/code-frame": ^7.22.5
     "@babel/parser": ^7.22.5
     "@babel/types": ^7.22.5
   checksum: c5746410164039aca61829cdb42e9a55410f43cace6f51ca443313f3d0bdfa9a5a330d0b0df73dc17ef885c72104234ae05efede37c1cc8a72dc9f93425977a3
   languageName: node
   linkType: hard
 
-"@babel/traverse@npm:^7.22.5, @babel/traverse@npm:^7.7.2":
-  version: 7.22.5
-  resolution: "@babel/traverse@npm:7.22.5"
+"@babel/traverse@npm:^7.22.5, @babel/traverse@npm:^7.22.6, @babel/traverse@npm:^7.22.8":
+  version: 7.22.8
+  resolution: "@babel/traverse@npm:7.22.8"
   dependencies:
     "@babel/code-frame": ^7.22.5
-    "@babel/generator": ^7.22.5
+    "@babel/generator": ^7.22.7
     "@babel/helper-environment-visitor": ^7.22.5
     "@babel/helper-function-name": ^7.22.5
     "@babel/helper-hoist-variables": ^7.22.5
-    "@babel/helper-split-export-declaration": ^7.22.5
-    "@babel/parser": ^7.22.5
+    "@babel/helper-split-export-declaration": ^7.22.6
+    "@babel/parser": ^7.22.7
     "@babel/types": ^7.22.5
     debug: ^4.1.0
     globals: ^11.1.0
-  checksum: 560931422dc1761f2df723778dcb4e51ce0d02e560cf2caa49822921578f49189a5a7d053b78a32dca33e59be886a6b2200a6e24d4ae9b5086ca0ba803815694
+  checksum: a381369bc3eedfd13ed5fef7b884657f1c29024ea7388198149f0edc34bd69ce3966e9f40188d15f56490a5e12ba250ccc485f2882b53d41b054fccefb233e33
   languageName: node
   linkType: hard
 
 "@babel/types@npm:^7.0.0, @babel/types@npm:^7.20.7, @babel/types@npm:^7.22.5, @babel/types@npm:^7.3.3, @babel/types@npm:^7.4.4, @babel/types@npm:^7.8.3":
   version: 7.22.5
   resolution: "@babel/types@npm:7.22.5"
   dependencies:
@@ -1598,21 +1604,21 @@
   dependencies:
     "@codemirror/language": ^6.0.0
   checksum: fa5f5477fb9e19267251e2ecd3de8c1a4c2512813555bb60111dce3951f2c3f6080a2985a573b7542534ba1d2c34115f7e39ee23fdf8f6f81db6f8ce447c1efc
   languageName: node
   linkType: hard
 
 "@codemirror/lint@npm:^6.0.0":
-  version: 6.3.0
-  resolution: "@codemirror/lint@npm:6.3.0"
+  version: 6.4.0
+  resolution: "@codemirror/lint@npm:6.4.0"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: 4ac907c1a4b5d69e44dcf214ece17050a6175ff5fae517e41118e34b3245d963fc671e7a021bff6a3efddf8c13f688f5f88f06907b9820f91ac52a8426525716
+  checksum: ba15f7dd87afbceafaa0b68f94b0d53727e4aacca7a81a4ed3278706df5787fdf18cd3f0d807a136f902b2fc2296bf3490462fd543d1d4ced17a0d8c171820fd
   languageName: node
   linkType: hard
 
 "@codemirror/search@npm:^6.3.0":
   version: 6.5.0
   resolution: "@codemirror/search@npm:6.5.0"
   dependencies:
@@ -1627,21 +1633,21 @@
   version: 6.2.1
   resolution: "@codemirror/state@npm:6.2.1"
   checksum: d12a321d0471b264b9d3259042bff913a8b939e8d28d408ff452004538a71ca9d5329df3f8a1d8a9183f5b42a7ef5b200737bcab1065714f5ae8e0a5ba9d59d3
   languageName: node
   linkType: hard
 
 "@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.2.2, @codemirror/view@npm:^6.6.0, @codemirror/view@npm:^6.9.6":
-  version: 6.14.0
-  resolution: "@codemirror/view@npm:6.14.0"
+  version: 6.14.1
+  resolution: "@codemirror/view@npm:6.14.1"
   dependencies:
     "@codemirror/state": ^6.1.4
     style-mod: ^4.0.0
     w3c-keyname: ^2.2.4
-  checksum: f8fbb8e8cf1bc23de8cd64b1e645112d13f72cd2f1609fb9047d616908c2189ff518b89f21484371e7a37ba1804288452558e96488791f0c850f62b8e28dc163
+  checksum: 19114ee05b3795ebe07a69cf00c36e8351b3500ce105b8412d90e757d459f71370ead3de852f0fda069041803276e6c38e6f1f943f77e85c9b5c279ab7fa1c4a
   languageName: node
   linkType: hard
 
 "@csstools/selector-specificity@npm:^2.0.2":
   version: 2.2.0
   resolution: "@csstools/selector-specificity@npm:2.2.0"
   peerDependencies:
@@ -1729,241 +1735,241 @@
 "@istanbuljs/schema@npm:^0.1.2":
   version: 0.1.3
   resolution: "@istanbuljs/schema@npm:0.1.3"
   checksum: 5282759d961d61350f33d9118d16bcaed914ebf8061a52f4fa474b2cb08720c9c81d165e13b82f2e5a8a212cc5af482f0c6fc1ac27b9e067e5394c9a6ed186c9
   languageName: node
   linkType: hard
 
-"@jest/console@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/console@npm:29.5.0"
+"@jest/console@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/console@npm:29.6.1"
   dependencies:
-    "@jest/types": ^29.5.0
+    "@jest/types": ^29.6.1
     "@types/node": "*"
     chalk: ^4.0.0
-    jest-message-util: ^29.5.0
-    jest-util: ^29.5.0
+    jest-message-util: ^29.6.1
+    jest-util: ^29.6.1
     slash: ^3.0.0
-  checksum: 9f4f4b8fabd1221361b7f2e92d4a90f5f8c2e2b29077249996ab3c8b7f765175ffee795368f8d6b5b2bb3adb32dc09319f7270c7c787b0d259e624e00e0f64a5
+  checksum: d0ab23a00947bfb4bff8c0a7e5a7afd16519de16dde3fe7e77b9f13e794c6df7043ecf7fcdde66ac0d2b5fb3262e9cab3d92eaf61f89a12d3b8e3602e06a9902
   languageName: node
   linkType: hard
 
-"@jest/core@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/core@npm:29.5.0"
+"@jest/core@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/core@npm:29.6.1"
   dependencies:
-    "@jest/console": ^29.5.0
-    "@jest/reporters": ^29.5.0
-    "@jest/test-result": ^29.5.0
-    "@jest/transform": ^29.5.0
-    "@jest/types": ^29.5.0
+    "@jest/console": ^29.6.1
+    "@jest/reporters": ^29.6.1
+    "@jest/test-result": ^29.6.1
+    "@jest/transform": ^29.6.1
+    "@jest/types": ^29.6.1
     "@types/node": "*"
     ansi-escapes: ^4.2.1
     chalk: ^4.0.0
     ci-info: ^3.2.0
     exit: ^0.1.2
     graceful-fs: ^4.2.9
     jest-changed-files: ^29.5.0
-    jest-config: ^29.5.0
-    jest-haste-map: ^29.5.0
-    jest-message-util: ^29.5.0
+    jest-config: ^29.6.1
+    jest-haste-map: ^29.6.1
+    jest-message-util: ^29.6.1
     jest-regex-util: ^29.4.3
-    jest-resolve: ^29.5.0
-    jest-resolve-dependencies: ^29.5.0
-    jest-runner: ^29.5.0
-    jest-runtime: ^29.5.0
-    jest-snapshot: ^29.5.0
-    jest-util: ^29.5.0
-    jest-validate: ^29.5.0
-    jest-watcher: ^29.5.0
+    jest-resolve: ^29.6.1
+    jest-resolve-dependencies: ^29.6.1
+    jest-runner: ^29.6.1
+    jest-runtime: ^29.6.1
+    jest-snapshot: ^29.6.1
+    jest-util: ^29.6.1
+    jest-validate: ^29.6.1
+    jest-watcher: ^29.6.1
     micromatch: ^4.0.4
-    pretty-format: ^29.5.0
+    pretty-format: ^29.6.1
     slash: ^3.0.0
     strip-ansi: ^6.0.0
   peerDependencies:
     node-notifier: ^8.0.1 || ^9.0.0 || ^10.0.0
   peerDependenciesMeta:
     node-notifier:
       optional: true
-  checksum: 9e8f5243fe82d5a57f3971e1b96f320058df7c315328a3a827263f3b17f64be10c80f4a9c1b1773628b64d2de6d607c70b5b2d5bf13e7f5ad04223e9ef6aac06
+  checksum: 736dcc90c6c58dd9e1d2da122103b851187719ce3b3d4167689c63e68252632cd817712955b52ddaa648eba9c6f98f86cd58677325f0db4185f76899c64d7dac
   languageName: node
   linkType: hard
 
-"@jest/environment@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/environment@npm:29.5.0"
+"@jest/environment@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/environment@npm:29.6.1"
   dependencies:
-    "@jest/fake-timers": ^29.5.0
-    "@jest/types": ^29.5.0
+    "@jest/fake-timers": ^29.6.1
+    "@jest/types": ^29.6.1
     "@types/node": "*"
-    jest-mock: ^29.5.0
-  checksum: 921de6325cd4817dec6685e5ff299b499b6379f3f9cf489b4b13588ee1f3820a0c77b49e6a087996b6de8f629f6f5251e636cba08d1bdb97d8071cc7d033c88a
+    jest-mock: ^29.6.1
+  checksum: fb671f91f27e7aa1ba04983ef87a83f0794a597aba0a57d08cbb1fcb484c2aedc2201e99f85fafe27aec9be78af6f2d1d7e6ea88267938992a1d0f9d4615f5b2
   languageName: node
   linkType: hard
 
-"@jest/expect-utils@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/expect-utils@npm:29.5.0"
+"@jest/expect-utils@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/expect-utils@npm:29.6.1"
   dependencies:
     jest-get-type: ^29.4.3
-  checksum: c46fb677c88535cf83cf29f0a5b1f376c6a1109ddda266ad7da1a9cbc53cb441fa402dd61fc7b111ffc99603c11a9b3357ee41a1c0e035a58830bcb360871476
+  checksum: 037ee017eca62f7b45e1465fb5c6f9e92d5709a9ac716b8bff0bd294240a54de734e8f968fb69309cc4aef6c83b9552d5a821f3b18371af394bf04783859d706
   languageName: node
   linkType: hard
 
-"@jest/expect@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/expect@npm:29.5.0"
+"@jest/expect@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/expect@npm:29.6.1"
   dependencies:
-    expect: ^29.5.0
-    jest-snapshot: ^29.5.0
-  checksum: bd10e295111547e6339137107d83986ab48d46561525393834d7d2d8b2ae9d5626653f3f5e48e5c3fa742ac982e97bdf1f541b53b9e1d117a247b08e938527f6
+    expect: ^29.6.1
+    jest-snapshot: ^29.6.1
+  checksum: 5c56977b3cc8489744d97d9dc2dcb196c1dfecc83a058a7ef0fd4f63d68cf120a23d27669272d1e1b184fb4337b85e4ac1fc7f886e3988fdf243d42d73973eac
   languageName: node
   linkType: hard
 
-"@jest/fake-timers@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/fake-timers@npm:29.5.0"
+"@jest/fake-timers@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/fake-timers@npm:29.6.1"
   dependencies:
-    "@jest/types": ^29.5.0
+    "@jest/types": ^29.6.1
     "@sinonjs/fake-timers": ^10.0.2
     "@types/node": "*"
-    jest-message-util: ^29.5.0
-    jest-mock: ^29.5.0
-    jest-util: ^29.5.0
-  checksum: 69930c6922341f244151ec0d27640852ec96237f730fc024da1f53143d31b43cde75d92f9d8e5937981cdce3b31416abc3a7090a0d22c2377512c4a6613244ee
+    jest-message-util: ^29.6.1
+    jest-mock: ^29.6.1
+    jest-util: ^29.6.1
+  checksum: 86991276944b7d6c2ada3703a272517f5f8f2f4e2af1fe26065f6db1dac4dc6299729a88c46bcb781dcc1b20504c1d4bbd8119fd8a0838ac81a9a4b5d2c8e429
   languageName: node
   linkType: hard
 
-"@jest/globals@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/globals@npm:29.5.0"
+"@jest/globals@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/globals@npm:29.6.1"
   dependencies:
-    "@jest/environment": ^29.5.0
-    "@jest/expect": ^29.5.0
-    "@jest/types": ^29.5.0
-    jest-mock: ^29.5.0
-  checksum: b309ab8f21b571a7c672608682e84bbdd3d2b554ddf81e4e32617fec0a69094a290ab42e3c8b2c66ba891882bfb1b8b2736720ea1285b3ad646d55c2abefedd9
+    "@jest/environment": ^29.6.1
+    "@jest/expect": ^29.6.1
+    "@jest/types": ^29.6.1
+    jest-mock: ^29.6.1
+  checksum: fcca0b970a8b4894a1cdff0f500a86b45609e72c0a4319875e9504237b839df1a46c44d2f1362c6d87fdc7a05928edcc4b5a3751c9e6648dd70a761cdab64c94
   languageName: node
   linkType: hard
 
-"@jest/reporters@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/reporters@npm:29.5.0"
+"@jest/reporters@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/reporters@npm:29.6.1"
   dependencies:
     "@bcoe/v8-coverage": ^0.2.3
-    "@jest/console": ^29.5.0
-    "@jest/test-result": ^29.5.0
-    "@jest/transform": ^29.5.0
-    "@jest/types": ^29.5.0
-    "@jridgewell/trace-mapping": ^0.3.15
+    "@jest/console": ^29.6.1
+    "@jest/test-result": ^29.6.1
+    "@jest/transform": ^29.6.1
+    "@jest/types": ^29.6.1
+    "@jridgewell/trace-mapping": ^0.3.18
     "@types/node": "*"
     chalk: ^4.0.0
     collect-v8-coverage: ^1.0.0
     exit: ^0.1.2
     glob: ^7.1.3
     graceful-fs: ^4.2.9
     istanbul-lib-coverage: ^3.0.0
     istanbul-lib-instrument: ^5.1.0
     istanbul-lib-report: ^3.0.0
     istanbul-lib-source-maps: ^4.0.0
     istanbul-reports: ^3.1.3
-    jest-message-util: ^29.5.0
-    jest-util: ^29.5.0
-    jest-worker: ^29.5.0
+    jest-message-util: ^29.6.1
+    jest-util: ^29.6.1
+    jest-worker: ^29.6.1
     slash: ^3.0.0
     string-length: ^4.0.1
     strip-ansi: ^6.0.0
     v8-to-istanbul: ^9.0.1
   peerDependencies:
     node-notifier: ^8.0.1 || ^9.0.0 || ^10.0.0
   peerDependenciesMeta:
     node-notifier:
       optional: true
-  checksum: 481268aac9a4a75cc49c4df1273d6b111808dec815e9d009dad717c32383ebb0cebac76e820ad1ab44e207540e1c2fe1e640d44c4f262de92ab1933e057fdeeb
+  checksum: b7dae415f3f6342b4db2671261bbee29af20a829f42135316c3dd548b9ef85290c9bb64a0e3aec4a55486596be1257ac8216a0f8d9794acd43f8b8fb686fc7e3
   languageName: node
   linkType: hard
 
-"@jest/schemas@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/schemas@npm:29.4.3"
+"@jest/schemas@npm:^29.6.0":
+  version: 29.6.0
+  resolution: "@jest/schemas@npm:29.6.0"
   dependencies:
-    "@sinclair/typebox": ^0.25.16
-  checksum: ac754e245c19dc39e10ebd41dce09040214c96a4cd8efa143b82148e383e45128f24599195ab4f01433adae4ccfbe2db6574c90db2862ccd8551a86704b5bebd
+    "@sinclair/typebox": ^0.27.8
+  checksum: c00511c69cf89138a7d974404d3a5060af375b5a52b9c87215d91873129b382ca11c1ff25bd6d605951404bb381ddce5f8091004a61e76457da35db1f5c51365
   languageName: node
   linkType: hard
 
-"@jest/source-map@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/source-map@npm:29.4.3"
+"@jest/source-map@npm:^29.6.0":
+  version: 29.6.0
+  resolution: "@jest/source-map@npm:29.6.0"
   dependencies:
-    "@jridgewell/trace-mapping": ^0.3.15
+    "@jridgewell/trace-mapping": ^0.3.18
     callsites: ^3.0.0
     graceful-fs: ^4.2.9
-  checksum: 2301d225145f8123540c0be073f35a80fd26a2f5e59550fd68525d8cea580fb896d12bf65106591ffb7366a8a19790076dbebc70e0f5e6ceb51f81827ed1f89c
+  checksum: 9c6c40387410bb70b2fae8124287fc28f6bdd1b2d7f24348e8611e1bb638b404518228a4ce64a582365b589c536ae8e7ebab0126cef59a87874b71061d19783b
   languageName: node
   linkType: hard
 
-"@jest/test-result@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/test-result@npm:29.5.0"
+"@jest/test-result@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/test-result@npm:29.6.1"
   dependencies:
-    "@jest/console": ^29.5.0
-    "@jest/types": ^29.5.0
+    "@jest/console": ^29.6.1
+    "@jest/types": ^29.6.1
     "@types/istanbul-lib-coverage": ^2.0.0
     collect-v8-coverage: ^1.0.0
-  checksum: 2e8ff5242227ab960c520c3ea0f6544c595cc1c42fa3873c158e9f4f685f4ec9670ec08a4af94ae3885c0005a43550a9595191ffbc27a0965df27d9d98bbf901
+  checksum: 9397a3a3410c5df564e79297b1be4fe33807a6157a017a1f74b54a6ef14de1530f12b922299e822e66a82c53269da16661772bffde3d883a78c5eefd2cd6d1cc
   languageName: node
   linkType: hard
 
-"@jest/test-sequencer@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/test-sequencer@npm:29.5.0"
+"@jest/test-sequencer@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/test-sequencer@npm:29.6.1"
   dependencies:
-    "@jest/test-result": ^29.5.0
+    "@jest/test-result": ^29.6.1
     graceful-fs: ^4.2.9
-    jest-haste-map: ^29.5.0
+    jest-haste-map: ^29.6.1
     slash: ^3.0.0
-  checksum: eca34b4aeb2fda6dfb7f9f4b064c858a7adf64ec5c6091b6f4ed9d3c19549177cbadcf1c615c4c182688fa1cf085c8c55c3ca6eea40719a34554b0bf071d842e
+  checksum: f3437178b5dca0401ed2e990d8b69161442351856d56f5725e009a487f5232b51039f8829673884b9bea61c861120d08a53a36432f4a4b8aab38915a68f7000d
   languageName: node
   linkType: hard
 
-"@jest/transform@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/transform@npm:29.5.0"
+"@jest/transform@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/transform@npm:29.6.1"
   dependencies:
     "@babel/core": ^7.11.6
-    "@jest/types": ^29.5.0
-    "@jridgewell/trace-mapping": ^0.3.15
+    "@jest/types": ^29.6.1
+    "@jridgewell/trace-mapping": ^0.3.18
     babel-plugin-istanbul: ^6.1.1
     chalk: ^4.0.0
     convert-source-map: ^2.0.0
     fast-json-stable-stringify: ^2.1.0
     graceful-fs: ^4.2.9
-    jest-haste-map: ^29.5.0
+    jest-haste-map: ^29.6.1
     jest-regex-util: ^29.4.3
-    jest-util: ^29.5.0
+    jest-util: ^29.6.1
     micromatch: ^4.0.4
     pirates: ^4.0.4
     slash: ^3.0.0
     write-file-atomic: ^4.0.2
-  checksum: d55d604085c157cf5112e165ff5ac1fa788873b3b31265fb4734ca59892ee24e44119964cc47eb6d178dd9512bbb6c576d1e20e51a201ff4e24d31e818a1c92d
+  checksum: 1635cd66e4b3dbba0689ecefabc6137301756c9c12d1d23e25124dd0dd9b4a6a38653d51e825e90f74faa022152ac1eaf200591fb50417aa7e1f7d1d1c2bc11d
   languageName: node
   linkType: hard
 
-"@jest/types@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "@jest/types@npm:29.5.0"
+"@jest/types@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "@jest/types@npm:29.6.1"
   dependencies:
-    "@jest/schemas": ^29.4.3
+    "@jest/schemas": ^29.6.0
     "@types/istanbul-lib-coverage": ^2.0.0
     "@types/istanbul-reports": ^3.0.0
     "@types/node": "*"
     "@types/yargs": ^17.0.8
     chalk: ^4.0.0
-  checksum: 1811f94b19cf8a9460a289c4f056796cfc373480e0492692a6125a553cd1a63824bd846d7bb78820b7b6f758f6dd3c2d4558293bb676d541b2fa59c70fdf9d39
+  checksum: 89fc1ccf71a84fe0da643e0675b1cfe6a6f19ea72e935b2ab1dbdb56ec547e94433fb59b3536d3832a6e156c077865b7176fe9dae707dab9c3d2f9405ba6233c
   languageName: node
   linkType: hard
 
 "@jridgewell/gen-mapping@npm:^0.3.0, @jridgewell/gen-mapping@npm:^0.3.2":
   version: 0.3.3
   resolution: "@jridgewell/gen-mapping@npm:0.3.3"
   dependencies:
@@ -1985,20 +1991,20 @@
   version: 1.1.2
   resolution: "@jridgewell/set-array@npm:1.1.2"
   checksum: 69a84d5980385f396ff60a175f7177af0b8da4ddb81824cb7016a9ef914eee9806c72b6b65942003c63f7983d4f39a5c6c27185bbca88eb4690b62075602e28e
   languageName: node
   linkType: hard
 
 "@jridgewell/source-map@npm:^0.3.3":
-  version: 0.3.3
-  resolution: "@jridgewell/source-map@npm:0.3.3"
+  version: 0.3.5
+  resolution: "@jridgewell/source-map@npm:0.3.5"
   dependencies:
     "@jridgewell/gen-mapping": ^0.3.0
     "@jridgewell/trace-mapping": ^0.3.9
-  checksum: ae1302146339667da5cd6541260ecbef46ae06819a60f88da8f58b3e64682f787c09359933d050dea5d2173ea7fa40f40dd4d4e7a8d325c5892cccd99aaf8959
+  checksum: 1ad4dec0bdafbade57920a50acec6634f88a0eb735851e0dda906fa9894e7f0549c492678aad1a10f8e144bfe87f238307bf2a914a1bc85b7781d345417e9f6f
   languageName: node
   linkType: hard
 
 "@jridgewell/sourcemap-codec@npm:1.4.14":
   version: 1.4.14
   resolution: "@jridgewell/sourcemap-codec@npm:1.4.14"
   checksum: 61100637b6d173d3ba786a5dff019e1a74b1f394f323c1fee337ff390239f053b87266c7a948777f4b1ee68c01a8ad0ab61e5ff4abb5a012a0b091bec391ab97
@@ -2008,15 +2014,15 @@
 "@jridgewell/sourcemap-codec@npm:^1.4.10":
   version: 1.4.15
   resolution: "@jridgewell/sourcemap-codec@npm:1.4.15"
   checksum: b881c7e503db3fc7f3c1f35a1dd2655a188cc51a3612d76efc8a6eb74728bef5606e6758ee77423e564092b4a518aba569bbb21c9bac5ab7a35b0c6ae7e344c8
   languageName: node
   linkType: hard
 
-"@jridgewell/trace-mapping@npm:^0.3.12, @jridgewell/trace-mapping@npm:^0.3.15, @jridgewell/trace-mapping@npm:^0.3.17, @jridgewell/trace-mapping@npm:^0.3.9":
+"@jridgewell/trace-mapping@npm:^0.3.12, @jridgewell/trace-mapping@npm:^0.3.17, @jridgewell/trace-mapping@npm:^0.3.18, @jridgewell/trace-mapping@npm:^0.3.9":
   version: 0.3.18
   resolution: "@jridgewell/trace-mapping@npm:0.3.18"
   dependencies:
     "@jridgewell/resolve-uri": 3.1.0
     "@jridgewell/sourcemap-codec": 1.4.14
   checksum: 0572669f855260808c16fe8f78f5f1b4356463b11d3f2c7c0b5580c8ba1cbf4ae53efe9f627595830856e57dbac2325ac17eb0c3dd0ec42102e6f227cc289c02
   languageName: node
@@ -2026,44 +2032,44 @@
   version: 7.1.3
   resolution: "@jsdevtools/ono@npm:7.1.3"
   checksum: 2297fcd472ba810bffe8519d2249171132844c7174f3a16634f9260761c8c78bc0428a4190b5b6d72d45673c13918ab9844d706c3ed4ef8f62ab11a2627a08ad
   languageName: node
   linkType: hard
 
 "@jupyter-widgets/base@npm:^6.0.2":
-  version: 6.0.4
-  resolution: "@jupyter-widgets/base@npm:6.0.4"
+  version: 6.0.5
+  resolution: "@jupyter-widgets/base@npm:6.0.5"
   dependencies:
-    "@jupyterlab/services": ^6.0.0
-    "@lumino/coreutils": ^1.11.1
-    "@lumino/messaging": ^1.10.1
-    "@lumino/widgets": ^1.30.0
+    "@jupyterlab/services": ^6.0.0 || ^7.0.0
+    "@lumino/coreutils": ^1.11.1 || ^2.1
+    "@lumino/messaging": ^1.10.1 || ^2.1
+    "@lumino/widgets": ^1.30.0 || ^2.1
     "@types/backbone": 1.4.14
     "@types/lodash": ^4.14.134
     backbone: 1.4.0
     jquery: ^3.1.1
     lodash: ^4.17.4
-  checksum: f82b4eec8fc819adaab6728077700484fc0ab7b64c6ecbf95bf960bbfff0515a18b88ab5c84f92f3ea1636e03f8dc4c4db264ca69d9783fd37149ca1f970ac1c
+  checksum: d9090c172d6504f95a7b1906e4b8c7be722318103b5721fa447140d04888448ebc31f47887c1dfc9022fff183b41cf6dbb7a2d2b3f821d05fe17350281fc3a17
   languageName: node
   linkType: hard
 
 "@jupyter/docprovider@npm:^1.0.0-alpha.8":
-  version: 1.0.0
-  resolution: "@jupyter/docprovider@npm:1.0.0"
+  version: 1.0.1
+  resolution: "@jupyter/docprovider@npm:1.0.1"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/services": ^7.0.0
     "@lumino/coreutils": ^2.1.0
     "@lumino/disposable": ^2.1.0
     "@lumino/signaling": ^2.1.0
     y-protocols: ^1.0.5
     y-websocket: ^1.3.15
     yjs: ^13.5.40
-  checksum: b45001cea36877f2a29a8cdf7f6bce6d625c28499fd4679aeeb6da0298c23447809ea3b74772aad4aebce83d08e53096fde20a4ffe644d569ade5ddd7572f39b
+  checksum: 52d11c5f75aa599ba2f3aaaa75f8a5ca59124b7af1edbbc91164d0a0aaa2e5a6640fce30db3294885b31628204852b86ded02751e861da925155f7646cc48d85
   languageName: node
   linkType: hard
 
 "@jupyter/ydoc@npm:^1.0.2":
   version: 1.0.2
   resolution: "@jupyter/ydoc@npm:1.0.2"
   dependencies:
@@ -2304,29 +2310,14 @@
     react: ^18.2.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: 0f9207ccb0e3a3b1ac72c548ffadf31fe5cc535d4526f95ee9b4081ed509560318d8666027c91a615d4f7c24b3832d11e8587278ebee1a2a64f7e11e1e0f1f0a
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^5.6.5":
-  version: 5.6.5
-  resolution: "@jupyterlab/coreutils@npm:5.6.5"
-  dependencies:
-    "@lumino/coreutils": ^1.11.0
-    "@lumino/disposable": ^1.10.0
-    "@lumino/signaling": ^1.10.0
-    minimist: ~1.2.0
-    moment: ^2.24.0
-    path-browserify: ^1.0.0
-    url-parse: ~1.5.1
-  checksum: 6abd7d3bc12ceaf2b06ddfc22aa07e7bae86db1de32339e42fa41425508b3d450427d9d0a81aed829a3a15e596bc260846e287cc3c46d7a7f95d9cdb8507ba23
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/coreutils@npm:^6.0.0, @jupyterlab/coreutils@npm:^6.0.0-alpha.18, @jupyterlab/coreutils@npm:^6.0.2":
   version: 6.0.2
   resolution: "@jupyterlab/coreutils@npm:6.0.2"
   dependencies:
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
@@ -2490,23 +2481,14 @@
   resolution: "@jupyterlab/nbformat@npm:4.0.2"
   dependencies:
     "@lumino/coreutils": ^2.1.1
   checksum: cccd1c7fd8717ccece1f7642f3f7218103c3baa479fce85666770719b3359116e5279cdd97e2b584122a793b437fc9ece7055d1da27ad35a090f90398a76d59f
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.6.5":
-  version: 3.6.5
-  resolution: "@jupyterlab/nbformat@npm:3.6.5"
-  dependencies:
-    "@lumino/coreutils": ^1.11.0
-  checksum: 15c663c13bad604e9ae26e67907faf968ec0105e2e9934a14f16c8a7bc9d47221bbb4af37cf98d1b824bb7806e01dc4268bf309cd9d50b84ed333561095bb0d6
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/notebook@npm:^4.0.0, @jupyterlab/notebook@npm:^4.0.2":
   version: 4.0.2
   resolution: "@jupyterlab/notebook@npm:4.0.2"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
     "@jupyterlab/apputils": ^4.1.2
     "@jupyterlab/cells": ^4.0.2
@@ -2535,27 +2517,14 @@
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
   checksum: 053cde5377aceac7ff6fe30e734354df1839cbf84bfd19f7d3992a1aaddcd66f5c8470bb2537c94b28dfdb194dfdacfaa38207fd2d4989b0575b27c20396bbfe
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^4.6.5":
-  version: 4.6.5
-  resolution: "@jupyterlab/observables@npm:4.6.5"
-  dependencies:
-    "@lumino/algorithm": ^1.9.0
-    "@lumino/coreutils": ^1.11.0
-    "@lumino/disposable": ^1.10.0
-    "@lumino/messaging": ^1.10.0
-    "@lumino/signaling": ^1.10.0
-  checksum: 503b4f1c7d61fa3e7c69dc740a4d4a45948257434ebdcb875e86b03a818573250fe9824725a68c0d78715e1bac5c40cd412f387a159c8a40211115542a202030
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/observables@npm:^5.0.0, @jupyterlab/observables@npm:^5.0.2":
   version: 5.0.2
   resolution: "@jupyterlab/observables@npm:5.0.2"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
@@ -2613,35 +2582,15 @@
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     lodash.escape: ^4.0.1
   checksum: 6118adf39cfe3c5918c9b677ff5d8dbe97ce469427f9969e1d16fba944b53d6e6c9d2c1e2deaaf928cdb94222a8941c7bb7cfc81693683fd07c08e92bc3d6cea
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^6.0.0":
-  version: 6.6.5
-  resolution: "@jupyterlab/services@npm:6.6.5"
-  dependencies:
-    "@jupyterlab/coreutils": ^5.6.5
-    "@jupyterlab/nbformat": ^3.6.5
-    "@jupyterlab/observables": ^4.6.5
-    "@jupyterlab/settingregistry": ^3.6.5
-    "@jupyterlab/statedb": ^3.6.5
-    "@lumino/algorithm": ^1.9.0
-    "@lumino/coreutils": ^1.11.0
-    "@lumino/disposable": ^1.10.0
-    "@lumino/polling": ^1.9.0
-    "@lumino/signaling": ^1.10.0
-    node-fetch: ^2.6.0
-    ws: ^7.4.6
-  checksum: 020bd3005c3aee858657233b8a73d1ee3cad14c88ed033bf6c67254ce6d799f6c34f1d0fa128eb42d96c59bd3dbc41557092410e70e17760e8283e211bae5b27
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/services@npm:^7.0.0, @jupyterlab/services@npm:^7.0.0-alpha.18, @jupyterlab/services@npm:^7.0.2":
+"@jupyterlab/services@npm:^6.0.0 || ^7.0.0, @jupyterlab/services@npm:^7.0.0, @jupyterlab/services@npm:^7.0.0-alpha.18, @jupyterlab/services@npm:^7.0.2":
   version: 7.0.2
   resolution: "@jupyterlab/services@npm:7.0.2"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
     "@jupyterlab/coreutils": ^6.0.2
     "@jupyterlab/nbformat": ^4.0.2
     "@jupyterlab/settingregistry": ^4.0.2
@@ -2652,29 +2601,14 @@
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     ws: ^8.11.0
   checksum: 4a4b5328f2f50ec1d501f67d63fbfb329f37a6c090227e0aecdbbb7316d9df0e5891af47cb948958e9307a0afc52f0ddf05c2be7acb9e2f44e54cf568dc3b90c
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^3.6.5":
-  version: 3.6.5
-  resolution: "@jupyterlab/settingregistry@npm:3.6.5"
-  dependencies:
-    "@jupyterlab/statedb": ^3.6.5
-    "@lumino/commands": ^1.19.0
-    "@lumino/coreutils": ^1.11.0
-    "@lumino/disposable": ^1.10.0
-    "@lumino/signaling": ^1.10.0
-    ajv: ^6.12.3
-    json5: ^2.1.1
-  checksum: c105001da9917922d6e37f853945a31bbdaae96a7a3a66cf82da208efa692f8c8dfb00f0049a00df0be9f8f59da090da04ee146d35f0365f5186bbefaa884b06
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/settingregistry@npm:^4.0.2":
   version: 4.0.2
   resolution: "@jupyterlab/settingregistry@npm:4.0.2"
   dependencies:
     "@jupyterlab/nbformat": ^4.0.2
     "@jupyterlab/statedb": ^4.0.2
     "@lumino/commands": ^2.1.1
@@ -2686,27 +2620,14 @@
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
   checksum: c2e019f70a4f19cf99bc2029c136197f2a750f319e16f8605a6f8d690b6930ac32e24678b090a09f9e949e540cf6b4214d3d3597ec119bd6896db3b456ac6299
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^3.6.5":
-  version: 3.6.5
-  resolution: "@jupyterlab/statedb@npm:3.6.5"
-  dependencies:
-    "@lumino/commands": ^1.19.0
-    "@lumino/coreutils": ^1.11.0
-    "@lumino/disposable": ^1.10.0
-    "@lumino/properties": ^1.8.0
-    "@lumino/signaling": ^1.10.0
-  checksum: 5973d9b17016110bd6791f10864a2a0d124821cd3456c343d003fecac98db8d09abf5b5345053c91b1597ddb4376b8909eac6277a8040deb802289c2ab35330b
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/statedb@npm:^4.0.2":
   version: 4.0.2
   resolution: "@jupyterlab/statedb@npm:4.0.2"
   dependencies:
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
@@ -2837,30 +2758,30 @@
   version: 1.0.3
   resolution: "@lezer/common@npm:1.0.3"
   checksum: cc90dc2f0aeaebeb3fe886cbd27f8b1e8bee817d8c2efff178604807debd68c5db820fd23afb830962780063d21891afbdf564420221faca2822e77bc6327184
   languageName: node
   linkType: hard
 
 "@lezer/cpp@npm:^1.0.0":
-  version: 1.1.0
-  resolution: "@lezer/cpp@npm:1.1.0"
+  version: 1.1.1
+  resolution: "@lezer/cpp@npm:1.1.1"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 9b25c881fc9b64fd2b019a077a85b0ba7cfda0bbdd92dbb0ff43300c9ba1ec4360128fe912bfe0f06a1c1bb5a564c5ace375c8aad254d07a717768a8f268695d
+  checksum: c9e1db19776eafbfe0c3b8448d46c94d9a1d30f7fef630292e63bab82e6d5d6903a043ee8cf341bcbf84c00ee0d79b8c255bab8fd8e0a91355ae912b53c78935
   languageName: node
   linkType: hard
 
 "@lezer/css@npm:^1.0.0, @lezer/css@npm:^1.1.0":
-  version: 1.1.2
-  resolution: "@lezer/css@npm:1.1.2"
+  version: 1.1.3
+  resolution: "@lezer/css@npm:1.1.3"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 02218fe6901428e191a91a1f1a3728a051af982bafaf37144884c9261a7e24b2ad1dfdaa6e7feeb160e5bc34157ce92213cd92ae244cdf0b8485b8b8113850f8
+  checksum: c8069ef0a6751441d2dc9180f7ebfd7aeb35df0ca2f1a748a2f26203a9ef6cc30f17f3074e2b49520453eb39329dadfdbbb901c6d9d067dc955ceb58c1f8cc6a
   languageName: node
   linkType: hard
 
 "@lezer/generator@npm:^1.2.2":
   version: 1.3.0
   resolution: "@lezer/generator@npm:1.3.0"
   dependencies:
@@ -2878,114 +2799,114 @@
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 411a702394c4c996b7d7f145a38f3a85a8cc698b3918acc7121c629255bb76d4ab383753f69009e011dc415210c6acbbb5b27bde613259ab67e600b29397b03b
   languageName: node
   linkType: hard
 
 "@lezer/html@npm:^1.3.0":
-  version: 1.3.4
-  resolution: "@lezer/html@npm:1.3.4"
+  version: 1.3.5
+  resolution: "@lezer/html@npm:1.3.5"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 81dd134ac094edf7c40bae4c3b7126d336ce4c3c87756344bf604eff64d89b06fcb55f91618a4622eb0dae6d6015722f5bab58e2252d86e81fca8c3ced1a0c4d
+  checksum: 19fcf262d06a89d8a1d3c6c825585f4b555dbdeaf60179fbe00164f72c0dbdf8cde8057172fd3660b13be63f0dcf1380cea9196ade7c1a9bc58a2aecd2b03125
   languageName: node
   linkType: hard
 
 "@lezer/java@npm:^1.0.0":
-  version: 1.0.3
-  resolution: "@lezer/java@npm:1.0.3"
+  version: 1.0.4
+  resolution: "@lezer/java@npm:1.0.4"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 2fffea6627d130413ffad4e61040267974cca3167d98881b9e5b5e2455530de74a82c234d93603e92a4972fad314671453c49c0a76b0f4547c4617d671fd7b99
+  checksum: 97f5a2c2d733afba5dc57a0da9a97515b19b5e63bb5937717dac4e8c9baed74d15c0cb5c1580858b678931f11d517c56d89f903968fa48931f9c62e2ea67a107
   languageName: node
   linkType: hard
 
 "@lezer/javascript@npm:^1.0.0":
-  version: 1.4.3
-  resolution: "@lezer/javascript@npm:1.4.3"
+  version: 1.4.4
+  resolution: "@lezer/javascript@npm:1.4.4"
   dependencies:
     "@lezer/highlight": ^1.1.3
     "@lezer/lr": ^1.3.0
-  checksum: 520dc2d84c84841ef554993c1c0dfe503487aa9be398ebcf617b51d06f99121841d4ca1cf25f3f53d00efa820ea778cc2271da425a606ac66e9f09a4c8cc6677
+  checksum: 29797dbb4c0632718cc5a3d0c6baeefe4240562f8b1ef1f60c58d0481c53ac4bbbac354369aa95e4131dfe0bbc4464bc025620f58f01739bd896974bb08dbad5
   languageName: node
   linkType: hard
 
 "@lezer/json@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "@lezer/json@npm:1.0.0"
+  version: 1.0.1
+  resolution: "@lezer/json@npm:1.0.1"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: c1ca0cdf681415b58a383a669944bed66da3aa830870d32d1e471d545cff0fe43d9ac8a0d2a318a96daa99cd5a645b1d58ba8fbdd2e8d7ca4d33a62c7582cbab
+  checksum: fcd17178f6a58e71c83e08fdc047e3708528b28591ba8f08ed35268f370d1ec9b63af0afa9d82a77fec26e9eb477ab3cfdc31c951e080d118ef607f9f9bb52e3
   languageName: node
   linkType: hard
 
 "@lezer/lr@npm:^1.0.0, @lezer/lr@npm:^1.1.0, @lezer/lr@npm:^1.3.0":
-  version: 1.3.7
-  resolution: "@lezer/lr@npm:1.3.7"
+  version: 1.3.9
+  resolution: "@lezer/lr@npm:1.3.9"
   dependencies:
     "@lezer/common": ^1.0.0
-  checksum: 77d7b894f453e59a95f436146fde452405bc76ef41b31569444219244d596033b0110da65ac9bc87093cd2222e2a472ca411c6712bc8b35f74ddaa1f2ea1b7d8
+  checksum: d10982bae6c0b2f5a3ab8710a41dc689a4f9e81afafd3d2de4f0bec169f5c3fc9a321c0e90010a51682d41a6755ae90e1f3199134ff194b3ff4058ea5bcdf353
   languageName: node
   linkType: hard
 
 "@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.0.2":
-  version: 1.0.3
-  resolution: "@lezer/markdown@npm:1.0.3"
+  version: 1.0.5
+  resolution: "@lezer/markdown@npm:1.0.5"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
-  checksum: 73ccd8d0664849d45912db8148a3b974328e85ba055f9a811e7506c205f112b4d891fca41a849f619456bc6e0f2ce59cd657f88f800ebd5f2f492bc0214374a0
+  checksum: e862d7362faab54a4536c9913171580d0062ae5ffa9d46d6dcb4850b2b8f2fb6f2f28f98a30232640bfcd980682673ccb051230b06422814db89abea5f07d99e
   languageName: node
   linkType: hard
 
 "@lezer/php@npm:^1.0.0":
   version: 1.0.1
   resolution: "@lezer/php@npm:1.0.1"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.1.0
   checksum: a847c255c030b4d38913ddf1d5bd7324d83be7ef8d1d244542870be03b9bf7dc71283afeb2415c40dfd188cb99f0cc44bad760b5f3b7c35c3b8e5e00253848fc
   languageName: node
   linkType: hard
 
 "@lezer/python@npm:^1.1.4":
-  version: 1.1.7
-  resolution: "@lezer/python@npm:1.1.7"
+  version: 1.1.8
+  resolution: "@lezer/python@npm:1.1.8"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 7ae6b4ae770b3cd849eee3d8fb1d904745aee202a76e7db0a079725a97571c4778fa5bd74878206e44aa3349044bf056008e19e7a90650fad93d51890f685077
+  checksum: e4a4e0b0fd871acff25111d4f767944b5015479776504b85c4431859c8a2859fdfa6362f204f3027cf9858c7ea907fd57244852a18b67da9eba3b2fe38d31b03
   languageName: node
   linkType: hard
 
 "@lezer/rust@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "@lezer/rust@npm:1.0.0"
+  version: 1.0.1
+  resolution: "@lezer/rust@npm:1.0.1"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 0c42f415674f60ca2ef4274b446577621cdeec8f31168b1c3b90888a4377c513f02a89ee346421c264ec3a77fe2fa3e134996be6463ed506dbbc79b4b4505375
+  checksum: 1e02fdf09206979e7d4f87b020589f410c4c5e452a7b7b0296f6772ce3571c1bd7ed37495fbeeecf3d4423000f2efdabd462ba8a949c2b351fd35550327a7613
   languageName: node
   linkType: hard
 
 "@lezer/xml@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@lezer/xml@npm:1.0.1"
+  version: 1.0.2
+  resolution: "@lezer/xml@npm:1.0.2"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 271319aa7802c123845b70ffa63d7065c0f92fc6a1ddb1f8ec9f3aa965bca3df3c9fad4d4de53187ddf230e833cd3ab3a84cb2aded76ab5f6831e9a2fc310923
+  checksum: e834bcc5c0dee3eecb5362b3f10187e80908b6a293ebacf5750547a64b57ec710a068497334f109ecf4e5ea05e09e7e9c00e48ebbd30050673ea67b0929e5398
   languageName: node
   linkType: hard
 
-"@lumino/algorithm@npm:^1.9.0, @lumino/algorithm@npm:^1.9.2":
+"@lumino/algorithm@npm:^1.9.2":
   version: 1.9.2
   resolution: "@lumino/algorithm@npm:1.9.2"
   checksum: a89e7c63504236119634858e271db1cc649684d30ced5a6ebe2788af7c0837f1e05a6fd3047d8525eb756c42ce137f76b3688f75fd3ef915b71cd4f213dfbb96
   languageName: node
   linkType: hard
 
 "@lumino/algorithm@npm:^2.0.0":
@@ -3020,29 +2941,14 @@
   resolution: "@lumino/collections@npm:2.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
   checksum: 4a7fc3571e92a1368a1ef01300ad7b6e0d4ff13cb78b89533d5962eea66d4a7550e15d8b80fa3ab1816b1a89382f35015f9dddf72ab04654c17e5b516b845d8f
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^1.19.0, @lumino/commands@npm:^1.21.1":
-  version: 1.21.1
-  resolution: "@lumino/commands@npm:1.21.1"
-  dependencies:
-    "@lumino/algorithm": ^1.9.2
-    "@lumino/coreutils": ^1.12.1
-    "@lumino/disposable": ^1.10.4
-    "@lumino/domutils": ^1.8.2
-    "@lumino/keyboard": ^1.8.2
-    "@lumino/signaling": ^1.11.1
-    "@lumino/virtualdom": ^1.14.3
-  checksum: 1e2ee7ce14b7241aee829df76f2bee6c046a82c2c137c6bb58049142c52a67f8ae74168fdcc4027b0d5a1c9f2ffa8b8f5231ef89f6f0ea8dcc4cab8d475e1ad4
-  languageName: node
-  linkType: hard
-
 "@lumino/commands@npm:^2.1.0, @lumino/commands@npm:^2.1.1, @lumino/commands@npm:^2.1.2":
   version: 2.1.2
   resolution: "@lumino/commands@npm:2.1.2"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
@@ -3050,98 +2956,55 @@
     "@lumino/keyboard": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
   checksum: c0b5ce8c5e1a86a98a90f54bb07b74742748110cf3362b86ff8328c1b5475c4dc05f1c4c9f50bf79e51c4e2ddc5cd69d6194f3d39dd5b58f357b0f30758bf35b
   languageName: node
   linkType: hard
 
-"@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.1, @lumino/coreutils@npm:^2.0.0-alpha.6, @lumino/coreutils@npm:^2.1.0, @lumino/coreutils@npm:^2.1.1":
+"@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.1, @lumino/coreutils@npm:^1.11.1 || ^2.1, @lumino/coreutils@npm:^2.0.0-alpha.6, @lumino/coreutils@npm:^2.1.0, @lumino/coreutils@npm:^2.1.1":
   version: 2.1.1
   resolution: "@lumino/coreutils@npm:2.1.1"
   checksum: dfdeb2b0282caae17b6c3edfebadf4ce7c75fc879fa60cacfef9b154412f4b35e4ffd95b1833b99d8dacb99aaaa04513570129ae2024c3f33e2677a01f0576ce
   languageName: node
   linkType: hard
 
-"@lumino/coreutils@npm:^1.11.0, @lumino/coreutils@npm:^1.11.1, @lumino/coreutils@npm:^1.12.1":
-  version: 1.12.1
-  resolution: "@lumino/coreutils@npm:1.12.1"
-  peerDependencies:
-    crypto: 1.0.1
-  checksum: 55f1b87997f8dd0af28ff23c2d4b3aa252e515b9d3bc91b350a5c6c8526ceae61b14b55dc0d8d01691c69d42974b3d559f2b49bc7ced0f474b8f5dc52b3e83ed
-  languageName: node
-  linkType: hard
-
 "@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^2.1.0, @lumino/disposable@npm:^2.1.1":
   version: 2.1.1
   resolution: "@lumino/disposable@npm:2.1.1"
   dependencies:
     "@lumino/signaling": ^2.1.1
   checksum: ed6cdfe13f3346178a087690d4e7baeccaed7e73ca23cb239765202409f5c01b4729a4058b4717f963462ee9ef2e5cb14ad1974e3163741267290edc3715c85c
   languageName: node
   linkType: hard
 
-"@lumino/disposable@npm:^1.10.0, @lumino/disposable@npm:^1.10.4":
-  version: 1.10.4
-  resolution: "@lumino/disposable@npm:1.10.4"
-  dependencies:
-    "@lumino/algorithm": ^1.9.2
-    "@lumino/signaling": ^1.11.1
-  checksum: b53e259830f1d3231455548e6b95c9ae0f4b91e1b501980a1d0bb9708322bf5469b5cbb4e5005653d6f33b549d4bb7e58ce02226477876f51c124ea755152a33
-  languageName: node
-  linkType: hard
-
-"@lumino/domutils@npm:^1.8.2":
-  version: 1.8.2
-  resolution: "@lumino/domutils@npm:1.8.2"
-  checksum: 196f25316a17cd8df8f11dbe17f10cbd96e5ce166ea97aab6402307dc554382423d860859bb5d05226f05909748b781fb281bb9220690fe1f3ddc716072c2ed5
-  languageName: node
-  linkType: hard
-
 "@lumino/domutils@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/domutils@npm:2.0.0"
   checksum: 4a146bfc1006d5fd00ccecc61d9803965d269c15c48c892fd87216336ce967f0db91f31203c5616c83d260224cddf25af4abb6704a6770757d19e44068f690bf
   languageName: node
   linkType: hard
 
-"@lumino/dragdrop@npm:^1.14.5":
-  version: 1.14.5
-  resolution: "@lumino/dragdrop@npm:1.14.5"
-  dependencies:
-    "@lumino/coreutils": ^1.12.1
-    "@lumino/disposable": ^1.10.4
-  checksum: c10031e9aa9ef7f3ab71a1b73f761b84291dda85a449e5f4d2d7c462277759a947513eb7ee3e3d984f7cfc2730b1c96d0706124802492f9adbd7be00d13137ee
-  languageName: node
-  linkType: hard
-
 "@lumino/dragdrop@npm:^2.1.1, @lumino/dragdrop@npm:^2.1.2":
   version: 2.1.2
   resolution: "@lumino/dragdrop@npm:2.1.2"
   dependencies:
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
   checksum: 7ac64ec11423ec89fea937aa6c9ca818933ee98e775e500018a0a948f32171932033a1e302a48395cbe9bfeaa635acde2393fd935db14d7b1d569ca6a1daaa77
   languageName: node
   linkType: hard
 
-"@lumino/keyboard@npm:^1.8.2":
-  version: 1.8.2
-  resolution: "@lumino/keyboard@npm:1.8.2"
-  checksum: 30f8ced53ca0aa466dba33be3c9379a2a6abcf1c52485073d9f9d9bc119eb3327a7343fad764c2d63a8a30ae05c0047098c40ec605e60af215356f3edb9ab4a9
-  languageName: node
-  linkType: hard
-
 "@lumino/keyboard@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/keyboard@npm:2.0.0"
   checksum: 3852ba51f437b1c1d7e552a0f844592a05e04dd5012070dc6e4384c58965d1ebf536c6875c1b7bae03cde3c715ddc36cd290992fcefc1a8c39094194f4689fdd
   languageName: node
   linkType: hard
 
-"@lumino/messaging@npm:^1.10.0, @lumino/messaging@npm:^1.10.1, @lumino/messaging@npm:^1.10.3":
+"@lumino/messaging@npm:^1.10.1 || ^2.1":
   version: 1.10.3
   resolution: "@lumino/messaging@npm:1.10.3"
   dependencies:
     "@lumino/algorithm": ^1.9.2
     "@lumino/collections": ^1.9.3
   checksum: 1131e80379fa9b8a9b5d3418c90e25d4be48e2c92ec711518190772f9e8845a695bef45daddd06a129168cf6f158c8ad80ae86cb245f566e9195bbd9a0843b7a
   languageName: node
@@ -3153,43 +3016,25 @@
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/collections": ^2.0.0
   checksum: 1e82dcf9b110834d4342dc63dfeac0ee780880fb99051bd82d00a1f83afd91b276c1cea5af85a414d92c527adc365d54f20ec780123b562f89c5a2cd3e96bf81
   languageName: node
   linkType: hard
 
-"@lumino/polling@npm:^1.9.0":
-  version: 1.11.4
-  resolution: "@lumino/polling@npm:1.11.4"
-  dependencies:
-    "@lumino/coreutils": ^1.12.1
-    "@lumino/disposable": ^1.10.4
-    "@lumino/signaling": ^1.11.1
-  checksum: d4625da7bf5399f6bffed29251daaeb4bf14a0733ad77ad1573c9893973480961be445d8700a5d004102d14ab5a2cf4b79244b1fe74680d060167e55db211c04
-  languageName: node
-  linkType: hard
-
 "@lumino/polling@npm:^2.1.1":
   version: 2.1.1
   resolution: "@lumino/polling@npm:2.1.1"
   dependencies:
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
   checksum: 69177b26d5fc541e72533cbe7d7f7999eea541d392f1082d20dbd9e1797e7d46fba47bae9c65c06f9ccb2780cbae636e9354d9bf4423b5e1020754d4b07d4f6b
   languageName: node
   linkType: hard
 
-"@lumino/properties@npm:^1.8.0, @lumino/properties@npm:^1.8.2":
-  version: 1.8.2
-  resolution: "@lumino/properties@npm:1.8.2"
-  checksum: 9a53709fe58d3abbc99062f0c0fda4d5f64a4c7dca509251f0f89cdcaf881fdf6172ee852dbfe70594ee34bb97255acca771a722d62e7e2150ba8cf6f7e7d15c
-  languageName: node
-  linkType: hard
-
 "@lumino/properties@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/properties@npm:2.0.0"
   checksum: 81187a11a779eed4e20ff0035e77dee99bd271b0cf649096c4e8809dd6bdd06955b1a974bc1a115e536f8d2840b30183bb78a362b2c6991824477df6d17e6c59
   languageName: node
   linkType: hard
 
@@ -3199,62 +3044,24 @@
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
   checksum: 283ad4239b8577f68aca3d0b2606f73cc1c775f84cab25cf49aa6cd195f0d87949ef43fdff03b38b5a49ebbf2468581c6786d5f8b6159a04b2051260be5eab86
   languageName: node
   linkType: hard
 
-"@lumino/signaling@npm:^1.10.0, @lumino/signaling@npm:^1.11.1":
-  version: 1.11.1
-  resolution: "@lumino/signaling@npm:1.11.1"
-  dependencies:
-    "@lumino/algorithm": ^1.9.2
-    "@lumino/properties": ^1.8.2
-  checksum: 3d822be705d9ba8adc46ec405a4422cd4f76ed774f94da5386a511f01df4325c3c8bfa288c9c812184c94cfd0c3ef7b1121dcc9c9489750ad6cfaa7ffb2a3a67
-  languageName: node
-  linkType: hard
-
-"@lumino/virtualdom@npm:^1.14.3":
-  version: 1.14.3
-  resolution: "@lumino/virtualdom@npm:1.14.3"
-  dependencies:
-    "@lumino/algorithm": ^1.9.2
-  checksum: dd6acc5402eb7961ab05f5ce9afaebce4258eb92111f4d97b58ac87a6453686376d2b7d0a2041a54eef6e78091e36a430c74834c97b862fba31fa82ef43c72cb
-  languageName: node
-  linkType: hard
-
 "@lumino/virtualdom@npm:^2.0.0, @lumino/virtualdom@npm:^2.0.0-alpha.6":
   version: 2.0.0
   resolution: "@lumino/virtualdom@npm:2.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
   checksum: 6fc1d88e7d4a656be7664ccfc5745eb1d4e3d2034db0b11ad6abefcc642f22d265003eef0e1d02bca2e42b6da127123118c631369006f78e88a08885a6f36c25
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^1.30.0":
-  version: 1.37.2
-  resolution: "@lumino/widgets@npm:1.37.2"
-  dependencies:
-    "@lumino/algorithm": ^1.9.2
-    "@lumino/commands": ^1.21.1
-    "@lumino/coreutils": ^1.12.1
-    "@lumino/disposable": ^1.10.4
-    "@lumino/domutils": ^1.8.2
-    "@lumino/dragdrop": ^1.14.5
-    "@lumino/keyboard": ^1.8.2
-    "@lumino/messaging": ^1.10.3
-    "@lumino/properties": ^1.8.2
-    "@lumino/signaling": ^1.11.1
-    "@lumino/virtualdom": ^1.14.3
-  checksum: 3193f8cca4bad2c9d59031515b7b81b8a3655088f2b8c4f69f575116140d45c5caed935da0ed3fab9dc5ce96fde037bfa5fef0c129921955b3fb73cf725d1b06
-  languageName: node
-  linkType: hard
-
-"@lumino/widgets@npm:^1.37.2 || ^2.1.1, @lumino/widgets@npm:^2.0.0-alpha.6, @lumino/widgets@npm:^2.1.0, @lumino/widgets@npm:^2.1.1, @lumino/widgets@npm:^2.2.0":
+"@lumino/widgets@npm:^1.30.0 || ^2.1, @lumino/widgets@npm:^1.37.2 || ^2.1.1, @lumino/widgets@npm:^2.0.0-alpha.6, @lumino/widgets@npm:^2.1.0, @lumino/widgets@npm:^2.1.1, @lumino/widgets@npm:^2.2.0":
   version: 2.2.0
   resolution: "@lumino/widgets@npm:2.2.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/commands": ^2.1.2
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
@@ -3265,14 +3072,23 @@
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
   checksum: 963c0e54102b786a9cbf3467041c9f6f5c275af751afc311ebeba30d56516767c463c425e321bb389eaa66726dfc4420119a9a58573dcbf3110aba9515c80606
   languageName: node
   linkType: hard
 
+"@nicolo-ribaudo/semver-v6@npm:^6.3.3":
+  version: 6.3.3
+  resolution: "@nicolo-ribaudo/semver-v6@npm:6.3.3"
+  bin:
+    semver: bin/semver.js
+  checksum: 8290855b1591477d2298364541fda64fafd4acc110b387067a71c9b05f4105c0a4ac079857ae9cd107c42ee884e8724a406b5116f069575e02d7ab87a35a5272
+  languageName: node
+  linkType: hard
+
 "@nodelib/fs.scandir@npm:2.1.5":
   version: 2.1.5
   resolution: "@nodelib/fs.scandir@npm:2.1.5"
   dependencies:
     "@nodelib/fs.stat": 2.0.5
     run-parallel: ^1.1.9
   checksum: a970d595bd23c66c880e0ef1817791432dbb7acbb8d44b7e7d0e7a22f4521260d4a83f7f9fd61d44fda4610105577f8f58a60718105fb38352baed612fd79e59
@@ -3309,48 +3125,48 @@
   version: 0.11.0
   resolution: "@pkgjs/parseargs@npm:0.11.0"
   checksum: 6ad6a00fc4f2f2cfc6bff76fb1d88b8ee20bc0601e18ebb01b6d4be583733a860239a521a7fbca73b612e66705078809483549d2b18f370eb346c5155c8e4a0f
   languageName: node
   linkType: hard
 
 "@rjsf/core@npm:^5.1.0":
-  version: 5.8.2
-  resolution: "@rjsf/core@npm:5.8.2"
+  version: 5.9.0
+  resolution: "@rjsf/core@npm:5.9.0"
   dependencies:
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     markdown-to-jsx: ^7.2.1
     nanoid: ^3.3.6
     prop-types: ^15.8.1
   peerDependencies:
     "@rjsf/utils": ^5.8.x
     react: ^16.14.0 || >=17
-  checksum: 05b665f2be100325190da084971749aecb0f1581f80c0f75445e10eb9dffe711fd94dddeb4c8f8723f605c1488d41d66079892b349d56b5b5ae0ff7489a40f87
+  checksum: 52406fcf560af51cb5b45ce95eb826ff1ad4ed1366c70b16b16137455f6b252cef507f76f139524228e12ccf2d49816b3538747431886476574ac2911f29aac1
   languageName: node
   linkType: hard
 
 "@rjsf/utils@npm:^5.1.0":
-  version: 5.8.2
-  resolution: "@rjsf/utils@npm:5.8.2"
+  version: 5.9.0
+  resolution: "@rjsf/utils@npm:5.9.0"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: 0733e8d2e50debdd5a6f75b65f8547b2ebb2c4f3ac26c2a866a7f84993b7e911a50d36230eac21830d869d0dfd705c905d08851f7f29bbdcc075e07ba4c7a1f0
+  checksum: f1a1070539b24763b64631bb8d0d16a504fa46f029775a34e57c47e58b913b07e2869b45de6c993745a6320df3b6571f101abc2d07be59054a971e43facae6ea
   languageName: node
   linkType: hard
 
-"@sinclair/typebox@npm:^0.25.16":
-  version: 0.25.24
-  resolution: "@sinclair/typebox@npm:0.25.24"
-  checksum: 10219c58f40b8414c50b483b0550445e9710d4fe7b2c4dccb9b66533dd90ba8e024acc776026cebe81e87f06fa24b07fdd7bc30dd277eb9cc386ec50151a3026
+"@sinclair/typebox@npm:^0.27.8":
+  version: 0.27.8
+  resolution: "@sinclair/typebox@npm:0.27.8"
+  checksum: 00bd7362a3439021aa1ea51b0e0d0a0e8ca1351a3d54c606b115fdcc49b51b16db6e5f43b4fe7a28c38688523e22a94d49dd31168868b655f0d4d50f032d07a1
   languageName: node
   linkType: hard
 
 "@sinonjs/commons@npm:^3.0.0":
   version: 3.0.0
   resolution: "@sinonjs/commons@npm:3.0.0"
   dependencies:
@@ -3552,17 +3368,17 @@
   version: 1.2.2
   resolution: "@types/minimist@npm:1.2.2"
   checksum: b8da83c66eb4aac0440e64674b19564d9d86c80ae273144db9681e5eeff66f238ade9515f5006ffbfa955ceff8b89ad2bd8ec577d7caee74ba101431fb07045d
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 20.3.2
-  resolution: "@types/node@npm:20.3.2"
-  checksum: 5929ce2b9b12b1e2a2304a0921a953c72a81f5753ad39ac43b99ce6312fbb2b4fb5bc6b60d64a2550704e3223cd5de1299467d36085ac69888899db978f2653a
+  version: 20.4.0
+  resolution: "@types/node@npm:20.4.0"
+  checksum: 8ad632ee131611651fc5f4ac3a47427640e2492ab314fe1c4d0c3b97af71784ef48c53221d5f9922aab4724375dcb4f33137b3107ba2c356d9366216a31678aa
   languageName: node
   linkType: hard
 
 "@types/normalize-package-data@npm:^2.4.0":
   version: 2.4.1
   resolution: "@types/normalize-package-data@npm:2.4.1"
   checksum: e87bccbf11f95035c89a132b52b79ce69a1e3652fe55962363063c9c0dae0fe2477ebc585e03a9652adc6f381d24ba5589cc5e51849df4ced3d3e004a7d40ed5
@@ -4049,19 +3865,19 @@
   bin:
     acorn: bin/acorn
   checksum: 1860f23c2107c910c6177b7b7be71be350db9e1080d814493fae143ae37605189504152d1ba8743ba3178d0b37269ce1ffc42b101547fdc1827078f82671e407
   languageName: node
   linkType: hard
 
 "acorn@npm:^8.1.0, acorn@npm:^8.7.1, acorn@npm:^8.8.1, acorn@npm:^8.8.2":
-  version: 8.9.0
-  resolution: "acorn@npm:8.9.0"
+  version: 8.10.0
+  resolution: "acorn@npm:8.10.0"
   bin:
     acorn: bin/acorn
-  checksum: 25dfb94952386ecfb847e61934de04a4e7c2dc21c2e700fc4e2ef27ce78cb717700c4c4f279cd630bb4774948633c3859fc16063ec8573bda4568e0a312e6744
+  checksum: 538ba38af0cc9e5ef983aee196c4b8b4d87c0c94532334fa7e065b2c8a1f85863467bb774231aae91613fcda5e68740c15d97b1967ae3394d20faddddd8af61d
   languageName: node
   linkType: hard
 
 "agent-base@npm:6, agent-base@npm:^6.0.2":
   version: 6.0.2
   resolution: "agent-base@npm:6.0.2"
   dependencies:
@@ -4121,15 +3937,15 @@
     fast-deep-equal: ^3.1.3
   peerDependencies:
     ajv: ^8.8.2
   checksum: c35193940b853119242c6757787f09ecf89a2c19bcd36d03ed1a615e710d19d450cb448bfda407b939aba54b002368c8bff30529cc50a0536a8e10bcce300421
   languageName: node
   linkType: hard
 
-"ajv@npm:^6.10.0, ajv@npm:^6.12.3, ajv@npm:^6.12.4, ajv@npm:^6.12.5":
+"ajv@npm:^6.10.0, ajv@npm:^6.12.4, ajv@npm:^6.12.5":
   version: 6.12.6
   resolution: "ajv@npm:6.12.6"
   dependencies:
     fast-deep-equal: ^3.1.1
     fast-json-stable-stringify: ^2.0.0
     json-schema-traverse: ^0.4.1
     uri-js: ^4.2.2
@@ -4309,28 +4125,28 @@
 "available-typed-arrays@npm:^1.0.5":
   version: 1.0.5
   resolution: "available-typed-arrays@npm:1.0.5"
   checksum: 20eb47b3cefd7db027b9bbb993c658abd36d4edd3fe1060e83699a03ee275b0c9b216cc076ff3f2db29073225fb70e7613987af14269ac1fe2a19803ccc97f1a
   languageName: node
   linkType: hard
 
-"babel-jest@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "babel-jest@npm:29.5.0"
+"babel-jest@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "babel-jest@npm:29.6.1"
   dependencies:
-    "@jest/transform": ^29.5.0
+    "@jest/transform": ^29.6.1
     "@types/babel__core": ^7.1.14
     babel-plugin-istanbul: ^6.1.1
     babel-preset-jest: ^29.5.0
     chalk: ^4.0.0
     graceful-fs: ^4.2.9
     slash: ^3.0.0
   peerDependencies:
     "@babel/core": ^7.8.0
-  checksum: eafb6d37deb71f0c80bf3c80215aa46732153e5e8bcd73f6ff47d92e5c0c98c8f7f75995d0efec6289c371edad3693cd8fa2367b0661c4deb71a3a7117267ede
+  checksum: bc46cfba468edde91f34a8292501d4448a39fab72d80d7d95f4349feb114fa21becb01def007d6166de7933ab9633bf5b5e1b72ba6ffeaa991f7abf014a2f61d
   languageName: node
   linkType: hard
 
 "babel-plugin-istanbul@npm:^6.1.1":
   version: 6.1.1
   resolution: "babel-plugin-istanbul@npm:6.1.1"
   dependencies:
@@ -4351,47 +4167,47 @@
     "@babel/types": ^7.3.3
     "@types/babel__core": ^7.1.14
     "@types/babel__traverse": ^7.0.6
   checksum: 099b5254073b6bc985b6d2d045ad26fb8ed30ff8ae6404c4fe8ee7cd0e98a820f69e3dfb871c7c65aae0f4b65af77046244c07bb92d49ef9005c90eedf681539
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-corejs2@npm:^0.4.3":
-  version: 0.4.3
-  resolution: "babel-plugin-polyfill-corejs2@npm:0.4.3"
+"babel-plugin-polyfill-corejs2@npm:^0.4.4":
+  version: 0.4.4
+  resolution: "babel-plugin-polyfill-corejs2@npm:0.4.4"
   dependencies:
-    "@babel/compat-data": ^7.17.7
-    "@babel/helper-define-polyfill-provider": ^0.4.0
-    semver: ^6.1.1
+    "@babel/compat-data": ^7.22.6
+    "@babel/helper-define-polyfill-provider": ^0.4.1
+    "@nicolo-ribaudo/semver-v6": ^6.3.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 09ba40b9f8ac66a733628b2f12722bb764bdcc4f9600b93d60f1994418a8f84bc4b1ed9ab07c9d288debbf6210413fdff0721a3a43bd89c7f77adf76b0310adc
+  checksum: 0273f3d74ccbf78086a3b14bb11b1fb94933830f51c576a24229d75b3b91c8b357c3a381d4ab3146abf9b052fa4c33ec9368dd010ada9ee355e1d03ff64e1ff0
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-corejs3@npm:^0.8.1":
-  version: 0.8.1
-  resolution: "babel-plugin-polyfill-corejs3@npm:0.8.1"
+"babel-plugin-polyfill-corejs3@npm:^0.8.2":
+  version: 0.8.2
+  resolution: "babel-plugin-polyfill-corejs3@npm:0.8.2"
   dependencies:
-    "@babel/helper-define-polyfill-provider": ^0.4.0
-    core-js-compat: ^3.30.1
+    "@babel/helper-define-polyfill-provider": ^0.4.1
+    core-js-compat: ^3.31.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: c23a581973c141a4687126cf964981180ef27e3eb0b34b911161db4f5caf9ba7ff60bee0ebe46d650ba09e03a6a3ac2cd6a6ae5f4f5363a148470e5cd8447df2
+  checksum: 0bc3e9e0114eba18f4fea8a9ff5a6016cae73b74cb091290c3f75fd7b9e34e712ee26f95b52d796f283970d7c6256fb01196e3608e8db03f620e3389d56d37c6
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-regenerator@npm:^0.5.0":
-  version: 0.5.0
-  resolution: "babel-plugin-polyfill-regenerator@npm:0.5.0"
+"babel-plugin-polyfill-regenerator@npm:^0.5.1":
+  version: 0.5.1
+  resolution: "babel-plugin-polyfill-regenerator@npm:0.5.1"
   dependencies:
-    "@babel/helper-define-polyfill-provider": ^0.4.0
+    "@babel/helper-define-polyfill-provider": ^0.4.1
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: ef2bcffc7c9a5e4426fc2dbf89bf3a46999a8415c21cd741c3ab3cb4b5ab804aaa3d71ef733f0eda1bcc0b91d9d80f98d33983a66dab9b8bed166ec38f8f8ad1
+  checksum: 85a56d28b34586fbe482225fb6a9592fc793a459c5eea987a3427fb723c7aa2f76916348a9fc5e9ca48754ebf6086cfbb9226f4cd0cf9c6257f94553622562ed
   languageName: node
   linkType: hard
 
 "babel-preset-current-node-syntax@npm:^1.0.0":
   version: 1.0.1
   resolution: "babel-preset-current-node-syntax@npm:1.0.1"
   dependencies:
@@ -4486,15 +4302,15 @@
   resolution: "braces@npm:3.0.2"
   dependencies:
     fill-range: ^7.0.1
   checksum: e2a8e769a863f3d4ee887b5fe21f63193a891c68b612ddb4b68d82d1b5f3ff9073af066c343e9867a393fe4c2555dcb33e89b937195feb9c1613d259edfcd459
   languageName: node
   linkType: hard
 
-"browserslist@npm:^4.14.5, browserslist@npm:^4.21.3, browserslist@npm:^4.21.5":
+"browserslist@npm:^4.14.5, browserslist@npm:^4.21.9":
   version: 4.21.9
   resolution: "browserslist@npm:4.21.9"
   dependencies:
     caniuse-lite: ^1.0.30001503
     electron-to-chromium: ^1.4.431
     node-releases: ^2.0.12
     update-browserslist-db: ^1.0.11
@@ -4605,17 +4421,17 @@
   version: 6.3.0
   resolution: "camelcase@npm:6.3.0"
   checksum: 8c96818a9076434998511251dcb2761a94817ea17dbdc37f47ac080bd088fc62c7369429a19e2178b993497132c8cbcf5cc1f44ba963e76782ba469c0474938d
   languageName: node
   linkType: hard
 
 "caniuse-lite@npm:^1.0.30001503":
-  version: 1.0.30001508
-  resolution: "caniuse-lite@npm:1.0.30001508"
-  checksum: 0a083ed92194d87e608fc35cac65830a27900249729eb8a68e270f866f2c4f83396c2e54eb47b0ef71360682174dd74e2e68eac0b8d407d125611c7bc12488eb
+  version: 1.0.30001513
+  resolution: "caniuse-lite@npm:1.0.30001513"
+  checksum: 7d783f4f40584e7bdeda3f3abc23ffff21f14c37e1fadf1a6b3d2e299727fe9d5a61096101d9d4e4174f881d4ff4c62204fc41f3bc950f4da1b0edfdea025fa4
   languageName: node
   linkType: hard
 
 "chalk@npm:^2.0.0, chalk@npm:^2.3.0, chalk@npm:^2.4.1":
   version: 2.4.2
   resolution: "chalk@npm:2.4.2"
   dependencies:
@@ -4724,17 +4540,17 @@
   version: 4.6.0
   resolution: "co@npm:4.6.0"
   checksum: 5210d9223010eb95b29df06a91116f2cf7c8e0748a9013ed853b53f362ea0e822f1e5bb054fb3cefc645239a4cf966af1f6133a3b43f40d591f3b68ed6cf0510
   languageName: node
   linkType: hard
 
 "collect-v8-coverage@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "collect-v8-coverage@npm:1.0.1"
-  checksum: 4efe0a1fccd517b65478a2364b33dadd0a43fc92a56f59aaece9b6186fe5177b2de471253587de7c91516f07c7268c2f6770b6cbcffc0e0ece353b766ec87e55
+  version: 1.0.2
+  resolution: "collect-v8-coverage@npm:1.0.2"
+  checksum: c10f41c39ab84629d16f9f6137bc8a63d332244383fc368caf2d2052b5e04c20cd1fd70f66fcf4e2422b84c8226598b776d39d5f2d2a51867cc1ed5d1982b4da
   languageName: node
   linkType: hard
 
 "color-convert@npm:^1.9.0":
   version: 1.9.3
   resolution: "color-convert@npm:1.9.3"
   dependencies:
@@ -4866,20 +4682,20 @@
 "convert-source-map@npm:^2.0.0":
   version: 2.0.0
   resolution: "convert-source-map@npm:2.0.0"
   checksum: 63ae9933be5a2b8d4509daca5124e20c14d023c820258e484e32dc324d34c2754e71297c94a05784064ad27615037ef677e3f0c00469fb55f409d2bb21261035
   languageName: node
   linkType: hard
 
-"core-js-compat@npm:^3.30.1, core-js-compat@npm:^3.30.2":
-  version: 3.31.0
-  resolution: "core-js-compat@npm:3.31.0"
+"core-js-compat@npm:^3.31.0":
+  version: 3.31.1
+  resolution: "core-js-compat@npm:3.31.1"
   dependencies:
-    browserslist: ^4.21.5
-  checksum: 5c76ac5e4ab39480391f93a5aef14a2cfa188cda7bd6a7b8532de1f8bc5d89099a5025b2640d2ef70a2928614792363dcbcf8bd254aa7b2e11b85aeed7ac460f
+    browserslist: ^4.21.9
+  checksum: 9a16d6992621f4e099169297381a28d5712cdef7df1fa85352a7c285a5885d5d7a117ec2eae9ad715ed88c7cc774787a22cdb8aceababf6775fbc8b0cbeccdb7
   languageName: node
   linkType: hard
 
 "cosmiconfig@npm:^7.1.0":
   version: 7.1.0
   resolution: "cosmiconfig@npm:7.1.0"
   dependencies:
@@ -5065,15 +4881,15 @@
 "dedent@npm:^0.7.0":
   version: 0.7.0
   resolution: "dedent@npm:0.7.0"
   checksum: 87de191050d9a40dd70cad01159a0bcf05ecb59750951242070b6abf9569088684880d00ba92a955b4058804f16eeaf91d604f283929b4f614d181cd7ae633d2
   languageName: node
   linkType: hard
 
-"deep-is@npm:^0.1.3, deep-is@npm:~0.1.3":
+"deep-is@npm:^0.1.3":
   version: 0.1.4
   resolution: "deep-is@npm:0.1.4"
   checksum: edb65dd0d7d1b9c40b2f50219aef30e116cedd6fc79290e740972c132c09106d2e80aa0bc8826673dd5a00222d4179c84b36a790eef63a4c4bca75a37ef90804
   languageName: node
   linkType: hard
 
 "deepmerge@npm:^4.2.2":
@@ -5219,17 +5035,17 @@
   version: 0.2.0
   resolution: "eastasianwidth@npm:0.2.0"
   checksum: 7d00d7cd8e49b9afa762a813faac332dee781932d6f2c848dc348939c4253f1d4564341b7af1d041853bc3f32c2ef141b58e0a4d9862c17a7f08f68df1e0f1ed
   languageName: node
   linkType: hard
 
 "electron-to-chromium@npm:^1.4.431":
-  version: 1.4.441
-  resolution: "electron-to-chromium@npm:1.4.441"
-  checksum: 807a3659daf9ac376c3b7a2d19965e186a8c8a4b2498a911c96bc80f43701ec6e9268c382b4e3155ce0def4c9e35071de6a0506dd69b822bd9592ad8de71bc91
+  version: 1.4.453
+  resolution: "electron-to-chromium@npm:1.4.453"
+  checksum: dcd354388b2b60fb0158a6daf7a3a93796b9f6e0045bc507021bcbbf72790cb94c5bb549f699150e18d090321bca0583d729bc479d2d48a0c94a29b1a2f0165e
   languageName: node
   linkType: hard
 
 "emittery@npm:^0.13.1":
   version: 0.13.1
   resolution: "emittery@npm:0.13.1"
   checksum: 2b089ab6306f38feaabf4f6f02792f9ec85fc054fda79f44f6790e61bbf6bc4e1616afb9b232e0c5ec5289a8a452f79bfa6d905a6fd64e94b49981f0934001c6
@@ -5494,29 +5310,28 @@
   version: 4.0.0
   resolution: "escape-string-regexp@npm:4.0.0"
   checksum: 98b48897d93060f2322108bf29db0feba7dd774be96cd069458d1453347b25ce8682ecc39859d4bca2203cc0ab19c237bcc71755eff49a0f8d90beadeeba5cc5
   languageName: node
   linkType: hard
 
 "escodegen@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "escodegen@npm:2.0.0"
+  version: 2.1.0
+  resolution: "escodegen@npm:2.1.0"
   dependencies:
     esprima: ^4.0.1
     estraverse: ^5.2.0
     esutils: ^2.0.2
-    optionator: ^0.8.1
     source-map: ~0.6.1
   dependenciesMeta:
     source-map:
       optional: true
   bin:
     escodegen: bin/escodegen.js
     esgenerate: bin/esgenerate.js
-  checksum: 5aa6b2966fafe0545e4e77936300cc94ad57cfe4dc4ebff9950492eaba83eef634503f12d7e3cbd644ecc1bab388ad0e92b06fd32222c9281a75d1cf02ec6cef
+  checksum: 096696407e161305cd05aebb95134ad176708bc5cb13d0dcc89a5fcbb959b8ed757e7f2591a5f8036f8f4952d4a724de0df14cd419e29212729fa6df5ce16bf6
   languageName: node
   linkType: hard
 
 "eslint-config-prettier@npm:^6.15.0":
   version: 6.15.0
   resolution: "eslint-config-prettier@npm:6.15.0"
   dependencies:
@@ -5735,24 +5550,25 @@
 "exit@npm:^0.1.2":
   version: 0.1.2
   resolution: "exit@npm:0.1.2"
   checksum: abc407f07a875c3961e4781dfcb743b58d6c93de9ab263f4f8c9d23bb6da5f9b7764fc773f86b43dd88030444d5ab8abcb611cb680fba8ca075362b77114bba3
   languageName: node
   linkType: hard
 
-"expect@npm:^29.0.0, expect@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "expect@npm:29.5.0"
+"expect@npm:^29.0.0, expect@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "expect@npm:29.6.1"
   dependencies:
-    "@jest/expect-utils": ^29.5.0
+    "@jest/expect-utils": ^29.6.1
+    "@types/node": "*"
     jest-get-type: ^29.4.3
-    jest-matcher-utils: ^29.5.0
-    jest-message-util: ^29.5.0
-    jest-util: ^29.5.0
-  checksum: 58f70b38693df6e5c6892db1bcd050f0e518d6f785175dc53917d4fa6a7359a048e5690e19ddcb96b65c4493881dd89a3dabdab1a84dfa55c10cdbdabf37b2d7
+    jest-matcher-utils: ^29.6.1
+    jest-message-util: ^29.6.1
+    jest-util: ^29.6.1
+  checksum: 4e712e52c90f6c54e748fd2876be33c43ada6a59088ddf6a1acb08b18b3b97b3a672124684abe32599986d2f2a438d5afad148837ee06ea386d2a4bf0348de78
   languageName: node
   linkType: hard
 
 "exponential-backoff@npm:^3.1.1":
   version: 3.1.1
   resolution: "exponential-backoff@npm:3.1.1"
   checksum: 3d21519a4f8207c99f7457287291316306255a328770d320b401114ec8481986e4e467e854cb9914dd965e0a1ca810a23ccb559c642c88f4c7f55c55778a9b48
@@ -5779,34 +5595,34 @@
   version: 1.3.0
   resolution: "fast-diff@npm:1.3.0"
   checksum: d22d371b994fdc8cce9ff510d7b8dc4da70ac327bcba20df607dd5b9cae9f908f4d1028f5fe467650f058d1e7270235ae0b8230809a262b4df587a3b3aa216c3
   languageName: node
   linkType: hard
 
 "fast-glob@npm:^3.2.12, fast-glob@npm:^3.2.9":
-  version: 3.2.12
-  resolution: "fast-glob@npm:3.2.12"
+  version: 3.3.0
+  resolution: "fast-glob@npm:3.3.0"
   dependencies:
     "@nodelib/fs.stat": ^2.0.2
     "@nodelib/fs.walk": ^1.2.3
     glob-parent: ^5.1.2
     merge2: ^1.3.0
     micromatch: ^4.0.4
-  checksum: 0b1990f6ce831c7e28c4d505edcdaad8e27e88ab9fa65eedadb730438cfc7cde4910d6c975d6b7b8dc8a73da4773702ebcfcd6e3518e73938bb1383badfe01c2
+  checksum: 20df62be28eb5426fe8e40e0d05601a63b1daceb7c3d87534afcad91bdcf1e4b1743cf2d5247d6e225b120b46df0b9053a032b2691ba34ee121e033acd81f547
   languageName: node
   linkType: hard
 
 "fast-json-stable-stringify@npm:2.x, fast-json-stable-stringify@npm:^2.0.0, fast-json-stable-stringify@npm:^2.1.0":
   version: 2.1.0
   resolution: "fast-json-stable-stringify@npm:2.1.0"
   checksum: b191531e36c607977e5b1c47811158733c34ccb3bfde92c44798929e9b4154884378536d26ad90dfecd32e1ffc09c545d23535ad91b3161a27ddbb8ebe0cbecb
   languageName: node
   linkType: hard
 
-"fast-levenshtein@npm:^2.0.6, fast-levenshtein@npm:~2.0.6":
+"fast-levenshtein@npm:^2.0.6":
   version: 2.0.6
   resolution: "fast-levenshtein@npm:2.0.6"
   checksum: 92cfec0a8dfafd9c7a15fba8f2cc29cd0b62b85f056d99ce448bbcd9f708e18ab2764bda4dd5158364f4145a7c72788538994f0d1787b956ef0d1062b0f7c24c
   languageName: node
   linkType: hard
 
 "fastest-levenshtein@npm:^1.0.12, fastest-levenshtein@npm:^1.0.16":
@@ -6115,25 +5931,25 @@
   version: 0.4.1
   resolution: "glob-to-regexp@npm:0.4.1"
   checksum: e795f4e8f06d2a15e86f76e4d92751cf8bbfcf0157cea5c2f0f35678a8195a750b34096b1256e436f0cebc1883b5ff0888c47348443e69546a5a87f9e1eb1167
   languageName: node
   linkType: hard
 
 "glob@npm:^10.2.2":
-  version: 10.3.0
-  resolution: "glob@npm:10.3.0"
+  version: 10.3.1
+  resolution: "glob@npm:10.3.1"
   dependencies:
     foreground-child: ^3.1.0
     jackspeak: ^2.0.3
     minimatch: ^9.0.1
     minipass: ^5.0.0 || ^6.0.2
-    path-scurry: ^1.7.0
+    path-scurry: ^1.10.0
   bin:
     glob: dist/cjs/src/bin.js
-  checksum: 6fa4ac0a86ffec1c5715a2e6fbdd63e1e7f1c2c8f5db08cc3256cdfcb81093678e7c80a3d100b502a1b9d141369ecf87bc24fe2bcb72acec7b14626d358a4eb0
+  checksum: 19c8c2805658b1002fecf0722cd609a33153d756a0d5260676bd0e9c5e6ef889ec9cce6d3dac0411aa90bce8de3d14f25b6f5589a3292582cccbfeddd0e98cc4
   languageName: node
   linkType: hard
 
 "glob@npm:^7.1.3, glob@npm:^7.1.4, glob@npm:^7.1.6":
   version: 7.2.3
   resolution: "glob@npm:7.2.3"
   dependencies:
@@ -6941,203 +6757,203 @@
   dependencies:
     execa: ^5.0.0
     p-limit: ^3.1.0
   checksum: a67a7cb3c11f8f92bd1b7c79e84f724cbd11a9ad51f3cdadafe3ce7ee3c79ee50dbea128f920f5fddc807e9e4e83f5462143094391feedd959a77dd20ab96cf3
   languageName: node
   linkType: hard
 
-"jest-circus@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-circus@npm:29.5.0"
-  dependencies:
-    "@jest/environment": ^29.5.0
-    "@jest/expect": ^29.5.0
-    "@jest/test-result": ^29.5.0
-    "@jest/types": ^29.5.0
+"jest-circus@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-circus@npm:29.6.1"
+  dependencies:
+    "@jest/environment": ^29.6.1
+    "@jest/expect": ^29.6.1
+    "@jest/test-result": ^29.6.1
+    "@jest/types": ^29.6.1
     "@types/node": "*"
     chalk: ^4.0.0
     co: ^4.6.0
     dedent: ^0.7.0
     is-generator-fn: ^2.0.0
-    jest-each: ^29.5.0
-    jest-matcher-utils: ^29.5.0
-    jest-message-util: ^29.5.0
-    jest-runtime: ^29.5.0
-    jest-snapshot: ^29.5.0
-    jest-util: ^29.5.0
+    jest-each: ^29.6.1
+    jest-matcher-utils: ^29.6.1
+    jest-message-util: ^29.6.1
+    jest-runtime: ^29.6.1
+    jest-snapshot: ^29.6.1
+    jest-util: ^29.6.1
     p-limit: ^3.1.0
-    pretty-format: ^29.5.0
+    pretty-format: ^29.6.1
     pure-rand: ^6.0.0
     slash: ^3.0.0
     stack-utils: ^2.0.3
-  checksum: 44ff5d06acedae6de6c866e20e3b61f83e29ab94cf9f960826e7e667de49c12dd9ab9dffd7fa3b7d1f9688a8b5bfb1ebebadbea69d9ed0d3f66af4a0ff8c2b27
+  checksum: f3e39a74b601929448df92037f0599978d4d7a4b8f636f64e8020533d2d2b2f669d6729c80c6efed69341ca26753e5061e9787a0acd6c70af2127a94375ebb76
   languageName: node
   linkType: hard
 
-"jest-cli@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-cli@npm:29.5.0"
+"jest-cli@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-cli@npm:29.6.1"
   dependencies:
-    "@jest/core": ^29.5.0
-    "@jest/test-result": ^29.5.0
-    "@jest/types": ^29.5.0
+    "@jest/core": ^29.6.1
+    "@jest/test-result": ^29.6.1
+    "@jest/types": ^29.6.1
     chalk: ^4.0.0
     exit: ^0.1.2
     graceful-fs: ^4.2.9
     import-local: ^3.0.2
-    jest-config: ^29.5.0
-    jest-util: ^29.5.0
-    jest-validate: ^29.5.0
+    jest-config: ^29.6.1
+    jest-util: ^29.6.1
+    jest-validate: ^29.6.1
     prompts: ^2.0.1
     yargs: ^17.3.1
   peerDependencies:
     node-notifier: ^8.0.1 || ^9.0.0 || ^10.0.0
   peerDependenciesMeta:
     node-notifier:
       optional: true
   bin:
     jest: bin/jest.js
-  checksum: 39897bbbc0f0d8a6b975ab12fd13887eaa28d92e3dee9e0173a5cb913ae8cc2ae46e090d38c6d723e84d9d6724429cd08685b4e505fa447d31ca615630c7dbba
+  checksum: f5854ffea977b9a12520ea71f8d0cc8a626cbb93d7e1e6eea18a2a1f2b25f70f1b6b08a89f11b4dc7dd36a1776a9ac2cf8ec5c7998086f913ee690c06c07c949
   languageName: node
   linkType: hard
 
-"jest-config@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-config@npm:29.5.0"
+"jest-config@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-config@npm:29.6.1"
   dependencies:
     "@babel/core": ^7.11.6
-    "@jest/test-sequencer": ^29.5.0
-    "@jest/types": ^29.5.0
-    babel-jest: ^29.5.0
+    "@jest/test-sequencer": ^29.6.1
+    "@jest/types": ^29.6.1
+    babel-jest: ^29.6.1
     chalk: ^4.0.0
     ci-info: ^3.2.0
     deepmerge: ^4.2.2
     glob: ^7.1.3
     graceful-fs: ^4.2.9
-    jest-circus: ^29.5.0
-    jest-environment-node: ^29.5.0
+    jest-circus: ^29.6.1
+    jest-environment-node: ^29.6.1
     jest-get-type: ^29.4.3
     jest-regex-util: ^29.4.3
-    jest-resolve: ^29.5.0
-    jest-runner: ^29.5.0
-    jest-util: ^29.5.0
-    jest-validate: ^29.5.0
+    jest-resolve: ^29.6.1
+    jest-runner: ^29.6.1
+    jest-util: ^29.6.1
+    jest-validate: ^29.6.1
     micromatch: ^4.0.4
     parse-json: ^5.2.0
-    pretty-format: ^29.5.0
+    pretty-format: ^29.6.1
     slash: ^3.0.0
     strip-json-comments: ^3.1.1
   peerDependencies:
     "@types/node": "*"
     ts-node: ">=9.0.0"
   peerDependenciesMeta:
     "@types/node":
       optional: true
     ts-node:
       optional: true
-  checksum: c37c4dab964c54ab293d4e302d40b09687037ac9d00b88348ec42366970747feeaf265e12e3750cd3660b40c518d4031335eda11ac10b70b10e60797ebbd4b9c
+  checksum: 3a30afeb28cc5658ef9cd95f2551ab8a29641bb6d377eb239cba8e7522eb4611c9a98cdcf173d87f5ad7b5e1ad242c3cd5434a260107bd3c7e8305d05023e05c
   languageName: node
   linkType: hard
 
-"jest-diff@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-diff@npm:29.5.0"
+"jest-diff@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-diff@npm:29.6.1"
   dependencies:
     chalk: ^4.0.0
     diff-sequences: ^29.4.3
     jest-get-type: ^29.4.3
-    pretty-format: ^29.5.0
-  checksum: dfd0f4a299b5d127779c76b40106c37854c89c3e0785098c717d52822d6620d227f6234c3a9291df204d619e799e3654159213bf93220f79c8e92a55475a3d39
+    pretty-format: ^29.6.1
+  checksum: c6350178ca27d92c7fd879790fb2525470c1ff1c5d29b1834a240fecd26c6904fb470ebddb98dc96dd85389c56c3b50e6965a1f5203e9236d213886ed9806219
   languageName: node
   linkType: hard
 
 "jest-docblock@npm:^29.4.3":
   version: 29.4.3
   resolution: "jest-docblock@npm:29.4.3"
   dependencies:
     detect-newline: ^3.0.0
   checksum: e0e9df1485bb8926e5b33478cdf84b3387d9caf3658e7dc1eaa6dc34cb93dea0d2d74797f6e940f0233a88f3dadd60957f2288eb8f95506361f85b84bf8661df
   languageName: node
   linkType: hard
 
-"jest-each@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-each@npm:29.5.0"
+"jest-each@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-each@npm:29.6.1"
   dependencies:
-    "@jest/types": ^29.5.0
+    "@jest/types": ^29.6.1
     chalk: ^4.0.0
     jest-get-type: ^29.4.3
-    jest-util: ^29.5.0
-    pretty-format: ^29.5.0
-  checksum: b8b297534d25834c5d4e31e4c687359787b1e402519e42664eb704cc3a12a7a91a017565a75acb02e8cf9afd3f4eef3350bd785276bec0900184641b765ff7a5
+    jest-util: ^29.6.1
+    pretty-format: ^29.6.1
+  checksum: 9d2ea7ed5326ee8c22523b22c66c85fe73754ea39f9b389881956508ee441392c61072a5fbf673e39beddd31d011bb94acae3edc77053ba4f9aa5c060114a5c8
   languageName: node
   linkType: hard
 
 "jest-environment-jsdom@npm:^29.3.0":
-  version: 29.5.0
-  resolution: "jest-environment-jsdom@npm:29.5.0"
+  version: 29.6.1
+  resolution: "jest-environment-jsdom@npm:29.6.1"
   dependencies:
-    "@jest/environment": ^29.5.0
-    "@jest/fake-timers": ^29.5.0
-    "@jest/types": ^29.5.0
+    "@jest/environment": ^29.6.1
+    "@jest/fake-timers": ^29.6.1
+    "@jest/types": ^29.6.1
     "@types/jsdom": ^20.0.0
     "@types/node": "*"
-    jest-mock: ^29.5.0
-    jest-util: ^29.5.0
+    jest-mock: ^29.6.1
+    jest-util: ^29.6.1
     jsdom: ^20.0.0
   peerDependencies:
     canvas: ^2.5.0
   peerDependenciesMeta:
     canvas:
       optional: true
-  checksum: 3df7fc85275711f20b483ac8cd8c04500704ed0f69791eb55c574b38f5a39470f03d775cf20c1025bc1884916ac0573aa2fa4db1bb74225bc7fdd95ba97ad0da
+  checksum: e8a9bff00a011235b004699f34bc85b18fdac82049513410cbf2dc1c2dd332bc1b4f108976412df1d29f2fa8bf0360aaf84eb0f5b4db1db2fb7fc7155dc14be7
   languageName: node
   linkType: hard
 
-"jest-environment-node@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-environment-node@npm:29.5.0"
+"jest-environment-node@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-environment-node@npm:29.6.1"
   dependencies:
-    "@jest/environment": ^29.5.0
-    "@jest/fake-timers": ^29.5.0
-    "@jest/types": ^29.5.0
+    "@jest/environment": ^29.6.1
+    "@jest/fake-timers": ^29.6.1
+    "@jest/types": ^29.6.1
     "@types/node": "*"
-    jest-mock: ^29.5.0
-    jest-util: ^29.5.0
-  checksum: 57981911cc20a4219b0da9e22b2e3c9f31b505e43f78e61c899e3227ded455ce1a3a9483842c69cfa4532f02cfb536ae0995bf245f9211608edacfc1e478d411
+    jest-mock: ^29.6.1
+    jest-util: ^29.6.1
+  checksum: a50287e1ff29d131646bd09acc3222ac6ea0ad61e86bf73851d318ef2be0633a421b8558c4a15ddc67e0ffcfc32da7f6a0d8a2ddbfa85453837899dec88d256c
   languageName: node
   linkType: hard
 
 "jest-get-type@npm:^29.4.3":
   version: 29.4.3
   resolution: "jest-get-type@npm:29.4.3"
   checksum: 6ac7f2dde1c65e292e4355b6c63b3a4897d7e92cb4c8afcf6d397f2682f8080e094c8b0b68205a74d269882ec06bf696a9de6cd3e1b7333531e5ed7b112605ce
   languageName: node
   linkType: hard
 
-"jest-haste-map@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-haste-map@npm:29.5.0"
+"jest-haste-map@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-haste-map@npm:29.6.1"
   dependencies:
-    "@jest/types": ^29.5.0
+    "@jest/types": ^29.6.1
     "@types/graceful-fs": ^4.1.3
     "@types/node": "*"
     anymatch: ^3.0.3
     fb-watchman: ^2.0.0
     fsevents: ^2.3.2
     graceful-fs: ^4.2.9
     jest-regex-util: ^29.4.3
-    jest-util: ^29.5.0
-    jest-worker: ^29.5.0
+    jest-util: ^29.6.1
+    jest-worker: ^29.6.1
     micromatch: ^4.0.4
     walker: ^1.0.8
   dependenciesMeta:
     fsevents:
       optional: true
-  checksum: 3828ff7783f168e34be2c63887f82a01634261f605dcae062d83f979a61c37739e21b9607ecb962256aea3fbe5a530a1acee062d0026fcb47c607c12796cf3b7
+  checksum: 7c74d5a0f6aafa9f4e60fae7949d4774770c0243fb529c24f2f4c81229db479fa318dc8b81e8d226865aef1d600af10bd8404dd208e802318434b46f75d5d869
   languageName: node
   linkType: hard
 
 "jest-junit@npm:^15.0.0":
   version: 15.0.0
   resolution: "jest-junit@npm:15.0.0"
   dependencies:
@@ -7145,61 +6961,61 @@
     strip-ansi: ^6.0.1
     uuid: ^8.3.2
     xml: ^1.0.1
   checksum: e8fe4d2f2ab843383ac41820a6fe495739d154ec435cd44ba590b44ec7fd62095676f3eef13f98392f81d4a3727ea58b4f4fad231fe367ac31243952b9ad716f
   languageName: node
   linkType: hard
 
-"jest-leak-detector@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-leak-detector@npm:29.5.0"
+"jest-leak-detector@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-leak-detector@npm:29.6.1"
   dependencies:
     jest-get-type: ^29.4.3
-    pretty-format: ^29.5.0
-  checksum: 0fb845da7ac9cdfc9b3b2e35f6f623a41c547d7dc0103ceb0349013459d00de5870b5689a625e7e37f9644934b40e8f1dcdd5422d14d57470600350364676313
+    pretty-format: ^29.6.1
+  checksum: 5122d40c248effaede4c9ee3a99046a3f30088fef7bfc4af534678b432455161399357af46deb6423de7e05c6597920d6ee8cd570e26048886a90d541334f8c8
   languageName: node
   linkType: hard
 
-"jest-matcher-utils@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-matcher-utils@npm:29.5.0"
+"jest-matcher-utils@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-matcher-utils@npm:29.6.1"
   dependencies:
     chalk: ^4.0.0
-    jest-diff: ^29.5.0
+    jest-diff: ^29.6.1
     jest-get-type: ^29.4.3
-    pretty-format: ^29.5.0
-  checksum: 1d3e8c746e484a58ce194e3aad152eff21fd0896e8b8bf3d4ab1a4e2cbfed95fb143646f4ad9fdf6e42212b9e8fc033268b58e011b044a9929df45485deb5ac9
+    pretty-format: ^29.6.1
+  checksum: d2efa6aed6e4820758b732b9fefd315c7fa4508ee690da656e1c5ac4c1a0f4cee5b04c9719ee1fda9aeb883b4209186c145089ced521e715b9fa70afdfa4a9c6
   languageName: node
   linkType: hard
 
-"jest-message-util@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-message-util@npm:29.5.0"
+"jest-message-util@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-message-util@npm:29.6.1"
   dependencies:
     "@babel/code-frame": ^7.12.13
-    "@jest/types": ^29.5.0
+    "@jest/types": ^29.6.1
     "@types/stack-utils": ^2.0.0
     chalk: ^4.0.0
     graceful-fs: ^4.2.9
     micromatch: ^4.0.4
-    pretty-format: ^29.5.0
+    pretty-format: ^29.6.1
     slash: ^3.0.0
     stack-utils: ^2.0.3
-  checksum: daddece6bbf846eb6a2ab9be9f2446e54085bef4e5cecd13d2a538fa9c01cb89d38e564c6b74fd8e12d37ed9eface8a362240ae9f21d68b214590631e7a0d8bf
+  checksum: 3e7cb2ff087fe72255292e151d24e4fbb4cd6134885c0a67a4b302f233fe4110bf7580b176f427f05ad7550eb878ed94237209785d09d659a7d171ffa59c068f
   languageName: node
   linkType: hard
 
-"jest-mock@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-mock@npm:29.5.0"
+"jest-mock@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-mock@npm:29.6.1"
   dependencies:
-    "@jest/types": ^29.5.0
+    "@jest/types": ^29.6.1
     "@types/node": "*"
-    jest-util: ^29.5.0
-  checksum: 2a9cf07509948fa8608898c445f04fe4dd6e2049ff431e5531eee028c808d3ba3c67f226ac87b0cf383feaa1055776900d197c895e89783016886ac17a4ff10c
+    jest-util: ^29.6.1
+  checksum: 5e902f1a7eba1eb1a64eb6c19947fe1316834359d9869d0e2644d8979b9cad0465885dc4c9909c471888cddeea835c938cec6263d386d3d1aad720fc74e52ea1
   languageName: node
   linkType: hard
 
 "jest-pnp-resolver@npm:^1.2.2":
   version: 1.2.3
   resolution: "jest-pnp-resolver@npm:1.2.3"
   peerDependencies:
@@ -7214,214 +7030,212 @@
 "jest-regex-util@npm:^29.4.3":
   version: 29.4.3
   resolution: "jest-regex-util@npm:29.4.3"
   checksum: 96fc7fc28cd4dd73a63c13a526202c4bd8b351d4e5b68b1a2a2c88da3308c2a16e26feaa593083eb0bac38cca1aa9dd05025412e7de013ba963fb8e66af22b8a
   languageName: node
   linkType: hard
 
-"jest-resolve-dependencies@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-resolve-dependencies@npm:29.5.0"
+"jest-resolve-dependencies@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-resolve-dependencies@npm:29.6.1"
   dependencies:
     jest-regex-util: ^29.4.3
-    jest-snapshot: ^29.5.0
-  checksum: 479d2e5365d58fe23f2b87001e2e0adcbffe0147700e85abdec8f14b9703b0a55758c1929a9989e3f5d5e954fb88870ea4bfa04783523b664562fcf5f10b0edf
+    jest-snapshot: ^29.6.1
+  checksum: cee0a0fe53fd4531492a526b6ccd32377baad1eff6e6c124f04e9dc920219fd23fd39be88bb9551ee68d5fe92a3af627b423c9bc65a2aa0ac8a223c0e74dbbbb
   languageName: node
   linkType: hard
 
-"jest-resolve@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-resolve@npm:29.5.0"
+"jest-resolve@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-resolve@npm:29.6.1"
   dependencies:
     chalk: ^4.0.0
     graceful-fs: ^4.2.9
-    jest-haste-map: ^29.5.0
+    jest-haste-map: ^29.6.1
     jest-pnp-resolver: ^1.2.2
-    jest-util: ^29.5.0
-    jest-validate: ^29.5.0
+    jest-util: ^29.6.1
+    jest-validate: ^29.6.1
     resolve: ^1.20.0
     resolve.exports: ^2.0.0
     slash: ^3.0.0
-  checksum: 9a125f3cf323ceef512089339d35f3ee37f79fe16a831fb6a26773ea6a229b9e490d108fec7af334142e91845b5996de8e7cdd85a4d8d617078737d804e29c8f
+  checksum: 9ce979a0f4a751bea58caea76415112df2a3f4d58e294019872244728aadd001f0ec20c873a3c805dd8f7c762143b3c14d00f87d124ed87c9981fbf8723090ef
   languageName: node
   linkType: hard
 
-"jest-runner@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-runner@npm:29.5.0"
+"jest-runner@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-runner@npm:29.6.1"
   dependencies:
-    "@jest/console": ^29.5.0
-    "@jest/environment": ^29.5.0
-    "@jest/test-result": ^29.5.0
-    "@jest/transform": ^29.5.0
-    "@jest/types": ^29.5.0
+    "@jest/console": ^29.6.1
+    "@jest/environment": ^29.6.1
+    "@jest/test-result": ^29.6.1
+    "@jest/transform": ^29.6.1
+    "@jest/types": ^29.6.1
     "@types/node": "*"
     chalk: ^4.0.0
     emittery: ^0.13.1
     graceful-fs: ^4.2.9
     jest-docblock: ^29.4.3
-    jest-environment-node: ^29.5.0
-    jest-haste-map: ^29.5.0
-    jest-leak-detector: ^29.5.0
-    jest-message-util: ^29.5.0
-    jest-resolve: ^29.5.0
-    jest-runtime: ^29.5.0
-    jest-util: ^29.5.0
-    jest-watcher: ^29.5.0
-    jest-worker: ^29.5.0
+    jest-environment-node: ^29.6.1
+    jest-haste-map: ^29.6.1
+    jest-leak-detector: ^29.6.1
+    jest-message-util: ^29.6.1
+    jest-resolve: ^29.6.1
+    jest-runtime: ^29.6.1
+    jest-util: ^29.6.1
+    jest-watcher: ^29.6.1
+    jest-worker: ^29.6.1
     p-limit: ^3.1.0
     source-map-support: 0.5.13
-  checksum: 437dea69c5dddca22032259787bac74790d5a171c9d804711415f31e5d1abfb64fa52f54a9015bb17a12b858fd0cf3f75ef6f3c9e94255a8596e179f707229c4
+  checksum: 0e4dbda26669ae31fee32f8a62b3119bba510f2d17a098d6157b48a73ed2fc9842405bf893f3045c12b3632c7c0e3399fb22684b18ab5566aff4905b26c79a9a
   languageName: node
   linkType: hard
 
-"jest-runtime@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-runtime@npm:29.5.0"
+"jest-runtime@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-runtime@npm:29.6.1"
   dependencies:
-    "@jest/environment": ^29.5.0
-    "@jest/fake-timers": ^29.5.0
-    "@jest/globals": ^29.5.0
-    "@jest/source-map": ^29.4.3
-    "@jest/test-result": ^29.5.0
-    "@jest/transform": ^29.5.0
-    "@jest/types": ^29.5.0
+    "@jest/environment": ^29.6.1
+    "@jest/fake-timers": ^29.6.1
+    "@jest/globals": ^29.6.1
+    "@jest/source-map": ^29.6.0
+    "@jest/test-result": ^29.6.1
+    "@jest/transform": ^29.6.1
+    "@jest/types": ^29.6.1
     "@types/node": "*"
     chalk: ^4.0.0
     cjs-module-lexer: ^1.0.0
     collect-v8-coverage: ^1.0.0
     glob: ^7.1.3
     graceful-fs: ^4.2.9
-    jest-haste-map: ^29.5.0
-    jest-message-util: ^29.5.0
-    jest-mock: ^29.5.0
+    jest-haste-map: ^29.6.1
+    jest-message-util: ^29.6.1
+    jest-mock: ^29.6.1
     jest-regex-util: ^29.4.3
-    jest-resolve: ^29.5.0
-    jest-snapshot: ^29.5.0
-    jest-util: ^29.5.0
+    jest-resolve: ^29.6.1
+    jest-snapshot: ^29.6.1
+    jest-util: ^29.6.1
     slash: ^3.0.0
     strip-bom: ^4.0.0
-  checksum: 7af27bd9d54cf1c5735404cf8d76c6509d5610b1ec0106a21baa815c1aff15d774ce534ac2834bc440dccfe6348bae1885fd9a806f23a94ddafdc0f5bae4b09d
+  checksum: 7c360c9694467d996f3d6d914fefa0e7bda554adda8c2b9fba31546dba663d71a64eda103ff68120a2422f3c16db8f0bc2c445923fe8fb934f37e53ef74fb429
   languageName: node
   linkType: hard
 
-"jest-snapshot@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-snapshot@npm:29.5.0"
+"jest-snapshot@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-snapshot@npm:29.6.1"
   dependencies:
     "@babel/core": ^7.11.6
     "@babel/generator": ^7.7.2
     "@babel/plugin-syntax-jsx": ^7.7.2
     "@babel/plugin-syntax-typescript": ^7.7.2
-    "@babel/traverse": ^7.7.2
     "@babel/types": ^7.3.3
-    "@jest/expect-utils": ^29.5.0
-    "@jest/transform": ^29.5.0
-    "@jest/types": ^29.5.0
-    "@types/babel__traverse": ^7.0.6
+    "@jest/expect-utils": ^29.6.1
+    "@jest/transform": ^29.6.1
+    "@jest/types": ^29.6.1
     "@types/prettier": ^2.1.5
     babel-preset-current-node-syntax: ^1.0.0
     chalk: ^4.0.0
-    expect: ^29.5.0
+    expect: ^29.6.1
     graceful-fs: ^4.2.9
-    jest-diff: ^29.5.0
+    jest-diff: ^29.6.1
     jest-get-type: ^29.4.3
-    jest-matcher-utils: ^29.5.0
-    jest-message-util: ^29.5.0
-    jest-util: ^29.5.0
+    jest-matcher-utils: ^29.6.1
+    jest-message-util: ^29.6.1
+    jest-util: ^29.6.1
     natural-compare: ^1.4.0
-    pretty-format: ^29.5.0
-    semver: ^7.3.5
-  checksum: fe5df54122ed10eed625de6416a45bc4958d5062b018f05b152bf9785ab7f355dcd55e40cf5da63895bf8278f8d7b2bb4059b2cfbfdee18f509d455d37d8aa2b
+    pretty-format: ^29.6.1
+    semver: ^7.5.3
+  checksum: e8f69d1fd4a29d354d4dca9eb2a22674b300f8ef509e4f1e75337c880414a00d2bdc9d3849a6855dbb5a76bfbe74603f33435378a3877e69f0838e4cc2244350
   languageName: node
   linkType: hard
 
-"jest-util@npm:^29.0.0, jest-util@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-util@npm:29.5.0"
+"jest-util@npm:^29.0.0, jest-util@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-util@npm:29.6.1"
   dependencies:
-    "@jest/types": ^29.5.0
+    "@jest/types": ^29.6.1
     "@types/node": "*"
     chalk: ^4.0.0
     ci-info: ^3.2.0
     graceful-fs: ^4.2.9
     picomatch: ^2.2.3
-  checksum: fd9212950d34d2ecad8c990dda0d8ea59a8a554b0c188b53ea5d6c4a0829a64f2e1d49e6e85e812014933d17426d7136da4785f9cf76fff1799de51b88bc85d3
+  checksum: fc553556c1350c443449cadaba5fb9d604628e8b5ceb6ceaf4e7e08975b24277d0a14bf2e0f956024e03c23e556fcb074659423422a06fbedf2ab52978697ac7
   languageName: node
   linkType: hard
 
-"jest-validate@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-validate@npm:29.5.0"
+"jest-validate@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-validate@npm:29.6.1"
   dependencies:
-    "@jest/types": ^29.5.0
+    "@jest/types": ^29.6.1
     camelcase: ^6.2.0
     chalk: ^4.0.0
     jest-get-type: ^29.4.3
     leven: ^3.1.0
-    pretty-format: ^29.5.0
-  checksum: 43ca5df7cb75572a254ac3e92fbbe7be6b6a1be898cc1e887a45d55ea003f7a112717d814a674d37f9f18f52d8de40873c8f084f17664ae562736c78dd44c6a1
+    pretty-format: ^29.6.1
+  checksum: d2491f3f33d9bbc2dcaaa6acbff26f257b59c5eeceb65a52a9c1cec2f679b836ec2a4658b7004c0ef9d90cd0d9bd664e41d5ed6900f932bea742dd8e6b85e7f1
   languageName: node
   linkType: hard
 
-"jest-watcher@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-watcher@npm:29.5.0"
+"jest-watcher@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-watcher@npm:29.6.1"
   dependencies:
-    "@jest/test-result": ^29.5.0
-    "@jest/types": ^29.5.0
+    "@jest/test-result": ^29.6.1
+    "@jest/types": ^29.6.1
     "@types/node": "*"
     ansi-escapes: ^4.2.1
     chalk: ^4.0.0
     emittery: ^0.13.1
-    jest-util: ^29.5.0
+    jest-util: ^29.6.1
     string-length: ^4.0.1
-  checksum: 62303ac7bdc7e61a8b4239a239d018f7527739da2b2be6a81a7be25b74ca769f1c43ee8558ce8e72bb857245c46d6e03af331227ffb00a57280abb2a928aa776
+  checksum: 69bd5a602284fdce6eba5486c5c57aca6b511d91cb0907c34c104d6dd931e18ce67baa7f8e280fa473e5d81ea3e7b9e7d94f712c37ab0b3b8cc2aec30676955d
   languageName: node
   linkType: hard
 
 "jest-worker@npm:^27.4.5":
   version: 27.5.1
   resolution: "jest-worker@npm:27.5.1"
   dependencies:
     "@types/node": "*"
     merge-stream: ^2.0.0
     supports-color: ^8.0.0
   checksum: 98cd68b696781caed61c983a3ee30bf880b5bd021c01d98f47b143d4362b85d0737f8523761e2713d45e18b4f9a2b98af1eaee77afade4111bb65c77d6f7c980
   languageName: node
   linkType: hard
 
-"jest-worker@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest-worker@npm:29.5.0"
+"jest-worker@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "jest-worker@npm:29.6.1"
   dependencies:
     "@types/node": "*"
-    jest-util: ^29.5.0
+    jest-util: ^29.6.1
     merge-stream: ^2.0.0
     supports-color: ^8.0.0
-  checksum: 1151a1ae3602b1ea7c42a8f1efe2b5a7bf927039deaa0827bf978880169899b705744e288f80a63603fb3fc2985e0071234986af7dc2c21c7a64333d8777c7c9
+  checksum: 0af309ea4db17c4c47e84a9246f907960a15577683c005fdeafc8f3c06bc455136f95a6f28fa2a3e924b767eb4dacd9b40915a7707305f88586f099af3ac27a8
   languageName: node
   linkType: hard
 
 "jest@npm:^29.2.0, jest@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "jest@npm:29.5.0"
+  version: 29.6.1
+  resolution: "jest@npm:29.6.1"
   dependencies:
-    "@jest/core": ^29.5.0
-    "@jest/types": ^29.5.0
+    "@jest/core": ^29.6.1
+    "@jest/types": ^29.6.1
     import-local: ^3.0.2
-    jest-cli: ^29.5.0
+    jest-cli: ^29.6.1
   peerDependencies:
     node-notifier: ^8.0.1 || ^9.0.0 || ^10.0.0
   peerDependenciesMeta:
     node-notifier:
       optional: true
   bin:
     jest: bin/jest.js
-  checksum: a8ff2eb0f421623412236e23cbe67c638127fffde466cba9606bc0c0553b4c1e5cb116d7e0ef990b5d1712851652c8ee461373b578df50857fe635b94ff455d5
+  checksum: 7b8c0ca72f483e00ec19dcf9549f9a9af8ae468ab62925b148d714b58eb52d5fea9a082625193bc833d2d9b64cf65a11f3d37857636c5551af05c10aec4ce71b
   languageName: node
   linkType: hard
 
 "jquery@npm:^3.1.1":
   version: 3.7.0
   resolution: "jquery@npm:3.7.0"
   checksum: 907785e133afc427650a131af5fccef66a404885037513b3d4d7d63aee6409bcc32a39836868c60e59b05aa0fb8ace8961c18b2ee3ffdf6ffdb571d6d7cd88ff
@@ -7607,15 +7421,15 @@
 "json-stringify-safe@npm:^5.0.1":
   version: 5.0.1
   resolution: "json-stringify-safe@npm:5.0.1"
   checksum: 48ec0adad5280b8a96bb93f4563aa1667fd7a36334f79149abd42446d0989f2ddc58274b479f4819f1f00617957e6344c886c55d05a4e15ebb4ab931e4a6a8ee
   languageName: node
   linkType: hard
 
-"json5@npm:^2.1.1, json5@npm:^2.1.2, json5@npm:^2.2.2, json5@npm:^2.2.3":
+"json5@npm:^2.1.2, json5@npm:^2.2.2, json5@npm:^2.2.3":
   version: 2.2.3
   resolution: "json5@npm:2.2.3"
   bin:
     json5: lib/cli.js
   checksum: 2a7436a93393830bce797d4626275152e37e877b265e94ca69c99e3d20c2b9dab021279146a39cdb700e71b2dd32a4cebd1514cd57cee102b1af906ce5040349
   languageName: node
   linkType: hard
@@ -7777,24 +7591,14 @@
   dependencies:
     prelude-ls: ^1.2.1
     type-check: ~0.4.0
   checksum: 12c5021c859bd0f5248561bf139121f0358285ec545ebf48bb3d346820d5c61a4309535c7f387ed7d84361cf821e124ce346c6b7cef8ee09a67c1473b46d0fc4
   languageName: node
   linkType: hard
 
-"levn@npm:~0.3.0":
-  version: 0.3.0
-  resolution: "levn@npm:0.3.0"
-  dependencies:
-    prelude-ls: ~1.1.2
-    type-check: ~0.3.2
-  checksum: 0d084a524231a8246bb10fec48cdbb35282099f6954838604f3c7fc66f2e16fa66fd9cc2f3f20a541a113c4dafdf181e822c887c8a319c9195444e6c64ac395e
-  languageName: node
-  linkType: hard
-
 "lib0@npm:^0.2.31, lib0@npm:^0.2.42, lib0@npm:^0.2.52, lib0@npm:^0.2.74, lib0@npm:^0.2.76":
   version: 0.2.78
   resolution: "lib0@npm:0.2.78"
   dependencies:
     isomorphic.js: ^0.2.4
   bin:
     0gentesthtml: bin/gentesthtml.js
@@ -7950,18 +7754,18 @@
 "lru-cache@npm:^7.7.1":
   version: 7.18.3
   resolution: "lru-cache@npm:7.18.3"
   checksum: e550d772384709deea3f141af34b6d4fa392e2e418c1498c078de0ee63670f1f46f5eee746e8ef7e69e1c895af0d4224e62ee33e66a543a14763b0f2e74c1356
   languageName: node
   linkType: hard
 
-"lru-cache@npm:^9.1.1":
-  version: 9.1.2
-  resolution: "lru-cache@npm:9.1.2"
-  checksum: d3415634be3908909081fc4c56371a8d562d9081eba70543d86871b978702fffd0e9e362b83921b27a29ae2b37b90f55675aad770a54ac83bb3e4de5049d4b15
+"lru-cache@npm:^9.1.1 || ^10.0.0":
+  version: 10.0.0
+  resolution: "lru-cache@npm:10.0.0"
+  checksum: 18f101675fe283bc09cda0ef1e3cc83781aeb8373b439f086f758d1d91b28730950db785999cd060d3c825a8571c03073e8c14512b6655af2188d623031baf50
   languageName: node
   linkType: hard
 
 "lru-queue@npm:^0.1.0":
   version: 0.1.0
   resolution: "lru-queue@npm:0.1.0"
   dependencies:
@@ -8178,19 +7982,19 @@
   dependencies:
     brace-expansion: ^1.1.7
   checksum: c154e566406683e7bcb746e000b84d74465b3a832c45d59912b9b55cd50dee66e5c4b1e5566dba26154040e51672f9aa450a9aef0c97cfc7336b78b7afb9540a
   languageName: node
   linkType: hard
 
 "minimatch@npm:^9.0.1":
-  version: 9.0.2
-  resolution: "minimatch@npm:9.0.2"
+  version: 9.0.3
+  resolution: "minimatch@npm:9.0.3"
   dependencies:
     brace-expansion: ^2.0.1
-  checksum: 2eb12e2047a062fdb973fb51b9803f2455e3a00977858c038d66646d303a5a15bbcbc6ed5a2fc403bc869b1309f829ed3acd881d3246faf044ea7a494974b924
+  checksum: 253487976bf485b612f16bf57463520a14f512662e592e95c571afdab1442a6a6864b6c88f248ce6fc4ff0b6de04ac7aa6c8bb51e868e99d1d65eb0658a708b5
   languageName: node
   linkType: hard
 
 "minimist-options@npm:4.1.0":
   version: 4.1.0
   resolution: "minimist-options@npm:4.1.0"
   dependencies:
@@ -8297,21 +8101,14 @@
   resolution: "mkdirp@npm:1.0.4"
   bin:
     mkdirp: bin/cmd.js
   checksum: a96865108c6c3b1b8e1d5e9f11843de1e077e57737602de1b82030815f311be11f96f09cce59bd5b903d0b29834733e5313f9301e3ed6d6f6fba2eae0df4298f
   languageName: node
   linkType: hard
 
-"moment@npm:^2.24.0":
-  version: 2.29.4
-  resolution: "moment@npm:2.29.4"
-  checksum: 0ec3f9c2bcba38dc2451b1daed5daded747f17610b92427bebe1d08d48d8b7bdd8d9197500b072d14e326dd0ccf3e326b9e3d07c5895d3d49e39b6803b76e80e
-  languageName: node
-  linkType: hard
-
 "ms@npm:2.1.2":
   version: 2.1.2
   resolution: "ms@npm:2.1.2"
   checksum: 673cdb2c3133eb050c745908d8ce632ed2c02d85640e2edb3ace856a2266a813b30c613569bf3354fdf4ea7d1a1494add3bfa95e2713baa27d0c2c71fc44f58f
   languageName: node
   linkType: hard
 
@@ -8381,24 +8178,24 @@
   version: 1.0.5
   resolution: "nice-try@npm:1.0.5"
   checksum: 0b4af3b5bb5d86c289f7a026303d192a7eb4417231fe47245c460baeabae7277bcd8fd9c728fb6bd62c30b3e15cd6620373e2cf33353b095d8b403d3e8a15aff
   languageName: node
   linkType: hard
 
 "node-fetch@npm:^2.6.0":
-  version: 2.6.11
-  resolution: "node-fetch@npm:2.6.11"
+  version: 2.6.12
+  resolution: "node-fetch@npm:2.6.12"
   dependencies:
     whatwg-url: ^5.0.0
   peerDependencies:
     encoding: ^0.1.0
   peerDependenciesMeta:
     encoding:
       optional: true
-  checksum: 249d0666a9497553384d46b5ab296ba223521ac88fed4d8a17d6ee6c2efb0fc890f3e8091cafe7f9fba8151a5b8d925db2671543b3409a56c3cd522b468b47b3
+  checksum: 3bc1655203d47ee8e313c0d96664b9673a3d4dd8002740318e9d27d14ef306693a4b2ef8d6525775056fd912a19e23f3ac0d7111ad8925877b7567b29a625592
   languageName: node
   linkType: hard
 
 "node-gyp-build@npm:~4.1.0":
   version: 4.1.1
   resolution: "node-gyp-build@npm:4.1.1"
   bin:
@@ -8434,17 +8231,17 @@
   version: 0.4.0
   resolution: "node-int64@npm:0.4.0"
   checksum: d0b30b1ee6d961851c60d5eaa745d30b5c95d94bc0e74b81e5292f7c42a49e3af87f1eb9e89f59456f80645d679202537de751b7d72e9e40ceea40c5e449057e
   languageName: node
   linkType: hard
 
 "node-releases@npm:^2.0.12":
-  version: 2.0.12
-  resolution: "node-releases@npm:2.0.12"
-  checksum: b8c56db82c4642a0f443332b331a4396dae452a2ac5a65c8dbd93ef89ecb2fbb0da9d42ac5366d4764973febadca816cf7587dad492dce18d2a6b2af59cda260
+  version: 2.0.13
+  resolution: "node-releases@npm:2.0.13"
+  checksum: 17ec8f315dba62710cae71a8dad3cd0288ba943d2ece43504b3b1aa8625bf138637798ab470b1d9035b0545996f63000a8a926e0f6d35d0996424f8b6d36dda3
   languageName: node
   linkType: hard
 
 "nopt@npm:^6.0.0":
   version: 6.0.0
   resolution: "nopt@npm:6.0.0"
   dependencies:
@@ -8525,17 +8322,17 @@
     gauge: ^4.0.3
     set-blocking: ^2.0.0
   checksum: ae238cd264a1c3f22091cdd9e2b106f684297d3c184f1146984ecbe18aaa86343953f26b9520dedd1b1372bc0316905b736c1932d778dbeb1fcf5a1001390e2a
   languageName: node
   linkType: hard
 
 "nwsapi@npm:^2.2.2":
-  version: 2.2.5
-  resolution: "nwsapi@npm:2.2.5"
-  checksum: 3acfe387214e2a9a03960662ad600ecb41fc24385c9de91262a881608407f02d14686e5df3e6e87af0cf7b173ed2a6a202a569ab7bef376ec1841cd9b6cbf0a6
+  version: 2.2.7
+  resolution: "nwsapi@npm:2.2.7"
+  checksum: cab25f7983acec7e23490fec3ef7be608041b460504229770e3bfcf9977c41d6fe58f518994d3bd9aa3a101f501089a3d4a63536f4ff8ae4b8c4ca23bdbfda4e
   languageName: node
   linkType: hard
 
 "object-assign@npm:^4.0.1, object-assign@npm:^4.1.1":
   version: 4.1.1
   resolution: "object-assign@npm:4.1.1"
   checksum: fcc6e4ea8c7fe48abfbb552578b1c53e0d194086e2e6bbbf59e0a536381a292f39943c6e9628af05b5528aa5e3318bb30d6b2e53cadaf5b8fe9e12c4b69af23f
@@ -8582,39 +8379,25 @@
   resolution: "onetime@npm:5.1.2"
   dependencies:
     mimic-fn: ^2.1.0
   checksum: 2478859ef817fc5d4e9c2f9e5728512ddd1dbc9fb7829ad263765bb6d3b91ce699d6e2332eef6b7dff183c2f490bd3349f1666427eaba4469fba0ac38dfd0d34
   languageName: node
   linkType: hard
 
-"optionator@npm:^0.8.1":
-  version: 0.8.3
-  resolution: "optionator@npm:0.8.3"
-  dependencies:
-    deep-is: ~0.1.3
-    fast-levenshtein: ~2.0.6
-    levn: ~0.3.0
-    prelude-ls: ~1.1.2
-    type-check: ~0.3.2
-    word-wrap: ~1.2.3
-  checksum: b8695ddf3d593203e25ab0900e265d860038486c943ff8b774f596a310f8ceebdb30c6832407a8198ba3ec9debe1abe1f51d4aad94843612db3b76d690c61d34
-  languageName: node
-  linkType: hard
-
 "optionator@npm:^0.9.1":
-  version: 0.9.1
-  resolution: "optionator@npm:0.9.1"
+  version: 0.9.3
+  resolution: "optionator@npm:0.9.3"
   dependencies:
+    "@aashutoshrathi/word-wrap": ^1.2.3
     deep-is: ^0.1.3
     fast-levenshtein: ^2.0.6
     levn: ^0.4.1
     prelude-ls: ^1.2.1
     type-check: ^0.4.0
-    word-wrap: ^1.2.3
-  checksum: dbc6fa065604b24ea57d734261914e697bd73b69eff7f18e967e8912aa2a40a19a9f599a507fa805be6c13c24c4eae8c71306c239d517d42d4c041c942f508a0
+  checksum: 09281999441f2fe9c33a5eeab76700795365a061563d66b098923eb719251a42bdbe432790d35064d0816ead9296dbeb1ad51a733edf4167c96bd5d0882e428a
   languageName: node
   linkType: hard
 
 "p-limit@npm:^2.2.0":
   version: 2.3.0
   resolution: "p-limit@npm:2.3.0"
   dependencies:
@@ -8742,21 +8525,21 @@
 "path-parse@npm:^1.0.7":
   version: 1.0.7
   resolution: "path-parse@npm:1.0.7"
   checksum: 49abf3d81115642938a8700ec580da6e830dde670be21893c62f4e10bd7dd4c3742ddc603fe24f898cba7eb0c6bc1777f8d9ac14185d34540c6d4d80cd9cae8a
   languageName: node
   linkType: hard
 
-"path-scurry@npm:^1.7.0":
-  version: 1.9.2
-  resolution: "path-scurry@npm:1.9.2"
+"path-scurry@npm:^1.10.0":
+  version: 1.10.0
+  resolution: "path-scurry@npm:1.10.0"
   dependencies:
-    lru-cache: ^9.1.1
+    lru-cache: ^9.1.1 || ^10.0.0
     minipass: ^5.0.0 || ^6.0.2
-  checksum: 92888dfb68e285043c6d3291c8e971d5d2bc2f5082f4d7b5392896f34be47024c9d0a8b688dd7ae6d125acc424699195474927cb4f00049a9b1ec7c4256fa8e0
+  checksum: 3b66a4a6ab66e45755b577c966ecf0da92d3e068b3c992d8f69aa2cc908ef4eda9358253e9b4f86cad43d3ad810ec445be164105975f5cb3fdab68459c59dc6e
   languageName: node
   linkType: hard
 
 "path-type@npm:^3.0.0":
   version: 3.0.0
   resolution: "path-type@npm:3.0.0"
   dependencies:
@@ -8899,38 +8682,31 @@
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
   languageName: node
   linkType: hard
 
 "postcss@npm:^8.3.11, postcss@npm:^8.4.19, postcss@npm:^8.4.21":
-  version: 8.4.24
-  resolution: "postcss@npm:8.4.24"
+  version: 8.4.25
+  resolution: "postcss@npm:8.4.25"
   dependencies:
     nanoid: ^3.3.6
     picocolors: ^1.0.0
     source-map-js: ^1.0.2
-  checksum: 814e2126dacfea313588eda09cc99a9b4c26ec55c059188aa7a916d20d26d483483106dc5ff9e560731b59f45c5bb91b945dfadc670aed875cc90ddbbf4e787d
+  checksum: 9ed3ab8af43ad5210c28f56f916fd9b8c9f94fbeaebbf645dcf579bc28bdd8056c2a7ecc934668d399b81fedb6128f0c4b299f931e50454964bc911c25a3a0a2
   languageName: node
   linkType: hard
 
 "prelude-ls@npm:^1.2.1":
   version: 1.2.1
   resolution: "prelude-ls@npm:1.2.1"
   checksum: cd192ec0d0a8e4c6da3bb80e4f62afe336df3f76271ac6deb0e6a36187133b6073a19e9727a1ff108cd8b9982e4768850d413baa71214dd80c7979617dca827a
   languageName: node
   linkType: hard
 
-"prelude-ls@npm:~1.1.2":
-  version: 1.1.2
-  resolution: "prelude-ls@npm:1.1.2"
-  checksum: c4867c87488e4a0c233e158e4d0d5565b609b105d75e4c05dc760840475f06b731332eb93cc8c9cecb840aa8ec323ca3c9a56ad7820ad2e63f0261dadcb154e4
-  languageName: node
-  linkType: hard
-
 "prettier-linter-helpers@npm:^1.0.0":
   version: 1.0.0
   resolution: "prettier-linter-helpers@npm:1.0.0"
   dependencies:
     fast-diff: ^1.1.2
   checksum: 00ce8011cf6430158d27f9c92cfea0a7699405633f7f1d4a45f07e21bf78e99895911cbcdc3853db3a824201a7c745bd49bfea8abd5fb9883e765a90f74f8392
   languageName: node
@@ -8941,22 +8717,22 @@
   resolution: "prettier@npm:2.8.8"
   bin:
     prettier: bin-prettier.js
   checksum: b49e409431bf129dd89238d64299ba80717b57ff5a6d1c1a8b1a28b590d998a34e083fa13573bc732bb8d2305becb4c9a4407f8486c81fa7d55100eb08263cf8
   languageName: node
   linkType: hard
 
-"pretty-format@npm:^29.0.0, pretty-format@npm:^29.5.0":
-  version: 29.5.0
-  resolution: "pretty-format@npm:29.5.0"
+"pretty-format@npm:^29.0.0, pretty-format@npm:^29.6.1":
+  version: 29.6.1
+  resolution: "pretty-format@npm:29.6.1"
   dependencies:
-    "@jest/schemas": ^29.4.3
+    "@jest/schemas": ^29.6.0
     ansi-styles: ^5.0.0
     react-is: ^18.0.0
-  checksum: 4065356b558e6db25b4d41a01efb386935a6c06a0c9c104ef5ce59f2f476b8210edb8b3949b386e60ada0a6dc5ebcb2e6ccddc8c64dfd1a9943c3c3a9e7eaf89
+  checksum: 6f923a2379a37a425241dc223d76f671c73c4f37dba158050575a54095867d565c068b441843afdf3d7c37bed9df4bbadf46297976e60d4149972b779474203a
   languageName: node
   linkType: hard
 
 "process@npm:^0.11.10":
   version: 0.11.10
   resolution: "process@npm:0.11.10"
   checksum: bfcce49814f7d172a6e6a14d5fa3ac92cc3d0c3b9feb1279774708a719e19acd673995226351a082a9ae99978254e320ccda4240ddc474ba31a76c79491ca7c3
@@ -9440,34 +9216,34 @@
   resolution: "semver@npm:5.7.1"
   bin:
     semver: ./bin/semver
   checksum: 57fd0acfd0bac382ee87cd52cd0aaa5af086a7dc8d60379dfe65fea491fb2489b6016400813930ecd61fd0952dae75c115287a1b16c234b1550887117744dfaf
   languageName: node
   linkType: hard
 
-"semver@npm:7.x, semver@npm:^7.2.1, semver@npm:^7.3.4, semver@npm:^7.3.5, semver@npm:^7.3.8":
+"semver@npm:^6.0.0, semver@npm:^6.3.0":
+  version: 6.3.0
+  resolution: "semver@npm:6.3.0"
+  bin:
+    semver: ./bin/semver.js
+  checksum: 1b26ecf6db9e8292dd90df4e781d91875c0dcc1b1909e70f5d12959a23c7eebb8f01ea581c00783bbee72ceeaad9505797c381756326073850dc36ed284b21b9
+  languageName: node
+  linkType: hard
+
+"semver@npm:^7.2.1, semver@npm:^7.3.4, semver@npm:^7.3.5, semver@npm:^7.3.8, semver@npm:^7.5.3":
   version: 7.5.3
   resolution: "semver@npm:7.5.3"
   dependencies:
     lru-cache: ^6.0.0
   bin:
     semver: bin/semver.js
   checksum: 9d58db16525e9f749ad0a696a1f27deabaa51f66e91d2fa2b0db3de3e9644e8677de3b7d7a03f4c15bc81521e0c3916d7369e0572dbde250d9bedf5194e2a8a7
   languageName: node
   linkType: hard
 
-"semver@npm:^6.0.0, semver@npm:^6.1.1, semver@npm:^6.1.2, semver@npm:^6.3.0":
-  version: 6.3.0
-  resolution: "semver@npm:6.3.0"
-  bin:
-    semver: ./bin/semver.js
-  checksum: 1b26ecf6db9e8292dd90df4e781d91875c0dcc1b1909e70f5d12959a23c7eebb8f01ea581c00783bbee72ceeaad9505797c381756326073850dc36ed284b21b9
-  languageName: node
-  linkType: hard
-
 "serialize-javascript@npm:^6.0.1":
   version: 6.0.1
   resolution: "serialize-javascript@npm:6.0.1"
   dependencies:
     randombytes: ^2.1.0
   checksum: 3c4f4cb61d0893b988415bdb67243637333f3f574e9e9cc9a006a2ced0b390b0b3b44aef8d51c951272a9002ec50885eefdc0298891bc27eb2fe7510ea87dc4f
   languageName: node
@@ -10096,24 +9872,24 @@
     uglify-js:
       optional: true
   checksum: 41705713d6f9cb83287936b21e27c658891c78c4392159f5148b5623f0e8c48559869779619b058382a4c9758e7820ea034695e57dc7c474b4962b79f553bc5f
   languageName: node
   linkType: hard
 
 "terser@npm:^5.16.8":
-  version: 5.18.1
-  resolution: "terser@npm:5.18.1"
+  version: 5.18.2
+  resolution: "terser@npm:5.18.2"
   dependencies:
     "@jridgewell/source-map": ^0.3.3
     acorn: ^8.8.2
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: 15d1af05aae451ce844f7dc3627db09ec79f842fa9a3cf2b40221a639249d70fcd91fd3baa9c970842d75e1dd2fb957eb1afd8a0fcfc9b2a3296076a4e72528a
+  checksum: 50988412533bfd5a07294df002d772ad5b1277a9d1164dd19c8876a2094ced7b78fcf36cb32122a9a5238ba2597d77178a2385dfc6c4d506622309493f613cf4
   languageName: node
   linkType: hard
 
 "test-exclude@npm:^6.0.0":
   version: 6.0.0
   resolution: "test-exclude@npm:6.0.0"
   dependencies:
@@ -10223,24 +9999,24 @@
   version: 3.0.1
   resolution: "trim-newlines@npm:3.0.1"
   checksum: b530f3fadf78e570cf3c761fb74fef655beff6b0f84b29209bac6c9622db75ad1417f4a7b5d54c96605dcd72734ad44526fef9f396807b90839449eb543c6206
   languageName: node
   linkType: hard
 
 "ts-jest@npm:^29.1.0":
-  version: 29.1.0
-  resolution: "ts-jest@npm:29.1.0"
+  version: 29.1.1
+  resolution: "ts-jest@npm:29.1.1"
   dependencies:
     bs-logger: 0.x
     fast-json-stable-stringify: 2.x
     jest-util: ^29.0.0
     json5: ^2.2.3
     lodash.memoize: 4.x
     make-error: 1.x
-    semver: 7.x
+    semver: ^7.5.3
     yargs-parser: ^21.0.1
   peerDependencies:
     "@babel/core": ">=7.0.0-beta.0 <8"
     "@jest/types": ^29.0.0
     babel-jest: ^29.0.0
     jest: ^29.0.0
     typescript: ">=4.3 <6"
@@ -10251,15 +10027,15 @@
       optional: true
     babel-jest:
       optional: true
     esbuild:
       optional: true
   bin:
     ts-jest: cli.js
-  checksum: 535dc42ad523cbe1e387701fb2e448518419b515c082f09b25411f0b3dd0b854cf3e8141c316d6f4b99883aeb4a4f94159cbb1edfb06d7f77ea6229fadb2e1bf
+  checksum: a8c9e284ed4f819526749f6e4dc6421ec666f20ab44d31b0f02b4ed979975f7580b18aea4813172d43e39b29464a71899f8893dd29b06b4a351a3af8ba47b402
   languageName: node
   linkType: hard
 
 "tslib@npm:^1.8.1":
   version: 1.14.1
   resolution: "tslib@npm:1.14.1"
   checksum: dbe628ef87f66691d5d2959b3e41b9ca0045c3ee3c7c7b906cc1e328b39f199bb1ad9e671c39025bd56122ac57dfbf7385a94843b1cc07c60a4db74795829acd
@@ -10282,23 +10058,14 @@
   resolution: "type-check@npm:0.4.0"
   dependencies:
     prelude-ls: ^1.2.1
   checksum: ec688ebfc9c45d0c30412e41ca9c0cdbd704580eb3a9ccf07b9b576094d7b86a012baebc95681999dd38f4f444afd28504cb3a89f2ef16b31d4ab61a0739025a
   languageName: node
   linkType: hard
 
-"type-check@npm:~0.3.2":
-  version: 0.3.2
-  resolution: "type-check@npm:0.3.2"
-  dependencies:
-    prelude-ls: ~1.1.2
-  checksum: dd3b1495642731bc0e1fc40abe5e977e0263005551ac83342ecb6f4f89551d106b368ec32ad3fb2da19b3bd7b2d1f64330da2ea9176d8ddbfe389fb286eb5124
-  languageName: node
-  linkType: hard
-
 "type-detect@npm:4.0.8":
   version: 4.0.8
   resolution: "type-detect@npm:4.0.8"
   checksum: 62b5628bff67c0eb0b66afa371bd73e230399a8d2ad30d852716efcc4656a7516904570cd8631a49a3ce57c10225adf5d0cbdcb47f6b0255fe6557c453925a15
   languageName: node
   linkType: hard
 
@@ -10493,15 +10260,15 @@
   resolution: "uri-js@npm:4.4.1"
   dependencies:
     punycode: ^2.1.0
   checksum: 7167432de6817fe8e9e0c9684f1d2de2bb688c94388f7569f7dbdb1587c9f4ca2a77962f134ec90be0cc4d004c939ff0d05acc9f34a0db39a3c797dada262633
   languageName: node
   linkType: hard
 
-"url-parse@npm:^1.5.3, url-parse@npm:~1.5.1, url-parse@npm:~1.5.4":
+"url-parse@npm:^1.5.3, url-parse@npm:~1.5.4":
   version: 1.5.10
   resolution: "url-parse@npm:1.5.10"
   dependencies:
     querystringify: ^2.1.1
     requires-port: ^1.0.0
   checksum: fbdba6b1d83336aca2216bbdc38ba658d9cfb8fc7f665eb8b17852de638ff7d1a162c198a8e4ed66001ddbf6c9888d41e4798912c62b4fd777a31657989f7bdf
   languageName: node
@@ -10752,16 +10519,16 @@
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
 "webpack@npm:^5.76.1, webpack@npm:^5.77.0":
-  version: 5.88.0
-  resolution: "webpack@npm:5.88.0"
+  version: 5.88.1
+  resolution: "webpack@npm:5.88.1"
   dependencies:
     "@types/eslint-scope": ^3.7.3
     "@types/estree": ^1.0.0
     "@webassemblyjs/ast": ^1.11.5
     "@webassemblyjs/wasm-edit": ^1.11.5
     "@webassemblyjs/wasm-parser": ^1.11.5
     acorn: ^8.7.1
@@ -10784,15 +10551,15 @@
     watchpack: ^2.4.0
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: 9fd1568b34ec2e99ba97c8509a15ab2576ec80c396e7015551ec814b24cfc11de173acba3e114dafe95f1a6d460781b09d6201e6a1fb15110e1d01a09f61a283
+  checksum: 726e7e05ab2e7c142609a673dd6aa1a711ed97f349418a2a393d650c5ddad172d191257f60e1e37f6b2a77261571c202aabd5ce9240791a686774f0801cf5ec2
   languageName: node
   linkType: hard
 
 "whatwg-encoding@npm:^2.0.0":
   version: 2.0.0
   resolution: "whatwg-encoding@npm:2.0.0"
   dependencies:
@@ -10907,21 +10674,14 @@
 "wildcard@npm:^2.0.0":
   version: 2.0.1
   resolution: "wildcard@npm:2.0.1"
   checksum: e0c60a12a219e4b12065d1199802d81c27b841ed6ad6d9d28240980c73ceec6f856771d575af367cbec2982d9ae7838759168b551776577f155044f5a5ba843c
   languageName: node
   linkType: hard
 
-"word-wrap@npm:^1.2.3, word-wrap@npm:~1.2.3":
-  version: 1.2.3
-  resolution: "word-wrap@npm:1.2.3"
-  checksum: 30b48f91fcf12106ed3186ae4fa86a6a1842416df425be7b60485de14bec665a54a68e4b5156647dec3a70f25e84d270ca8bc8cd23182ed095f5c7206a938c1f
-  languageName: node
-  linkType: hard
-
 "worker-loader@npm:^3.0.2":
   version: 3.0.8
   resolution: "worker-loader@npm:3.0.8"
   dependencies:
     loader-utils: ^2.0.0
     schema-utils: ^3.0.0
   peerDependencies:
@@ -10974,29 +10734,14 @@
   resolution: "ws@npm:6.2.2"
   dependencies:
     async-limiter: ~1.0.0
   checksum: aec3154ec51477c094ac2cb5946a156e17561a581fa27005cbf22c53ac57f8d4e5f791dd4bbba6a488602cb28778c8ab7df06251d590507c3c550fd8ebeee949
   languageName: node
   linkType: hard
 
-"ws@npm:^7.4.6":
-  version: 7.5.9
-  resolution: "ws@npm:7.5.9"
-  peerDependencies:
-    bufferutil: ^4.0.1
-    utf-8-validate: ^5.0.2
-  peerDependenciesMeta:
-    bufferutil:
-      optional: true
-    utf-8-validate:
-      optional: true
-  checksum: c3c100a181b731f40b7f2fddf004aa023f79d64f489706a28bc23ff88e87f6a64b3c6651fbec3a84a53960b75159574d7a7385709847a62ddb7ad6af76f49138
-  languageName: node
-  linkType: hard
-
 "ws@npm:^8.11.0":
   version: 8.13.0
   resolution: "ws@npm:8.13.0"
   peerDependencies:
     bufferutil: ^4.0.1
     utf-8-validate: ">=5.0.2"
   peerDependenciesMeta:
```

### Comparing `glue_jupyterlab-0.2.0/examples/session.glu` & `glue_jupyterlab-0.3.0/examples/session.glu`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/examples/session2.glu` & `glue_jupyterlab-0.3.0/examples/session2.glu`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/examples/session3.glu` & `glue_jupyterlab-0.3.0/examples/session3.glu`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/__init__.py` & `glue_jupyterlab-0.3.0/glue_jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/glue_session.py` & `glue_jupyterlab-0.3.0/glue_jupyterlab/glue_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         if display_view:
             display(self._viewers[tab_name][viewer_id]["output"])
 
     def render_viewer(self) -> None:
         """Fill the place holder output with glu-jupyter widgets"""
 
         all_tabs = self._document.get_tab_names()
-        for frontend_tab in self._viewers:
+        for frontend_tab in list(self._viewers):
             if frontend_tab not in all_tabs:
                 # Tab removed from the frontend
                 self.remove_tab(frontend_tab)
 
         for tab_name in all_tabs:
             document_tab_data = self._document.get_tab_data(tab_name)
             if document_tab_data is None:
@@ -345,14 +345,24 @@
         self._ywidget = Widget(
             comm_metadata=dict(
                 ymodel_name="GlueSession", create_ydoc=False, path=self._path
             ),
             ydoc=self._sessionYDoc,
         )
 
+    def add_viewer_layer(self, tab_name: str, viewer_name: str, data_name: str) -> None:
+        """Add a layer with new dataset to a viewer"""
+        viewer = (
+            self._viewers.get(tab_name, {}).get(viewer_name, {}).get("widget", None)
+        )
+        if not viewer:
+            return
+        data = self._data[data_name]
+        viewer.add_data(data)
+
     def add_data(self, file_path: str) -> None:
         """Add a new data file to the session"""
         relative_path = Path(file_path).relative_to(Path(self._path).parent)
         assert os.path.exists(relative_path)
 
         data = self.app.load_data(str(relative_path))
```

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/glue_utils.py` & `glue_jupyterlab-0.3.0/glue_jupyterlab/glue_utils.py`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/glue_ydoc.py` & `glue_jupyterlab-0.3.0/glue_jupyterlab/glue_ydoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,38 +65,34 @@
         contents.setdefault("__main__", {})
 
         tab_names = sorted(list(tabs.keys()))
         contents["__main__"]["tab_names"] = tab_names
 
         contents["__main__"].setdefault("viewers", [])
 
-        while len(contents["__main__"]["viewers"]) != len(tab_names):
-            contents["__main__"]["viewers"].append([])
-
-        viewer_names = []
-        for idx, tab in enumerate(tab_names):
-            viewers = tabs[tab]
+        contents["__main__"]["viewers"] = []
+        for tab in tab_names:
+            viewers = tabs.get(tab, {})
             viewer_names = sorted(list(viewers.keys()))
 
-            contents["__main__"]["viewers"][idx] = viewer_names
+            contents["__main__"]["viewers"].append(viewer_names)
             for viewer in viewer_names:
                 contents[viewer] = viewers[viewer]
 
         if self._data_collection_name:
             data_names = sorted(list(dataset.keys()))
             link_names = sorted(list(links.keys()))
 
             contents[self._data_collection_name]["data"] = data_names
             contents[self._data_collection_name]["links"] = link_names
 
             for data_name in data_names:
                 contents[data_name] = dataset[data_name]
 
             self.add_links_to_contents(links, contents)
-
         return json.dumps(contents, indent=2, sort_keys=True)
 
     def set(self, value: str) -> None:
         """
         Sets the content of the document.
         :param value: The content of the document.
         :type value: Any
```

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/handlers.py` & `glue_jupyterlab-0.3.0/glue_jupyterlab/handlers.py`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/package.json` & `glue_jupyterlab-0.3.0/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.97%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.3.0'"}*

```diff
@@ -55,19 +55,14 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/QuantStack/glue-jupyterlab",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.7851783ebd012eb24a52.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "glue-jupyterlab"
                 },
                 "managers": [
                     "pip"
@@ -133,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/185.0cff412fc25ed146b7c1.js` & `glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/185.0cff412fc25ed146b7c1.js`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/398.bd2742885fb1b39ca17d.js` & `glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/722.e912ef3d95501737406e.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,66 +1,62 @@
 (self.webpackChunkglue_jupyterlab = self.webpackChunkglue_jupyterlab || []).push([
-    [398], {
-        7398: (e, t, s) => {
+    [722], {
+        7722: (e, t, s) => {
             "use strict";
             s.r(t), s.d(t, {
-                ICollaborativeDrive: () => Re,
-                WebSocketProvider: () => Ee,
-                YDrive: () => Ae
+                ICollaborativeDrive: () => Ne,
+                MessageType: () => Ue,
+                WebSocketAwarenessProvider: () => Ie,
+                WebSocketProvider: () => Le,
+                YDrive: () => Ee
             });
-            var n = s(9993),
-                o = s(4238),
-                r = s(5350),
-                c = s(7930),
-                a = s(4901),
-                i = s(981);
-            const l = () => new Map,
-                h = (e, t, s) => {
-                    let n = e.get(t);
-                    return void 0 === n && e.set(t, n = s()), n
-                },
-                d = () => new Set,
-                u = String.fromCharCode,
-                f = (String.fromCodePoint, u(65535), /^\s*/g),
-                p = /([A-Z])/g,
-                g = (e, t) => (e => e.replace(f, ""))(e.replace(p, (e => `${t}${(e=>e.toLowerCase())(e)}`))),
-                y = "undefined" != typeof TextEncoder ? new TextEncoder : null,
-                w = y ? e => y.encode(e) : e => {
+            var n = s(4901);
+            const o = String.fromCharCode,
+                r = (String.fromCodePoint, o(65535), /^\s*/g),
+                a = /([A-Z])/g,
+                i = (e, t) => (e => e.replace(r, ""))(e.replace(a, (e => `${t}${(e=>e.toLowerCase())(e)}`))),
+                c = "undefined" != typeof TextEncoder ? new TextEncoder : null,
+                l = c ? e => c.encode(e) : e => {
                     const t = unescape(encodeURIComponent(e)),
                         s = t.length,
                         n = new Uint8Array(s);
                     for (let e = 0; e < s; e++) n[e] = t.codePointAt(e);
                     return n
                 };
-            let m = "undefined" == typeof TextDecoder ? null : new TextDecoder("utf-8", {
+            let h = "undefined" == typeof TextDecoder ? null : new TextDecoder("utf-8", {
                 fatal: !0,
                 ignoreBOM: !0
             });
-            m && 1 === m.decode(new Uint8Array).length && (m = null);
-            let b = new class {
+            h && 1 === h.decode(new Uint8Array).length && (h = null);
+            const d = () => new Map,
+                u = (e, t, s) => {
+                    let n = e.get(t);
+                    return void 0 === n && e.set(t, n = s()), n
+                };
+            let f = new class {
                     constructor() {
                         this.map = new Map
                     }
                     setItem(e, t) {
                         this.map.set(e, t)
                     }
                     getItem(e) {
                         return this.map.get(e)
                     }
                 },
-                v = !0;
+                p = !0;
             try {
-                "undefined" != typeof localStorage && (b = localStorage, v = !1)
+                "undefined" != typeof localStorage && (f = localStorage, p = !1)
             } catch (e) {}
-            const _ = b,
-                C = Array.from,
-                S = (Array.isArray, Object.assign, Object.keys),
-                k = e => S(e).length,
-                I = (e, t) => Object.prototype.hasOwnProperty.call(e, t),
-                U = (e, t) => {
+            const g = f,
+                y = Array.from,
+                w = (Array.isArray, Object.assign, Object.keys),
+                m = e => w(e).length,
+                b = (e, t) => Object.prototype.hasOwnProperty.call(e, t),
+                v = (e, t) => {
                     if (null == e || null == t) return ((e, t) => e === t)(e, t);
                     if (e.constructor !== t.constructor) return !1;
                     if (e === t) return !0;
                     switch (e.constructor) {
                         case ArrayBuffer:
                             e = new Uint8Array(e), t = new Uint8Array(t);
                         case Uint8Array:
@@ -72,258 +68,259 @@
                             if (e.size !== t.size) return !1;
                             for (const s of e)
                                 if (!t.has(s)) return !1;
                             break;
                         case Map:
                             if (e.size !== t.size) return !1;
                             for (const s of e.keys())
-                                if (!t.has(s) || !U(e.get(s), t.get(s))) return !1;
+                                if (!t.has(s) || !v(e.get(s), t.get(s))) return !1;
                             break;
                         case Object:
-                            if (k(e) !== k(t)) return !1;
+                            if (m(e) !== m(t)) return !1;
                             for (const s in e)
-                                if (!I(e, s) || !U(e[s], t[s])) return !1;
+                                if (!b(e, s) || !v(e[s], t[s])) return !1;
                             break;
                         case Array:
                             if (e.length !== t.length) return !1;
                             for (let s = 0; s < e.length; s++)
-                                if (!U(e[s], t[s])) return !1;
+                                if (!v(e[s], t[s])) return !1;
                             break;
                         default:
                             return !1
                     }
                     return !0
                 };
-            var T = s(4155);
-            const L = void 0 !== T && T.release && /node|io\.js/.test(T.release.name),
-                M = "undefined" != typeof window && "undefined" != typeof document && !L;
-            let E;
+            var _ = s(4155);
+            const C = void 0 !== _ && _.release && /node|io\.js/.test(_.release.name),
+                S = "undefined" != typeof window && "undefined" != typeof document && !C;
+            let k;
             "undefined" != typeof navigator && /Mac/.test(navigator.platform);
-            const A = [],
-                D = e => (() => {
-                    if (void 0 === E)
-                        if (L) {
-                            E = l();
-                            const e = T.argv;
+            const U = [],
+                I = e => (() => {
+                    if (void 0 === k)
+                        if (C) {
+                            k = d();
+                            const e = _.argv;
                             let t = null;
                             for (let s = 0; s < e.length; s++) {
                                 const n = e[s];
-                                "-" === n[0] ? (null !== t && E.set(t, ""), t = n) : null !== t ? (E.set(t, n), t = null) : A.push(n)
+                                "-" === n[0] ? (null !== t && k.set(t, ""), t = n) : null !== t ? (k.set(t, n), t = null) : U.push(n)
                             }
-                            null !== t && E.set(t, "")
-                        } else "object" == typeof location ? (E = l(), (location.search || "?").slice(1).split("&").forEach((e => {
+                            null !== t && k.set(t, "")
+                        } else "object" == typeof location ? (k = d(), (location.search || "?").slice(1).split("&").forEach((e => {
                             if (0 !== e.length) {
                                 const [t, s] = e.split("=");
-                                E.set(`--${g(t,"-")}`, s), E.set(`-${g(t,"-")}`, s)
+                                k.set(`--${i(t,"-")}`, s), k.set(`-${i(t,"-")}`, s)
                             }
-                        }))) : E = l();
-                    return E
+                        }))) : k = d();
+                    return k
                 })().has(e),
-                R = e => {
-                    return void 0 === (t = L ? T.env[e.toUpperCase()] : _.getItem(e)) ? null : t;
+                T = e => {
+                    return void 0 === (t = C ? _.env[e.toUpperCase()] : g.getItem(e)) ? null : t;
                     var t
                 };
-            D("--" + "production") || R("production");
-            const $ = L && (N = T.env.FORCE_COLOR, ["true", "1", "2"].includes(N));
-            var N;
-            !D("no-colors") && (!L || T.stdout.isTTY || $) && (!L || D("color") || $ || null !== R("COLORTERM") || (R("TERM") || "").includes("color"));
-            const O = (e, t, s) => new Uint8Array(e, t, s),
-                P = M ? e => {
+            I("--" + "production") || T("production");
+            const M = C && (A = _.env.FORCE_COLOR, ["true", "1", "2"].includes(A));
+            var A;
+            !I("no-colors") && (!C || _.stdout.isTTY || M) && (!C || I("color") || M || null !== T("COLORTERM") || (T("TERM") || "").includes("color"));
+            const D = (e, t, s) => new Uint8Array(e, t, s),
+                L = S ? e => {
                     let t = "";
-                    for (let s = 0; s < e.byteLength; s++) t += u(e[s]);
+                    for (let s = 0; s < e.byteLength; s++) t += o(e[s]);
                     return btoa(t)
                 } : e => Buffer.from(e.buffer, e.byteOffset, e.byteLength).toString("base64"),
-                x = M ? e => {
+                E = S ? e => {
                     const t = atob(e),
                         s = (n = t.length, new Uint8Array(n));
                     var n;
                     for (let e = 0; e < t.length; e++) s[e] = t.charCodeAt(e);
                     return s
                 } : e => {
                     const t = Buffer.from(e, "base64");
                     return new Uint8Array(t.buffer, t.byteOffset, t.byteLength)
                 },
-                B = new Map,
-                W = "undefined" == typeof BroadcastChannel ? class {
-                    constructor(e) {
-                        var t;
-                        this.room = e, this.onmessage = null, this._onChange = t => t.key === e && null !== this.onmessage && this.onmessage({
-                            data: x(t.newValue || "")
-                        }), t = this._onChange, v || addEventListener("storage", t)
-                    }
-                    postMessage(e) {
-                        _.setItem(this.room, P(new Uint8Array(e)))
-                    }
-                    close() {
-                        var e;
-                        e = this._onChange, v || removeEventListener("storage", e)
-                    }
-                } : BroadcastChannel,
-                j = e => h(B, e, (() => {
-                    const t = d(),
-                        s = new W(e);
-                    return s.onmessage = e => t.forEach((t => t(e.data, "broadcastchannel"))), {
-                        bc: s,
-                        subs: t
+                R = 127,
+                N = Math.floor,
+                O = (Math.ceil, Math.abs, Math.imul, Math.round, Math.log10, Math.log2, Math.log, Math.sqrt, (e, t) => e < t ? e : t),
+                $ = (Number.isNaN, Math.pow),
+                P = (Math.sign, Number.MAX_SAFE_INTEGER),
+                x = (Number.MIN_SAFE_INTEGER, Number.isInteger, Number.isNaN, Number.parseInt, e => new Error(e)),
+                B = x("Unexpected end of array"),
+                H = x("Integer out of Range");
+            class W {
+                constructor(e) {
+                    this.arr = e, this.pos = 0
+                }
+            }
+            const F = e => new W(e),
+                j = e => ((e, t) => {
+                    const s = D(e.arr.buffer, e.pos + e.arr.byteOffset, t);
+                    return e.pos += t, s
+                })(e, J(e)),
+                z = e => e.arr[e.pos++],
+                J = e => {
+                    let t = 0,
+                        s = 1;
+                    const n = e.arr.length;
+                    for (; e.pos < n;) {
+                        const n = e.arr[e.pos++];
+                        if (t += (n & R) * s, s *= 128, n < 128) return t;
+                        if (t > P) throw H
                     }
-                })),
-                F = (e, t, s = null) => {
-                    const n = j(e);
-                    n.bc.postMessage(t), n.subs.forEach((e => e(t, s)))
+                    throw B
                 },
-                H = Date.now,
-                z = Math.floor,
-                J = (Math.ceil, Math.abs, Math.imul, Math.round, Math.log10, Math.log2, Math.log, Math.sqrt, (e, t) => e < t ? e : t),
-                V = (Number.isNaN, Math.pow),
-                Y = (Math.sign, 128),
-                q = 127;
-            class G {
+                V = h ? e => h.decode(j(e)) : e => {
+                    let t = J(e);
+                    if (0 === t) return ""; {
+                        let s = String.fromCodePoint(z(e));
+                        if (--t < 100)
+                            for (; t--;) s += String.fromCodePoint(z(e));
+                        else
+                            for (; t > 0;) {
+                                const n = t < 1e4 ? t : 1e4,
+                                    o = e.arr.subarray(e.pos, e.pos + n);
+                                e.pos += n, s += String.fromCodePoint.apply(null, o), t -= n
+                            }
+                        return decodeURIComponent(escape(s))
+                    }
+                };
+            class Y {
                 constructor() {
                     this.cpos = 0, this.cbuf = new Uint8Array(100), this.bufs = []
                 }
             }
-            const X = () => new G,
-                Z = e => {
+            const q = () => new Y,
+                G = e => {
                     let t = e.cpos;
                     for (let s = 0; s < e.bufs.length; s++) t += e.bufs[s].length;
                     return t
                 },
-                K = e => {
-                    const t = new Uint8Array(Z(e));
+                X = e => {
+                    const t = new Uint8Array(G(e));
                     let s = 0;
                     for (let n = 0; n < e.bufs.length; n++) {
                         const o = e.bufs[n];
                         t.set(o, s), s += o.length
                     }
-                    return t.set(O(e.cbuf.buffer, 0, e.cpos), s), t
+                    return t.set(D(e.cbuf.buffer, 0, e.cpos), s), t
                 },
-                Q = (e, t) => {
+                Z = (e, t) => {
                     const s = e.cbuf.length;
                     e.cpos === s && (e.bufs.push(e.cbuf), e.cbuf = new Uint8Array(2 * s), e.cpos = 0), e.cbuf[e.cpos++] = t
                 },
-                ee = (e, t) => {
-                    for (; t > q;) Q(e, Y | q & t), t = z(t / 128);
-                    Q(e, q & t)
-                },
-                te = new Uint8Array(3e4),
-                se = te.length / 3,
-                ne = y && y.encodeInto ? (e, t) => {
-                    if (t.length < se) {
-                        const s = y.encodeInto(t, te).written || 0;
-                        ee(e, s);
-                        for (let t = 0; t < s; t++) Q(e, te[t])
-                    } else oe(e, w(t))
+                K = (e, t) => {
+                    for (; t > R;) Z(e, 128 | R & t), t = N(t / 128);
+                    Z(e, R & t)
+                },
+                Q = new Uint8Array(3e4),
+                ee = Q.length / 3,
+                te = c && c.encodeInto ? (e, t) => {
+                    if (t.length < ee) {
+                        const s = c.encodeInto(t, Q).written || 0;
+                        K(e, s);
+                        for (let t = 0; t < s; t++) Z(e, Q[t])
+                    } else se(e, l(t))
                 } : (e, t) => {
                     const s = unescape(encodeURIComponent(t)),
                         n = s.length;
-                    ee(e, n);
-                    for (let t = 0; t < n; t++) Q(e, s.codePointAt(t))
+                    K(e, n);
+                    for (let t = 0; t < n; t++) Z(e, s.codePointAt(t))
                 },
-                oe = (e, t) => {
-                    ee(e, t.byteLength), ((e, t) => {
+                se = (e, t) => {
+                    K(e, t.byteLength), ((e, t) => {
                         const s = e.cbuf.length,
                             n = e.cpos,
-                            o = J(s - n, t.length),
+                            o = O(s - n, t.length),
                             r = t.length - o;
-                        var c, a;
-                        e.cbuf.set(t.subarray(0, o), n), e.cpos += o, r > 0 && (e.bufs.push(e.cbuf), e.cbuf = new Uint8Array((c = 2 * s) > (a = r) ? c : a), e.cbuf.set(t.subarray(o)), e.cpos = r)
+                        var a, i;
+                        e.cbuf.set(t.subarray(0, o), n), e.cpos += o, r > 0 && (e.bufs.push(e.cbuf), e.cbuf = new Uint8Array((a = 2 * s) > (i = r) ? a : i), e.cbuf.set(t.subarray(o)), e.cpos = r)
                     })(e, t)
                 };
             new DataView(new ArrayBuffer(4));
-            const re = Number.MAX_SAFE_INTEGER,
-                ce = (Number.MIN_SAFE_INTEGER, Number.isInteger, Number.isNaN, Number.parseInt, e => new Error(e)),
-                ae = ce("Unexpected end of array"),
-                ie = ce("Integer out of Range");
-            class le {
-                constructor(e) {
-                    this.arr = e, this.pos = 0
-                }
-            }
-            const he = e => new le(e),
-                de = e => ((e, t) => {
-                    const s = O(e.arr.buffer, e.pos + e.arr.byteOffset, t);
-                    return e.pos += t, s
-                })(e, fe(e)),
-                ue = e => e.arr[e.pos++],
-                fe = e => {
-                    let t = 0,
-                        s = 1;
-                    const n = e.arr.length;
-                    for (; e.pos < n;) {
-                        const n = e.arr[e.pos++];
-                        if (t += (n & q) * s, s *= 128, n < Y) return t;
-                        if (t > re) throw ie
+            var ne = s(981);
+            const oe = () => new Set,
+                re = new Map,
+                ae = "undefined" == typeof BroadcastChannel ? class {
+                    constructor(e) {
+                        var t;
+                        this.room = e, this.onmessage = null, this._onChange = t => t.key === e && null !== this.onmessage && this.onmessage({
+                            data: E(t.newValue || "")
+                        }), t = this._onChange, p || addEventListener("storage", t)
                     }
-                    throw ae
-                },
-                pe = m ? e => m.decode(de(e)) : e => {
-                    let t = fe(e);
-                    if (0 === t) return ""; {
-                        let s = String.fromCodePoint(ue(e));
-                        if (--t < 100)
-                            for (; t--;) s += String.fromCodePoint(ue(e));
-                        else
-                            for (; t > 0;) {
-                                const n = t < 1e4 ? t : 1e4,
-                                    o = e.arr.subarray(e.pos, e.pos + n);
-                                e.pos += n, s += String.fromCodePoint.apply(null, o), t -= n
-                            }
-                        return decodeURIComponent(escape(s))
+                    postMessage(e) {
+                        g.setItem(this.room, L(new Uint8Array(e)))
+                    }
+                    close() {
+                        var e;
+                        e = this._onChange, p || removeEventListener("storage", e)
                     }
+                } : BroadcastChannel,
+                ie = e => u(re, e, (() => {
+                    const t = oe(),
+                        s = new ae(e);
+                    return s.onmessage = e => t.forEach((t => t(e.data, "broadcastchannel"))), {
+                        bc: s,
+                        subs: t
+                    }
+                })),
+                ce = (e, t, s = null) => {
+                    const n = ie(e);
+                    n.bc.postMessage(t), n.subs.forEach((e => e(t, s)))
                 },
-                ge = (e, t) => {
-                    ee(e, 0);
-                    const s = i.encodeStateVector(t);
-                    oe(e, s)
+                le = Date.now,
+                he = (e, t) => {
+                    K(e, 0);
+                    const s = ne.encodeStateVector(t);
+                    se(e, s)
                 },
-                ye = (e, t, s) => {
-                    ee(e, 1), oe(e, i.encodeStateAsUpdate(t, s))
+                de = (e, t, s) => {
+                    K(e, 1), se(e, ne.encodeStateAsUpdate(t, s))
                 },
-                we = (e, t, s) => {
+                ue = (e, t, s) => {
                     try {
-                        i.applyUpdate(t, de(e), s)
+                        ne.applyUpdate(t, j(e), s)
                     } catch (e) {
                         console.error("Caught error while handling a Yjs update", e)
                     }
                 },
-                me = we;
-            class be {
+                fe = ue;
+            class pe {
                 constructor() {
-                    this._observers = l()
+                    this._observers = d()
                 }
                 on(e, t) {
-                    h(this._observers, e, d).add(t)
+                    u(this._observers, e, oe).add(t)
                 }
                 once(e, t) {
                     const s = (...n) => {
                         this.off(e, s), t(...n)
                     };
                     this.on(e, s)
                 }
                 off(e, t) {
                     const s = this._observers.get(e);
                     void 0 !== s && (s.delete(t), 0 === s.size && this._observers.delete(e))
                 }
                 emit(e, t) {
-                    return C((this._observers.get(e) || l()).values()).forEach((e => e(...t)))
+                    return y((this._observers.get(e) || d()).values()).forEach((e => e(...t)))
                 }
                 destroy() {
-                    this._observers = l()
+                    this._observers = d()
                 }
             }
-            class ve extends be {
+            class ge extends pe {
                 constructor(e) {
                     super(), this.doc = e, this.clientID = e.clientID, this.states = new Map, this.meta = new Map, this._checkInterval = setInterval((() => {
-                        const e = H();
+                        const e = le();
                         null !== this.getLocalState() && 15e3 <= e - this.meta.get(this.clientID).lastUpdated && this.setLocalState(this.getLocalState());
                         const t = [];
                         this.meta.forEach(((s, n) => {
                             n !== this.clientID && 3e4 <= e - s.lastUpdated && this.states.has(n) && t.push(n)
-                        })), t.length > 0 && _e(this, t, "timeout")
-                    }), z(3e3)), e.on("destroy", (() => {
+                        })), t.length > 0 && ye(this, t, "timeout")
+                    }), N(3e3)), e.on("destroy", (() => {
                         this.destroy()
                     })), this.setLocalState({})
                 }
                 destroy() {
                     this.emit("destroy", [this]), this.setLocalState(null), super.destroy(), clearInterval(this._checkInterval)
                 }
                 getLocalState() {
@@ -332,51 +329,51 @@
                 setLocalState(e) {
                     const t = this.clientID,
                         s = this.meta.get(t),
                         n = void 0 === s ? 0 : s.clock + 1,
                         o = this.states.get(t);
                     null === e ? this.states.delete(t) : this.states.set(t, e), this.meta.set(t, {
                         clock: n,
-                        lastUpdated: H()
+                        lastUpdated: le()
                     });
                     const r = [],
-                        c = [],
                         a = [],
-                        i = [];
-                    null === e ? i.push(t) : null == o ? null != e && r.push(t) : (c.push(t), U(o, e) || a.push(t)), (r.length > 0 || a.length > 0 || i.length > 0) && this.emit("change", [{
+                        i = [],
+                        c = [];
+                    null === e ? c.push(t) : null == o ? null != e && r.push(t) : (a.push(t), v(o, e) || i.push(t)), (r.length > 0 || i.length > 0 || c.length > 0) && this.emit("change", [{
                         added: r,
-                        updated: a,
-                        removed: i
+                        updated: i,
+                        removed: c
                     }, "local"]), this.emit("update", [{
                         added: r,
-                        updated: c,
-                        removed: i
+                        updated: a,
+                        removed: c
                     }, "local"])
                 }
                 setLocalStateField(e, t) {
                     const s = this.getLocalState();
                     null !== s && this.setLocalState({
                         ...s,
                         [e]: t
                     })
                 }
                 getStates() {
                     return this.states
                 }
             }
-            const _e = (e, t, s) => {
+            const ye = (e, t, s) => {
                     const n = [];
                     for (let s = 0; s < t.length; s++) {
                         const o = t[s];
                         if (e.states.has(o)) {
                             if (e.states.delete(o), o === e.clientID) {
                                 const t = e.meta.get(o);
                                 e.meta.set(o, {
                                     clock: t.clock + 1,
-                                    lastUpdated: H()
+                                    lastUpdated: le()
                                 })
                             }
                             n.push(o)
                         }
                     }
                     n.length > 0 && (e.emit("change", [{
                         added: [],
@@ -384,295 +381,333 @@
                         removed: n
                     }, s]), e.emit("update", [{
                         added: [],
                         updated: [],
                         removed: n
                     }, s]))
                 },
-                Ce = (e, t, s = e.states) => {
+                we = (e, t, s = e.states) => {
                     const n = t.length,
-                        o = X();
-                    ee(o, n);
+                        o = q();
+                    K(o, n);
                     for (let r = 0; r < n; r++) {
                         const n = t[r],
-                            c = s.get(n) || null,
-                            a = e.meta.get(n).clock;
-                        ee(o, n), ee(o, a), ne(o, JSON.stringify(c))
+                            a = s.get(n) || null,
+                            i = e.meta.get(n).clock;
+                        K(o, n), K(o, i), te(o, JSON.stringify(a))
                     }
-                    return K(o)
+                    return X(o)
                 };
-            var Se = s(4155);
-            const ke = [];
-            ke[0] = (e, t, s, n, o) => {
-                ee(e, 0);
+            var me = s(4155);
+            const be = [];
+            be[0] = (e, t, s, n, o) => {
+                K(e, 0);
                 const r = ((e, t, s, n) => {
-                    const o = fe(e);
+                    const o = J(e);
                     switch (o) {
                         case 0:
                             ((e, t, s) => {
-                                ye(t, s, de(e))
+                                de(t, s, j(e))
                             })(e, t, s);
                             break;
                         case 1:
-                            we(e, s, n);
+                            ue(e, s, n);
                             break;
                         case 2:
-                            me(e, s, n);
+                            fe(e, s, n);
                             break;
                         default:
                             throw new Error("Unknown message type")
                     }
                     return o
                 })(t, e, s.doc, s);
                 n && 1 === r && !s.synced && (s.synced = !0)
-            }, ke[3] = (e, t, s, n, o) => {
-                ee(e, 1), oe(e, Ce(s.awareness, Array.from(s.awareness.getStates().keys())))
-            }, ke[1] = (e, t, s, n, o) => {
+            }, be[3] = (e, t, s, n, o) => {
+                K(e, 1), se(e, we(s.awareness, Array.from(s.awareness.getStates().keys())))
+            }, be[1] = (e, t, s, n, o) => {
                 ((e, t, s) => {
-                    const n = he(t),
-                        o = H(),
+                    const n = F(t),
+                        o = le(),
                         r = [],
-                        c = [],
                         a = [],
                         i = [],
-                        l = fe(n);
+                        c = [],
+                        l = J(n);
                     for (let t = 0; t < l; t++) {
-                        const t = fe(n);
-                        let s = fe(n);
-                        const l = JSON.parse(pe(n)),
+                        const t = J(n);
+                        let s = J(n);
+                        const l = JSON.parse(V(n)),
                             h = e.meta.get(t),
                             d = e.states.get(t),
                             u = void 0 === h ? 0 : h.clock;
                         (u < s || u === s && null === l && e.states.has(t)) && (null === l ? t === e.clientID && null != e.getLocalState() ? s++ : e.states.delete(t) : e.states.set(t, l), e.meta.set(t, {
                             clock: s,
                             lastUpdated: o
-                        }), void 0 === h && null !== l ? r.push(t) : void 0 !== h && null === l ? i.push(t) : null !== l && (U(l, d) || a.push(t), c.push(t)))
-                    }(r.length > 0 || a.length > 0 || i.length > 0) && e.emit("change", [{
+                        }), void 0 === h && null !== l ? r.push(t) : void 0 !== h && null === l ? c.push(t) : null !== l && (v(l, d) || i.push(t), a.push(t)))
+                    }(r.length > 0 || i.length > 0 || c.length > 0) && e.emit("change", [{
                         added: r,
-                        updated: a,
-                        removed: i
-                    }, s]), (r.length > 0 || c.length > 0 || i.length > 0) && e.emit("update", [{
+                        updated: i,
+                        removed: c
+                    }, s]), (r.length > 0 || a.length > 0 || c.length > 0) && e.emit("update", [{
                         added: r,
-                        updated: c,
-                        removed: i
+                        updated: a,
+                        removed: c
                     }, s])
-                })(s.awareness, de(t), s)
-            }, ke[2] = (e, t, s, n, o) => {
+                })(s.awareness, j(t), s)
+            }, be[2] = (e, t, s, n, o) => {
                 ((e, t, s) => {
-                    0 === fe(e) && s(0, pe(e))
-                })(t, s.doc, ((e, t) => Ie(s, t)))
+                    0 === J(e) && s(0, V(e))
+                })(t, s.doc, ((e, t) => ve(s, t)))
             };
-            const Ie = (e, t) => console.warn(`Permission denied to access ${e.url}.\n${t}`),
-                Ue = (e, t, s) => {
-                    const n = he(t),
-                        o = X(),
-                        r = fe(n),
-                        c = e.messageHandlers[r];
-                    return c ? c(o, n, e, s, r) : console.error("Unable to compute message"), o
+            const ve = (e, t) => console.warn(`Permission denied to access ${e.url}.\n${t}`),
+                _e = (e, t, s) => {
+                    const n = F(t),
+                        o = q(),
+                        r = J(n),
+                        a = e.messageHandlers[r];
+                    return a ? a(o, n, e, s, r) : console.error("Unable to compute message"), o
                 },
-                Te = e => {
+                Ce = e => {
                     if (e.shouldConnect && null === e.ws) {
                         const t = new e._WS(e.url);
                         t.binaryType = "arraybuffer", e.ws = t, e.wsconnecting = !0, e.wsconnected = !1, e.synced = !1, t.onmessage = s => {
-                            e.wsLastMessageReceived = H();
-                            const n = Ue(e, new Uint8Array(s.data), !0);
-                            Z(n) > 1 && t.send(K(n))
+                            e.wsLastMessageReceived = le();
+                            const n = _e(e, new Uint8Array(s.data), !0);
+                            G(n) > 1 && t.send(X(n))
                         }, t.onerror = t => {
                             e.emit("connection-error", [t, e])
                         }, t.onclose = t => {
-                            e.emit("connection-close", [t, e]), e.ws = null, e.wsconnecting = !1, e.wsconnected ? (e.wsconnected = !1, e.synced = !1, _e(e.awareness, Array.from(e.awareness.getStates().keys()).filter((t => t !== e.doc.clientID)), e), e.emit("status", [{
+                            e.emit("connection-close", [t, e]), e.ws = null, e.wsconnecting = !1, e.wsconnected ? (e.wsconnected = !1, e.synced = !1, ye(e.awareness, Array.from(e.awareness.getStates().keys()).filter((t => t !== e.doc.clientID)), e), e.emit("status", [{
                                 status: "disconnected"
-                            }])) : e.wsUnsuccessfulReconnects++, setTimeout(Te, J(100 * V(2, e.wsUnsuccessfulReconnects), e.maxBackoffTime), e)
+                            }])) : e.wsUnsuccessfulReconnects++, setTimeout(Ce, O(100 * $(2, e.wsUnsuccessfulReconnects), e.maxBackoffTime), e)
                         }, t.onopen = () => {
-                            e.wsLastMessageReceived = H(), e.wsconnecting = !1, e.wsconnected = !0, e.wsUnsuccessfulReconnects = 0, e.emit("status", [{
+                            e.wsLastMessageReceived = le(), e.wsconnecting = !1, e.wsconnected = !0, e.wsUnsuccessfulReconnects = 0, e.emit("status", [{
                                 status: "connected"
                             }]);
-                            const s = X();
-                            if (ee(s, 0), ge(s, e.doc), t.send(K(s)), null !== e.awareness.getLocalState()) {
-                                const s = X();
-                                ee(s, 1), oe(s, Ce(e.awareness, [e.doc.clientID])), t.send(K(s))
+                            const s = q();
+                            if (K(s, 0), he(s, e.doc), t.send(X(s)), null !== e.awareness.getLocalState()) {
+                                const s = q();
+                                K(s, 1), se(s, we(e.awareness, [e.doc.clientID])), t.send(X(s))
                             }
                         }, e.emit("status", [{
                             status: "connecting"
                         }])
                     }
                 },
-                Le = (e, t) => {
+                Se = (e, t) => {
                     const s = e.ws;
-                    e.wsconnected && s && s.readyState === s.OPEN && s.send(t), e.bcconnected && F(e.bcChannel, t, e)
+                    e.wsconnected && s && s.readyState === s.OPEN && s.send(t), e.bcconnected && ce(e.bcChannel, t, e)
                 };
-            class Me extends be {
+            class ke extends pe {
                 constructor(e, t, s, {
                     connect: n = !0,
-                    awareness: o = new ve(s),
+                    awareness: o = new ge(s),
                     params: r = {},
-                    WebSocketPolyfill: c = WebSocket,
-                    resyncInterval: a = -1,
-                    maxBackoffTime: i = 2500,
+                    WebSocketPolyfill: a = WebSocket,
+                    resyncInterval: i = -1,
+                    maxBackoffTime: c = 2500,
                     disableBc: l = !1
                 } = {}) {
                     for (super();
                         "/" === e[e.length - 1];) e = e.slice(0, e.length - 1);
                     const h = (e => ((e, t) => {
                         const s = [];
                         for (const n in e) s.push(t(e[n], n));
                         return s
                     })(e, ((e, t) => `${encodeURIComponent(t)}=${encodeURIComponent(e)}`)).join("&"))(r);
-                    this.maxBackoffTime = i, this.bcChannel = e + "/" + t, this.url = e + "/" + t + (0 === h.length ? "" : "?" + h), this.roomname = t, this.doc = s, this._WS = c, this.awareness = o, this.wsconnected = !1, this.wsconnecting = !1, this.bcconnected = !1, this.disableBc = l, this.wsUnsuccessfulReconnects = 0, this.messageHandlers = ke.slice(), this._synced = !1, this.ws = null, this.wsLastMessageReceived = 0, this.shouldConnect = n, this._resyncInterval = 0, a > 0 && (this._resyncInterval = setInterval((() => {
+                    this.maxBackoffTime = c, this.bcChannel = e + "/" + t, this.url = e + "/" + t + (0 === h.length ? "" : "?" + h), this.roomname = t, this.doc = s, this._WS = a, this.awareness = o, this.wsconnected = !1, this.wsconnecting = !1, this.bcconnected = !1, this.disableBc = l, this.wsUnsuccessfulReconnects = 0, this.messageHandlers = be.slice(), this._synced = !1, this.ws = null, this.wsLastMessageReceived = 0, this.shouldConnect = n, this._resyncInterval = 0, i > 0 && (this._resyncInterval = setInterval((() => {
                         if (this.ws && this.ws.readyState === WebSocket.OPEN) {
-                            const e = X();
-                            ee(e, 0), ge(e, s), this.ws.send(K(e))
+                            const e = q();
+                            K(e, 0), he(e, s), this.ws.send(X(e))
                         }
-                    }), a)), this._bcSubscriber = (e, t) => {
+                    }), i)), this._bcSubscriber = (e, t) => {
                         if (t !== this) {
-                            const t = Ue(this, new Uint8Array(e), !1);
-                            Z(t) > 1 && F(this.bcChannel, K(t), this)
+                            const t = _e(this, new Uint8Array(e), !1);
+                            G(t) > 1 && ce(this.bcChannel, X(t), this)
                         }
                     }, this._updateHandler = (e, t) => {
                         if (t !== this) {
-                            const t = X();
-                            ee(t, 0), ((e, t) => {
-                                ee(e, 2), oe(e, t)
-                            })(t, e), Le(this, K(t))
+                            const t = q();
+                            K(t, 0), ((e, t) => {
+                                K(e, 2), se(e, t)
+                            })(t, e), Se(this, X(t))
                         }
                     }, this.doc.on("update", this._updateHandler), this._awarenessUpdateHandler = ({
                         added: e,
                         updated: t,
                         removed: s
                     }, n) => {
                         const r = e.concat(t).concat(s),
-                            c = X();
-                        ee(c, 1), oe(c, Ce(o, r)), Le(this, K(c))
+                            a = q();
+                        K(a, 1), se(a, we(o, r)), Se(this, X(a))
                     }, this._unloadHandler = () => {
-                        _e(this.awareness, [s.clientID], "window unload")
-                    }, "undefined" != typeof window ? window.addEventListener("unload", this._unloadHandler) : void 0 !== Se && Se.on("exit", this._unloadHandler), o.on("update", this._awarenessUpdateHandler), this._checkInterval = setInterval((() => {
-                        this.wsconnected && 3e4 < H() - this.wsLastMessageReceived && this.ws.close()
+                        ye(this.awareness, [s.clientID], "window unload")
+                    }, "undefined" != typeof window ? window.addEventListener("unload", this._unloadHandler) : void 0 !== me && me.on("exit", this._unloadHandler), o.on("update", this._awarenessUpdateHandler), this._checkInterval = setInterval((() => {
+                        this.wsconnected && 3e4 < le() - this.wsLastMessageReceived && this.ws.close()
                     }), 3e3), n && this.connect()
                 }
                 get synced() {
                     return this._synced
                 }
                 set synced(e) {
                     this._synced !== e && (this._synced = e, this.emit("synced", [e]), this.emit("sync", [e]))
                 }
                 destroy() {
-                    0 !== this._resyncInterval && clearInterval(this._resyncInterval), clearInterval(this._checkInterval), this.disconnect(), "undefined" != typeof window ? window.removeEventListener("unload", this._unloadHandler) : void 0 !== Se && Se.off("exit", this._unloadHandler), this.awareness.off("update", this._awarenessUpdateHandler), this.doc.off("update", this._updateHandler), super.destroy()
+                    0 !== this._resyncInterval && clearInterval(this._resyncInterval), clearInterval(this._checkInterval), this.disconnect(), "undefined" != typeof window ? window.removeEventListener("unload", this._unloadHandler) : void 0 !== me && me.off("exit", this._unloadHandler), this.awareness.off("update", this._awarenessUpdateHandler), this.doc.off("update", this._updateHandler), super.destroy()
                 }
                 connectBc() {
                     if (this.disableBc) return;
                     var e, t;
-                    this.bcconnected || (e = this.bcChannel, t = this._bcSubscriber, j(e).subs.add(t), this.bcconnected = !0);
-                    const s = X();
-                    ee(s, 0), ge(s, this.doc), F(this.bcChannel, K(s), this);
-                    const n = X();
-                    ee(n, 0), ye(n, this.doc), F(this.bcChannel, K(n), this);
-                    const o = X();
-                    ee(o, 3), F(this.bcChannel, K(o), this);
-                    const r = X();
-                    ee(r, 1), oe(r, Ce(this.awareness, [this.doc.clientID])), F(this.bcChannel, K(r), this)
+                    this.bcconnected || (e = this.bcChannel, t = this._bcSubscriber, ie(e).subs.add(t), this.bcconnected = !0);
+                    const s = q();
+                    K(s, 0), he(s, this.doc), ce(this.bcChannel, X(s), this);
+                    const n = q();
+                    K(n, 0), de(n, this.doc), ce(this.bcChannel, X(n), this);
+                    const o = q();
+                    K(o, 3), ce(this.bcChannel, X(o), this);
+                    const r = q();
+                    K(r, 1), se(r, we(this.awareness, [this.doc.clientID])), ce(this.bcChannel, X(r), this)
                 }
                 disconnectBc() {
-                    const e = X();
-                    ee(e, 1), oe(e, Ce(this.awareness, [this.doc.clientID], new Map)), Le(this, K(e)), this.bcconnected && (((e, t) => {
-                        const s = j(e);
-                        s.subs.delete(t) && 0 === s.subs.size && (s.bc.close(), B.delete(e))
+                    const e = q();
+                    K(e, 1), se(e, we(this.awareness, [this.doc.clientID], new Map)), Se(this, X(e)), this.bcconnected && (((e, t) => {
+                        const s = ie(e);
+                        s.subs.delete(t) && 0 === s.subs.size && (s.bc.close(), re.delete(e))
                     })(this.bcChannel, this._bcSubscriber), this.bcconnected = !1)
                 }
                 disconnect() {
                     this.shouldConnect = !1, this.disconnectBc(), null !== this.ws && this.ws.close()
                 }
                 connect() {
-                    this.shouldConnect = !0, this.wsconnected || null !== this.ws || (Te(this), this.connectBc())
+                    this.shouldConnect = !0, this.wsconnected || null !== this.ws || (Ce(this), this.connectBc())
+                }
+            }
+            var Ue;
+            ! function(e) {
+                e[e.CHAT = 125] = "CHAT"
+            }(Ue || (Ue = {}));
+            class Ie extends ke {
+                constructor(e) {
+                    super(e.url, e.roomID, e.awareness.doc, {
+                        awareness: e.awareness
+                    }), this._isDisposed = !1, this._awareness = e.awareness;
+                    const t = e.user;
+                    t.ready.then((() => this._onUserChanged(t))).catch((e => console.error(e))), t.userChanged.connect(this._onUserChanged, this), this._chatMessage = new n.Signal(this), this.messageHandlers[Ue.CHAT] = (e, t, s, n, o) => {
+                        const r = V(t),
+                            a = JSON.parse(r);
+                        console.debug("Chat:", a), this._chatMessage.emit(a)
+                    }
+                }
+                get isDisposed() {
+                    return this._isDisposed
+                }
+                get chatMessage() {
+                    return this._chatMessage
+                }
+                dispose() {
+                    this._isDisposed || (this.destroy(), this._isDisposed = !0)
+                }
+                sendMessage(e) {
+                    console.debug("Send message:", e);
+                    const t = q();
+                    K(t, Ue.CHAT), te(t, e), this.ws.send(X(t))
+                }
+                _onUserChanged(e) {
+                    this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            class Ee {
+            var Te = s(9993),
+                Me = s(4238),
+                Ae = s(5350),
+                De = s(7930);
+            class Le {
                 constructor(e) {
                     this._onConnectionClosed = e => {
-                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, r.showErrorMessage)(this._trans.__("Document session error"), e.reason, [r.Dialog.okButton()]), this._sharedModel.dispose())
+                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, Ae.showErrorMessage)(this._trans.__("Document session error"), e.reason, [Ae.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var t;
                         e && (this._ready.resolve(), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync))
-                    }, this._ready = new c.PromiseDelegate, this._isDisposed = !1, this._path = e.path, this._contentType = e.contentType, this._format = e.format, this._serverUrl = e.url, this._sharedModel = e.model, this._awareness = e.model.awareness, this._yWebsocketProvider = null, this._trans = e.translator;
+                    }, this._ready = new De.PromiseDelegate, this._isDisposed = !1, this._path = e.path, this._contentType = e.contentType, this._format = e.format, this._serverUrl = e.url, this._sharedModel = e.model, this._awareness = e.model.awareness, this._yWebsocketProvider = null, this._trans = e.translator;
                     const t = e.user;
                     t.ready.then((() => {
                         this._onUserChanged(t)
                     })).catch((e => console.error(e))), t.userChanged.connect(this._onUserChanged, this), this._connect().catch((e => console.warn(e)))
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get ready() {
                     return this._ready.promise
                 }
                 dispose() {
                     var e, t, s;
-                    this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync), null === (s = this._yWebsocketProvider) || void 0 === s || s.destroy(), a.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (t = this._yWebsocketProvider) || void 0 === t || t.off("sync", this._onSync), null === (s = this._yWebsocketProvider) || void 0 === s || s.destroy(), n.Signal.clearData(this))
                 }
                 async _connect() {
                     const e = await async function(e, t, s) {
-                        const r = o.ServerConnection.makeSettings(),
-                            c = n.URLExt.join(r.baseUrl, "api/collaboration/session", encodeURIComponent(s)),
-                            a = {
+                        const n = Me.ServerConnection.makeSettings(),
+                            o = Te.URLExt.join(n.baseUrl, "api/collaboration/session", encodeURIComponent(s)),
+                            r = {
                                 method: "PUT",
                                 body: JSON.stringify({
                                     format: e,
                                     type: t
                                 })
                             };
-                        let i;
+                        let a;
                         try {
-                            i = await o.ServerConnection.makeRequest(c, a, r)
+                            a = await Me.ServerConnection.makeRequest(o, r, n)
                         } catch (e) {
-                            throw new o.ServerConnection.NetworkError(e)
+                            throw new Me.ServerConnection.NetworkError(e)
                         }
-                        let l = await i.text();
-                        if (l.length > 0) try {
-                            l = JSON.parse(l)
+                        let i = await a.text();
+                        if (i.length > 0) try {
+                            i = JSON.parse(i)
                         } catch (e) {
-                            console.log("Not a JSON response body.", i)
+                            console.log("Not a JSON response body.", a)
                         }
-                        if (!i.ok) throw new o.ServerConnection.ResponseError(i, l.message || l);
-                        return l
+                        if (!a.ok) throw new Me.ServerConnection.ResponseError(a, i.message || i);
+                        return i
                     }(this._format, this._contentType, this._path);
-                    this._yWebsocketProvider = new Me(this._serverUrl, `${e.format}:${e.type}:${e.fileId}`, this._sharedModel.ydoc, {
+                    this._yWebsocketProvider = new ke(this._serverUrl, `${e.format}:${e.type}:${e.fileId}`, this._sharedModel.ydoc, {
                         disableBc: !0,
                         params: {
                             sessionId: e.sessionId
                         },
                         awareness: this._awareness
                     }), this._yWebsocketProvider.on("sync", this._onSync), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            class Ae extends o.Drive {
+            class Ee extends Me.Drive {
                 constructor(e, t) {
                     super({
                         name: "RTC"
                     }), this._onCreate = (e, t) => {
                         if ("string" == typeof e.format) try {
-                            const s = new Ee({
-                                    url: n.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
+                            const s = new Le({
+                                    url: Te.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
                                     path: e.path,
                                     format: e.format,
                                     contentType: e.contentType,
                                     model: t,
                                     user: this._user,
                                     translator: this._trans
                                 }),
-                                o = `${e.format}:${e.contentType}:${e.path}`;
-                            this._providers.set(o, s), t.disposed.connect((() => {
-                                const e = this._providers.get(o);
-                                e && (e.dispose(), this._providers.delete(o))
+                                n = `${e.format}:${e.contentType}:${e.path}`;
+                            this._providers.set(n, s), t.disposed.connect((() => {
+                                const e = this._providers.get(n);
+                                e && (e.dispose(), this._providers.delete(n))
                             }))
                         } catch (t) {
                             console.error(`Failed to open websocket connection for ${e.path}.\n:${t}`)
                         }
-                    }, this._user = e, this._trans = t, this._providers = new Map, this.sharedModelFactory = new De(this._onCreate)
+                    }, this._user = e, this._trans = t, this._providers = new Map, this.sharedModelFactory = new Re(this._onCreate)
                 }
                 dispose() {
                     this.isDisposed || (this._providers.forEach((e => e.dispose())), this._providers.clear(), super.dispose())
                 }
                 async get(e, t) {
                     if (t && t.format && t.type) {
                         const s = `${t.format}:${t.type}:${e}`,
@@ -694,15 +729,15 @@
                             ...t,
                             content: !1
                         })
                     }
                     return super.save(e, t)
                 }
             }
-            class De {
+            class Re {
                 constructor(e) {
                     this._onCreate = e, this.collaborative = !0, this._documentFactories = new Map
                 }
                 registerDocumentFactory(e, t) {
                     if (this._documentFactories.has(e)) throw new Error(`The content type ${e} already exists`);
                     this._documentFactories.set(e, t)
                 }
@@ -711,28 +746,28 @@
                         if (e.collaborative && this._documentFactories.has(e.contentType)) {
                             const t = this._documentFactories.get(e.contentType)(e);
                             return this._onCreate(e, t), t
                         }
                     } else console.warn(`Only defined format are supported; got ${e.format}.`)
                 }
             }
-            const Re = new c.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
+            const Ne = new De.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
         },
         4155: e => {
             var t, s, n = e.exports = {};
 
             function o() {
                 throw new Error("setTimeout has not been defined")
             }
 
             function r() {
                 throw new Error("clearTimeout has not been defined")
             }
 
-            function c(e) {
+            function a(e) {
                 if (t === setTimeout) return setTimeout(e, 0);
                 if ((t === o || !t) && setTimeout) return t = setTimeout, setTimeout(e, 0);
                 try {
                     return t(e, 0)
                 } catch (s) {
                     try {
                         return t.call(null, e, 0)
@@ -748,31 +783,31 @@
                 }
                 try {
                     s = "function" == typeof clearTimeout ? clearTimeout : r
                 } catch (e) {
                     s = r
                 }
             }();
-            var a, i = [],
+            var i, c = [],
                 l = !1,
                 h = -1;
 
             function d() {
-                l && a && (l = !1, a.length ? i = a.concat(i) : h = -1, i.length && u())
+                l && i && (l = !1, i.length ? c = i.concat(c) : h = -1, c.length && u())
             }
 
             function u() {
                 if (!l) {
-                    var e = c(d);
+                    var e = a(d);
                     l = !0;
-                    for (var t = i.length; t;) {
-                        for (a = i, i = []; ++h < t;) a && a[h].run();
-                        h = -1, t = i.length
+                    for (var t = c.length; t;) {
+                        for (i = c, c = []; ++h < t;) i && i[h].run();
+                        h = -1, t = c.length
                     }
-                    a = null, l = !1,
+                    i = null, l = !1,
                         function(e) {
                             if (s === clearTimeout) return clearTimeout(e);
                             if ((s === r || !s) && clearTimeout) return s = clearTimeout, clearTimeout(e);
                             try {
                                 return s(e)
                             } catch (t) {
                                 try {
@@ -790,15 +825,15 @@
             }
 
             function p() {}
             n.nextTick = function(e) {
                 var t = new Array(arguments.length - 1);
                 if (arguments.length > 1)
                     for (var s = 1; s < arguments.length; s++) t[s - 1] = arguments[s];
-                i.push(new f(e, t)), 1 !== i.length || l || c(u)
+                c.push(new f(e, t)), 1 !== c.length || l || a(u)
             }, f.prototype.run = function() {
                 this.fun.apply(null, this.array)
             }, n.title = "browser", n.browser = !0, n.env = {}, n.argv = [], n.version = "", n.versions = {}, n.on = p, n.addListener = p, n.once = p, n.off = p, n.removeListener = p, n.removeAllListeners = p, n.emit = p, n.prependListener = p, n.prependOnceListener = p, n.listeners = function(e) {
                 return []
             }, n.binding = function(e) {
                 throw new Error("process.binding is not supported")
             }, n.cwd = function() {
```

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/797.6a3ff8bb4f69a7056ffc.js` & `glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/797.6775a9c675159fcc67ec.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -297,17 +297,17 @@
                 }
             }
             var _ = s(2164),
                 m = s(6029);
             const p = "application/x-gluejupyter-dataset";
             var b;
             ! function(e) {
-                e.createNew = "glue-control:new-session", e.new1DHistogram = "glue-control:new-1d-histogram-viewer", e.new1DProfile = "glue-control:new-1d-profile-viewer", e.new2DImage = "glue-control:new-2d-image-viewer", e.new2DScatter = "glue-control:new-2d-scatter-viewer", e.new3DScatter = "glue-control:new-3d-scatter-viewer", e.newTable = "glue-control:new-table-viewer", e.openControlPanel = "glue-control:open-control-panel", e.closeControlPanel = "glue-control:close-control-panel"
+                e.createNew = "glue-control:new-session", e.new1DHistogram = "glue-control:new-1d-histogram-viewer", e.new1DProfile = "glue-control:new-1d-profile-viewer", e.new2DImage = "glue-control:new-2d-image-viewer", e.new2DScatter = "glue-control:new-2d-scatter-viewer", e.new3DScatter = "glue-control:new-3d-scatter-viewer", e.newTable = "glue-control:new-table-viewer", e.openControlPanel = "glue-control:open-control-panel", e.closeControlPanel = "glue-control:close-control-panel", e.addViewerLayer = "glue-control:add-viewer-layer"
             }(b || (b = {}));
-            class C extends d.ReactWidget {
+            class v extends d.ReactWidget {
                 constructor(e) {
                     super(), this._dataNames = [], this._currentSharedModel = null;
                     const {
                         model: t,
                         commands: s
                     } = e;
                     this._model = t, this.title.label = "Datasets", this._model.glueSessionChanged.connect(this._sessionChanged, this), this._menu = new o.Menu({
@@ -368,15 +368,15 @@
                 render() {
                     return m.createElement("ul", {
                         className: "glue-Control-datasets-container",
                         onContextMenu: this._contextMenu.bind(this)
                     }, this._dataNames.map(this._getDatasetItem.bind(this)))
                 }
             }
-            class v extends o.Widget {
+            class C extends o.Widget {
                 constructor(e) {
                     super(), this.title.label = "Subsets", this._model = e.model, this._model
                 }
             }
             class y extends d.SidePanel {
                 constructor(e) {
                     super(), this.title.label = "Data", this.toolbar.addItem("Add data", new d.ToolbarButton({
@@ -400,20 +400,20 @@
                                 }
                         }
                     })), this._model = e.model, this.toolbar.addItem("New Subset", new d.ToolbarButton({
                         tooltip: "New Subset",
                         label: "New Subset",
                         onClick: () => console.log("clicked")
                     }));
-                    const t = new C({
+                    const t = new v({
                         model: this._model,
                         commands: e.commands
                     });
                     this.addWidget(t);
-                    const s = new v({
+                    const s = new C({
                         model: this._model
                     });
                     this.addWidget(s)
                 }
             }
             class w extends o.Widget {
                 constructor() {
@@ -471,26 +471,26 @@
                 svgstr: '<?xml version="1.0" encoding="UTF-8"?>\n<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN" "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">\n<svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="20px" height="20px" style="shape-rendering:geometricPrecision; text-rendering:geometricPrecision; image-rendering:optimizeQuality; fill-rule:evenodd; clip-rule:evenodd" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 200 200">\n<g><path style="opacity:0.974" fill="#1b1819" d="M 75.5,5.5 C 87.8333,5.5 100.167,5.5 112.5,5.5C 112.5,27.5 112.5,49.5 112.5,71.5C 123.167,71.5 133.833,71.5 144.5,71.5C 144.5,79.1667 144.5,86.8333 144.5,94.5C 155.167,94.5 165.833,94.5 176.5,94.5C 176.5,125.833 176.5,157.167 176.5,188.5C 121.5,188.5 66.5,188.5 11.5,188.5C 11.5,154.5 11.5,120.5 11.5,86.5C 22.1667,86.5 32.8333,86.5 43.5,86.5C 43.5,67.8333 43.5,49.1667 43.5,30.5C 54.1667,30.5 64.8333,30.5 75.5,30.5C 75.5,22.1667 75.5,13.8333 75.5,5.5 Z"/></g>\n<g><path style="opacity:1" fill="#95979b" d="M 80.5,10.5 C 89.5,10.5 98.5,10.5 107.5,10.5C 107.5,30.8333 107.5,51.1667 107.5,71.5C 107.5,109.167 107.5,146.833 107.5,184.5C 98.5,184.5 89.5,184.5 80.5,184.5C 80.5,126.5 80.5,68.5 80.5,10.5 Z"/></g>\n<g><path style="opacity:1" fill="#59585a" d="M 80.5,10.5 C 89.6517,9.50644 98.985,9.17311 108.5,9.5C 108.831,30.3401 108.497,51.0067 107.5,71.5C 107.5,51.1667 107.5,30.8333 107.5,10.5C 98.5,10.5 89.5,10.5 80.5,10.5 Z"/></g>\n<g><path style="opacity:1" fill="#95989b" d="M 112.5,76.5 C 121.5,76.5 130.5,76.5 139.5,76.5C 139.5,112.167 139.5,147.833 139.5,183.5C 130.5,183.5 121.5,183.5 112.5,183.5C 112.5,147.833 112.5,112.167 112.5,76.5 Z"/></g>\n<g><path style="opacity:1" fill="#5b5b5d" d="M 43.5,91.5 C 34.5,91.5 25.5,91.5 16.5,91.5C 16.5,122.167 16.5,152.833 16.5,183.5C 25.5,183.5 34.5,183.5 43.5,183.5C 34.3483,184.494 25.015,184.827 15.5,184.5C 15.5,153.167 15.5,121.833 15.5,90.5C 25.015,90.1731 34.3483,90.5064 43.5,91.5 Z"/></g>\n<g><path style="opacity:1" fill="#95989b" d="M 43.5,91.5 C 43.5,122.167 43.5,152.833 43.5,183.5C 34.5,183.5 25.5,183.5 16.5,183.5C 16.5,152.833 16.5,122.167 16.5,91.5C 25.5,91.5 34.5,91.5 43.5,91.5 Z"/></g>\n<g><path style="opacity:1" fill="#626164" d="M 112.5,76.5 C 121.652,75.5064 130.985,75.1731 140.5,75.5C 140.5,111.833 140.5,148.167 140.5,184.5C 130.985,184.827 121.652,184.494 112.5,183.5C 121.5,183.5 130.5,183.5 139.5,183.5C 139.5,147.833 139.5,112.167 139.5,76.5C 130.5,76.5 121.5,76.5 112.5,76.5 Z"/></g>\n<g><path style="opacity:1" fill="#95989b" d="M 171.5,99.5 C 171.5,127.5 171.5,155.5 171.5,183.5C 162.5,183.5 153.5,183.5 144.5,183.5C 144.5,155.5 144.5,127.5 144.5,99.5C 153.5,99.5 162.5,99.5 171.5,99.5 Z"/></g>\n<g><path style="opacity:1" fill="#727275" d="M 171.5,99.5 C 172.498,127.662 172.831,155.995 172.5,184.5C 162.985,184.827 153.652,184.494 144.5,183.5C 153.5,183.5 162.5,183.5 171.5,183.5C 171.5,155.5 171.5,127.5 171.5,99.5 Z"/></g>\n<g><path style="opacity:1" fill="#86101a" d="M 48.5,35.5 C 48.5,84.8333 48.5,134.167 48.5,183.5C 57.5,183.5 66.5,183.5 75.5,183.5C 75.5,134.167 75.5,84.8333 75.5,35.5C 76.4989,84.9972 76.8322,134.664 76.5,184.5C 66.8333,184.5 57.1667,184.5 47.5,184.5C 47.1678,134.664 47.5011,84.9972 48.5,35.5 Z"/></g>\n<g><path style="opacity:1" fill="#e4001b" d="M 48.5,35.5 C 57.5,35.5 66.5,35.5 75.5,35.5C 75.5,84.8333 75.5,134.167 75.5,183.5C 66.5,183.5 57.5,183.5 48.5,183.5C 48.5,134.167 48.5,84.8333 48.5,35.5 Z"/></g>\n</svg>\n'
             });
             var M = s(4163),
                 D = s(7930);
             const I = new D.Token("glueCanvasTracker");
             var E = s(4470),
                 x = s(3781),
-                T = s(1554);
-            const L = {
+                L = s(1554);
+            const T = {
                 id: "glue-jupyterlab:control-panel",
                 autoStart: !0,
                 requires: [M.ILayoutRestorer, I, E.IRenderMimeRegistry],
                 activate: (e, t, s, i) => {
                     const {
                         shell: a,
                         commands: d
                     } = e, o = new n({
                         tracker: s
-                    }), r = new x.DocumentRegistry, l = new T.DocumentManager({
+                    }), r = new x.DocumentRegistry, l = new L.DocumentManager({
                         registry: r,
                         manager: e.serviceManager,
                         opener
                     }), h = new S({
                         model: o,
                         tracker: s,
                         commands: d,
@@ -632,28 +632,38 @@
                                         gridItem: null == e ? void 0 : e.gridItem
                                     })
                                 }
                             }), e.addCommand(b.closeControlPanel, {
                                 execute: () => {
                                     t.sharedModel && t.clearConfig()
                                 }
+                            }), e.addCommand(b.addViewerLayer, {
+                                execute: async e => {
+                                    const s = t.currentSessionKernel();
+                                    if (void 0 === s) return;
+                                    const i = `\n      GLUE_SESSION.add_viewer_layer("${e.tab}", "${e.viewer}", "${e.data}")\n      `,
+                                        n = s.requestExecute({
+                                            code: i
+                                        }, !1);
+                                    await n.done
+                                }
                             })
                         }(d, o)
                 }
             };
             var P = s(858),
                 W = s(5350),
                 N = s(3262),
                 B = s(1919),
                 O = s(8844);
             const A = JSON.parse('{"DataCollection":{"_protocol":4,"_type":"glue.core.data_collection.DataCollection","cids":[],"components":[],"data":[],"groups":[],"links":[],"subset_group_count":0},"Session":{"_type":"glue.core.session.Session"},"__main__":{"_type":"glue.app.qt.application.GlueApplication","data":"DataCollection","plugins":[],"session":"Session","tab_names":["Tab 1"],"viewers":[[]]}}');
-            var H = s(2293),
-                R = s(981);
-            const z = (0, H.createMutex)();
-            class G extends H.YDocument {
+            var R = s(2293),
+                H = s(981);
+            const z = (0, R.createMutex)();
+            class G extends R.YDocument {
                 constructor() {
                     super(), this.version = "1.0.0", this._contentsObserver = e => {
                         const t = this.contents;
                         this._changed.emit(t), this._contentsChanged.emit(t)
                     }, this._attributesObserver = e => {
                         this._attributesChanged.emit({})
                     }, this._datasetObserver = e => {
@@ -720,19 +730,24 @@
                 setValue(e, t) {
                     this._contents.set(e, t)
                 }
                 addTab() {
                     let e = 1,
                         t = "Tab 1";
                     for (; this._tabs.has(t);) e += 1, t = `Tab ${e}`;
-                    const s = new R.Map;
+                    const s = new H.Map;
                     this.transact((() => {
                         this._tabs.set(t, s)
                     }), !1)
                 }
+                removeTab(e) {
+                    this._tabs.has(e) && this.transact((() => {
+                        this._tabs.delete(e)
+                    }), !1)
+                }
                 getTabNames() {
                     return [...this._tabs.keys()]
                 }
                 getTabData(e) {
                     const t = this._tabs.get(e);
                     if (t) return D.JSONExt.deepCopy(t.toJSON())
                 }
@@ -870,24 +885,368 @@
             }
             class U extends W.WidgetTracker {
                 currentSharedModel() {
                     var e;
                     return null === (e = this.currentWidget) || void 0 === e ? void 0 : e.context.model.sharedModel
                 }
             }
-            var J, F = s(7120),
-                V = s(5633),
-                $ = s(4784);
-            class Z extends o.Layout {
+            var V = s(9993),
+                J = s(4238);
+            const F = "glue.core.component_link.ComponentLink",
+                $ = "glue.core.link_helpers.identity",
+                Z = {
+                    _type: "types.FunctionType",
+                    function: $
+                };
+            class K {
+                constructor(e) {
+                    this._currentDatasets = ["", ""], this._datasetsChanged = new i.Signal(this), this._advLinksPromise = new D.PromiseDelegate, this._advLinkCategories = {}, this._identityLinks = new Map, this._advancedLinks = new Map, this._linksChanged = new i.Signal(this), this._sharedModel = e.sharedModel, this._sharedModel.linksChanged.connect(this.onLinksChanged, this), this._sharedModel.datasetChanged.connect(this.onDatasetsChanged, this), this._getAdvancedLinksCategories()
+                }
+                get sharedModel() {
+                    return this._sharedModel
+                }
+                get currentDatasets() {
+                    return this._currentDatasets
+                }
+                set currentDatasets(e) {
+                    this._currentDatasets = e, this._datasetsChanged.emit(this._currentDatasets)
+                }
+                setCurrentDataset(e, t) {
+                    this._currentDatasets[e] = t, this._datasetsChanged.emit(this._currentDatasets)
+                }
+                get currentDatasetsChanged() {
+                    return this._datasetsChanged
+                }
+                get identityLinks() {
+                    return this._identityLinks
+                }
+                get advLinkCategories() {
+                    return this._advLinkCategories
+                }
+                get advancedLinks() {
+                    return this._advancedLinks
+                }
+                get linksChanged() {
+                    return this._linksChanged
+                }
+                get advLinksPromise() {
+                    return this._advLinksPromise.promise
+                }
+                async _getAdvancedLinksCategories() {
+                    const e = J.ServerConnection.makeSettings(),
+                        t = V.URLExt.join(e.baseUrl, "/glue-jupyterlab/advanced-links");
+                    let s;
+                    try {
+                        s = await J.ServerConnection.makeRequest(t, {}, e)
+                    } catch (e) {
+                        throw new J.ServerConnection.NetworkError(e)
+                    }
+                    const i = await s.json();
+                    if (!s.ok) throw this._advLinksPromise.reject(i.message), new J.ServerConnection.ResponseError(s, i.message);
+                    Object.entries(i.data).forEach((([e, t]) => {
+                        this._advLinkCategories[e] = t
+                    })), this._advLinksPromise.resolve(this._advLinkCategories)
+                }
+                onDatasetsChanged() {
+                    if (this._sharedModel.dataset) {
+                        const e = Object.keys(this._sharedModel.dataset);
+                        this._currentDatasets = [e.length > 1 ? e[0] : "", e.length > 1 ? e[1] : ""], this._datasetsChanged.emit(this._currentDatasets)
+                    }
+                }
+                onLinksChanged() {
+                    var e;
+                    this._identityLinks = new Map, this._advancedLinks = new Map, Object.entries(null === (e = this._sharedModel) || void 0 === e ? void 0 : e.links).forEach((([e, t], s) => {
+                        var i;
+                        t._type === F && (null === (i = t.using) || void 0 === i ? void 0 : i.function) === $ ? this._identityLinks.set(e, t) : this._advancedLinks.set(e, t)
+                    })), this._linksChanged.emit()
+                }
+            }
+            class Y extends o.Panel {
+                constructor(e) {
+                    super(), this._header = void 0, this._content = void 0, this._linkEditorModel = e.linkEditorModel, this._sharedModel = e.sharedModel, this.addClass("glue-LinkEditor-widget"), this._sharedModel.changed.connect(this.onSharedModelChanged, this)
+                }
+                get header() {
+                    return this._header
+                }
+                set header(e) {
+                    this._header && this._header.dispose(), e && (e.addClass("glue-LinkEditor-header"), this._header = e, this.insertWidget(0, this._header))
+                }
+                get content() {
+                    return this._content
+                }
+                set content(e) {
+                    this._content && this._content.dispose(), e && (e.addClass("glue-LinkEditor-content"), this._content = e, this.addWidget(this._content))
+                }
+                onSharedModelChanged() {}
+            }
+            class X extends Y {
+                constructor(e) {
+                    super(e), this.onDatasetChange = (e, t) => {}, this.glueIdentity = () => {
+                        if (!this._identityAttributes[0] || !this._identityAttributes[1]) return;
+                        const e = {
+                                _type: F,
+                                cids1: [this._identityAttributes[0].name],
+                                cids2: [this._identityAttributes[1].name],
+                                cids1_labels: [this._identityAttributes[0].label],
+                                cids2_labels: [this._identityAttributes[1].label],
+                                data1: this._linkEditorModel.currentDatasets[0],
+                                data2: this._linkEditorModel.currentDatasets[1],
+                                inverse: Z,
+                                using: Z
+                            },
+                            t = Q.newLinkName("ComponentLink", this._sharedModel);
+                        this._sharedModel.setLink(t, e)
+                    }, this._identityAttributes = [void 0, void 0], this._reloadGlueButton = new i.Signal(this), this.addClass("glue-LinkEditor-linking"), this._datasetsPanels = [this._emptyDatasetPanel(), this._emptyDatasetPanel()], this._attributesPanels = [this._emptyAttributePanel("firstAttributePanel"), this._emptyAttributePanel("secondAttributePanel")], this.header = d.ReactWidget.create(m.createElement(Q.header, {
+                        reloadButton: this._reloadGlueButton,
+                        glueCallback: this.glueIdentity
+                    })), this.content = new o.Widget({
+                        node: this._linkingContent()
+                    }), this._sharedModel.datasetChanged.connect(this.onDatasetsChange, this), this._linkEditorModel.currentDatasetsChanged.connect(this.onDatasetChange, this), this._linkEditorModel.currentDatasets && this.onDatasetChange(this._linkEditorModel, this._linkEditorModel.currentDatasets), this.updateDatasets()
+                }
+                onDatasetsChange() {
+                    this.updateDatasets()
+                }
+                updateDatasets() {
+                    const e = this._linkEditorModel.currentDatasets;
+                    [0, 1].forEach((t => {
+                        var s;
+                        const i = Object.keys(this._sharedModel.dataset);
+                        for (; this._datasetsPanels[t].firstChild;) null === (s = this._datasetsPanels[t].lastChild) || void 0 === s || s.remove();
+                        let n;
+                        i.sort(), i.forEach((s => {
+                            const i = document.createElement("div");
+                            i.title = s, i.classList.add("glue-LinkEditor-linkingItem"), i.innerText = s, i.onclick = () => {
+                                this.onDatasetSelected(t, i)
+                            }, this._datasetsPanels[t].append(i), e[t] === s && (n = i)
+                        })), n ? this.onDatasetSelected(t, n) : this._datasetsPanels[t].childNodes[t] && this.onDatasetSelected(t, this._datasetsPanels[t].childNodes[t])
+                    }))
+                }
+                onDatasetSelected(e, t) {
+                    var s;
+                    t.classList.contains("selected") || (null === (s = t.parentNode) || void 0 === s || s.querySelectorAll(".selected").forEach((e => {
+                        e.classList.remove("selected")
+                    })), t.classList.add("selected"), this.updateAttributes(e, t.title), this._linkEditorModel.setCurrentDataset(e, t.title))
+                }
+                updateAttributes(e, t) {
+                    for (var s; this._attributesPanels[e].firstChild;) null === (s = this._attributesPanels[e].lastChild) || void 0 === s || s.remove();
+                    if (!t) return;
+                    let i = this._sharedModel.dataset[t].primary_owner;
+                    i = i.sort(), i.forEach((t => {
+                        let s;
+                        this._sharedModel.attributes[t] && (s = this._sharedModel.attributes[t].label);
+                        const i = document.createElement("div");
+                        i.title = t, i.classList.add("glue-LinkEditor-linkingItem"), i.innerText = s || t, i.onclick = () => {
+                            this.onIdentityAttributeClicked(i, e)
+                        }, this._attributesPanels[e].append(i)
+                    })), this._identityAttributes[e] = void 0, this._updateGlueButtonStatus()
+                }
+                onIdentityAttributeClicked(e, t) {
+                    var s;
+                    const i = e.classList.contains("selected");
+                    null === (s = e.parentNode) || void 0 === s || s.querySelectorAll(".selected").forEach((e => {
+                        e.classList.remove("selected")
+                    })), i ? this._identityAttributes[t] = void 0 : (e.classList.add("selected"), this._identityAttributes[t] = {
+                        name: e.title,
+                        label: e.innerText
+                    }), this._updateGlueButtonStatus()
+                }
+                _updateGlueButtonStatus() {
+                    const e = this._linkEditorModel.currentDatasets,
+                        t = this._identityAttributes.every((e => !!e)) && e[0] !== e[1];
+                    this._reloadGlueButton.emit(!t)
+                }
+                _linkingContent() {
+                    const e = document.createElement("div");
+                    return e.classList.add("glue-LinkEditor-linkingContent"), e.append(this._datasetsPanels[0]), e.append(this._attributesPanels[0]), e.append(this._attributesPanels[1]), e.append(this._datasetsPanels[1]), e
+                }
+                _emptyDatasetPanel(e) {
+                    const t = document.createElement("div");
+                    return t.classList.add("glue-LinkEditor-linkingDatasetsPanel"), t
+                }
+                _emptyAttributePanel(e) {
+                    const t = document.createElement("div");
+                    return t.classList.add("glue-LinkEditor-linkingAttributesPanel"), e && t.classList.add(e), t
+                }
+            }
+            var Q, ee;
+            ! function(e) {
+                e.header = function(e) {
+                    return m.createElement("div", {
+                        className: "glue-LinkEditor-linkingHeader"
+                    }, m.createElement("div", {
+                        className: "glue-LinkEditor-linkingHeaderDatasets"
+                    }, m.createElement("div", {
+                        style: {
+                            fontWeight: "bold",
+                            fontSize: "var(--jp-ui-font-size1)"
+                        }
+                    }, "Dataset 1"), m.createElement("div", null, "Select a first dataset")), m.createElement("div", {
+                        className: "glue-LinkEditor-linkingHeaderAttributes"
+                    }, m.createElement("div", null, m.createElement("div", {
+                        style: {
+                            fontWeight: "bold"
+                        }
+                    }, "Attributes"), m.createElement("div", null, "Select an attribute from each column")), m.createElement(d.UseSignal, {
+                        signal: e.reloadButton
+                    }, ((t, s) => m.createElement(d.Button, {
+                        onClick: e.glueCallback,
+                        disabled: null == s || s,
+                        className: "glue-LinkEditor-linkingGlueButton"
+                    }, "GLUE")))), m.createElement("div", {
+                        className: "glue-LinkEditor-linkingHeaderDatasets"
+                    }, m.createElement("div", {
+                        style: {
+                            fontWeight: "bold"
+                        }
+                    }, "Dataset 2"), m.createElement("div", null, "Select a second dataset")))
+                }, e.newLinkName = function(e, t) {
+                    let s;
+                    const i = RegExp(`^${e}(?:_([0-9]+))?$`);
+                    return Object.keys(t.links).forEach((e => {
+                        const t = i.exec(e);
+                        t && (t[1] ? s = Math.max(s || -1, parseInt(t[1])) : void 0 === s && (s = -1))
+                    })), `${e}${void 0!==s?`_${s+1}`:""}`
+                }
+            }(Q || (Q = {}));
+            class te extends Y {
+                constructor(e) {
+                    super(e), this.onDeleteLink = e => {
+                        this._sharedModel.removeLink(e)
+                    }, this.addClass("glue-LinkEditor-summary");
+                    const t = ee.createLayout({});
+                    this._links = new o.AccordionPanel({
+                        layout: t
+                    }), this._links.addClass("glue-LinkEditor-identity"), this.header = d.ReactWidget.create(m.createElement(ee.header, null)), this.content = this._links, this._linkEditorModel.currentDatasetsChanged.connect(this.onDatasetsChange, this), this._linkEditorModel.linksChanged.connect(this.linksChanged, this), this._linkEditorModel.currentDatasets && this.updateLinks()
+                }
+                linksChanged() {
+                    this.updateLinks()
+                }
+                onDatasetsChange() {
+                    this.updateLinks()
+                }
+                updateLinks() {
+                    const e = new Map;
+                    for (; this._links.widgets.length;) this._links.widgets[0].dispose();
+                    this._linkEditorModel.identityLinks.forEach(((t, s) => {
+                        var i;
+                        const n = [t.data1, t.data2].sort(),
+                            a = JSON.stringify(n),
+                            d = {
+                                type: "identity",
+                                name: s,
+                                value: t,
+                                revert: t.data2 === n[0]
+                            };
+                        e.get(a) ? null === (i = e.get(a)) || void 0 === i || i.push(d) : e.set(a, [d])
+                    })), e.forEach(((e, t) => {
+                        const s = d.ReactWidget.create(ee.datasetLinks(e, this.onDeleteLink));
+                        s.title.dataset = {
+                            datasets: t,
+                            count: e.length.toString()
+                        }, this._links.addWidget(s)
+                    }))
+                }
+            }! function(e) {
+                class t extends o.AccordionPanel.Renderer {
+                    createCollapseIcon(e) {
+                        const t = document.createElement("div");
+                        return t.classList.add("glue-LinkEditor-accordionCollapser"), d.caretRightIcon.element({
+                            container: t
+                        }), t
+                    }
+                    createSectionTitle(e) {
+                        const t = JSON.parse(e.dataset.datasets),
+                            s = document.createElement("div");
+                        s.classList.add("glue-LinkEditor-accordionTitle"), t.forEach((e => {
+                            const t = document.createElement("div");
+                            t.innerText = e, s.append(t)
+                        }));
+                        const i = document.createElement("div");
+                        return i.innerHTML = e.dataset.count, s.append(i), s.append(this.createCollapseIcon(e)), s
+                    }
+                }
+                e.Renderer = t, e.defaultRenderer = new t, e.createLayout = function(t) {
+                    var s;
+                    return t.layout || new o.AccordionLayout({
+                        renderer: t.renderer || e.defaultRenderer,
+                        orientation: t.orientation,
+                        alignment: t.alignment,
+                        spacing: t.spacing,
+                        titleSpace: null !== (s = t.titleSpace) && void 0 !== s ? s : 29
+                    })
+                }, e.header = function() {
+                    return m.createElement("div", {
+                        className: "glue-LinkEditor-summaryHeader"
+                    }, m.createElement("div", {
+                        style: {
+                            width: "80%"
+                        }
+                    }, "Linked datasets"), m.createElement("div", null, "#"))
+                }, e.datasetLinks = function(e, t) {
+                    const s = e.filter((e => "identity" === e.type));
+                    return m.createElement("div", null, s.map((e => m.createElement("div", {
+                        key: e.name,
+                        className: "glue-LinkEditor-summaryIdentity"
+                    }, m.createElement("div", null, e.revert ? e.value.cids2_labels[0] : e.value.cids1_labels[0]), m.createElement("div", null, e.revert ? e.value.cids1_labels[0] : e.value.cids2_labels[0]), m.createElement("div", null, m.createElement(d.Button, {
+                        className: "glue-LinkEditor-deleteButton",
+                        onClick: () => t(e.name),
+                        minimal: !0
+                    }, m.createElement(d.LabIcon.resolveReact, {
+                        icon: d.deleteIcon,
+                        height: "24px",
+                        width: "24px"
+                    })))))))
+                }
+            }(ee || (ee = {}));
+            class se extends o.SplitPanel {
+                constructor(e) {
+                    super({}), this._sharedModel = e.sharedModel, this.addClass("glue-linkEditor"), this.title.label = "Link Data", this.title.className = "glue-LinkEditor-tab";
+                    const t = new K({
+                            sharedModel: this._sharedModel
+                        }),
+                        s = new X({
+                            linkEditorModel: t,
+                            sharedModel: this._sharedModel
+                        }),
+                        i = new te({
+                            linkEditorModel: t,
+                            sharedModel: this._sharedModel
+                        });
+                    this.addWidget(s), this.addWidget(i), o.SplitPanel.setStretch(s, 3), o.SplitPanel.setStretch(i, 2)
+                }
+                get sharedModel() {
+                    return this._sharedModel
+                }
+                onAfterShow(e) {
+                    this._computeHeaderHeight()
+                }
+                onResize(e) {
+                    this._computeHeaderHeight()
+                }
+                _computeHeaderHeight() {
+                    let e = 0;
+                    const t = this.widgets.map((e => e.header));
+                    e = Math.max(...t.map((e => {
+                        var t;
+                        return (null === (t = null == e ? void 0 : e.node.firstChild) || void 0 === t ? void 0 : t.offsetHeight) || 0
+                    }))), t.forEach((t => {
+                        t && (t.node.style.minHeight = `${e}px`)
+                    }))
+                }
+            }
+            var ie, ne = s(7120),
+                ae = s(5633),
+                de = s(4784);
+            class oe extends o.Layout {
                 constructor(e) {
                     super(), this._onResizeStops = () => {
                         this._gridItems.forEach((e => {
-                            V.MessageLoop.sendMessage(e, o.Widget.Msg.UpdateRequest)
+                            ae.MessageLoop.sendMessage(e, o.Widget.Msg.UpdateRequest)
                         }))
-                    }, this._gridItemChanged = new i.Signal(this), this._resizeTimeout = 0, this._commands = e, this._gridItems = new Map, this._gridHost = document.createElement("div"), this._gridHost.className = "grid-stack", this._gridHost.classList.add("glue-Session-gridhost"), this._grid = $.GridStack.init({
+                    }, this._gridItemChanged = new i.Signal(this), this._resizeTimeout = 0, this._commands = e, this._gridItems = new Map, this._gridHost = document.createElement("div"), this._gridHost.className = "grid-stack", this._gridHost.classList.add("glue-Session-gridhost"), this._grid = de.GridStack.init({
                         float: !0,
                         column: 12,
                         margin: 3,
                         cellHeight: 40,
                         styleInHead: !0,
                         disableOneColumnMode: !0,
                         draggable: {
@@ -927,25 +1286,25 @@
                     this._grid.destroy(), super.dispose()
                 }
                 init() {
                     super.init(), this.parent && this.parent.node.appendChild(this._gridHost), window.dispatchEvent(new Event("resize"))
                 }
                 removeWidget(e) {}
                 addGridItem(e) {
-                    const t = J.pixelToGrid(this._grid.cellWidth(), {
+                    const t = ie.pixelToGrid(this._grid.cellWidth(), {
                         id: e.cellIdentity,
                         size: e.size,
                         pos: e.pos
                     });
                     e.changed.connect(this._onItemChanged, this), this._gridItems.set(e.cellIdentity, e), e.node.addEventListener("click", (() => {
                         this._handleEdit(e)
-                    })), V.MessageLoop.sendMessage(e, o.Widget.Msg.BeforeAttach), this._grid.addWidget(e.node, t), V.MessageLoop.sendMessage(e, o.Widget.Msg.AfterAttach)
+                    })), ae.MessageLoop.sendMessage(e, o.Widget.Msg.BeforeAttach), this._grid.addWidget(e.node, t), ae.MessageLoop.sendMessage(e, o.Widget.Msg.AfterAttach)
                 }
                 updateGridItem(e, t) {
-                    const s = J.pixelToGrid(this._grid.cellWidth(), {
+                    const s = ie.pixelToGrid(this._grid.cellWidth(), {
                             id: t.id,
                             size: t.size,
                             pos: t.pos
                         }),
                         i = this._gridItems.get(e);
                     if (!i) return;
                     i.size = t.size, i.pos = t.pos;
@@ -996,16 +1355,23 @@
                 }
                 _handleEdit(e) {
                     this.unselectGridItems(), e.node.classList.add("grid-selected"), this._commands.execute(b.openControlPanel, {
                         cellId: e.cellIdentity,
                         gridItem: e
                     })
                 }
+                _addViewerLayer(e, t) {
+                    this._commands.execute(b.addViewerLayer, {
+                        tab: e.tabName,
+                        viewer: e.cellIdentity,
+                        data: t
+                    })
+                }
                 _onChange(e, t) {
-                    const s = t.map((e => J.gridToPixel(this._grid.cellWidth(), e)));
+                    const s = t.map((e => ie.gridToPixel(this._grid.cellWidth(), e)));
                     this._gridItemChanged.emit({
                         action: "move",
                         items: s
                     })
                 }
                 _onRemoved(e, t) {
                     const s = t.map((e => e.id));
@@ -1013,28 +1379,32 @@
                         action: "remove",
                         items: s
                     })
                 }
                 _onResize(e, t) {
                     const s = this._gridItems.get(t.id);
                     if (!s) return;
-                    V.MessageLoop.sendMessage(s, o.Widget.Msg.UpdateRequest);
-                    const i = J.gridToPixel(this._grid.cellWidth(), t);
+                    ae.MessageLoop.sendMessage(s, o.Widget.Msg.UpdateRequest);
+                    const i = ie.gridToPixel(this._grid.cellWidth(), t);
                     this._gridItemChanged.emit({
                         action: "move",
                         items: [i]
                     })
                 }
                 _onItemChanged(e, t) {
                     switch (t.action) {
                         case "close":
                             e.changed.disconnect(this._onItemChanged, this), this.removeGridItem(e.cellIdentity);
                             break;
                         case "edit":
-                            this._handleEdit(e)
+                            this._handleEdit(e);
+                            break;
+                        case "layer":
+                            if (!t.dataLayer) return;
+                            this._addViewerLayer(e, t.dataLayer)
                     }
                 }
                 _prepareGrid() {
                     const e = this.parent.node.getBoundingClientRect();
                     this._gridHost.style.minHeight = `${e.height}px`, this._grid.onParentResize()
                 }
             }! function(e) {
@@ -1050,32 +1420,33 @@
                 }, e.gridToPixel = function(e, t) {
                     return {
                         id: t.id,
                         size: [Math.ceil(t.w * e), Math.ceil(40 * t.h)],
                         pos: [Math.ceil(t.x * e), Math.ceil(40 * t.y)]
                     }
                 }
-            }(J || (J = {}));
-            class K extends o.Panel {
+            }(ie || (ie = {}));
+            class re extends o.Panel {
                 constructor(e) {
                     super(), this.removeClass("lm-Widget"), this.removeClass("p-Widget"), this.addClass("grid-stack-item"), this.addClass("glue-item");
                     const {
                         cellIdentity: t,
                         cell: s,
                         itemTitle: n = "",
                         pos: a,
-                        size: d
+                        size: d,
+                        tabName: r
                     } = e;
-                    this._cellOutput = s, this.cellIdentity = t, this._pos = a, this._size = d, this._title = n;
-                    const r = new o.Panel;
-                    r.addClass("grid-stack-item-content");
-                    const l = this._createToolbar(n);
-                    r.addWidget(l), s.addClass("grid-item-widget"), r.addWidget(s), this._spinner = document.createElement("div"), this._spinner.classList.add("glue-Spinner");
-                    const h = document.createElement("div");
-                    h.classList.add("glue-SpinnerContent"), this._spinner.appendChild(h), s.node.appendChild(this._spinner), this.addWidget(r), this._changed = new i.Signal(this)
+                    this._cellOutput = s, this.cellIdentity = t, this._pos = a, this._size = d, this._title = n, this._tabName = r;
+                    const l = new o.Panel;
+                    l.addClass("grid-stack-item-content");
+                    const h = this._createToolbar(n);
+                    l.addWidget(h), s.addClass("grid-item-widget"), l.addWidget(s), this._spinner = document.createElement("div"), this._spinner.classList.add("glue-Spinner");
+                    const c = document.createElement("div");
+                    c.classList.add("glue-SpinnerContent"), this._spinner.appendChild(c), s.node.appendChild(this._spinner), this.addWidget(l), this._changed = new i.Signal(this)
                 }
                 get cellOutput() {
                     return this._cellOutput
                 }
                 get itemTitle() {
                     return this._title
                 }
@@ -1087,17 +1458,37 @@
                 }
                 get size() {
                     return this._size
                 }
                 set size(e) {
                     this._size = e
                 }
+                get tabName() {
+                    return this._tabName
+                }
+                set tabName(e) {
+                    this._tabName = e
+                }
                 get changed() {
                     return this._changed
                 }
+                onAfterAttach(e) {
+                    super.onAfterAttach(e), this.node.addEventListener("drop", this._ondrop.bind(this))
+                }
+                onBeforeDetach(e) {
+                    this.node.removeEventListener("drop", this._ondrop.bind(this)), super.onBeforeDetach(e)
+                }
+                async _ondrop(e) {
+                    var t;
+                    const s = null === (t = e.dataTransfer) || void 0 === t ? void 0 : t.getData(p);
+                    s && this._changed.emit({
+                        action: "layer",
+                        dataLayer: s
+                    })
+                }
                 _createToolbar(e) {
                     const t = new d.Toolbar;
                     t.node.addEventListener("click", (() => {
                         this._changed.emit({
                             action: "edit"
                         })
                     })), t.addClass("glue-Session-tab-toolbar"), t.addItem("Close", new d.ToolbarButton({
@@ -1107,33 +1498,36 @@
                             action: "close"
                         })
                     }));
                     const s = new o.Widget;
                     return s.node.innerText = e, s.node.style.flexGrow = "1", s.node.style.justifyContent = "center", t.addItem("Title", s), t
                 }
             }
-            class Y extends o.Widget {
+            class le extends o.Widget {
                 constructor(e) {
                     super(), this._selectedItem = null, this.addClass("grid-editor");
                     const {
                         model: t,
                         tabName: s,
                         context: i,
                         rendermime: n,
                         commands: a
                     } = e;
                     this._model = t, this._tabName = this.title.label = s, this._context = i, this._rendermime = n;
-                    const d = this.layout = new Z(a);
-                    this._localCommands = new F.CommandRegistry, this._contextMenu = new o.ContextMenu({
+                    const d = this.layout = new oe(a);
+                    this._localCommands = new ne.CommandRegistry, this._contextMenu = new o.ContextMenu({
                         commands: this._localCommands
                     }), this._addCommands(), this._context.sessionContext.ready.then((() => this._initGrid())), d.gridItemChanged.connect(this._onLayoutChanged, this), this._model.tabChanged.connect(this._onTabChanged, this), this._model.localStateChanged.connect(this._onLocalStateChanged, this)
                 }
                 dispose() {
                     this.disposed || (this.layout.gridItemChanged.disconnect(this._onLayoutChanged, this), this._model.tabChanged.disconnect(this._onTabChanged, this), this._model.localStateChanged.disconnect(this._onLocalStateChanged), super.dispose())
                 }
+                onCloseRequest(e) {
+                    this.dispose()
+                }
                 get tabName() {
                     return this._tabName
                 }
                 get tabData() {
                     var e;
                     return null !== (e = this._model.getTabData(this._tabName)) && void 0 !== e ? e : {}
                 }
@@ -1163,20 +1557,21 @@
                         const i = new c.OutputAreaModel({
                                 trusted: !0
                             }),
                             d = new c.SimplifiedOutputArea({
                                 model: i,
                                 rendermime: this._rendermime
                             }),
-                            o = new K({
+                            o = new re({
                                 cellIdentity: t,
                                 cell: d,
                                 itemTitle: null === (n = a.match(/($[a-z])|[A-Z][^A-Z]+/g)) || void 0 === n ? void 0 : n.join(" "),
                                 pos: s.pos,
-                                size: s.size
+                                size: s.size,
+                                tabName: e
                             }),
                             r = o.cellOutput;
                         return this._context && c.SimplifiedOutputArea.execute(`\n          GLUE_SESSION.create_viewer("${e}", "${t}")\n          `, r, this._context.sessionContext), o
                     }
                 }
                 _addCommands() {
                     this._localCommands.addCommand("moveItem", {
@@ -1270,373 +1665,37 @@
                             }))
                     }
                 }
                 _onLocalStateChanged(e, t) {
                     t.keys.includes("selectedTab") && this.layout.unselectGridItems()
                 }
             }
-            var X = s(9993),
-                Q = s(4238);
-            const ee = "glue.core.component_link.ComponentLink",
-                te = "glue.core.link_helpers.identity",
-                se = {
-                    _type: "types.FunctionType",
-                    function: te
-                };
-            class ie {
-                constructor(e) {
-                    this._currentDatasets = ["", ""], this._datasetsChanged = new i.Signal(this), this._advLinksPromise = new D.PromiseDelegate, this._advLinkCategories = {}, this._identityLinks = new Map, this._advancedLinks = new Map, this._linksChanged = new i.Signal(this), this._sharedModel = e.sharedModel, this._sharedModel.linksChanged.connect(this.onLinksChanged, this), this._sharedModel.datasetChanged.connect(this.onDatasetsChanged, this), this._getAdvancedLinksCategories()
-                }
-                get sharedModel() {
-                    return this._sharedModel
-                }
-                get currentDatasets() {
-                    return this._currentDatasets
-                }
-                set currentDatasets(e) {
-                    this._currentDatasets = e, this._datasetsChanged.emit(this._currentDatasets)
-                }
-                setCurrentDataset(e, t) {
-                    this._currentDatasets[e] = t, this._datasetsChanged.emit(this._currentDatasets)
-                }
-                get currentDatasetsChanged() {
-                    return this._datasetsChanged
-                }
-                get identityLinks() {
-                    return this._identityLinks
-                }
-                get advLinkCategories() {
-                    return this._advLinkCategories
-                }
-                get advancedLinks() {
-                    return this._advancedLinks
-                }
-                get linksChanged() {
-                    return this._linksChanged
-                }
-                get advLinksPromise() {
-                    return this._advLinksPromise.promise
-                }
-                async _getAdvancedLinksCategories() {
-                    const e = Q.ServerConnection.makeSettings(),
-                        t = X.URLExt.join(e.baseUrl, "/glue-jupyterlab/advanced-links");
-                    let s;
-                    try {
-                        s = await Q.ServerConnection.makeRequest(t, {}, e)
-                    } catch (e) {
-                        throw new Q.ServerConnection.NetworkError(e)
-                    }
-                    const i = await s.json();
-                    if (!s.ok) throw this._advLinksPromise.reject(i.message), new Q.ServerConnection.ResponseError(s, i.message);
-                    Object.entries(i.data).forEach((([e, t]) => {
-                        this._advLinkCategories[e] = t
-                    })), this._advLinksPromise.resolve(this._advLinkCategories)
-                }
-                onDatasetsChanged() {
-                    if (this._sharedModel.dataset) {
-                        const e = Object.keys(this._sharedModel.dataset);
-                        this._currentDatasets = [e.length > 1 ? e[0] : "", e.length > 1 ? e[1] : ""], this._datasetsChanged.emit(this._currentDatasets)
-                    }
-                }
-                onLinksChanged() {
-                    var e;
-                    this._identityLinks = new Map, this._advancedLinks = new Map, Object.entries(null === (e = this._sharedModel) || void 0 === e ? void 0 : e.links).forEach((([e, t], s) => {
-                        var i;
-                        t._type === ee && (null === (i = t.using) || void 0 === i ? void 0 : i.function) === te ? this._identityLinks.set(e, t) : this._advancedLinks.set(e, t)
-                    })), this._linksChanged.emit()
-                }
-            }
-            class ne extends o.Panel {
-                constructor(e) {
-                    super(), this._header = void 0, this._content = void 0, this._linkEditorModel = e.linkEditorModel, this._sharedModel = e.sharedModel, this.addClass("glue-LinkEditor-widget"), this._sharedModel.changed.connect(this.onSharedModelChanged, this)
-                }
-                get header() {
-                    return this._header
-                }
-                set header(e) {
-                    this._header && this._header.dispose(), e && (e.addClass("glue-LinkEditor-header"), this._header = e, this.insertWidget(0, this._header))
-                }
-                get content() {
-                    return this._content
-                }
-                set content(e) {
-                    this._content && this._content.dispose(), e && (e.addClass("glue-LinkEditor-content"), this._content = e, this.addWidget(this._content))
-                }
-                onSharedModelChanged() {}
-            }
-            class ae extends ne {
-                constructor(e) {
-                    super(e), this.onDatasetChange = (e, t) => {}, this.glueIdentity = () => {
-                        if (!this._identityAttributes[0] || !this._identityAttributes[1]) return;
-                        const e = {
-                                _type: ee,
-                                cids1: [this._identityAttributes[0].name],
-                                cids2: [this._identityAttributes[1].name],
-                                cids1_labels: [this._identityAttributes[0].label],
-                                cids2_labels: [this._identityAttributes[1].label],
-                                data1: this._linkEditorModel.currentDatasets[0],
-                                data2: this._linkEditorModel.currentDatasets[1],
-                                inverse: se,
-                                using: se
-                            },
-                            t = de.newLinkName("ComponentLink", this._sharedModel);
-                        this._sharedModel.setLink(t, e)
-                    }, this._identityAttributes = [void 0, void 0], this._reloadGlueButton = new i.Signal(this), this.addClass("glue-LinkEditor-linking"), this._datasetsPanels = [this._emptyDatasetPanel(), this._emptyDatasetPanel()], this._attributesPanels = [this._emptyAttributePanel("firstAttributePanel"), this._emptyAttributePanel("secondAttributePanel")], this.header = d.ReactWidget.create(m.createElement(de.header, {
-                        reloadButton: this._reloadGlueButton,
-                        glueCallback: this.glueIdentity
-                    })), this.content = new o.Widget({
-                        node: this._linkingContent()
-                    }), this._sharedModel.datasetChanged.connect(this.onDatasetsChange, this), this._linkEditorModel.currentDatasetsChanged.connect(this.onDatasetChange, this), this._linkEditorModel.currentDatasets && this.onDatasetChange(this._linkEditorModel, this._linkEditorModel.currentDatasets), this.updateDatasets()
-                }
-                onDatasetsChange() {
-                    this.updateDatasets()
-                }
-                updateDatasets() {
-                    const e = this._linkEditorModel.currentDatasets;
-                    [0, 1].forEach((t => {
-                        var s;
-                        const i = Object.keys(this._sharedModel.dataset);
-                        for (; this._datasetsPanels[t].firstChild;) null === (s = this._datasetsPanels[t].lastChild) || void 0 === s || s.remove();
-                        let n;
-                        i.sort(), i.forEach((s => {
-                            const i = document.createElement("div");
-                            i.title = s, i.classList.add("glue-LinkEditor-linkingItem"), i.innerText = s, i.onclick = () => {
-                                this.onDatasetSelected(t, i)
-                            }, this._datasetsPanels[t].append(i), e[t] === s && (n = i)
-                        })), n ? this.onDatasetSelected(t, n) : this._datasetsPanels[t].childNodes[t] && this.onDatasetSelected(t, this._datasetsPanels[t].childNodes[t])
-                    }))
-                }
-                onDatasetSelected(e, t) {
-                    var s;
-                    t.classList.contains("selected") || (null === (s = t.parentNode) || void 0 === s || s.querySelectorAll(".selected").forEach((e => {
-                        e.classList.remove("selected")
-                    })), t.classList.add("selected"), this.updateAttributes(e, t.title), this._linkEditorModel.setCurrentDataset(e, t.title))
-                }
-                updateAttributes(e, t) {
-                    for (var s; this._attributesPanels[e].firstChild;) null === (s = this._attributesPanels[e].lastChild) || void 0 === s || s.remove();
-                    if (!t) return;
-                    let i = this._sharedModel.dataset[t].primary_owner;
-                    i = i.sort(), i.forEach((t => {
-                        let s;
-                        this._sharedModel.attributes[t] && (s = this._sharedModel.attributes[t].label);
-                        const i = document.createElement("div");
-                        i.title = t, i.classList.add("glue-LinkEditor-linkingItem"), i.innerText = s || t, i.onclick = () => {
-                            this.onIdentityAttributeClicked(i, e)
-                        }, this._attributesPanels[e].append(i)
-                    })), this._identityAttributes[e] = void 0, this._updateGlueButtonStatus()
-                }
-                onIdentityAttributeClicked(e, t) {
-                    var s;
-                    const i = e.classList.contains("selected");
-                    null === (s = e.parentNode) || void 0 === s || s.querySelectorAll(".selected").forEach((e => {
-                        e.classList.remove("selected")
-                    })), i ? this._identityAttributes[t] = void 0 : (e.classList.add("selected"), this._identityAttributes[t] = {
-                        name: e.title,
-                        label: e.innerText
-                    }), this._updateGlueButtonStatus()
-                }
-                _updateGlueButtonStatus() {
-                    const e = this._linkEditorModel.currentDatasets,
-                        t = this._identityAttributes.every((e => !!e)) && e[0] !== e[1];
-                    this._reloadGlueButton.emit(!t)
-                }
-                _linkingContent() {
-                    const e = document.createElement("div");
-                    return e.classList.add("glue-LinkEditor-linkingContent"), e.append(this._datasetsPanels[0]), e.append(this._attributesPanels[0]), e.append(this._attributesPanels[1]), e.append(this._datasetsPanels[1]), e
-                }
-                _emptyDatasetPanel(e) {
-                    const t = document.createElement("div");
-                    return t.classList.add("glue-LinkEditor-linkingDatasetsPanel"), t
-                }
-                _emptyAttributePanel(e) {
-                    const t = document.createElement("div");
-                    return t.classList.add("glue-LinkEditor-linkingAttributesPanel"), e && t.classList.add(e), t
-                }
-            }
-            var de, oe;
-            ! function(e) {
-                e.header = function(e) {
-                    return m.createElement("div", {
-                        className: "glue-LinkEditor-linkingHeader"
-                    }, m.createElement("div", {
-                        className: "glue-LinkEditor-linkingHeaderDatasets"
-                    }, m.createElement("div", {
-                        style: {
-                            fontWeight: "bold",
-                            fontSize: "var(--jp-ui-font-size1)"
-                        }
-                    }, "Dataset 1"), m.createElement("div", null, "Select a first dataset")), m.createElement("div", {
-                        className: "glue-LinkEditor-linkingHeaderAttributes"
-                    }, m.createElement("div", null, m.createElement("div", {
-                        style: {
-                            fontWeight: "bold"
-                        }
-                    }, "Attributes"), m.createElement("div", null, "Select an attribute from each column")), m.createElement(d.UseSignal, {
-                        signal: e.reloadButton
-                    }, ((t, s) => m.createElement(d.Button, {
-                        onClick: e.glueCallback,
-                        disabled: null == s || s,
-                        className: "glue-LinkEditor-linkingGlueButton"
-                    }, "GLUE")))), m.createElement("div", {
-                        className: "glue-LinkEditor-linkingHeaderDatasets"
-                    }, m.createElement("div", {
-                        style: {
-                            fontWeight: "bold"
-                        }
-                    }, "Dataset 2"), m.createElement("div", null, "Select a second dataset")))
-                }, e.newLinkName = function(e, t) {
-                    let s;
-                    const i = RegExp(`^${e}(?:_([0-9]+))?$`);
-                    return Object.keys(t.links).forEach((e => {
-                        const t = i.exec(e);
-                        t && (t[1] ? s = Math.max(s || -1, parseInt(t[1])) : void 0 === s && (s = -1))
-                    })), `${e}${void 0!==s?`_${s+1}`:""}`
-                }
-            }(de || (de = {}));
-            class re extends ne {
-                constructor(e) {
-                    super(e), this.onDeleteLink = e => {
-                        this._sharedModel.removeLink(e)
-                    }, this.addClass("glue-LinkEditor-summary");
-                    const t = oe.createLayout({});
-                    this._links = new o.AccordionPanel({
-                        layout: t
-                    }), this._links.addClass("glue-LinkEditor-identity"), this.header = d.ReactWidget.create(m.createElement(oe.header, null)), this.content = this._links, this._linkEditorModel.currentDatasetsChanged.connect(this.onDatasetsChange, this), this._linkEditorModel.linksChanged.connect(this.linksChanged, this), this._linkEditorModel.currentDatasets && this.updateLinks()
-                }
-                linksChanged() {
-                    this.updateLinks()
-                }
-                onDatasetsChange() {
-                    this.updateLinks()
-                }
-                updateLinks() {
-                    const e = new Map;
-                    for (; this._links.widgets.length;) this._links.widgets[0].dispose();
-                    this._linkEditorModel.identityLinks.forEach(((t, s) => {
-                        var i;
-                        const n = [t.data1, t.data2].sort(),
-                            a = JSON.stringify(n),
-                            d = {
-                                type: "identity",
-                                name: s,
-                                value: t,
-                                revert: t.data2 === n[0]
-                            };
-                        e.get(a) ? null === (i = e.get(a)) || void 0 === i || i.push(d) : e.set(a, [d])
-                    })), e.forEach(((e, t) => {
-                        const s = d.ReactWidget.create(oe.datasetLinks(e, this.onDeleteLink));
-                        s.title.dataset = {
-                            datasets: t,
-                            count: e.length.toString()
-                        }, this._links.addWidget(s)
-                    }))
-                }
-            }! function(e) {
-                class t extends o.AccordionPanel.Renderer {
-                    createCollapseIcon(e) {
-                        const t = document.createElement("div");
-                        return t.classList.add("glue-LinkEditor-accordionCollapser"), d.caretRightIcon.element({
-                            container: t
-                        }), t
-                    }
-                    createSectionTitle(e) {
-                        const t = JSON.parse(e.dataset.datasets),
-                            s = document.createElement("div");
-                        s.classList.add("glue-LinkEditor-accordionTitle"), t.forEach((e => {
-                            const t = document.createElement("div");
-                            t.innerText = e, s.append(t)
-                        }));
-                        const i = document.createElement("div");
-                        return i.innerHTML = e.dataset.count, s.append(i), s.append(this.createCollapseIcon(e)), s
-                    }
-                }
-                e.Renderer = t, e.defaultRenderer = new t, e.createLayout = function(t) {
-                    var s;
-                    return t.layout || new o.AccordionLayout({
-                        renderer: t.renderer || e.defaultRenderer,
-                        orientation: t.orientation,
-                        alignment: t.alignment,
-                        spacing: t.spacing,
-                        titleSpace: null !== (s = t.titleSpace) && void 0 !== s ? s : 29
-                    })
-                }, e.header = function() {
-                    return m.createElement("div", {
-                        className: "glue-LinkEditor-summaryHeader"
-                    }, m.createElement("div", {
-                        style: {
-                            width: "80%"
-                        }
-                    }, "Linked datasets"), m.createElement("div", null, "#"))
-                }, e.datasetLinks = function(e, t) {
-                    const s = e.filter((e => "identity" === e.type));
-                    return m.createElement("div", null, s.map((e => m.createElement("div", {
-                        key: e.name,
-                        className: "glue-LinkEditor-summaryIdentity"
-                    }, m.createElement("div", null, e.revert ? e.value.cids2_labels[0] : e.value.cids1_labels[0]), m.createElement("div", null, e.revert ? e.value.cids1_labels[0] : e.value.cids2_labels[0]), m.createElement("div", null, m.createElement(d.Button, {
-                        className: "glue-LinkEditor-deleteButton",
-                        onClick: () => t(e.name),
-                        minimal: !0
-                    }, m.createElement(d.LabIcon.resolveReact, {
-                        icon: d.deleteIcon,
-                        height: "24px",
-                        width: "24px"
-                    })))))))
-                }
-            }(oe || (oe = {}));
-            class le extends o.SplitPanel {
-                constructor(e) {
-                    super({}), this._sharedModel = e.sharedModel, this.addClass("glue-linkEditor"), this.title.label = "Link Data", this.title.className = "glue-LinkEditor-tab";
-                    const t = new ie({
-                            sharedModel: this._sharedModel
-                        }),
-                        s = new ae({
-                            linkEditorModel: t,
-                            sharedModel: this._sharedModel
-                        }),
-                        i = new re({
-                            linkEditorModel: t,
-                            sharedModel: this._sharedModel
-                        });
-                    this.addWidget(s), this.addWidget(i), o.SplitPanel.setStretch(s, 3), o.SplitPanel.setStretch(i, 2)
-                }
-                get sharedModel() {
-                    return this._sharedModel
-                }
-                onAfterShow(e) {
-                    this._computeHeaderHeight()
-                }
-                onResize(e) {
-                    this._computeHeaderHeight()
-                }
-                _computeHeaderHeight() {
-                    let e = 0;
-                    const t = this.widgets.map((e => e.header));
-                    e = Math.max(...t.map((e => {
-                        var t;
-                        return (null === (t = null == e ? void 0 : e.node.firstChild) || void 0 === t ? void 0 : t.offsetHeight) || 0
-                    }))), t.forEach((t => {
-                        t && (t.node.style.minHeight = `${e}px`)
-                    }))
-                }
-            }
             class he extends o.BoxPanel {
                 constructor(e) {
                     super({
                         direction: "top-to-bottom"
                     }), this._tabViews = {}, this._pythonSessionCreated = new D.PromiseDelegate, this._linkWidget = void 0, this.addClass("grid-panel"), this.addClass("glue-Session-panel"), this._spinner = document.createElement("div"), this._spinner.classList.add("glue-Spinner");
                     const t = document.createElement("div");
                     t.classList.add("glue-SpinnerContent"), this._spinner.appendChild(t), this.node.appendChild(this._spinner), this._model = e.model, this._rendermime = e.rendermime.clone(), this._notebookTracker = e.notebookTracker, this._context = e.context, this._commands = e.commands, this._yWidgetManager = e.yWidgetManager, this._tabPanel = new l({
                         tabBarPosition: "bottom",
                         tabBarClassList: ["glue-Session-tabBar"],
                         tabBarOption: {
                             addButtonEnabled: !0
                         }
                     }), this._tabPanel.topBar.addRequested.connect((() => {
                         this._model.addTab()
-                    })), this._model && (this._linkWidget = new le({
+                    })), this._tabPanel.topBar.tabCloseRequested.connect((async (e, t) => {
+                        (await (0, W.showDialog)({
+                            title: "Delete Tab",
+                            body: "Are you sure you want to delete this tab?",
+                            buttons: [W.Dialog.cancelButton(), W.Dialog.okButton({
+                                label: "Delete"
+                            })]
+                        })).button.accept && (t.title.owner.close(), this._tabPanel.topBar.removeTabAt(t.index), this._model.removeTab(t.title.label))
+                    })), this._model && (this._linkWidget = new se({
                         sharedModel: this._model
                     }), this._tabPanel.addTab(this._linkWidget, 0)), this.addWidget(this._tabPanel), o.BoxPanel.setStretch(this._tabPanel, 1), this._model.tabsChanged.connect(this._onTabsChanged, this), this._tabPanel.topBar.currentChanged.connect(this._onFocusedTabChanged, this), this._kernel = void 0, this._startKernel()
                 }
                 get rendermime() {
                     return this._rendermime
                 }
                 get kernel() {
@@ -1649,14 +1708,15 @@
                     this.node.removeEventListener("dragover", this._ondragover.bind(this)), this.node.removeEventListener("drop", this._ondrop.bind(this)), super.onBeforeDetach(e)
                 }
                 _ondragover(e) {
                     e.preventDefault()
                 }
                 async _ondrop(e) {
                     var t;
+                    if (e.target.closest(".grid-stack-item.glue-item")) return;
                     const s = null === (t = e.dataTransfer) || void 0 === t ? void 0 : t.getData(p),
                         i = {
                             Histogram: b.new1DHistogram,
                             "1D Profile": b.new1DProfile,
                             "2D Scatter": b.new2DScatter,
                             "3D Scatter": b.new3DScatter,
                             "2D Image": b.new2DImage,
@@ -1705,27 +1765,30 @@
                             code: o
                         }, !1);
                     await r.done, this._pythonSessionCreated.resolve(), this._spinner.style.display = "none"
                 }
                 async _onTabsChanged() {
                     let e;
                     await this._pythonSessionCreated.promise;
-                    const t = this._tabPanel.topBar.currentIndex;
-                    this._model.getTabNames().forEach(((t, s) => {
+                    const t = this._tabPanel.topBar.currentIndex,
+                        s = this._model.getTabNames();
+                    Object.keys(this._tabViews).forEach((e => {
+                        s.includes(e) || (this._tabViews[e].dispose(), delete this._tabViews[e])
+                    })), s.forEach(((t, s) => {
                         if (t in this._tabViews) return;
                         e = s;
-                        const i = this._tabViews[t] = new Y({
+                        const i = this._tabViews[t] = new le({
                             tabName: t,
                             model: this._model,
                             rendermime: this._rendermime,
                             context: this._context,
                             notebookTracker: this._notebookTracker,
                             commands: this._commands
                         });
-                        this._tabPanel.addTab(i, s + 1)
+                        i.title.closable = !0, this._tabPanel.addTab(i, s + 1)
                     })), void 0 !== e && (0 === t && (e = 0), this._tabPanel.activateTab(e + 1))
                 }
                 _onFocusedTabChanged(e, t) {
                     this._model.setSelectedTab(t.currentIndex), this._commands.execute(b.closeControlPanel)
                 }
             }
             class ce extends x.DocumentWidget {
@@ -1853,25 +1916,25 @@
                     }
                 };
             class pe {
                 constructor(e, t, s) {
                     this.yModel = e, this.node = t, e.sharedModel.ydoc = s(e.sharedModel.commMetadata.path)
                 }
             }
-            const be = [ge, _e, L, {
+            const be = [ge, _e, T, {
                 id: "glue-jupyterlab:yjswidget-plugin",
                 autoStart: !0,
                 requires: [O.IJupyterYWidgetManager, I],
                 activate: (e, t, s) => {
                     class i extends O.JupyterYModel {
                         ydocFactory(e) {
                             const t = e.path,
                                 i = s.find((e => e.context.path.split(":")[1] === t));
                             let n;
-                            return n = i ? i.context.model.sharedModel.ydoc : new R.Doc, n
+                            return n = i ? i.context.model.sharedModel.ydoc : new H.Doc, n
                         }
                     }
                     t.registerWidget("GlueSession", i, pe)
                 }
             }, me]
         }
     }
```

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/929.a029633e30c80e22d788.js` & `glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/929.a029633e30c80e22d788.js`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/remoteEntry.7851783ebd012eb24a52.js` & `glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/remoteEntry.5c208e7340414ff77977.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, u, l, i, d, f, s, p, c, h, v, b, m, g, y, j, w, S, k = {
+    var e, r, t, a, n, o, u, l, i, f, d, s, c, p, h, v, b, m, g, y, j, w, S, k = {
             7356: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(623), t.e(797)]).then((() => () => t(8797))),
                         "./extension": () => Promise.all([t.e(623), t.e(797)]).then((() => () => t(8797))),
                         "./style": () => t.e(185).then((() => () => t(1185)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -44,50 +44,50 @@
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
         185: "0cff412fc25ed146b7c1",
-        398: "bd2742885fb1b39ca17d",
-        623: "c2a97358d4532e4eee4f",
-        797: "6a3ff8bb4f69a7056ffc",
+        623: "cca96e027ad4b198da36",
+        722: "e912ef3d95501737406e",
+        797: "6775a9c675159fcc67ec",
         929: "a029633e30c80e22d788"
     } [e] + ".js?v=" + {
         185: "0cff412fc25ed146b7c1",
-        398: "bd2742885fb1b39ca17d",
-        623: "c2a97358d4532e4eee4f",
-        797: "6a3ff8bb4f69a7056ffc",
+        623: "cca96e027ad4b198da36",
+        722: "e912ef3d95501737406e",
+        797: "6775a9c675159fcc67ec",
         929: "a029633e30c80e22d788"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "glue-jupyterlab:", E.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var u, l;
             if (void 0 !== n)
-                for (var i = document.getElementsByTagName("script"), d = 0; d < i.length; d++) {
-                    var f = i[d];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
-                        u = f;
+                for (var i = document.getElementsByTagName("script"), f = 0; f < i.length; f++) {
+                    var d = i[f];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
+                        u = d;
                         break
                     }
                 }
             u || (l = !0, (u = document.createElement("script")).charset = "utf-8", u.timeout = 120, E.nc && u.setAttribute("nonce", E.nc), u.setAttribute("data-webpack", r + n), u.src = t), e[t] = [a];
             var s = (r, a) => {
-                    u.onerror = u.onload = null, clearTimeout(p);
+                    u.onerror = u.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], u.parentNode && u.parentNode.removeChild(u), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: u
                 }), 12e4);
             u.onerror = s.bind(null, u.onerror), u.onload = s.bind(null, u.onload), l && document.head.appendChild(u)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -113,15 +113,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : u > l.from)) && (n[r] = {
                             get: t,
                             from: u,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (l("@jupyter/docprovider", "1.0.0", (() => Promise.all([E.e(398), E.e(623)]).then((() => () => E(7398))))), l("glue-jupyterlab", "0.2.0", (() => Promise.all([E.e(623), E.e(797)]).then((() => () => E(8797))))), l("gridstack", "6.0.3", (() => E.e(929).then((() => () => E(5929)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyter/docprovider", "1.0.1", (() => Promise.all([E.e(722), E.e(623)]).then((() => () => E(7722))))), l("glue-jupyterlab", "0.3.0", (() => Promise.all([E.e(623), E.e(797)]).then((() => () => E(8797))))), l("gridstack", "6.0.3", (() => E.e(929).then((() => () => E(5929)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -171,79 +171,79 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var u = 0, l = 1, i = !0;; l++, u++) {
-                var d, f, s = l < e.length ? (typeof e[l])[0] : "";
-                if (u >= r.length || "o" == (f = (typeof(d = r[u]))[0])) return !i || ("u" == s ? l > a && !n : "" == s != n);
-                if ("u" == f) {
+                var f, d, s = l < e.length ? (typeof e[l])[0] : "";
+                if (u >= r.length || "o" == (d = (typeof(f = r[u]))[0])) return !i || ("u" == s ? l > a && !n : "" == s != n);
+                if ("u" == d) {
                     if (!i || "u" != s) return !1
                 } else if (i)
-                    if (s == f)
+                    if (s == d)
                         if (l <= a) {
-                            if (d != e[l]) return !1
+                            if (f != e[l]) return !1
                         } else {
-                            if (n ? d > e[l] : d < e[l]) return !1;
-                            d != e[l] && (i = !1)
+                            if (n ? f > e[l] : f < e[l]) return !1;
+                            f != e[l] && (i = !1)
                         }
                 else if ("s" != s && "n" != s) {
                     if (n || l <= a) return !1;
                     i = !1, l--
                 } else {
-                    if (l <= a || f < s != n) return !1;
+                    if (l <= a || d < s != n) return !1;
                     i = !1
                 } else "s" != s && "n" != s && (i = !1, l--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (u = 1; u < e.length; u++) {
             var h = e[u];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, u = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, i = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, d = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
+    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", d = (e, r, t, a) => {
         var n = i(e, t);
-        return o(a, n) || c(d(e, t, n, a)), v(e[t][n])
+        return o(a, n) || p(f(e, t, n, a)), v(e[t][n])
     }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, p = (e, r, t, a) => {
+    }, c = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
-    }, c = e => {
+    }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, a) => {
-        c(p(e, r, t, a))
+        p(c(e, r, t, a))
     }, v = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, a, n) {
         var o = E.I(r);
         return o && o.then ? o.then(e.bind(e, r, E.S[r], t, a, n)) : e(r, E.S[r], t, a, n)
-    })(((e, r, t, a) => (u(e, t), v(s(r, t, a) || h(r, e, t, a) || l(r, t))))), g = b(((e, r, t, a) => (u(e, t), f(r, 0, t, a)))), y = b(((e, r, t, a, n) => {
+    })(((e, r, t, a) => (u(e, t), v(s(r, t, a) || h(r, e, t, a) || l(r, t))))), g = b(((e, r, t, a) => (u(e, t), d(r, 0, t, a)))), y = b(((e, r, t, a, n) => {
         var o = r && E.o(r, t) && s(r, t, a);
         return o ? v(o) : n()
     })), j = {}, w = {
         981: () => g("default", "yjs", [1, 13, 5, 40]),
         4238: () => g("default", "@jupyterlab/services", [1, 7, 0, 2]),
         4901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
         5350: () => g("default", "@jupyterlab/apputils", [1, 4, 1, 2]),
         7930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
         9993: () => g("default", "@jupyterlab/coreutils", [1, 6, 0, 2]),
-        858: () => y("default", "@jupyter/docprovider", [1, 1, 0, 0, , "alpha", 8], (() => E.e(398).then((() => () => E(7398))))),
+        858: () => y("default", "@jupyter/docprovider", [1, 1, 0, 0, , "alpha", 8], (() => E.e(722).then((() => () => E(7722))))),
         1554: () => g("default", "@jupyterlab/docmanager", [1, 4, 0, 2]),
         1919: () => g("default", "@jupyterlab/notebook", [1, 4, 0, 2]),
         2164: () => g("default", "@jupyterlab/filebrowser", [1, 4, 0, 2]),
         2189: () => g("default", "@jupyterlab/ui-components", [1, 4, 0, 2]),
         2293: () => g("default", "@jupyter/ydoc", [1, 1, 0, 2]),
         3262: () => g("default", "@jupyterlab/launcher", [1, 4, 0, 2]),
         3363: () => m("default", "@jupyterlab/outputarea", [1, 4, 0, 2]),
```

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/labextension/static/third-party-licenses.json` & `glue_jupyterlab-0.3.0/glue_jupyterlab/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '1.0.1'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/docprovider",
-            "versionInfo": "1.0.0"
+            "versionInfo": "1.0.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "6.8.1"
         },
```

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/tests/conftest.py` & `glue_jupyterlab-0.3.0/glue_jupyterlab/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/tests/test_glue_session.py` & `glue_jupyterlab-0.3.0/glue_jupyterlab/tests/test_glue_session.py`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/glue_jupyterlab/tests/test_ydoc.py` & `glue_jupyterlab-0.3.0/glue_jupyterlab/tests/test_ydoc.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,14 +40,26 @@
     updated_content = json.loads(yglue_doc.get())
 
     assert "Tab 3" in updated_content["__main__"]["tab_names"]
     assert len(updated_content["__main__"]["viewers"]) == 3
     assert "NewScatter" in updated_content["__main__"]["viewers"][2]
 
 
+def test_get_remove_tab(yglue_doc):
+    ## Fake editing of the y structure
+    with yglue_doc._ydoc.begin_transaction() as t:
+        # Remove a tab
+        yglue_doc._ytabs.pop(t, "Tab 1", None)
+
+    updated_content = json.loads(yglue_doc.get())
+
+    assert "Tab 1" not in updated_content["__main__"]["tab_names"]
+    assert len(updated_content["__main__"]["viewers"]) == 1
+
+
 def test_links(yglue_doc_links, identity_link):
     yglue_doc_links.get()
     links = yglue_doc_links.links
     required = [
         "_type",
         "data1",
         "data2",
```

### Comparing `glue_jupyterlab-0.2.0/src/commands.ts` & `glue_jupyterlab-0.3.0/src/commands.ts`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,16 @@
   export const new3DScatter = 'glue-control:new-3d-scatter-viewer';
 
   export const newTable = 'glue-control:new-table-viewer';
 
   export const openControlPanel = 'glue-control:open-control-panel';
 
   export const closeControlPanel = 'glue-control:close-control-panel';
+
+  export const addViewerLayer = 'glue-control:add-viewer-layer';
 }
 
 export interface INewViewerArgs {
   dataset?: string;
   position?: [number, number];
   size?: [number, number];
 }
```

### Comparing `glue_jupyterlab-0.2.0/src/tools.ts` & `glue_jupyterlab-0.3.0/src/tools.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/types.ts` & `glue_jupyterlab-0.3.0/src/types.ts`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
   contentsChanged: ISignal<IGlueSessionSharedModel, IDict>;
   datasetChanged: ISignal<IGlueSessionSharedModel, IDict>;
   linksChanged: ISignal<IGlueSessionSharedModel, IDict>;
   tabChanged: ISignal<IGlueSessionSharedModel, IDict>;
   tabsChanged: ISignal<IGlueSessionSharedModel, IDict>;
   localStateChanged: ISignal<IGlueSessionSharedModel, { keys: string[] }>;
   addTab(): void;
+  removeTab(tabName: string): void;
   getTabNames(): string[];
   getTabData(tabName: string): IDict<IGlueSessionViewerTypes> | undefined;
 
   getTabItem(
     tabName: string,
     itemID: string
   ): IGlueSessionViewerTypes | undefined;
```

### Comparing `glue_jupyterlab-0.2.0/src/yWidget.ts` & `glue_jupyterlab-0.3.0/src/yWidget.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/common/tabPanel.ts` & `glue_jupyterlab-0.3.0/src/common/tabPanel.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/document/docModel.ts` & `glue_jupyterlab-0.3.0/src/document/docModel.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/document/modelFactory.ts` & `glue_jupyterlab-0.3.0/src/document/modelFactory.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/document/plugin.ts` & `glue_jupyterlab-0.3.0/src/document/plugin.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/document/sharedModel.ts` & `glue_jupyterlab-0.3.0/src/document/sharedModel.ts`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,22 @@
     }
     const newTab = new Y.Map<IDict>();
     this.transact(() => {
       this._tabs.set(tabName, newTab);
     }, false);
   }
 
+  removeTab(name: string): void {
+    if (this._tabs.has(name)) {
+      this.transact(() => {
+        this._tabs.delete(name);
+      }, false);
+    }
+  }
+
   getTabNames(): string[] {
     return [...this._tabs.keys()];
   }
 
   getTabData(tabName: string): IDict<IGlueSessionViewerTypes> | undefined {
     const tab = this._tabs.get(tabName);
     if (tab) {
```

### Comparing `glue_jupyterlab-0.2.0/src/document/widgetFactory.ts` & `glue_jupyterlab-0.3.0/src/document/widgetFactory.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/leftPanel/model.ts` & `glue_jupyterlab-0.3.0/src/leftPanel/model.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/leftPanel/plugin.ts` & `glue_jupyterlab-0.3.0/src/leftPanel/plugin.ts`

 * *Files 3% similar despite different names*

```diff
@@ -225,14 +225,31 @@
     execute: () => {
       if (!controlModel.sharedModel) {
         return;
       }
       controlModel.clearConfig();
     }
   });
+
+  commands.addCommand(CommandIDs.addViewerLayer, {
+    execute: async args => {
+      const kernel = controlModel.currentSessionKernel();
+      if (kernel === undefined) {
+        // TODO Show an error dialog
+        return;
+      }
+
+      const code = `
+      GLUE_SESSION.add_viewer_layer("${args.tab}", "${args.viewer}", "${args.data}")
+      `;
+
+      const future = kernel.requestExecute({ code }, false);
+      await future.done;
+    }
+  });
 }
 
 export const controlPanel: JupyterFrontEndPlugin<void> = {
   id: 'glue-jupyterlab:control-panel',
   autoStart: true,
   requires: [ILayoutRestorer, IGlueSessionTracker, IRenderMimeRegistry],
   activate: (
```

### Comparing `glue_jupyterlab-0.2.0/src/leftPanel/widget.ts` & `glue_jupyterlab-0.3.0/src/leftPanel/widget.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/leftPanel/config/configPanel.ts` & `glue_jupyterlab-0.3.0/src/leftPanel/config/configPanel.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/leftPanel/config/configWidget.ts` & `glue_jupyterlab-0.3.0/src/leftPanel/config/configWidget.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/leftPanel/config/configWidgetModel.ts` & `glue_jupyterlab-0.3.0/src/leftPanel/config/configWidgetModel.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/leftPanel/data/dataPanel.ts` & `glue_jupyterlab-0.3.0/src/leftPanel/data/dataPanel.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/leftPanel/data/datasetsWidget.tsx` & `glue_jupyterlab-0.3.0/src/leftPanel/data/datasetsWidget.tsx`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/linkPanel/linkEditor.ts` & `glue_jupyterlab-0.3.0/src/linkPanel/linkEditor.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/linkPanel/linkEditorWidget.ts` & `glue_jupyterlab-0.3.0/src/linkPanel/linkEditorWidget.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/linkPanel/model.ts` & `glue_jupyterlab-0.3.0/src/linkPanel/model.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/linkPanel/types.ts` & `glue_jupyterlab-0.3.0/src/linkPanel/types.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/linkPanel/widgets/linking.tsx` & `glue_jupyterlab-0.3.0/src/linkPanel/widgets/linking.tsx`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/linkPanel/widgets/summary.tsx` & `glue_jupyterlab-0.3.0/src/linkPanel/widgets/summary.tsx`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/schemas/glue.schema.json` & `glue_jupyterlab-0.3.0/src/schemas/glue.schema.json`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/schemas/link.schema.json` & `glue_jupyterlab-0.3.0/src/schemas/link.schema.json`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/schemas/data/dataset.schema.json` & `glue_jupyterlab-0.3.0/src/schemas/data/dataset.schema.json`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/schemas/viewers/1dprofile.schema.json` & `glue_jupyterlab-0.3.0/src/schemas/viewers/1dprofile.schema.json`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/schemas/viewers/2dscatter.schema.json` & `glue_jupyterlab-0.3.0/src/schemas/viewers/2dscatter.schema.json`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/schemas/viewers/3dscatter.schema.json` & `glue_jupyterlab-0.3.0/src/schemas/viewers/3dscatter.schema.json`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/schemas/viewers/histogram.schema.json` & `glue_jupyterlab-0.3.0/src/schemas/viewers/histogram.schema.json`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/schemas/viewers/image.schema.json` & `glue_jupyterlab-0.3.0/src/schemas/viewers/image.schema.json`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/viewPanel/glueDocumentWidget.ts` & `glue_jupyterlab-0.3.0/src/viewPanel/glueDocumentWidget.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/src/viewPanel/gridStackItem.ts` & `glue_jupyterlab-0.3.0/src/viewPanel/gridStackItem.ts`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import { Panel, Widget } from '@lumino/widgets';
 import { Toolbar, ToolbarButton, closeIcon } from '@jupyterlab/ui-components';
+import { Message } from '@lumino/messaging';
 import { ISignal, Signal } from '@lumino/signaling';
+import { DATASET_MIME } from '../types';
 
 export class GridStackItem extends Panel {
   constructor(options: GridStackItem.IOptions) {
     super();
     this.removeClass('lm-Widget');
     this.removeClass('p-Widget');
     this.addClass('grid-stack-item');
     this.addClass('glue-item');
 
-    const { cellIdentity, cell, itemTitle = '', pos, size } = options;
+    const { cellIdentity, cell, itemTitle = '', pos, size, tabName } = options;
     this._cellOutput = cell;
     this.cellIdentity = cellIdentity;
     this._pos = pos;
     this._size = size;
     this._title = itemTitle;
+    this._tabName = tabName;
 
     const content = new Panel();
     content.addClass('grid-stack-item-content');
 
     const toolbar = this._createToolbar(itemTitle);
     content.addWidget(toolbar);
     cell.addClass('grid-item-widget');
@@ -59,18 +62,43 @@
     return this._size;
   }
 
   set size(value: number[]) {
     this._size = value;
   }
 
+  get tabName(): string {
+    return this._tabName;
+  }
+
+  set tabName(value: string) {
+    this._tabName = value;
+  }
   get changed(): ISignal<GridStackItem, GridStackItem.IChange> {
     return this._changed;
   }
 
+  protected onAfterAttach(msg: Message): void {
+    super.onAfterAttach(msg);
+    this.node.addEventListener('drop', this._ondrop.bind(this));
+  }
+
+  protected onBeforeDetach(msg: Message): void {
+    this.node.removeEventListener('drop', this._ondrop.bind(this));
+    super.onBeforeDetach(msg);
+  }
+
+  private async _ondrop(event: DragEvent) {
+    const datasetId = event.dataTransfer?.getData(DATASET_MIME);
+    if (!datasetId) {
+      return;
+    }
+    this._changed.emit({ action: 'layer', dataLayer: datasetId });
+  }
+
   private _createToolbar(itemTitle: string): Toolbar {
     const toolbar = new Toolbar();
     toolbar.node.addEventListener('click', () => {
       this._changed.emit({ action: 'edit' });
     });
     toolbar.addClass('glue-Session-tab-toolbar');
 
@@ -93,24 +121,26 @@
 
   private _spinner: HTMLDivElement;
 
   private _pos: number[];
   private _size: number[];
   private _title: string;
   private _cellOutput: Widget;
-
+  private _tabName: string;
   private _changed: Signal<GridStackItem, GridStackItem.IChange>;
 }
 
 export namespace GridStackItem {
   export interface IOptions {
     cellIdentity: string;
     cell: Widget;
     itemTitle?: string;
     pos: number[];
     size: number[];
+    tabName: string;
   }
 
   export interface IChange {
-    action: 'close' | 'lock' | 'edit';
+    action: 'close' | 'lock' | 'edit' | 'layer';
+    dataLayer?: string;
   }
 }
```

### Comparing `glue_jupyterlab-0.2.0/src/viewPanel/sessionWidget.ts` & `glue_jupyterlab-0.3.0/src/viewPanel/sessionWidget.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-import { PromiseDelegate } from '@lumino/coreutils';
-import { TabBar, BoxPanel, Widget } from '@lumino/widgets';
-
 import { Dialog, InputDialog, showDialog } from '@jupyterlab/apputils';
-import { IRenderMimeRegistry } from '@jupyterlab/rendermime';
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 import { INotebookTracker } from '@jupyterlab/notebook';
+import { IRenderMimeRegistry } from '@jupyterlab/rendermime';
+import { IKernelConnection } from '@jupyterlab/services/lib/kernel/kernel';
+import { CommandRegistry } from '@lumino/commands';
+import { PromiseDelegate } from '@lumino/coreutils';
+import { Message } from '@lumino/messaging';
+import { BoxPanel, TabBar, Widget } from '@lumino/widgets';
+import { IJupyterYWidgetManager } from 'yjs-widgets';
 
+import { CommandIDs } from '../commands';
 import { HTabPanel } from '../common/tabPanel';
-import { DATASET_MIME, IDict, IGlueSessionSharedModel } from '../types';
 import { GlueSessionModel } from '../document/docModel';
+import { LinkEditor } from '../linkPanel/linkEditor';
 import { mockNotebook } from '../tools';
+import { DATASET_MIME, IDict, IGlueSessionSharedModel } from '../types';
 import { TabView } from './tabView';
-import { LinkEditor } from '../linkPanel/linkEditor';
-
-import { Message } from '@lumino/messaging';
-import { CommandRegistry } from '@lumino/commands';
-import { CommandIDs } from '../commands';
-import { IJupyterYWidgetManager } from 'yjs-widgets';
-import { IKernelConnection } from '@jupyterlab/services/lib/kernel/kernel';
 
 export class SessionWidget extends BoxPanel {
   constructor(options: SessionWidget.IOptions) {
     super({ direction: 'top-to-bottom' });
     this.addClass('grid-panel');
     this.addClass('glue-Session-panel');
 
@@ -46,14 +44,26 @@
       tabBarOption: {
         addButtonEnabled: true
       }
     });
     this._tabPanel.topBar.addRequested.connect(() => {
       this._model.addTab();
     });
+    this._tabPanel.topBar.tabCloseRequested.connect(async (tab, arg) => {
+      const confirm = await showDialog({
+        title: 'Delete Tab',
+        body: 'Are you sure you want to delete this tab?',
+        buttons: [Dialog.cancelButton(), Dialog.okButton({ label: 'Delete' })]
+      });
+      if (confirm.button.accept) {
+        arg.title.owner.close();
+        this._tabPanel.topBar.removeTabAt(arg.index);
+        this._model.removeTab(arg.title.label);
+      }
+    });
     if (this._model) {
       this._linkWidget = new LinkEditor({ sharedModel: this._model });
       this._tabPanel.addTab(this._linkWidget, 0);
     }
 
     this.addWidget(this._tabPanel);
     BoxPanel.setStretch(this._tabPanel, 1);
@@ -92,16 +102,22 @@
   }
 
   private _ondragover(event: DragEvent) {
     event.preventDefault();
   }
 
   private async _ondrop(event: DragEvent) {
-    const datasetId = event.dataTransfer?.getData(DATASET_MIME);
+    const target = event.target as HTMLElement;
+    const viewer = target.closest('.grid-stack-item.glue-item');
+    // No-op if the target is a viewer, it will be managed by the viewer itself.
+    if (viewer) {
+      return;
+    }
 
+    const datasetId = event.dataTransfer?.getData(DATASET_MIME);
     const items: IDict<string> = {
       Histogram: CommandIDs.new1DHistogram,
       '1D Profile': CommandIDs.new1DProfile,
       '2D Scatter': CommandIDs.new2DScatter,
       '3D Scatter': CommandIDs.new3DScatter,
       '2D Image': CommandIDs.new2DImage,
       Table: CommandIDs.newTable
@@ -156,15 +172,20 @@
   }
 
   private async _onTabsChanged() {
     await this._pythonSessionCreated.promise;
     let newTabIndex: number | undefined = undefined;
     const currentIndex = this._tabPanel.topBar.currentIndex;
     const tabNames = this._model.getTabNames();
-
+    Object.keys(this._tabViews).forEach(k => {
+      if (!tabNames.includes(k)) {
+        this._tabViews[k].dispose();
+        delete this._tabViews[k];
+      }
+    });
     tabNames.forEach((tabName, idx) => {
       // Tab already exists, we don't do anything
       if (tabName in this._tabViews) {
         return;
       }
       newTabIndex = idx;
       // Tab does not exist, we create it
@@ -172,15 +193,15 @@
         tabName,
         model: this._model,
         rendermime: this._rendermime,
         context: this._context,
         notebookTracker: this._notebookTracker,
         commands: this._commands
       }));
-
+      tabWidget.title.closable = true;
       this._tabPanel.addTab(tabWidget, idx + 1);
     });
 
     // TODO Remove leftover tabs
     // for (const tabName in Object.keys(this._tabViews)) {
     //   if (!(tabName in tabNames)) {
     //     todo
```

### Comparing `glue_jupyterlab-0.2.0/src/viewPanel/tabLayout.ts` & `glue_jupyterlab-0.3.0/src/viewPanel/tabLayout.ts`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,29 @@
     this.unselectGridItems();
     item.node.classList.add('grid-selected');
     this._commands.execute(CommandIDs.openControlPanel, {
       cellId: item.cellIdentity,
       gridItem: item as any
     });
   }
+
+  /**
+   * Request to add a layer with a dataset to the viewer.
+   *
+   * @param item - the viewer where to add a layer.
+   * @param dataName - the data to add to the viewer.
+   */
+  private _addViewerLayer(item: GridStackItem, dataName: string): void {
+    this._commands.execute(CommandIDs.addViewerLayer, {
+      tab: item.tabName,
+      viewer: item.cellIdentity,
+      data: dataName
+    });
+  }
+
   /**
    * Handle change-event messages sent to from gridstack.
    */
   private _onChange(event: Event, items: GridStackNode[]): void {
     const data: ViewInfo[] = items.map(item => {
       return Private.gridToPixel(this._grid.cellWidth(), item);
     });
@@ -372,14 +387,20 @@
       case 'close':
         sender.changed.disconnect(this._onItemChanged, this);
         this.removeGridItem(sender.cellIdentity);
         break;
       case 'edit':
         this._handleEdit(sender);
         break;
+      case 'layer':
+        if (!change.dataLayer) {
+          return;
+        }
+        this._addViewerLayer(sender, change.dataLayer);
+        break;
       default:
         break;
     }
   }
 
   private _prepareGrid(): void {
     const rect = this.parent!.node.getBoundingClientRect();
@@ -387,15 +408,15 @@
     this._grid.onParentResize();
   }
 
   private _gridHost: HTMLElement;
   private _grid: GridStack;
   private _gridItems: Map<string, GridStackItem>;
   private _gridItemChanged = new Signal<this, TabLayout.IChange>(this);
-  private _resizeTimeout = 0;
+  private _resizeTimeout: any = 0;
   private _commands: CommandRegistry;
 }
 
 export namespace TabLayout {
   export interface IChange {
     action: 'remove' | 'move' | 'resize';
     items: ViewInfo[] | string[];
```

### Comparing `glue_jupyterlab-0.2.0/src/viewPanel/tabView.ts` & `glue_jupyterlab-0.3.0/src/viewPanel/tabView.ts`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,18 @@
       this
     );
     this._model.tabChanged.disconnect(this._onTabChanged, this);
     this._model.localStateChanged.disconnect(this._onLocalStateChanged);
     super.dispose();
   }
 
+  protected onCloseRequest(msg: Message): void {
+    this.dispose();
+  }
+
   /**
    * The tab name
    */
   get tabName(): string {
     return this._tabName;
   }
 
@@ -149,15 +153,16 @@
       });
 
       const item = new GridStackItem({
         cellIdentity: viewerId,
         cell: out,
         itemTitle: itemTitle.match(/($[a-z])|[A-Z][^A-Z]+/g)?.join(' '),
         pos: viewerData.pos,
-        size: viewerData.size
+        size: viewerData.size,
+        tabName: tabName
       });
       const cellOutput = item.cellOutput as SimplifiedOutputArea;
       if (this._context) {
         SimplifiedOutputArea.execute(
           `
           GLUE_SESSION.create_viewer("${tabName}", "${viewerId}")
           `,
```

### Comparing `glue_jupyterlab-0.2.0/style/base.css` & `glue_jupyterlab-0.3.0/style/base.css`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/style/icons/glue-icon.svg` & `glue_jupyterlab-0.3.0/style/icons/glue-icon.svg`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/README.md` & `glue_jupyterlab-0.3.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/playwright.config.js` & `glue_jupyterlab-0.3.0/ui-tests/playwright.config.js`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/yarn.lock` & `glue_jupyterlab-0.3.0/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/add-data-data-added-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/add-data-data-added-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/add-data-file-browser-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/add-data-file-browser-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/add-data-viewer-created-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/add-data-viewer-created-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/add-data-viewer-selection-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/add-data-viewer-selection-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/control-panel-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/control-panel-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/control-panel-switch-tab-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/control-panel-switch-tab-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/histogram-linked-selection-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/histogram-linked-selection-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/histogram-no-selection-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/histogram-no-selection-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/histogram-selection-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/histogram-selection-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/link-editor-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/link-editor-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/session-tab1-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/session-tab1-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/ui-tests/tests/test.spec.ts-snapshots/session-tab2-linux.png` & `glue_jupyterlab-0.3.0/ui-tests/tests/test.spec.ts-snapshots/session-tab2-linux.png`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/.gitignore` & `glue_jupyterlab-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/LICENSE` & `glue_jupyterlab-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/README.md` & `glue_jupyterlab-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/pyproject.toml` & `glue_jupyterlab-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `glue_jupyterlab-0.2.0/PKG-INFO` & `glue_jupyterlab-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-jupyterlab
-Version: 0.2.0
+Version: 0.3.0
 Summary: A JupyterLab extension for glue-viz
 Project-URL: Homepage, https://github.com/QuantStack/glue-jupyterlab
 Project-URL: Bug Tracker, https://github.com/QuantStack/glue-jupyterlab/issues
 Project-URL: Repository, https://github.com/QuantStack/glue-jupyterlab.git
 Author-email: QuantStack <info@quantstack.net>
 License: BSD 3-Clause License
```

