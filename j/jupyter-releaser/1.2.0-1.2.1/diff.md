# Comparing `tmp/jupyter_releaser-1.2.0.tar.gz` & `tmp/jupyter_releaser-1.2.1.tar.gz`

## Comparing `jupyter_releaser-1.2.0.tar` & `jupyter_releaser-1.2.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.readthedocs.yml
--rw-r--r--   0        0        0   126470 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/RELEASE.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/actions/check-release/action.yml
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/actions/finalize-release/action.yml
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/actions/install-releaser/action.yml
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/actions/populate-release/action.yml
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/actions/prep-release/action.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/scripts/bump_tag.sh
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/generate-changelog.yml
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/make.bat
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/index.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/_static/custom.css
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/_static/images/logo/favicon.svg
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/_static/images/logo/logo.svg
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/background/index.rst
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/background/theory.md
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/get_started/generate_changelog.md
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/get_started/index.rst
--rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/get_started/making_release_from_releaser.md
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/get_started/making_release_from_repo.md
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/how_to_guides/convert_repo_from_releaser.md
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/how_to_guides/convert_repo_from_repo.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/how_to_guides/index.rst
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/how_to_guides/maintain_fork.md
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/how_to_guides/write_config.md
--rw-r--r--   0        0        0   507289 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/draft_github_release.png
--rw-r--r--   0        0        0   586032 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/final_github_release.png
--rw-r--r--   0        0        0   169812 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/fork_fetch.png
--rw-r--r--   0        0        0   276246 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/generate_changelog.png
--rw-r--r--   0        0        0    99291 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/prep_release.png
--rw-r--r--   0        0        0   212895 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/prep_release_next_step.png
--rw-r--r--   0        0        0   237681 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/prep_release_repo.png
--rw-r--r--   0        0        0    74988 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/publish_release.png
--rw-r--r--   0        0        0   177023 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/publish_release_next_step.png
--rw-r--r--   0        0        0   191024 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/publish_release_repo.png
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/reference/api_docs.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/reference/configuration.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/reference/faq.md
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/reference/index.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/reference/releaser_cli.rst
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/example-workflows/full-release.yml
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/example-workflows/prep-release.yml
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/example-workflows/publish-release.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/__main__.py
--rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/changelog.py
--rw-r--r--   0        0        0    19620 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/cli.py
--rw-r--r--   0        0        0    19880 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/lib.py
--rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/mock_github.py
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/npm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/py.typed
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/python.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/schema.json
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tee.py
--rw-r--r--   0        0        0    24593 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/common.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/finalize_release.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/generate_changelog.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/populate_release.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/prep_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/__init__.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/conftest.py
--rw-r--r--   0        0        0    26596 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/test_cli.py
--rw-r--r--   0        0        0    12126 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/test_functions.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/test_mock_github.py
--rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/util.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.gitignore
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/LICENSE
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/README.md
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.readthedocs.yml
+-rw-r--r--   0        0        0   127289 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/RELEASE.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/actions/check-release/action.yml
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/actions/finalize-release/action.yml
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/actions/install-releaser/action.yml
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/actions/populate-release/action.yml
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/actions/prep-release/action.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/scripts/bump_tag.sh
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/workflows/generate-changelog.yml
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/make.bat
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/_static/custom.css
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/_static/images/logo/favicon.svg
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/_static/images/logo/logo.svg
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/background/index.rst
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/background/theory.md
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/get_started/generate_changelog.md
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/get_started/index.rst
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/get_started/making_release_from_releaser.md
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/get_started/making_release_from_repo.md
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/how_to_guides/convert_repo_from_releaser.md
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/how_to_guides/convert_repo_from_repo.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/how_to_guides/index.rst
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/how_to_guides/maintain_fork.md
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/how_to_guides/write_config.md
+-rw-r--r--   0        0        0   507289 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/images/draft_github_release.png
+-rw-r--r--   0        0        0   586032 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/images/final_github_release.png
+-rw-r--r--   0        0        0   169812 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/images/fork_fetch.png
+-rw-r--r--   0        0        0   276246 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/images/generate_changelog.png
+-rw-r--r--   0        0        0    99291 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/images/prep_release.png
+-rw-r--r--   0        0        0   212895 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/images/prep_release_next_step.png
+-rw-r--r--   0        0        0   237681 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/images/prep_release_repo.png
+-rw-r--r--   0        0        0    74988 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/images/publish_release.png
+-rw-r--r--   0        0        0   177023 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/images/publish_release_next_step.png
+-rw-r--r--   0        0        0   191024 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/images/publish_release_repo.png
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/reference/api_docs.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/reference/configuration.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/reference/faq.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/reference/index.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/docs/source/reference/releaser_cli.rst
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/example-workflows/full-release.yml
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/example-workflows/prep-release.yml
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/example-workflows/publish-release.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/__init__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/__main__.py
+-rw-r--r--   0        0        0    10543 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/changelog.py
+-rw-r--r--   0        0        0    19778 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/cli.py
+-rw-r--r--   0        0        0    19872 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/lib.py
+-rw-r--r--   0        0        0     8348 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/mock_github.py
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/npm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/py.typed
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/python.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/schema.json
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/tee.py
+-rw-r--r--   0        0        0    24593 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/actions/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/actions/common.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/actions/finalize_release.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/actions/generate_changelog.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/actions/populate_release.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/actions/prep_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/tests/__init__.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/tests/conftest.py
+-rw-r--r--   0        0        0    26596 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/tests/test_cli.py
+-rw-r--r--   0        0        0    12126 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/tests/test_functions.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/tests/test_mock_github.py
+-rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/jupyter_releaser/tests/util.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/README.md
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.1/PKG-INFO
```

### Comparing `jupyter_releaser-1.2.0/.pre-commit-config.yaml` & `jupyter_releaser-1.2.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.23.1
+    rev: 0.23.2
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
@@ -32,12 +32,12 @@
           [mdformat-gfm, mdformat-frontmatter, mdformat-footnote]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.276
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyter_releaser-1.2.0/CHANGELOG.md` & `jupyter_releaser-1.2.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.2.1
+
+([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...0469672a12bfdcd2d1c7834e05a82aaeec59f103))
+
+### Maintenance and upkeep improvements
+
+- Fix compat with pydantic 2 [#518](https://github.com/jupyter-server/jupyter_releaser/pull/518) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_releaser/graphs/contributors?from=2023-06-20&to=2023-07-10&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Ablink1073+updated%3A2023-06-20..2023-07-10&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Apre-commit-ci+updated%3A2023-06-20..2023-07-10&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.2.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...b1388d01b8d28ea077fab281bd78ecc1c9c18773))
 
 ### Enhancements made
 
 - Add support for PyPI trusted publisher and NPM provenance [#511](https://github.com/jupyter-server/jupyter_releaser/pull/511) ([@fcollonval](https://github.com/fcollonval))
@@ -21,16 +37,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_releaser/graphs/contributors?from=2023-06-19&to=2023-06-20&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Ablink1073+updated%3A2023-06-19..2023-06-20&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Afcollonval+updated%3A2023-06-19..2023-06-20&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.1.6
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...0b4c9cc2b257e799794c6d02735b659da09e2336))
 
 ### Maintenance and upkeep improvements
 
 - Pin ghapi [#512](https://github.com/jupyter-server/jupyter_releaser/pull/512) ([@blink1073](https://github.com/blink1073))
```

### Comparing `jupyter_releaser-1.2.0/CONTRIBUTING.md` & `jupyter_releaser-1.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/.github/actions/check-release/action.yml` & `jupyter_releaser-1.2.1/.github/actions/check-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/.github/actions/finalize-release/action.yml` & `jupyter_releaser-1.2.1/.github/actions/finalize-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/.github/actions/populate-release/action.yml` & `jupyter_releaser-1.2.1/.github/actions/populate-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/.github/actions/prep-release/action.yml` & `jupyter_releaser-1.2.1/.github/actions/prep-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/.github/workflows/check-release.yml` & `jupyter_releaser-1.2.1/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/.github/workflows/generate-changelog.yml` & `jupyter_releaser-1.2.1/.github/workflows/generate-changelog.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/.github/workflows/prep-release.yml` & `jupyter_releaser-1.2.1/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/.github/workflows/publish-release.yml` & `jupyter_releaser-1.2.1/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/.github/workflows/test.yml` & `jupyter_releaser-1.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/Makefile` & `jupyter_releaser-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/make.bat` & `jupyter_releaser-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/conf.py` & `jupyter_releaser-1.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/_static/images/logo/favicon.svg` & `jupyter_releaser-1.2.1/docs/source/_static/images/logo/favicon.svg`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/_static/images/logo/logo.svg` & `jupyter_releaser-1.2.1/docs/source/_static/images/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/background/theory.md` & `jupyter_releaser-1.2.1/docs/source/background/theory.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/get_started/generate_changelog.md` & `jupyter_releaser-1.2.1/docs/source/get_started/generate_changelog.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/get_started/making_release_from_releaser.md` & `jupyter_releaser-1.2.1/docs/source/get_started/making_release_from_releaser.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/get_started/making_release_from_repo.md` & `jupyter_releaser-1.2.1/docs/source/get_started/making_release_from_repo.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/how_to_guides/convert_repo_from_releaser.md` & `jupyter_releaser-1.2.1/docs/source/how_to_guides/convert_repo_from_releaser.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/how_to_guides/convert_repo_from_repo.md` & `jupyter_releaser-1.2.1/docs/source/how_to_guides/convert_repo_from_repo.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/how_to_guides/write_config.md` & `jupyter_releaser-1.2.1/docs/source/how_to_guides/write_config.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/images/draft_github_release.png` & `jupyter_releaser-1.2.1/docs/source/images/draft_github_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/images/final_github_release.png` & `jupyter_releaser-1.2.1/docs/source/images/final_github_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/images/fork_fetch.png` & `jupyter_releaser-1.2.1/docs/source/images/fork_fetch.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/images/generate_changelog.png` & `jupyter_releaser-1.2.1/docs/source/images/generate_changelog.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/images/prep_release.png` & `jupyter_releaser-1.2.1/docs/source/images/prep_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/images/prep_release_next_step.png` & `jupyter_releaser-1.2.1/docs/source/images/prep_release_next_step.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/images/prep_release_repo.png` & `jupyter_releaser-1.2.1/docs/source/images/prep_release_repo.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/images/publish_release.png` & `jupyter_releaser-1.2.1/docs/source/images/publish_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/images/publish_release_next_step.png` & `jupyter_releaser-1.2.1/docs/source/images/publish_release_next_step.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/images/publish_release_repo.png` & `jupyter_releaser-1.2.1/docs/source/images/publish_release_repo.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/reference/api_docs.rst` & `jupyter_releaser-1.2.1/docs/source/reference/api_docs.rst`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/docs/source/reference/faq.md` & `jupyter_releaser-1.2.1/docs/source/reference/faq.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/example-workflows/full-release.yml` & `jupyter_releaser-1.2.1/example-workflows/full-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/example-workflows/prep-release.yml` & `jupyter_releaser-1.2.1/example-workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/example-workflows/publish-release.yml` & `jupyter_releaser-1.2.1/example-workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/changelog.py` & `jupyter_releaser-1.2.1/jupyter_releaser/changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     -------
     str
         A formatted changelog entry with markers
     """
     branch = branch or util.get_branch()
     since = since or util.get_latest_tag(ref or branch, since_last_stable)
 
-    if since == "":  # noqa
+    if since == "":
         since = util.get_first_commit(ref or branch)
 
     util.log(f"Getting changes to {repo} since {since} on branch {branch}...")
 
     until = until.replace("%", "") if until else None
 
     md = generate_activity_md(
```

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/cli.py` & `jupyter_releaser-1.2.1/jupyter_releaser/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from jupyter_releaser import changelog, lib, npm, python, util
 
 
 class ReleaseHelperGroup(click.Group):
     """Click group tailored to jupyter-releaser"""
 
-    _needs_checkout_dir: t.Dict[str, bool] = {}
+    _needs_checkout_dir: t.Dict[str, bool] = {}  # noqa
 
     def invoke(self, ctx):  # noqa
         """Handle jupyter-releaser config while invoking a command"""
         # Get the command name and make sure it is valid
         cmd_name = ctx.protected_args[0]
         if cmd_name not in self.commands:
             super().invoke(ctx)
@@ -142,155 +142,157 @@
         os.chdir(orig_dir)
 
     def list_commands(self, ctx):
         """List commands in insertion order"""
         return self.commands.keys()
 
 
-@click.group(cls=ReleaseHelperGroup)
+@click.group(cls=ReleaseHelperGroup)  # type:ignore[arg-type]
 @click.option("--force", default=False, help="Force a command to run even when skipped by config")
 def main(force):
     """Jupyter Releaser scripts"""
     pass
 
 
 # Extracted common options
-version_spec_options = [
+version_spec_options: t.Any = [
     click.option(
         "--version-spec",
         envvar="RH_VERSION_SPEC",
         default="",
         help="The new version specifier",
     )
 ]
 
 
-post_version_spec_options = [
+post_version_spec_options: t.Any = [
     click.option(
         "--post-version-spec",
         envvar="RH_POST_VERSION_SPEC",
         default="",
         help="The post release version (usually dev)",
     ),
     click.option(
         "--post-version-message",
         default="Bumped version to {post_version}",
         envvar="RH_POST_VERSION_MESSAGE",
         help="The post release message",
     ),
 ]
 
-version_cmd_options = [
+version_cmd_options: t.Any = [
     click.option("--version-cmd", envvar="RH_VERSION_COMMAND", help="The version command")
 ]
 
 
-branch_options = [
+branch_options: t.Any = [
     click.option("--ref", envvar="RH_REF", help="The source reference"),
     click.option("--branch", envvar="RH_BRANCH", help="The target branch"),
     click.option("--repo", envvar="RH_REPOSITORY", help="The git repo"),
 ]
 
-auth_options = [
+auth_options: t.Any = [
     click.option("--auth", envvar="GITHUB_ACCESS_TOKEN", help="The GitHub auth token"),
 ]
 
-username_options = [click.option("--username", envvar="GITHUB_ACTOR", help="The git username")]
+username_options: t.Any = [
+    click.option("--username", envvar="GITHUB_ACTOR", help="The git username")
+]
 
-dist_dir_options = [
+dist_dir_options: t.Any = [
     click.option(
         "--dist-dir",
         envvar="RH_DIST_DIR",
         default="dist",
         help="The folder to use for dist files",
     )
 ]
 
-python_packages_options = [
+python_packages_options: t.Any = [
     click.option(
         "--python-packages",
         envvar="RH_PYTHON_PACKAGES",
         default=["."],
         multiple=True,
         help='The list of strings of the form "path_to_package:name_of_package"',
     )
 ]
 
-check_imports_options = [
+check_imports_options: t.Any = [
     click.option(
         "--check-imports",
         envvar="RH_CHECK_IMPORTS",
         default=[],
         multiple=True,
         help="The Python packages import to check for; default to the Python package name.",
     )
 ]
 
-dry_run_options = [
+dry_run_options: t.Any = [
     click.option("--dry-run", is_flag=True, envvar="RH_DRY_RUN", help="Run as a dry run")
 ]
 
 
-git_url_options = [click.option("--git-url", help="A custom url for the git repository")]
+git_url_options: t.Any = [click.option("--git-url", help="A custom url for the git repository")]
 
 
-release_url_options = [
+release_url_options: t.Any = [
     click.option("--release-url", envvar="RH_RELEASE_URL", help="A draft GitHub release url")
 ]
 
 
-changelog_path_options = [
+changelog_path_options: t.Any = [
     click.option(
         "--changelog-path",
         envvar="RH_CHANGELOG",
         default="CHANGELOG.md",
         help="The path to changelog file",
     ),
 ]
 
-since_options = [
+since_options: t.Any = [
     click.option(
         "--since",
         envvar="RH_SINCE",
         default=None,
         help="Use PRs with activity since this date or git reference",
     ),
     click.option(
         "--since-last-stable",
         is_flag=True,
         envvar="RH_SINCE_LAST_STABLE",
         help="Use PRs with activity since the last stable git tag",
     ),
 ]
 
-changelog_options = (
+changelog_options: t.Any = (
     branch_options
     + auth_options
     + changelog_path_options
     + since_options
     + [
         click.option(
             "--resolve-backports",
             envvar="RH_RESOLVE_BACKPORTS",
             default=True,
             help="Resolve backport PRs to their originals",
         ),
     ]
 )
 
-npm_install_options = [
+npm_install_options: t.Any = [
     click.option(
         "--npm-install-options",
         envvar="RH_NPM_INSTALL_OPTIONS",
         default="",
         help="Options to pass when calling npm install",
     )
 ]
 
-pydist_check_options = [
+pydist_check_options: t.Any = [
     click.option(
         "--pydist-check-cmd",
         envvar="RH_PYDIST_CHECK_CMD",
         default="pipx run twine check --strict {dist_file}",
         help="The command to use to check a python distribution file",
     ),
     click.option(
```

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/lib.py` & `jupyter_releaser-1.2.1/jupyter_releaser/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     repo = repo or util.get_repo()
     branch = branch or util.get_branch()
 
     # Make a new branch with a uuid suffix
     pr_branch = f"changelog-{uuid.uuid1().hex}"
 
     if not dry_run:
-        dirty = util.run("git --no-pager diff --stat") != ""  # noqa
+        dirty = util.run("git --no-pager diff --stat") != ""
         if dirty:
             util.run("git stash")
         util.run(f"{util.GIT_FETCH_CMD} {branch}")
         util.run(f"git checkout -b {pr_branch} origin/{branch}")
         if dirty:
             util.run("git stash apply")
```

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/mock_github.py` & `jupyter_releaser-1.2.1/jupyter_releaser/mock_github.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,18 @@
 def write_to_file(name, data):
     """Write model data to a file."""
     source_file = os.path.join(static_dir, name + ".json")
     result = {}
     for key in data:
         value = data[key]
         if isinstance(value, BaseModel):
-            value = json.loads(value.json())
+            if hasattr(value, 'model_dump_json'):
+                value = json.loads(value.model_dump_json())
+            else:
+                value = json.loads(value.json())
         result[key] = value
     with open(source_file, "w") as fid:
         json.dump(result, fid)
 
 
 class Asset(BaseModel):
     """An asset model."""
@@ -141,15 +144,15 @@
     """https://docs.github.com/en/rest/releases/releases#list-releases"""
     return list(releases.values())
 
 
 @app.post("/repos/{owner}/{repo}/releases")
 async def create_a_release(owner: str, repo: str, request: Request) -> Release:
     """https://docs.github.com/en/rest/releases/releases#create-a-release"""
-    release_id = uuid.uuid4().int
+    release_id = uuid.uuid4().int % (2**32 - 1)
     data = await request.json()
     base_url = get_mock_github_url()
     url = f"{base_url}/repos/{owner}/{repo}/releases/{release_id}"
     html_url = f"{base_url}/{owner}/{repo}/releases/tag/{data['tag_name']}"
     upload_url = f"{base_url}/repos/{owner}/{repo}/releases/{release_id}/assets"
     fmt_str = r"%Y-%m-%dT%H:%M:%SZ"
     created_at = datetime.now(tz=timezone.utc).strftime(fmt_str)
@@ -179,15 +182,15 @@
 
 
 @app.post("/repos/{owner}/{repo}/releases/{release_id}/assets")
 async def upload_a_release_asset(owner: str, repo: str, release_id: int, request: Request) -> None:
     """https://docs.github.com/en/rest/releases/assets#upload-a-release-asset"""
     base_url = get_mock_github_url()
     model = releases[str(release_id)]
-    asset_id = uuid.uuid4().int
+    asset_id = uuid.uuid4().int % (2**32 - 1)
     name = request.query_params["name"]
     with open(f"{static_dir}/{asset_id}", "wb") as fid:
         async for chunk in request.stream():
             fid.write(chunk)
     headers = request.headers
     url = f"{base_url}/static/{asset_id}"
     asset = Asset(
@@ -238,15 +241,19 @@
     write_to_file("pulls", pulls)
     return pull
 
 
 @app.post("/repos/{owner}/{repo}/issues/{issue_number}/labels")
 def add_labels_to_an_issue(owner: str, repo: str, issue_number: int) -> BaseModel:
     """https://docs.github.com/en/rest/issues/labels#add-labels-to-an-issue"""
-    return BaseModel()
+
+    class _Inner(BaseModel):
+        pass
+
+    return _Inner()
 
 
 @app.post("/repos/{owner}/{repo}/git/refs")
 async def create_tag_ref(owner: str, repo: str, request: Request) -> None:
     """https://docs.github.com/en/rest/git/refs#create-a-reference"""
     data = await request.json()
     tag_ref = data["ref"]
```

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/npm.py` & `jupyter_releaser-1.2.1/jupyter_releaser/npm.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/python.py` & `jupyter_releaser-1.2.1/jupyter_releaser/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         util.run(f"python -m venv {env_path}")
         util.run(f"{bin_path}/python -m pip install -q -U pip")
         util.run(f"{bin_path}/pip install -q {dist_file}")
         try:
             for cmd in test_commands:
                 util.run(f"{bin_path}/{cmd}")
         except CalledProcessError as e:
-            if test_cmd == "":  # noqa
+            if test_cmd == "":
                 util.log(
                     'You may need to set "check_imports" to appropriate Python package names in the config file.'
                 )
             raise e
         for resource_path in resource_paths:
             name, _, _ = resource_path.partition("/")
             test_file = Path(td) / "test_path.py"
```

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/schema.json` & `jupyter_releaser-1.2.1/jupyter_releaser/schema.json`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/tee.py` & `jupyter_releaser-1.2.1/jupyter_releaser/tee.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/util.py` & `jupyter_releaser-1.2.1/jupyter_releaser/util.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/actions/common.py` & `jupyter_releaser-1.2.1/jupyter_releaser/actions/common.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/actions/generate_changelog.py` & `jupyter_releaser-1.2.1/jupyter_releaser/actions/generate_changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/actions/populate_release.py` & `jupyter_releaser-1.2.1/jupyter_releaser/actions/populate_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/actions/prep_release.py` & `jupyter_releaser-1.2.1/jupyter_releaser/actions/prep_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/tests/conftest.py` & `jupyter_releaser-1.2.1/jupyter_releaser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/tests/test_cli.py` & `jupyter_releaser-1.2.1/jupyter_releaser/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/tests/test_functions.py` & `jupyter_releaser-1.2.1/jupyter_releaser/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/tests/test_mock_github.py` & `jupyter_releaser-1.2.1/jupyter_releaser/tests/test_mock_github.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/jupyter_releaser/tests/util.py` & `jupyter_releaser-1.2.1/jupyter_releaser/tests/util.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/.gitignore` & `jupyter_releaser-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/LICENSE` & `jupyter_releaser-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/README.md` & `jupyter_releaser-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.2.0/pyproject.toml` & `jupyter_releaser-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 test = "mypy --install-types --non-interactive {args:jupyter_releaser}"
 
 [tool.hatch.envs.lint]
 dependencies = [
   "black==23.3.0",
   "mdformat>0.7",
   "mdformat-gfm>=0.3.5",
-  "ruff==0.0.270"
+  "ruff==0.0.276"
 ]
 detached = true
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs *.md}"
```

### Comparing `jupyter_releaser-1.2.0/PKG-INFO` & `jupyter_releaser-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_releaser
-Version: 1.2.0
+Version: 1.2.1
 Summary: Jupyter Releaser for Python and/or npm packages.
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: Copyright (c) 2021 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

