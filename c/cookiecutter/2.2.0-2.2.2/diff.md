# Comparing `tmp/cookiecutter-2.2.0.tar.gz` & `tmp/cookiecutter-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter-2.2.0.tar", last modified: Thu Jul  6 16:27:19 2023, max compression
+gzip compressed data, was "cookiecutter-2.2.2.tar", last modified: Mon Jul 10 13:27:00 2023, max compression
```

## Comparing `cookiecutter-2.2.0.tar` & `cookiecutter-2.2.2.tar`

### file list

```diff
@@ -1,341 +1,341 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.105624 cookiecutter-2.2.0/
--rw-r--r--   0 ericof     (501) staff       (20)    11796 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/AUTHORS.md
--rw-r--r--   0 ericof     (501) staff       (20)      326 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 ericof     (501) staff       (20)    12666 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/CONTRIBUTING.md
--rw-r--r--   0 ericof     (501) staff       (20)    72699 2023-07-06 16:16:26.000000 cookiecutter-2.2.0/HISTORY.md
--rw-r--r--   0 ericof     (501) staff       (20)     1493 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/LICENSE
--rw-r--r--   0 ericof     (501) staff       (20)      376 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)    12922 2023-07-06 16:27:19.105738 cookiecutter-2.2.0/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)    11356 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/README.md
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.019796 cookiecutter-2.2.0/cookiecutter/
--rw-r--r--   0 ericof     (501) staff       (20)       64 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      194 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/__main__.py
--rw-r--r--   0 ericof     (501) staff       (20)     7319 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/cli.py
--rw-r--r--   0 ericof     (501) staff       (20)     4250 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/config.py
--rw-r--r--   0 ericof     (501) staff       (20)     2280 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/cookiecutter/environment.py
--rw-r--r--   0 ericof     (501) staff       (20)     3886 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/exceptions.py
--rw-r--r--   0 ericof     (501) staff       (20)     3957 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/cookiecutter/extensions.py
--rw-r--r--   0 ericof     (501) staff       (20)      909 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/find.py
--rw-r--r--   0 ericof     (501) staff       (20)    15885 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/cookiecutter/generate.py
--rw-r--r--   0 ericof     (501) staff       (20)     4230 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/hooks.py
--rw-r--r--   0 ericof     (501) staff       (20)     1568 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/log.py
--rw-r--r--   0 ericof     (501) staff       (20)     6092 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/cookiecutter/main.py
--rw-r--r--   0 ericof     (501) staff       (20)     9324 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/cookiecutter/prompt.py
--rw-r--r--   0 ericof     (501) staff       (20)     1465 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/replay.py
--rw-r--r--   0 ericof     (501) staff       (20)     4237 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/repository.py
--rw-r--r--   0 ericof     (501) staff       (20)     3173 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/utils.py
--rw-r--r--   0 ericof     (501) staff       (20)     4382 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/vcs.py
--rw-r--r--   0 ericof     (501) staff       (20)     4451 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/zipfile.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.024893 cookiecutter-2.2.0/cookiecutter.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)    12922 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)    11578 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)       60 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-13 08:11:02.000000 cookiecutter-2.2.0/cookiecutter.egg-info/not-zip-safe
--rw-r--r--   0 ericof     (501) staff       (20)      115 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/top_level.txt
--rw-r--r--   0 ericof     (501) staff       (20)      161 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)      225 2023-07-06 16:27:19.106110 cookiecutter-2.2.0/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2405 2023-07-06 16:27:10.000000 cookiecutter-2.2.0/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.053549 cookiecutter-2.2.0/tests/
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     7329 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/conftest.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.053959 cookiecutter-2.2.0/tests/fake-nested-templates/
--rw-r--r--   0 ericof     (501) staff       (20)       58 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-nested-templates/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.054426 cookiecutter-2.2.0/tests/fake-nested-templates/fake-project/
--rw-r--r--   0 ericof     (501) staff       (20)        3 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-nested-templates/fake-project/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.054884 cookiecutter-2.2.0/tests/fake-repo/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.065236 cookiecutter-2.2.0/tests/fake-repo/fake-project/
--rw-r--r--   0 ericof     (501) staff       (20)       49 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo/fake-project/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.055105 cookiecutter-2.2.0/tests/fake-repo-bad/
--rw-r--r--   0 ericof     (501) staff       (20)       10 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/fake-repo-bad/no-project-in-here.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.055691 cookiecutter-2.2.0/tests/fake-repo-bad-json/
--rw-r--r--   0 ericof     (501) staff       (20)       33 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-bad-json/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.056021 cookiecutter-2.2.0/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/
--rw-r--r--   0 ericof     (501) staff       (20)      100 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.056570 cookiecutter-2.2.0/tests/fake-repo-dict/
--rw-r--r--   0 ericof     (501) staff       (20)      319 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-repo-dict/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.056849 cookiecutter-2.2.0/tests/fake-repo-dict/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)      353 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-dict/{{cookiecutter.project_slug}}/README.md
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.002222 cookiecutter-2.2.0/tests/fake-repo-dir/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.057776 cookiecutter-2.2.0/tests/fake-repo-dir/my-dir/
--rw-r--r--   0 ericof     (501) staff       (20)      289 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-repo-dir/my-dir/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.058219 cookiecutter-2.2.0/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/
--rw-r--r--   0 ericof     (501) staff       (20)      100 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.058389 cookiecutter-2.2.0/tests/fake-repo-pre/
--rw-r--r--   0 ericof     (501) staff       (20)      289 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-repo-pre/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.062090 cookiecutter-2.2.0/tests/fake-repo-pre/{{cookiecutter.repo_name}}/
--rw-r--r--   0 ericof     (501) staff       (20)      100 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-pre/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.062531 cookiecutter-2.2.0/tests/fake-repo-pre2/
--rw-r--r--   0 ericof     (501) staff       (20)      289 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-repo-pre2/cookiecutter.json
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-pre2/whatever.some.thing
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.062644 cookiecutter-2.2.0/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/
--rw-r--r--   0 ericof     (501) staff       (20)       49 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.062806 cookiecutter-2.2.0/tests/fake-repo-tmpl/
--rw-r--r--   0 ericof     (501) staff       (20)      342 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-repo-tmpl/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.065049 cookiecutter-2.2.0/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/
--rw-r--r--   0 ericof     (501) staff       (20)       49 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.064579 cookiecutter-2.2.0/tests/fake-repo-tmpl-_cookiecutter/
--rw-r--r--   0 ericof     (501) staff       (20)      430 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/fake-repo-tmpl-_cookiecutter/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.064858 cookiecutter-2.2.0/tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/
--rw-r--r--   0 ericof     (501) staff       (20)       49 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.071357 cookiecutter-2.2.0/tests/files/
--rw-r--r--   0 ericof     (501) staff       (20)       28 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/bad-zip-file.zip
--rw-r--r--   0 ericof     (501) staff       (20)       22 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/empty.zip
--rw-r--r--   0 ericof     (501) staff       (20)      994 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/fake-repo-tmpl.zip
--rw-r--r--   0 ericof     (501) staff       (20)      206 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/not-a-repo.zip
--rw-r--r--   0 ericof     (501) staff       (20)     1114 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/protected-fake-repo-tmpl.zip
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/files/syntax_error.txt
--rw-r--r--   0 ericof     (501) staff       (20)       89 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/files/unicode.txt
--rw-r--r--   0 ericof     (501) staff       (20)       64 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/files/{% if cookiecutter.generate_file == 'y' %}cheese.txt{% endif %}
--rw-r--r--   0 ericof     (501) staff       (20)       41 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/files/{{cookiecutter.generate_file}}.txt
--rw-r--r--   0 ericof     (501) staff       (20)       51 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/{{cookiecutter.generate_file}}_crlf_newlines.txt
--rw-r--r--   0 ericof     (501) staff       (20)       28 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/{{cookiecutter.generate_file}}_lf_newlines.txt
--rw-r--r--   0 ericof     (501) staff       (20)       29 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/{{cookiecutter.jsonify_file}}.txt
--rw-r--r--   0 ericof     (501) staff       (20)       47 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/{{cookiecutter.random_string_file}}.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.003216 cookiecutter-2.2.0/tests/hooks-abort-render/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.072659 cookiecutter-2.2.0/tests/hooks-abort-render/hooks/
--rw-r--r--   0 ericof     (501) staff       (20)      199 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/hooks-abort-render/hooks/post_gen_project.py
--rw-r--r--   0 ericof     (501) staff       (20)      197 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/hooks-abort-render/hooks/pre_gen_project.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.072948 cookiecutter-2.2.0/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/
--rw-r--r--   0 ericof     (501) staff       (20)       52 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.074524 cookiecutter-2.2.0/tests/replay/
--rw-r--r--   0 ericof     (501) staff       (20)      670 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/replay/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     3357 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/replay/test_dump.py
--rw-r--r--   0 ericof     (501) staff       (20)     1881 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/replay/test_load.py
--rw-r--r--   0 ericof     (501) staff       (20)     2304 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/replay/test_replay.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.076827 cookiecutter-2.2.0/tests/repository/
--rw-r--r--   0 ericof     (501) staff       (20)     1837 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_abbreviation_expansion.py
--rw-r--r--   0 ericof     (501) staff       (20)     3221 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_clones_repo.py
--rw-r--r--   0 ericof     (501) staff       (20)     1294 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py
--rw-r--r--   0 ericof     (501) staff       (20)     2389 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_finds_subdirectories.py
--rw-r--r--   0 ericof     (501) staff       (20)     2032 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_determine_repository_should_use_local_repo.py
--rw-r--r--   0 ericof     (501) staff       (20)     2229 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_is_repo_url.py
--rw-r--r--   0 ericof     (501) staff       (20)      606 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_repository_has_cookiecutter_json.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.078379 cookiecutter-2.2.0/tests/test-config/
--rw-r--r--   0 ericof     (501) staff       (20)       62 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-config/config-expand-user.yaml
--rw-r--r--   0 ericof     (501) staff       (20)       76 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-config/config-expand-vars.yaml
--rw-r--r--   0 ericof     (501) staff       (20)      162 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-config/invalid-config.yaml
--rw-r--r--   0 ericof     (501) staff       (20)      440 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-config/valid-config.yaml
--rw-r--r--   0 ericof     (501) staff       (20)      126 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-config/valid-partial-config.yaml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.004467 cookiecutter-2.2.0/tests/test-extensions/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.078554 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/
--rw-r--r--   0 ericof     (501) staff       (20)      111 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.078958 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/hooks/
--rw-r--r--   0 ericof     (501) staff       (20)      199 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/hooks/post_gen_project.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.079689 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)       30 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.080129 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/
--rw-r--r--   0 ericof     (501) staff       (20)      111 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.080442 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/hooks/
--rw-r--r--   0 ericof     (501) staff       (20)      198 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/hooks/pre_gen_project.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.080729 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)       30 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.080974 cookiecutter-2.2.0/tests/test-extensions/default/
--rw-r--r--   0 ericof     (501) staff       (20)      103 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-extensions/default/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.081597 cookiecutter-2.2.0/tests/test-extensions/default/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)       92 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/default/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 ericof     (501) staff       (20)       14 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-extensions/default/{{cookiecutter.project_slug}}/id
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.082259 cookiecutter-2.2.0/tests/test-extensions/hello_extension/
--rw-r--r--   0 ericof     (501) staff       (20)       23 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/hello_extension/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      786 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/hello_extension/hello_extension.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.082536 cookiecutter-2.2.0/tests/test-extensions/local_extension/
--rw-r--r--   0 ericof     (501) staff       (20)      298 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-extensions/local_extension/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.083011 cookiecutter-2.2.0/tests/test-extensions/local_extension/local_extensions/
--rw-r--r--   0 ericof     (501) staff       (20)       65 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/local_extension/local_extensions/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      548 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/local_extension/local_extensions/main.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.083214 cookiecutter-2.2.0/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)      139 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/HISTORY.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.083429 cookiecutter-2.2.0/tests/test-extensions/unknown/
--rw-r--r--   0 ericof     (501) staff       (20)      121 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-extensions/unknown/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.083826 cookiecutter-2.2.0/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)      119 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/HISTORY.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.004748 cookiecutter-2.2.0/tests/test-generate-binaries/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.084702 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/
--rw-r--r--   0 ericof     (501) staff       (20)    15364 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store
--rw-r--r--   0 ericof     (501) staff       (20)     4381 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png
--rw-r--r--   0 ericof     (501) staff       (20)       37 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/readme.txt
--rwxr-xr-x   0 ericof     (501) staff       (20)    18116 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.085815 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
--rw-r--r--   0 ericof     (501) staff       (20)    12292 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store
--rw-r--r--   0 ericof     (501) staff       (20)     4381 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
--rw-r--r--   0 ericof     (501) staff       (20)       37 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/readme.txt
--rwxr-xr-x   0 ericof     (501) staff       (20)    18116 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.086068 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
--rw-r--r--   0 ericof     (501) staff       (20)     4381 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.087093 cookiecutter-2.2.0/tests/test-generate-context/
--rw-r--r--   0 ericof     (501) staff       (20)      227 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-generate-context/choices_template.json
--rw-r--r--   0 ericof     (501) staff       (20)       33 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-context/invalid-syntax.json
--rw-r--r--   0 ericof     (501) staff       (20)      287 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-generate-context/nested_dict.json
--rw-r--r--   0 ericof     (501) staff       (20)       28 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-generate-context/non_ascii.json
--rw-r--r--   0 ericof     (501) staff       (20)       39 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-generate-context/test.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.005914 cookiecutter-2.2.0/tests/test-generate-copy-without-render/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.089847 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/
--rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.rst
--rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.090030 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/
--rw-r--r--   0 ericof     (501) staff       (20)       41 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.090637 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
--rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.091634 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
--rw-r--r--   0 ericof     (501) staff       (20)       45 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
--rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
--rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.005406 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.087567 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/
--rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.rst
--rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.088279 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/
--rw-r--r--   0 ericof     (501) staff       (20)       41 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.088587 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
--rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.089271 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
--rw-r--r--   0 ericof     (501) staff       (20)       45 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
--rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
--rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.007456 cookiecutter-2.2.0/tests/test-generate-files/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.094006 cookiecutter-2.2.0/tests/test-generate-files/input{{cookiecutter.food}}/
--rw-r--r--   0 ericof     (501) staff       (20)      111 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-conditions.txt
--rw-r--r--   0 ericof     (501) staff       (20)       51 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline-crlf.txt
--rw-r--r--   0 ericof     (501) staff       (20)       28 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline.txt
--rw-r--r--   0 ericof     (501) staff       (20)       30 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-generate-files/input{{cookiecutter.food}}/simple.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.091992 cookiecutter-2.2.0/tests/test-generate-files-line-end/
--rw-r--r--   0 ericof     (501) staff       (20)      183 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-generate-files-line-end/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.092290 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.092484 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/
--rw-r--r--   0 ericof     (501) staff       (20)       83 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/in_folder.txt
--rw-r--r--   0 ericof     (501) staff       (20)       76 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/something.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.092693 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
--rw-r--r--   0 ericof     (501) staff       (20)      125 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.007148 cookiecutter-2.2.0/tests/test-generate-files-nontemplated/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.092891 cookiecutter-2.2.0/tests/test-generate-files-nontemplated/input/
--rw-r--r--   0 ericof     (501) staff       (20)       17 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-generate-files-nontemplated/input/simple.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.007291 cookiecutter-2.2.0/tests/test-generate-files-permissions/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.093284 cookiecutter-2.2.0/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/
--rwxr-xr-x   0 ericof     (501) staff       (20)       32 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/script.sh
--rw-r--r--   0 ericof     (501) staff       (20)       17 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/simple.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.094164 cookiecutter-2.2.0/tests/test-output-folder/
--rw-r--r--   0 ericof     (501) staff       (20)      181 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-output-folder/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.094381 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.094644 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/folder/
--rw-r--r--   0 ericof     (501) staff       (20)       83 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/folder/in_folder.txt
--rw-r--r--   0 ericof     (501) staff       (20)       76 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/something.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.094859 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
--rw-r--r--   0 ericof     (501) staff       (20)      128 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.008051 cookiecutter-2.2.0/tests/test-pyhooks/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.095196 cookiecutter-2.2.0/tests/test-pyhooks/hooks/
--rw-r--r--   0 ericof     (501) staff       (20)      153 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyhooks/hooks/post_gen_project.py
--rw-r--r--   0 ericof     (501) staff       (20)      151 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyhooks/hooks/pre_gen_project.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.095344 cookiecutter-2.2.0/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.008295 cookiecutter-2.2.0/tests/test-pyshellhooks/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.095908 cookiecutter-2.2.0/tests/test-pyshellhooks/hooks/
--rw-r--r--   0 ericof     (501) staff       (20)      153 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyshellhooks/hooks/post_gen_project.py
--rwxr-xr-x   0 ericof     (501) staff       (20)       65 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyshellhooks/hooks/post_gen_project.sh
--rw-r--r--   0 ericof     (501) staff       (20)      152 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyshellhooks/hooks/pre_gen_project.py
--rwxr-xr-x   0 ericof     (501) staff       (20)       64 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyshellhooks/hooks/pre_gen_project.sh
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.096086 cookiecutter-2.2.0/tests/test-pyshellhooks/input{{pyshellhooks}}/
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyshellhooks/input{{pyshellhooks}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.096453 cookiecutter-2.2.0/tests/test-replay/
--rw-r--r--   0 ericof     (501) staff       (20)      161 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-replay/cookiedozer_load.json
--rw-r--r--   0 ericof     (501) staff       (20)      165 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-replay/invalid_replay.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.009154 cookiecutter-2.2.0/tests/test-shellhooks/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.098322 cookiecutter-2.2.0/tests/test-shellhooks/hooks/
--rwxr-xr-x   0 ericof     (501) staff       (20)       65 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks/hooks/post_gen_project.sh
--rwxr-xr-x   0 ericof     (501) staff       (20)       63 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks/hooks/pre_gen_project.sh
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.098529 cookiecutter-2.2.0/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.008595 cookiecutter-2.2.0/tests/test-shellhooks-empty/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.096652 cookiecutter-2.2.0/tests/test-shellhooks-empty/hooks/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks-empty/hooks/pre_gen_project.sh
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.096784 cookiecutter-2.2.0/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/
--rw-r--r--   0 ericof     (501) staff       (20)       43 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.008984 cookiecutter-2.2.0/tests/test-shellhooks-win/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.097392 cookiecutter-2.2.0/tests/test-shellhooks-win/hooks/
--rw-r--r--   0 ericof     (501) staff       (20)       59 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks-win/hooks/post_gen_project.bat
--rw-r--r--   0 ericof     (501) staff       (20)       57 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks-win/hooks/pre_gen_project.bat
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.097637 cookiecutter-2.2.0/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.009776 cookiecutter-2.2.0/tests/test-templates/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.098741 cookiecutter-2.2.0/tests/test-templates/extends/
--rw-r--r--   0 ericof     (501) staff       (20)       89 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-templates/extends/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.099398 cookiecutter-2.2.0/tests/test-templates/extends/templates/
--rw-r--r--   0 ericof     (501) staff       (20)      252 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/extends/templates/base-requirements.jinja
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/extends/templates/click-requirements.jinja
--rw-r--r--   0 ericof     (501) staff       (20)        7 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/extends/templates/pytest-requirements.jinja
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.099598 cookiecutter-2.2.0/tests/test-templates/extends/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)       40 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/extends/{{cookiecutter.project_slug}}/requirements.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.099920 cookiecutter-2.2.0/tests/test-templates/include/
--rw-r--r--   0 ericof     (501) staff       (20)       89 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-templates/include/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.100736 cookiecutter-2.2.0/tests/test-templates/include/templates/
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/include/templates/click-requirements.jinja
--rw-r--r--   0 ericof     (501) staff       (20)        7 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/include/templates/pytest-requirements.jinja
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.101060 cookiecutter-2.2.0/tests/test-templates/include/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)      213 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/include/{{cookiecutter.project_slug}}/requirements.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.101459 cookiecutter-2.2.0/tests/test-templates/no-templates/
--rw-r--r--   0 ericof     (501) staff       (20)       89 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-templates/no-templates/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.101687 cookiecutter-2.2.0/tests/test-templates/no-templates/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)      143 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/no-templates/{{cookiecutter.project_slug}}/requirements.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.101919 cookiecutter-2.2.0/tests/test-templates/super/
--rw-r--r--   0 ericof     (501) staff       (20)       89 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-templates/super/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.102726 cookiecutter-2.2.0/tests/test-templates/super/templates/
--rw-r--r--   0 ericof     (501) staff       (20)      297 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/super/templates/base-requirements.jinja
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/super/templates/click-requirements.jinja
--rw-r--r--   0 ericof     (501) staff       (20)        7 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/super/templates/pytest-requirements.jinja
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.102971 cookiecutter-2.2.0/tests/test-templates/super/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)       96 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/super/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 ericof     (501) staff       (20)     1203 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_abort_generate_on_hook_error.py
--rw-r--r--   0 ericof     (501) staff       (20)    20303 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_cli.py
--rw-r--r--   0 ericof     (501) staff       (20)      897 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_cookiecutter_invocation.py
--rw-r--r--   0 ericof     (501) staff       (20)     4558 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_cookiecutter_local_no_input.py
--rw-r--r--   0 ericof     (501) staff       (20)     1681 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_cookiecutter_local_with_input.py
--rw-r--r--   0 ericof     (501) staff       (20)      527 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_cookiecutter_nested_templates.py
--rw-r--r--   0 ericof     (501) staff       (20)     1256 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_custom_extensions_in_hooks.py
--rw-r--r--   0 ericof     (501) staff       (20)     1849 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_default_extensions.py
--rw-r--r--   0 ericof     (501) staff       (20)     1071 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test_environment.py
--rw-r--r--   0 ericof     (501) staff       (20)      712 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_exceptions.py
--rw-r--r--   0 ericof     (501) staff       (20)      555 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_find.py
--rw-r--r--   0 ericof     (501) staff       (20)     8477 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_generate_context.py
--rw-r--r--   0 ericof     (501) staff       (20)     2499 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_generate_copy_without_render.py
--rw-r--r--   0 ericof     (501) staff       (20)     3129 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_generate_copy_without_render_override.py
--rw-r--r--   0 ericof     (501) staff       (20)     6102 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_generate_file.py
--rw-r--r--   0 ericof     (501) staff       (20)    15950 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_generate_files.py
--rw-r--r--   0 ericof     (501) staff       (20)     8141 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_generate_hooks.py
--rw-r--r--   0 ericof     (501) staff       (20)     4396 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_get_config.py
--rw-r--r--   0 ericof     (501) staff       (20)     5403 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_get_user_config.py
--rw-r--r--   0 ericof     (501) staff       (20)    10502 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_hooks.py
--rw-r--r--   0 ericof     (501) staff       (20)     3957 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_log.py
--rw-r--r--   0 ericof     (501) staff       (20)     3117 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_main.py
--rw-r--r--   0 ericof     (501) staff       (20)     1918 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_output_folder.py
--rw-r--r--   0 ericof     (501) staff       (20)      847 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_preferred_encoding.py
--rw-r--r--   0 ericof     (501) staff       (20)    19445 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_prompt.py
--rw-r--r--   0 ericof     (501) staff       (20)      480 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_read_repo_password.py
--rw-r--r--   0 ericof     (501) staff       (20)     1233 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_read_user_choice.py
--rw-r--r--   0 ericof     (501) staff       (20)     3628 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_read_user_dict.py
--rw-r--r--   0 ericof     (501) staff       (20)      498 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_read_user_variable.py
--rw-r--r--   0 ericof     (501) staff       (20)      524 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_read_user_yes_no.py
--rw-r--r--   0 ericof     (501) staff       (20)      367 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_repo_not_found.py
--rw-r--r--   0 ericof     (501) staff       (20)     2323 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_specify_output_dir.py
--rw-r--r--   0 ericof     (501) staff       (20)      933 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_templates.py
--rw-r--r--   0 ericof     (501) staff       (20)     2439 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test_time_extension.py
--rw-r--r--   0 ericof     (501) staff       (20)     6791 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_utils.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.010313 cookiecutter-2.2.0/tests/undefined-variable/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.010071 cookiecutter-2.2.0/tests/undefined-variable/dir-name/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.103236 cookiecutter-2.2.0/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)       84 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.103587 cookiecutter-2.2.0/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/
--rw-r--r--   0 ericof     (501) staff       (20)      121 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/helloworld.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.010251 cookiecutter-2.2.0/tests/undefined-variable/file-content/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.103906 cookiecutter-2.2.0/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)      192 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.104180 cookiecutter-2.2.0/tests/undefined-variable/file-name/
--rw-r--r--   0 ericof     (501) staff       (20)       70 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/undefined-variable/file-name/cookiecutter.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.104396 cookiecutter-2.2.0/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/
--rw-r--r--   0 ericof     (501) staff       (20)       84 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.105185 cookiecutter-2.2.0/tests/vcs/
--rw-r--r--   0 ericof     (501) staff       (20)     7144 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/vcs/test_clone.py
--rw-r--r--   0 ericof     (501) staff       (20)     2573 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/vcs/test_identify_repo.py
--rw-r--r--   0 ericof     (501) staff       (20)      500 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/vcs/test_is_vcs_installed.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.105373 cookiecutter-2.2.0/tests/zipfile/
--rw-r--r--   0 ericof     (501) staff       (20)     9611 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/zipfile/test_unzip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.938853 cookiecutter-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    72932 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-07-10 13:27:00.938853 cookiecutter-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.886849 cookiecutter-2.2.2/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/zipfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.886849 cookiecutter-2.2.2/cookiecutter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-10 13:27:00.938853 cookiecutter-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-nested-templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-nested-templates/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-nested-templates/fake-project/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-nested-templates/fake-project/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo/fake-project/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo/fake-project/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-bad/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-bad/no-project-in-here.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-bad-json/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-bad-json/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-dict/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-dict/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-dict/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-dict/{{cookiecutter.project_slug}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.858847 cookiecutter-2.2.2/tests/fake-repo-dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-dir/my-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-dir/my-dir/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-pre/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-pre/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-pre/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-pre/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-pre2/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-pre2/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-pre2/whatever.some.thing
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo-tmpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-tmpl/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo-tmpl-_cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-tmpl-_cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.906851 cookiecutter-2.2.2/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/bad-zip-file.zip
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/empty.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/fake-repo-tmpl.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/not-a-repo.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/protected-fake-repo-tmpl.zip
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/syntax_error.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/unicode.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{% if cookiecutter.generate_file == 'y' %}cheese.txt{% endif %}
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{{cookiecutter.generate_file}}.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{{cookiecutter.generate_file}}_crlf_newlines.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{{cookiecutter.generate_file}}_lf_newlines.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{{cookiecutter.jsonify_file}}.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{{cookiecutter.random_string_file}}.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.862847 cookiecutter-2.2.2/tests/hooks-abort-render/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.906851 cookiecutter-2.2.2/tests/hooks-abort-render/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/hooks-abort-render/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/hooks-abort-render/hooks/pre_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.906851 cookiecutter-2.2.2/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.906851 cookiecutter-2.2.2/tests/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/replay/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/replay/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/replay/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/replay/test_replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_abbreviation_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_clones_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_finds_subdirectories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_determine_repository_should_use_local_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_is_repo_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_repository_has_cookiecutter_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-config/config-expand-user.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-config/config-expand-vars.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-config/invalid-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-config/valid-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-config/valid-partial-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.862847 cookiecutter-2.2.2/tests/test-extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/hooks/pre_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/default/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/default/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/default/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/default/{{cookiecutter.project_slug}}/id
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/hello_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/hello_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/hello_extension/hello_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/local_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/local_extension/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/local_extension/local_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/local_extension/local_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/local_extension/local_extensions/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/HISTORY.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/unknown/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/unknown/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/HISTORY.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.866847 cookiecutter-2.2.2/tests/test-generate-binaries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/
+-rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/readme.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18116 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/readme.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18116 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-context/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-context/choices_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-context/invalid-syntax.json
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-context/nested_dict.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-context/non_ascii.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-context/test.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.866847 cookiecutter-2.2.2/tests/test-generate-copy-without-render/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.866847 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-generate-files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-generate-files/input{{cookiecutter.food}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-conditions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline-crlf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files/input{{cookiecutter.food}}/simple.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-line-end/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-line-end/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/in_folder.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/something.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.866847 cookiecutter-2.2.2/tests/test-generate-files-nontemplated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-nontemplated/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-nontemplated/input/simple.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-generate-files-permissions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/script.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/simple.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-output-folder/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-output-folder/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/folder/in_folder.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/something.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-pyhooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-pyhooks/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyhooks/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyhooks/hooks/pre_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-pyshellhooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-pyshellhooks/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyshellhooks/hooks/post_gen_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyshellhooks/hooks/post_gen_project.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyshellhooks/hooks/pre_gen_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyshellhooks/hooks/pre_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-pyshellhooks/input{{pyshellhooks}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyshellhooks/input{{pyshellhooks}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-replay/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-replay/cookiedozer_load.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-replay/invalid_replay.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-shellhooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks/hooks/post_gen_project.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks/hooks/pre_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-shellhooks-empty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks-empty/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks-empty/hooks/pre_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-shellhooks-win/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks-win/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks-win/hooks/post_gen_project.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks-win/hooks/pre_gen_project.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.874848 cookiecutter-2.2.2/tests/test-templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-templates/extends/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/extends/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-templates/extends/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/extends/templates/base-requirements.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/extends/templates/click-requirements.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/extends/templates/pytest-requirements.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/extends/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/extends/{{cookiecutter.project_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/include/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/include/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/include/templates/click-requirements.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/include/templates/pytest-requirements.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/include/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/include/{{cookiecutter.project_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/no-templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/no-templates/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/no-templates/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/no-templates/{{cookiecutter.project_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/super/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/super/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/super/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/super/templates/base-requirements.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/super/templates/click-requirements.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/super/templates/pytest-requirements.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/super/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/super/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_abort_generate_on_hook_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20303 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_cookiecutter_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_cookiecutter_local_no_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_cookiecutter_local_with_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_cookiecutter_nested_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_custom_extensions_in_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_default_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_copy_without_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_copy_without_render_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_get_user_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_output_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_preferred_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_read_repo_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_read_user_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_read_user_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_read_user_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_read_user_yes_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_repo_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_specify_output_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_time_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.874848 cookiecutter-2.2.2/tests/undefined-variable/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.874848 cookiecutter-2.2.2/tests/undefined-variable/dir-name/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.874848 cookiecutter-2.2.2/tests/undefined-variable/file-content/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/undefined-variable/file-name/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/undefined-variable/file-name/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.938853 cookiecutter-2.2.2/tests/vcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/vcs/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/vcs/test_identify_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/vcs/test_is_vcs_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.938853 cookiecutter-2.2.2/tests/zipfile/
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/zipfile/test_unzip.py
```

### Comparing `cookiecutter-2.2.0/AUTHORS.md` & `cookiecutter-2.2.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/CONTRIBUTING.md` & `cookiecutter-2.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/HISTORY.md` & `cookiecutter-2.2.2/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # History
 
 History is important, but our current roadmap can be found [here](https://github.com/cookiecutter/cookiecutter/projects)
 
+## 2.2.2 (2023-07-10)
+
+### CI/CD and QA changes
+
+* Improve gitignore (#1889) @audreyfeldroy
+* Add warning for jinja2_time (#1890) @henryiii
+
+### This release is made by wonderful contributors:
+
+@audreyfeldroy, @ericof and @henryiii
+
 
 ## 2.2.0 (2023-07-06)
 
 ### Changes
 
 * Added timeout on request.get() for ensuring that if a recipient serve… (#1772) @openrefactory
 * Fixing Carriage Return Line Feed (CRLF) order in docs #1792 (#1793) @Lahiry
```

### Comparing `cookiecutter-2.2.0/LICENSE` & `cookiecutter-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/PKG-INFO` & `cookiecutter-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter
-Version: 2.2.0
+Version: 2.2.2
 Summary: A command-line utility that creates projects from project templates, e.g. creating a Python package project from a Python package project template.
 Home-page: https://github.com/cookiecutter/cookiecutter
 Author: Audrey Feldroy
 Author-email: audreyr@gmail.com
 License: BSD
 Project-URL: Documentation, https://cookiecutter.readthedocs.io
 Project-URL: Issues, https://github.com/cookiecutter/cookiecutter/issues
```

### Comparing `cookiecutter-2.2.0/README.md` & `cookiecutter-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/cli.py` & `cookiecutter-2.2.2/cookiecutter/cli.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/config.py` & `cookiecutter-2.2.2/cookiecutter/config.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/environment.py` & `cookiecutter-2.2.2/cookiecutter/environment.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/exceptions.py` & `cookiecutter-2.2.2/cookiecutter/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/extensions.py` & `cookiecutter-2.2.2/cookiecutter/extensions.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/find.py` & `cookiecutter-2.2.2/cookiecutter/find.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/generate.py` & `cookiecutter-2.2.2/cookiecutter/generate.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/hooks.py` & `cookiecutter-2.2.2/cookiecutter/hooks.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/log.py` & `cookiecutter-2.2.2/cookiecutter/log.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/main.py` & `cookiecutter-2.2.2/cookiecutter/main.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/prompt.py` & `cookiecutter-2.2.2/cookiecutter/prompt.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/replay.py` & `cookiecutter-2.2.2/cookiecutter/replay.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/repository.py` & `cookiecutter-2.2.2/cookiecutter/repository.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/utils.py` & `cookiecutter-2.2.2/cookiecutter/utils.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/vcs.py` & `cookiecutter-2.2.2/cookiecutter/vcs.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter/zipfile.py` & `cookiecutter-2.2.2/cookiecutter/zipfile.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/cookiecutter.egg-info/PKG-INFO` & `cookiecutter-2.2.2/cookiecutter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter
-Version: 2.2.0
+Version: 2.2.2
 Summary: A command-line utility that creates projects from project templates, e.g. creating a Python package project from a Python package project template.
 Home-page: https://github.com/cookiecutter/cookiecutter
 Author: Audrey Feldroy
 Author-email: audreyr@gmail.com
 License: BSD
 Project-URL: Documentation, https://cookiecutter.readthedocs.io
 Project-URL: Issues, https://github.com/cookiecutter/cookiecutter/issues
```

### Comparing `cookiecutter-2.2.0/cookiecutter.egg-info/SOURCES.txt` & `cookiecutter-2.2.2/cookiecutter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/setup.py` & `cookiecutter-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """cookiecutter distutils configuration."""
 from setuptools import setup
 
-version = "2.2.0"
+version = "2.2.2"
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 requirements = [
     'binaryornot>=0.4.4',
     'Jinja2>=2.7,<4.0.0',
```

### Comparing `cookiecutter-2.2.0/tests/conftest.py` & `cookiecutter-2.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/files/fake-repo-tmpl.zip` & `cookiecutter-2.2.2/tests/files/fake-repo-tmpl.zip`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/files/protected-fake-repo-tmpl.zip` & `cookiecutter-2.2.2/tests/files/protected-fake-repo-tmpl.zip`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/replay/conftest.py` & `cookiecutter-2.2.2/tests/replay/conftest.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/replay/test_dump.py` & `cookiecutter-2.2.2/tests/replay/test_dump.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/replay/test_load.py` & `cookiecutter-2.2.2/tests/replay/test_load.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/replay/test_replay.py` & `cookiecutter-2.2.2/tests/replay/test_replay.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/repository/test_abbreviation_expansion.py` & `cookiecutter-2.2.2/tests/repository/test_abbreviation_expansion.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_clones_repo.py` & `cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_clones_repo.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py` & `cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_finds_subdirectories.py` & `cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_finds_subdirectories.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/repository/test_determine_repository_should_use_local_repo.py` & `cookiecutter-2.2.2/tests/repository/test_determine_repository_should_use_local_repo.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/repository/test_is_repo_url.py` & `cookiecutter-2.2.2/tests/repository/test_is_repo_url.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/repository/test_repository_has_cookiecutter_json.py` & `cookiecutter-2.2.2/tests/repository/test_repository_has_cookiecutter_json.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test-extensions/hello_extension/hello_extension.py` & `cookiecutter-2.2.2/tests/test-extensions/hello_extension/hello_extension.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test-extensions/local_extension/local_extensions/main.py` & `cookiecutter-2.2.2/tests/test-extensions/local_extension/local_extensions/main.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store` & `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png` & `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf` & `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store` & `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png` & `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf` & `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png` & `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_abort_generate_on_hook_error.py` & `cookiecutter-2.2.2/tests/test_abort_generate_on_hook_error.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_cli.py` & `cookiecutter-2.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_cookiecutter_invocation.py` & `cookiecutter-2.2.2/tests/test_cookiecutter_invocation.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_cookiecutter_local_no_input.py` & `cookiecutter-2.2.2/tests/test_cookiecutter_local_no_input.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_cookiecutter_local_with_input.py` & `cookiecutter-2.2.2/tests/test_cookiecutter_local_with_input.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_cookiecutter_nested_templates.py` & `cookiecutter-2.2.2/tests/test_cookiecutter_nested_templates.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_custom_extensions_in_hooks.py` & `cookiecutter-2.2.2/tests/test_custom_extensions_in_hooks.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_default_extensions.py` & `cookiecutter-2.2.2/tests/test_default_extensions.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_environment.py` & `cookiecutter-2.2.2/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_exceptions.py` & `cookiecutter-2.2.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_find.py` & `cookiecutter-2.2.2/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_generate_context.py` & `cookiecutter-2.2.2/tests/test_generate_context.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_generate_copy_without_render.py` & `cookiecutter-2.2.2/tests/test_generate_copy_without_render.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_generate_copy_without_render_override.py` & `cookiecutter-2.2.2/tests/test_generate_copy_without_render_override.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_generate_file.py` & `cookiecutter-2.2.2/tests/test_generate_file.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_generate_files.py` & `cookiecutter-2.2.2/tests/test_generate_files.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_generate_hooks.py` & `cookiecutter-2.2.2/tests/test_generate_hooks.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_get_config.py` & `cookiecutter-2.2.2/tests/test_get_config.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_get_user_config.py` & `cookiecutter-2.2.2/tests/test_get_user_config.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_hooks.py` & `cookiecutter-2.2.2/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_log.py` & `cookiecutter-2.2.2/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_main.py` & `cookiecutter-2.2.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_output_folder.py` & `cookiecutter-2.2.2/tests/test_output_folder.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_preferred_encoding.py` & `cookiecutter-2.2.2/tests/test_preferred_encoding.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_prompt.py` & `cookiecutter-2.2.2/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_read_user_choice.py` & `cookiecutter-2.2.2/tests/test_read_user_choice.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_read_user_dict.py` & `cookiecutter-2.2.2/tests/test_read_user_dict.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_read_user_yes_no.py` & `cookiecutter-2.2.2/tests/test_read_user_yes_no.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_specify_output_dir.py` & `cookiecutter-2.2.2/tests/test_specify_output_dir.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_templates.py` & `cookiecutter-2.2.2/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_time_extension.py` & `cookiecutter-2.2.2/tests/test_time_extension.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/test_utils.py` & `cookiecutter-2.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/vcs/test_clone.py` & `cookiecutter-2.2.2/tests/vcs/test_clone.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/vcs/test_identify_repo.py` & `cookiecutter-2.2.2/tests/vcs/test_identify_repo.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.0/tests/zipfile/test_unzip.py` & `cookiecutter-2.2.2/tests/zipfile/test_unzip.py`

 * *Files identical despite different names*

