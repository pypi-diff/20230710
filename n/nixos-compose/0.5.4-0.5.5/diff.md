# Comparing `tmp/nixos_compose-0.5.4.tar.gz` & `tmp/nixos_compose-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixos_compose-0.5.4.tar", max compression
+gzip compressed data, was "nixos_compose-0.5.5.tar", max compression
```

## Comparing `nixos_compose-0.5.4.tar` & `nixos_compose-0.5.5.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1094 2022-02-22 14:04:48.131501 nixos_compose-0.5.4/LICENSE
--rw-r--r--   0        0        0      216 2023-01-26 10:45:07.461353 nixos_compose-0.5.4/examples/basic/composition.nix
--rw-r--r--   0        0        0      561 2022-11-24 15:29:17.851309 nixos_compose-0.5.4/examples/basic/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.851309 nixos_compose-0.5.4/examples/basic/nxc.json
--rw-r--r--   0        0        0      216 2023-01-26 10:45:07.461353 nixos_compose-0.5.4/examples/basic-nur/composition.nix
--rw-r--r--   0        0        0     1043 2022-11-24 15:29:17.851309 nixos_compose-0.5.4/examples/basic-nur/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.851309 nixos_compose-0.5.4/examples/basic-nur/nxc.json
--rw-r--r--   0        0        0      214 2023-01-26 10:45:07.461353 nixos_compose-0.5.4/examples/execo/composition.nix
--rw-r--r--   0        0        0     2543 2022-03-05 16:55:24.727775 nixos_compose-0.5.4/examples/execo/execo_script.py
--rw-r--r--   0        0        0      963 2022-11-24 15:29:17.851309 nixos_compose-0.5.4/examples/execo/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.852309 nixos_compose-0.5.4/examples/execo/nxc.json
--rw-r--r--   0        0        0      569 2022-02-22 14:04:48.132501 nixos_compose-0.5.4/examples/flake.lock
--rw-r--r--   0        0        0       96 2022-02-22 14:04:48.132501 nixos_compose-0.5.4/examples/kernel/compositions.nix
--rw-r--r--   0        0        0      577 2022-11-24 15:29:17.852309 nixos_compose-0.5.4/examples/kernel/flake.nix
--rw-r--r--   0        0        0      200 2023-01-26 10:45:07.462353 nixos_compose-0.5.4/examples/kernel/linux_5_4.nix
--rw-r--r--   0        0        0      907 2023-01-26 10:45:07.462353 nixos_compose-0.5.4/examples/kernel/linux_ipanema_5_4.nix
--rw-r--r--   0        0        0       51 2022-02-22 14:04:48.132501 nixos_compose-0.5.4/examples/kernel/nxc.json
--rw-r--r--   0        0        0      132 2023-01-26 10:45:07.462353 nixos_compose-0.5.4/examples/multi-compositions/bar-composition.nix
--rw-r--r--   0        0        0       80 2022-02-22 14:04:48.132501 nixos_compose-0.5.4/examples/multi-compositions/compositions.nix
--rw-r--r--   0        0        0      571 2022-11-24 15:29:17.852309 nixos_compose-0.5.4/examples/multi-compositions/flake.nix
--rw-r--r--   0        0        0      132 2023-01-26 10:45:07.462353 nixos_compose-0.5.4/examples/multi-compositions/foo-composition.nix
--rw-r--r--   0        0        0       51 2022-02-22 14:04:48.132501 nixos_compose-0.5.4/examples/multi-compositions/nxc.json
--rw-r--r--   0        0        0      569 2022-12-07 13:41:00.974492 nixos_compose-0.5.4/examples/nbp-mpi/composition.nix
--rw-r--r--   0        0        0      807 2022-12-06 21:39:45.820352 nixos_compose-0.5.4/examples/nbp-mpi/flake.nix
--rw-r--r--   0        0        0       60 2022-12-06 21:41:04.858427 nixos_compose-0.5.4/examples/nbp-mpi/nxc.json
--rw-r--r--   0        0        0     1113 2022-12-13 15:48:10.081561 nixos_compose-0.5.4/examples/nix_flake_templates.nix
--rw-r--r--   0        0        0     2141 2023-01-26 10:45:07.462353 nixos_compose-0.5.4/examples/nixos-cluster/composition.nix
--rw-r--r--   0        0        0      703 2022-11-24 15:29:17.852309 nixos_compose-0.5.4/examples/nixos-cluster/flake.nix
--rw-r--r--   0        0        0       49 2022-06-14 14:20:20.160507 nixos_compose-0.5.4/examples/nixos-cluster/nodes.yaml
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.852309 nixos_compose-0.5.4/examples/nixos-cluster/nxc.json
--rw-r--r--   0        0        0     4455 2022-06-14 14:20:20.160507 nixos_compose-0.5.4/examples/nixos-cluster/ssh-keys.nix
--rw-r--r--   0        0        0      499 2023-01-26 10:45:07.462353 nixos_compose-0.5.4/examples/scripts/composition.nix
--rw-r--r--   0        0        0      563 2022-11-24 15:29:17.852309 nixos_compose-0.5.4/examples/scripts/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.4/examples/scripts/nxc.json
--rw-r--r--   0        0        0      484 2022-04-14 09:01:13.303530 nixos_compose-0.5.4/examples/scripts/scripts/scripts.nix
--rw-r--r--   0        0        0       83 2022-04-14 09:01:13.303530 nixos_compose-0.5.4/examples/scripts/scripts/test_python.py
--rw-r--r--   0        0        0      465 2023-01-26 10:45:07.462353 nixos_compose-0.5.4/examples/setup/composition.nix
--rw-r--r--   0        0        0      593 2022-11-24 15:29:17.853309 nixos_compose-0.5.4/examples/setup/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.4/examples/setup/nxc.json
--rw-r--r--   0        0        0     2917 2022-11-29 09:02:17.732640 nixos_compose-0.5.4/examples/setup/setup.toml
--rw-r--r--   0        0        0      691 2022-12-13 15:48:45.830622 nixos_compose-0.5.4/examples/shared-directories-users/composition.nix
--rw-r--r--   0        0        0      807 2022-12-06 21:39:45.820352 nixos_compose-0.5.4/examples/shared-directories-users/flake.nix
--rw-r--r--   0        0        0       60 2022-12-06 21:41:04.858427 nixos_compose-0.5.4/examples/shared-directories-users/nxc.json
--rw-r--r--   0        0        0      561 2022-11-24 15:29:17.853309 nixos_compose-0.5.4/examples/spark/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.4/examples/spark/nxc.json
--rw-r--r--   0        0        0     1321 2022-02-22 14:04:48.133501 nixos_compose-0.5.4/examples/spark/spark_sample.py
--rw-r--r--   0        0        0      600 2023-01-26 10:45:07.462353 nixos_compose-0.5.4/examples/webserver/composition.nix
--rw-r--r--   0        0        0      571 2022-11-24 15:29:17.853309 nixos_compose-0.5.4/examples/webserver/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.4/examples/webserver/nxc.json
--rw-r--r--   0        0        0     1262 2022-12-02 16:34:24.566369 nixos_compose-0.5.4/nix/all-in-one.nix
--rw-r--r--   0        0        0     4160 2022-12-13 14:43:53.255994 nixos_compose-0.5.4/nix/compose.nix
--rw-r--r--   0        0        0     3246 2022-12-14 09:39:16.792209 nixos_compose-0.5.4/nix/flavours/docker/generate_docker_compose.nix
--rw-r--r--   0        0        0      569 2023-02-04 17:11:24.096024 nixos_compose-0.5.4/nix/flavours/docker/generate_image.nix
--rw-r--r--   0        0        0      816 2022-12-14 09:39:18.846217 nixos_compose-0.5.4/nix/flavours/docker/nxc-shared-dirs-docker.nix
--rw-r--r--   0        0        0      864 2022-07-15 20:53:49.903272 nixos_compose-0.5.4/nix/flavours/docker/systemd.nix
--rw-r--r--   0        0        0      229 2022-12-13 14:44:36.394071 nixos_compose-0.5.4/nix/flavours/docker.nix
--rw-r--r--   0        0        0      598 2022-02-22 14:04:48.134501 nixos_compose-0.5.4/nix/flavours/g5k-image.nix
--rw-r--r--   0        0        0     1966 2022-10-16 19:45:24.422173 nixos_compose-0.5.4/nix/flavours/g5k-nfs-store.nix
--rw-r--r--   0        0        0      273 2022-02-22 14:04:48.134501 nixos_compose-0.5.4/nix/flavours/g5k-ramdisk.nix
--rw-r--r--   0        0        0     1572 2022-02-22 14:04:48.134501 nixos_compose-0.5.4/nix/flavours/shared/base-hardware.nix
--rw-r--r--   0        0        0     1595 2022-12-12 21:04:21.027452 nixos_compose-0.5.4/nix/flavours/shared/base-vm.nix
--rw-r--r--   0        0        0      233 2023-02-04 17:12:54.022653 nixos_compose-0.5.4/nix/flavours/shared/base.nix
--rw-r--r--   0        0        0     5325 2023-02-04 17:14:20.565360 nixos_compose-0.5.4/nix/flavours/shared/common.nix
--rw-r--r--   0        0        0     1012 2022-12-12 21:01:47.752638 nixos_compose-0.5.4/nix/flavours/shared/g5k-common.nix
--rw-r--r--   0        0        0     1034 2022-02-22 14:04:48.134501 nixos_compose-0.5.4/nix/flavours/shared/g5k-ssh-host-keys.nix
--rw-r--r--   0        0        0     3508 2023-02-04 17:12:54.022653 nixos_compose-0.5.4/nix/flavours/shared/installation-device.nix
--rw-r--r--   0        0        0     2164 2022-02-22 14:04:48.134501 nixos_compose-0.5.4/nix/flavours/shared/netboot.nix
--rw-r--r--   0        0        0     1117 2022-12-13 15:41:18.469931 nixos_compose-0.5.4/nix/flavours/shared/nxc-shared-dirs-nfs.nix
--rw-r--r--   0        0        0     6669 2022-12-13 14:59:40.067304 nixos_compose-0.5.4/nix/flavours/shared/nxc.nix
--rw-r--r--   0        0        0     4183 2022-03-31 15:28:32.595831 nixos_compose-0.5.4/nix/flavours/shared/ssh-keys.nix
--rw-r--r--   0        0        0     6531 2022-12-02 16:37:56.969166 nixos_compose-0.5.4/nix/flavours/shared/stage-1-cmds.nix
--rw-r--r--   0        0        0     4044 2022-12-02 16:44:37.256556 nixos_compose-0.5.4/nix/flavours/shared/vm-stage-1-cmds.nix
--rw-r--r--   0        0        0      435 2022-04-08 15:45:40.641198 nixos_compose-0.5.4/nix/flavours/vm-ramdisk.nix
--rw-r--r--   0        0        0     1440 2023-01-27 16:32:56.174966 nixos_compose-0.5.4/nix/flavours/vm.nix
--rw-r--r--   0        0        0      982 2022-11-24 15:29:17.854309 nixos_compose-0.5.4/nix/flavours.json
--rw-r--r--   0        0        0      280 2022-11-24 15:29:17.854309 nixos_compose-0.5.4/nix/flavours.nix
--rw-r--r--   0        0        0      485 2022-02-22 14:08:06.721066 nixos_compose-0.5.4/nix/flavours2json.nix
--rw-r--r--   0        0        0     1970 2022-12-06 21:37:58.348959 nixos_compose-0.5.4/nix/generate_one_composition_info.nix
--rw-r--r--   0        0        0     1830 2022-03-09 21:28:29.653733 nixos_compose-0.5.4/nix/helpers.nix
--rw-r--r--   0        0        0      421 2022-03-07 19:13:07.567657 nixos_compose-0.5.4/nix/lib.nix
--rw-r--r--   0        0        0     1625 2022-02-22 14:04:48.135501 nixos_compose-0.5.4/nix/make-system-tarball.nix
--rw-r--r--   0        0        0     1540 2022-02-22 14:04:48.135501 nixos_compose-0.5.4/nix/make-system-tarball.sh
--rw-r--r--   0        0        0     6485 2022-12-01 14:50:43.355868 nixos_compose-0.5.4/nix/multiple_compositions.nix
--rw-r--r--   0        0        0      971 2022-03-20 18:16:06.981231 nixos_compose-0.5.4/nix/nur.nix
--rw-r--r--   0        0        0      795 2022-11-24 15:29:17.856309 nixos_compose-0.5.4/nix/one_composition.nix
--rw-r--r--   0        0        0     7234 2022-08-18 12:16:09.421462 nixos_compose-0.5.4/nix/setup.nix
--rw-r--r--   0        0        0        0 2022-09-22 15:03:49.416636 nixos_compose-0.5.4/nixos_compose/__init__.py
--rw-r--r--   0        0        0    30734 2023-01-26 14:02:56.121415 nixos_compose-0.5.4/nixos_compose/actions.py
--rw-r--r--   0        0        0     1877 2023-01-26 10:36:12.287610 nixos_compose-0.5.4/nixos_compose/cli.py
--rw-r--r--   0        0        0        0 2022-09-22 15:03:49.417636 nixos_compose-0.5.4/nixos_compose/commands/__init__.py
--rw-r--r--   0        0        0     9114 2023-01-26 10:31:30.360730 nixos_compose-0.5.4/nixos_compose/commands/cmd_build.py
--rw-r--r--   0        0        0      553 2022-02-22 14:04:48.136501 nixos_compose-0.5.4/nixos_compose/commands/cmd_clean.py
--rw-r--r--   0        0        0     1923 2022-10-28 08:47:49.562457 nixos_compose-0.5.4/nixos_compose/commands/cmd_connect.py
--rw-r--r--   0        0        0     2946 2022-10-20 15:49:47.707461 nixos_compose-0.5.4/nixos_compose/commands/cmd_driver.py
--rw-r--r--   0        0        0     2415 2023-02-15 14:46:39.245566 nixos_compose-0.5.4/nixos_compose/commands/cmd_helper.py
--rw-r--r--   0        0        0     4946 2023-01-26 10:36:12.284609 nixos_compose-0.5.4/nixos_compose/commands/cmd_init.py
--rw-r--r--   0        0        0    11693 2022-12-02 17:17:29.602117 nixos_compose-0.5.4/nixos_compose/commands/cmd_start.py
--rw-r--r--   0        0        0     1794 2022-02-22 14:04:48.136501 nixos_compose-0.5.4/nixos_compose/commands/cmd_stop.py
--rw-r--r--   0        0        0     9295 2023-02-01 16:48:32.365354 nixos_compose-0.5.4/nixos_compose/context.py
--rw-r--r--   0        0        0      388 2022-10-16 19:36:37.501675 nixos_compose-0.5.4/nixos_compose/default_role.py
--rwxr-xr-x   0        0        0      522 2022-02-22 14:04:48.136501 nixos_compose-0.5.4/nixos_compose/driver/__init__.py
--rw-r--r--   0        0        0     5210 2023-01-26 10:34:01.481292 nixos_compose-0.5.4/nixos_compose/driver/driver.py
--rw-r--r--   0        0        0     3250 2022-02-22 14:04:48.137501 nixos_compose-0.5.4/nixos_compose/driver/logger.py
--rw-r--r--   0        0        0    31187 2022-12-07 22:00:33.217394 nixos_compose-0.5.4/nixos_compose/driver/machine.py
--rw-r--r--   0        0        0     3395 2022-11-24 15:29:17.857309 nixos_compose-0.5.4/nixos_compose/driver/vlan.py
--rw-r--r--   0        0        0      706 2022-12-07 08:44:23.047801 nixos_compose-0.5.4/nixos_compose/flavour.py
--rw-r--r--   0        0        0     1568 2022-11-24 15:29:17.857309 nixos_compose-0.5.4/nixos_compose/flavours/__init__.py
--rw-r--r--   0        0        0     9765 2022-12-14 10:02:34.320312 nixos_compose-0.5.4/nixos_compose/flavours/docker.py
--rw-r--r--   0        0        0     7432 2022-11-30 12:35:31.158031 nixos_compose-0.5.4/nixos_compose/flavours/grid5000.py
--rw-r--r--   0        0        0     7077 2022-12-07 11:22:38.116441 nixos_compose-0.5.4/nixos_compose/flavours/vm.py
--rw-r--r--   0        0        0      602 2023-02-15 14:46:39.202566 nixos_compose-0.5.4/nixos_compose/g5k.py
--rw-r--r--   0        0        0     2187 2022-11-24 15:29:17.858309 nixos_compose-0.5.4/nixos_compose/httpd.py
--rw-r--r--   0        0        0     9488 2022-05-24 12:38:12.218571 nixos_compose-0.5.4/nixos_compose/nxc_execo.py
--rw-r--r--   0        0        0     3748 2022-11-24 15:29:17.858309 nixos_compose-0.5.4/nixos_compose/platform.py
--rw-r--r--   0        0        0     4034 2022-12-14 12:23:12.769245 nixos_compose-0.5.4/nixos_compose/setup.py
--rw-r--r--   0        0        0      953 2022-08-05 16:00:06.477496 nixos_compose-0.5.4/nixos_compose/state.py
--rw-r--r--   0        0        0        0 2022-03-26 18:59:34.690617 nixos_compose-0.5.4/nixos_compose/tools/__init__.py
--rwxr-xr-x   0        0        0      248 2022-03-26 19:00:47.951249 nixos_compose-0.5.4/nixos_compose/tools/g5k_set_pub_key_sleep.sh
--rwxr-xr-x   0        0        0     5010 2022-02-22 14:04:48.138501 nixos_compose-0.5.4/nixos_compose/tools/kataract.py
--rw-r--r--   0        0        0     2372 2022-02-22 14:04:48.138501 nixos_compose-0.5.4/nixos_compose/utils.py
--rw-r--r--   0        0        0     1064 2023-02-15 14:47:03.986386 nixos_compose-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 nixos_compose-0.5.4/setup.py
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 nixos_compose-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1094 2022-02-22 14:04:48.131501 nixos_compose-0.5.5/LICENSE
+-rw-r--r--   0        0        0      216 2023-01-26 10:45:07.461353 nixos_compose-0.5.5/examples/basic/composition.nix
+-rw-r--r--   0        0        0      561 2022-11-24 15:29:17.851309 nixos_compose-0.5.5/examples/basic/flake.nix
+-rw-r--r--   0        0        0       60 2022-11-24 15:29:17.851309 nixos_compose-0.5.5/examples/basic/nxc.json
+-rw-r--r--   0        0        0      216 2023-01-26 10:45:07.461353 nixos_compose-0.5.5/examples/basic-nur/composition.nix
+-rw-r--r--   0        0        0     1043 2022-11-24 15:29:17.851309 nixos_compose-0.5.5/examples/basic-nur/flake.nix
+-rw-r--r--   0        0        0       60 2022-11-24 15:29:17.851309 nixos_compose-0.5.5/examples/basic-nur/nxc.json
+-rw-r--r--   0        0        0      214 2023-01-26 10:45:07.461353 nixos_compose-0.5.5/examples/execo/composition.nix
+-rw-r--r--   0        0        0     2543 2022-03-05 16:55:24.727775 nixos_compose-0.5.5/examples/execo/execo_script.py
+-rw-r--r--   0        0        0      963 2022-11-24 15:29:17.851309 nixos_compose-0.5.5/examples/execo/flake.nix
+-rw-r--r--   0        0        0       60 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/execo/nxc.json
+-rw-r--r--   0        0        0      569 2022-02-22 14:04:48.132501 nixos_compose-0.5.5/examples/flake.lock
+-rw-r--r--   0        0        0      200 2023-06-01 07:45:30.792496 nixos_compose-0.5.5/examples/kernel/#linux_5_4.nix#
+-rw-r--r--   0        0        0       96 2022-02-22 14:04:48.132501 nixos_compose-0.5.5/examples/kernel/compositions.nix
+-rw-r--r--   0        0        0      577 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/kernel/flake.nix
+-rw-r--r--   0        0        0      200 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/kernel/linux_5_4.nix
+-rw-r--r--   0        0        0      907 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/kernel/linux_ipanema_5_4.nix
+-rw-r--r--   0        0        0       51 2022-02-22 14:04:48.132501 nixos_compose-0.5.5/examples/kernel/nxc.json
+-rw-r--r--   0        0        0      132 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/multi-compositions/bar-composition.nix
+-rw-r--r--   0        0        0       80 2022-02-22 14:04:48.132501 nixos_compose-0.5.5/examples/multi-compositions/compositions.nix
+-rw-r--r--   0        0        0      571 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/multi-compositions/flake.nix
+-rw-r--r--   0        0        0      132 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/multi-compositions/foo-composition.nix
+-rw-r--r--   0        0        0       51 2022-02-22 14:04:48.132501 nixos_compose-0.5.5/examples/multi-compositions/nxc.json
+-rw-r--r--   0        0        0      569 2022-12-07 13:41:00.974492 nixos_compose-0.5.5/examples/nbp-mpi/composition.nix
+-rw-r--r--   0        0        0      807 2022-12-06 21:39:45.820352 nixos_compose-0.5.5/examples/nbp-mpi/flake.nix
+-rw-r--r--   0        0        0       60 2022-12-06 21:41:04.858427 nixos_compose-0.5.5/examples/nbp-mpi/nxc.json
+-rw-r--r--   0        0        0     1113 2022-12-13 15:48:10.081561 nixos_compose-0.5.5/examples/nix_flake_templates.nix
+-rw-r--r--   0        0        0     2141 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/nixos-cluster/composition.nix
+-rw-r--r--   0        0        0      703 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/nixos-cluster/flake.nix
+-rw-r--r--   0        0        0       49 2022-06-14 14:20:20.160507 nixos_compose-0.5.5/examples/nixos-cluster/nodes.yaml
+-rw-r--r--   0        0        0       60 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/nixos-cluster/nxc.json
+-rw-r--r--   0        0        0     4455 2022-06-14 14:20:20.160507 nixos_compose-0.5.5/examples/nixos-cluster/ssh-keys.nix
+-rw-r--r--   0        0        0      499 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/scripts/composition.nix
+-rw-r--r--   0        0        0      563 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/scripts/flake.nix
+-rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/scripts/nxc.json
+-rw-r--r--   0        0        0      484 2022-04-14 09:01:13.303530 nixos_compose-0.5.5/examples/scripts/scripts/scripts.nix
+-rw-r--r--   0        0        0       83 2022-04-14 09:01:13.303530 nixos_compose-0.5.5/examples/scripts/scripts/test_python.py
+-rw-r--r--   0        0        0      465 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/setup/composition.nix
+-rw-r--r--   0        0        0      593 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/setup/flake.nix
+-rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/setup/nxc.json
+-rw-r--r--   0        0        0     2917 2022-11-29 09:02:17.732640 nixos_compose-0.5.5/examples/setup/setup.toml
+-rw-r--r--   0        0        0      691 2022-12-13 15:48:45.830622 nixos_compose-0.5.5/examples/shared-directories-users/composition.nix
+-rw-r--r--   0        0        0      807 2022-12-06 21:39:45.820352 nixos_compose-0.5.5/examples/shared-directories-users/flake.nix
+-rw-r--r--   0        0        0       60 2022-12-06 21:41:04.858427 nixos_compose-0.5.5/examples/shared-directories-users/nxc.json
+-rw-r--r--   0        0        0      561 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/spark/flake.nix
+-rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/spark/nxc.json
+-rw-r--r--   0        0        0     1321 2022-02-22 14:04:48.133501 nixos_compose-0.5.5/examples/spark/spark_sample.py
+-rw-r--r--   0        0        0      600 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/webserver/composition.nix
+-rw-r--r--   0        0        0      571 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/webserver/flake.nix
+-rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/webserver/nxc.json
+-rw-r--r--   0        0        0     1262 2022-12-02 16:34:24.566369 nixos_compose-0.5.5/nix/all-in-one.nix
+-rw-r--r--   0        0        0     4160 2022-12-13 14:43:53.255994 nixos_compose-0.5.5/nix/compose.nix
+-rw-r--r--   0        0        0     3246 2022-12-14 09:39:16.792209 nixos_compose-0.5.5/nix/flavours/docker/generate_docker_compose.nix
+-rw-r--r--   0        0        0      569 2023-02-04 17:11:24.096024 nixos_compose-0.5.5/nix/flavours/docker/generate_image.nix
+-rw-r--r--   0        0        0      816 2022-12-14 09:39:18.846217 nixos_compose-0.5.5/nix/flavours/docker/nxc-shared-dirs-docker.nix
+-rw-r--r--   0        0        0      864 2022-07-15 20:53:49.903272 nixos_compose-0.5.5/nix/flavours/docker/systemd.nix
+-rw-r--r--   0        0        0      229 2022-12-13 14:44:36.394071 nixos_compose-0.5.5/nix/flavours/docker.nix
+-rw-r--r--   0        0        0      598 2022-02-22 14:04:48.134501 nixos_compose-0.5.5/nix/flavours/g5k-image.nix
+-rw-r--r--   0        0        0     1966 2022-10-16 19:45:24.422173 nixos_compose-0.5.5/nix/flavours/g5k-nfs-store.nix
+-rw-r--r--   0        0        0      273 2022-02-22 14:04:48.134501 nixos_compose-0.5.5/nix/flavours/g5k-ramdisk.nix
+-rw-r--r--   0        0        0     1572 2022-02-22 14:04:48.134501 nixos_compose-0.5.5/nix/flavours/shared/base-hardware.nix
+-rw-r--r--   0        0        0     1595 2022-12-12 21:04:21.027452 nixos_compose-0.5.5/nix/flavours/shared/base-vm.nix
+-rw-r--r--   0        0        0      233 2023-02-04 17:12:54.022653 nixos_compose-0.5.5/nix/flavours/shared/base.nix
+-rw-r--r--   0        0        0     5325 2023-02-04 17:14:20.565360 nixos_compose-0.5.5/nix/flavours/shared/common.nix
+-rw-r--r--   0        0        0     1080 2023-03-22 14:08:21.310405 nixos_compose-0.5.5/nix/flavours/shared/g5k-common.nix
+-rw-r--r--   0        0        0     1034 2023-02-23 08:34:27.688629 nixos_compose-0.5.5/nix/flavours/shared/g5k-ssh-host-keys.nix
+-rw-r--r--   0        0        0     3508 2023-02-04 17:12:54.022653 nixos_compose-0.5.5/nix/flavours/shared/installation-device.nix
+-rw-r--r--   0        0        0     2164 2022-02-22 14:04:48.134501 nixos_compose-0.5.5/nix/flavours/shared/netboot.nix
+-rw-r--r--   0        0        0     1117 2022-12-13 15:41:18.469931 nixos_compose-0.5.5/nix/flavours/shared/nxc-shared-dirs-nfs.nix
+-rw-r--r--   0        0        0     6669 2022-12-13 14:59:40.067304 nixos_compose-0.5.5/nix/flavours/shared/nxc.nix
+-rw-r--r--   0        0        0     4183 2022-03-31 15:28:32.595831 nixos_compose-0.5.5/nix/flavours/shared/ssh-keys.nix
+-rw-r--r--   0        0        0     6531 2022-12-02 16:37:56.969166 nixos_compose-0.5.5/nix/flavours/shared/stage-1-cmds.nix
+-rw-r--r--   0        0        0     4044 2022-12-02 16:44:37.256556 nixos_compose-0.5.5/nix/flavours/shared/vm-stage-1-cmds.nix
+-rw-r--r--   0        0        0      435 2022-04-08 15:45:40.641198 nixos_compose-0.5.5/nix/flavours/vm-ramdisk.nix
+-rw-r--r--   0        0        0     1440 2023-07-10 15:40:24.993694 nixos_compose-0.5.5/nix/flavours/vm.nix
+-rw-r--r--   0        0        0      982 2022-11-24 15:29:17.854309 nixos_compose-0.5.5/nix/flavours.json
+-rw-r--r--   0        0        0      280 2022-11-24 15:29:17.854309 nixos_compose-0.5.5/nix/flavours.nix
+-rw-r--r--   0        0        0      485 2022-02-22 14:08:06.721066 nixos_compose-0.5.5/nix/flavours2json.nix
+-rw-r--r--   0        0        0     1970 2022-12-06 21:37:58.348959 nixos_compose-0.5.5/nix/generate_one_composition_info.nix
+-rw-r--r--   0        0        0     1830 2022-03-09 21:28:29.653733 nixos_compose-0.5.5/nix/helpers.nix
+-rw-r--r--   0        0        0      421 2022-03-07 19:13:07.567657 nixos_compose-0.5.5/nix/lib.nix
+-rw-r--r--   0        0        0     1625 2022-02-22 14:04:48.135501 nixos_compose-0.5.5/nix/make-system-tarball.nix
+-rw-r--r--   0        0        0     1540 2022-02-22 14:04:48.135501 nixos_compose-0.5.5/nix/make-system-tarball.sh
+-rw-r--r--   0        0        0     6485 2022-12-01 14:50:43.355868 nixos_compose-0.5.5/nix/multiple_compositions.nix
+-rw-r--r--   0        0        0      989 2023-03-22 14:08:21.286405 nixos_compose-0.5.5/nix/nur.nix
+-rw-r--r--   0        0        0      795 2022-11-24 15:29:17.856309 nixos_compose-0.5.5/nix/one_composition.nix
+-rw-r--r--   0        0        0     7234 2022-08-18 12:16:09.421462 nixos_compose-0.5.5/nix/setup.nix
+-rw-r--r--   0        0        0        0 2022-09-22 15:03:49.416636 nixos_compose-0.5.5/nixos_compose/__init__.py
+-rw-r--r--   0        0        0    30734 2023-01-26 14:02:56.121415 nixos_compose-0.5.5/nixos_compose/actions.py
+-rw-r--r--   0        0        0     1877 2023-01-26 10:36:12.287610 nixos_compose-0.5.5/nixos_compose/cli.py
+-rw-r--r--   0        0        0        0 2022-09-22 15:03:49.417636 nixos_compose-0.5.5/nixos_compose/commands/__init__.py
+-rw-r--r--   0        0        0     9282 2023-04-12 07:53:33.247814 nixos_compose-0.5.5/nixos_compose/commands/cmd_build.py
+-rw-r--r--   0        0        0      553 2022-02-22 14:04:48.136501 nixos_compose-0.5.5/nixos_compose/commands/cmd_clean.py
+-rw-r--r--   0        0        0     1923 2022-10-28 08:47:49.562457 nixos_compose-0.5.5/nixos_compose/commands/cmd_connect.py
+-rw-r--r--   0        0        0     2946 2022-10-20 15:49:47.707461 nixos_compose-0.5.5/nixos_compose/commands/cmd_driver.py
+-rw-r--r--   0        0        0     2415 2023-03-22 14:08:21.301405 nixos_compose-0.5.5/nixos_compose/commands/cmd_helper.py
+-rw-r--r--   0        0        0     4946 2023-01-26 10:36:12.284609 nixos_compose-0.5.5/nixos_compose/commands/cmd_init.py
+-rw-r--r--   0        0        0    11838 2023-06-02 12:45:49.039451 nixos_compose-0.5.5/nixos_compose/commands/cmd_start.py
+-rw-r--r--   0        0        0     1794 2022-02-22 14:04:48.136501 nixos_compose-0.5.5/nixos_compose/commands/cmd_stop.py
+-rw-r--r--   0        0        0     9295 2023-02-01 16:48:32.365354 nixos_compose-0.5.5/nixos_compose/context.py
+-rw-r--r--   0        0        0      388 2022-10-16 19:36:37.501675 nixos_compose-0.5.5/nixos_compose/default_role.py
+-rwxr-xr-x   0        0        0      522 2022-02-22 14:04:48.136501 nixos_compose-0.5.5/nixos_compose/driver/__init__.py
+-rw-r--r--   0        0        0     5210 2023-01-26 10:34:01.481292 nixos_compose-0.5.5/nixos_compose/driver/driver.py
+-rw-r--r--   0        0        0     3250 2022-02-22 14:04:48.137501 nixos_compose-0.5.5/nixos_compose/driver/logger.py
+-rw-r--r--   0        0        0    31187 2022-12-07 22:00:33.217394 nixos_compose-0.5.5/nixos_compose/driver/machine.py
+-rw-r--r--   0        0        0     3395 2022-11-24 15:29:17.857309 nixos_compose-0.5.5/nixos_compose/driver/vlan.py
+-rw-r--r--   0        0        0      706 2022-12-07 08:44:23.047801 nixos_compose-0.5.5/nixos_compose/flavour.py
+-rw-r--r--   0        0        0     1568 2022-11-24 15:29:17.857309 nixos_compose-0.5.5/nixos_compose/flavours/__init__.py
+-rw-r--r--   0        0        0     9765 2022-12-14 10:02:34.320312 nixos_compose-0.5.5/nixos_compose/flavours/docker.py
+-rw-r--r--   0        0        0     7864 2023-07-10 15:36:50.778526 nixos_compose-0.5.5/nixos_compose/flavours/grid5000.py
+-rw-r--r--   0        0        0     7077 2022-12-07 11:22:38.116441 nixos_compose-0.5.5/nixos_compose/flavours/vm.py
+-rw-r--r--   0        0        0      602 2023-03-22 14:08:21.301405 nixos_compose-0.5.5/nixos_compose/g5k.py
+-rw-r--r--   0        0        0     2187 2022-11-24 15:29:17.858309 nixos_compose-0.5.5/nixos_compose/httpd.py
+-rw-r--r--   0        0        0     4285 2023-06-02 12:45:49.039451 nixos_compose-0.5.5/nixos_compose/nxc_execo.py
+-rw-r--r--   0        0        0     3748 2022-11-24 15:29:17.858309 nixos_compose-0.5.5/nixos_compose/platform.py
+-rw-r--r--   0        0        0     4034 2022-12-14 12:23:12.769245 nixos_compose-0.5.5/nixos_compose/setup.py
+-rw-r--r--   0        0        0      953 2022-08-05 16:00:06.477496 nixos_compose-0.5.5/nixos_compose/state.py
+-rw-r--r--   0        0        0        0 2022-03-26 18:59:34.690617 nixos_compose-0.5.5/nixos_compose/tools/__init__.py
+-rwxr-xr-x   0        0        0      248 2022-03-26 19:00:47.951249 nixos_compose-0.5.5/nixos_compose/tools/g5k_set_pub_key_sleep.sh
+-rwxr-xr-x   0        0        0     5010 2022-02-22 14:04:48.138501 nixos_compose-0.5.5/nixos_compose/tools/kataract.py
+-rw-r--r--   0        0        0     2372 2022-02-22 14:04:48.138501 nixos_compose-0.5.5/nixos_compose/utils.py
+-rw-r--r--   0        0        0     1064 2023-07-10 15:43:11.937605 nixos_compose-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 nixos_compose-0.5.5/PKG-INFO
```

### Comparing `nixos_compose-0.5.4/LICENSE` & `nixos_compose-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/basic/flake.nix` & `nixos_compose-0.5.5/examples/basic/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/basic-nur/flake.nix` & `nixos_compose-0.5.5/examples/basic-nur/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/execo/execo_script.py` & `nixos_compose-0.5.5/examples/execo/execo_script.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/execo/flake.nix` & `nixos_compose-0.5.5/examples/execo/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/flake.lock` & `nixos_compose-0.5.5/examples/flake.lock`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/kernel/flake.nix` & `nixos_compose-0.5.5/examples/kernel/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/kernel/linux_ipanema_5_4.nix` & `nixos_compose-0.5.5/examples/kernel/linux_ipanema_5_4.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/multi-compositions/flake.nix` & `nixos_compose-0.5.5/examples/multi-compositions/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/nbp-mpi/composition.nix` & `nixos_compose-0.5.5/examples/nbp-mpi/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/nbp-mpi/flake.nix` & `nixos_compose-0.5.5/examples/nbp-mpi/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/nix_flake_templates.nix` & `nixos_compose-0.5.5/examples/nix_flake_templates.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/nixos-cluster/composition.nix` & `nixos_compose-0.5.5/examples/nixos-cluster/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/nixos-cluster/flake.nix` & `nixos_compose-0.5.5/examples/nixos-cluster/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/nixos-cluster/ssh-keys.nix` & `nixos_compose-0.5.5/examples/nixos-cluster/ssh-keys.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/scripts/flake.nix` & `nixos_compose-0.5.5/examples/scripts/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/setup/flake.nix` & `nixos_compose-0.5.5/examples/setup/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/setup/setup.toml` & `nixos_compose-0.5.5/examples/setup/setup.toml`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/shared-directories-users/composition.nix` & `nixos_compose-0.5.5/examples/shared-directories-users/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/shared-directories-users/flake.nix` & `nixos_compose-0.5.5/examples/shared-directories-users/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/spark/flake.nix` & `nixos_compose-0.5.5/examples/spark/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/spark/spark_sample.py` & `nixos_compose-0.5.5/examples/spark/spark_sample.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/webserver/composition.nix` & `nixos_compose-0.5.5/examples/webserver/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/examples/webserver/flake.nix` & `nixos_compose-0.5.5/examples/webserver/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/all-in-one.nix` & `nixos_compose-0.5.5/nix/all-in-one.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/compose.nix` & `nixos_compose-0.5.5/nix/compose.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/docker/generate_docker_compose.nix` & `nixos_compose-0.5.5/nix/flavours/docker/generate_docker_compose.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/docker/generate_image.nix` & `nixos_compose-0.5.5/nix/flavours/docker/generate_image.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/docker/nxc-shared-dirs-docker.nix` & `nixos_compose-0.5.5/nix/flavours/docker/nxc-shared-dirs-docker.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/docker/systemd.nix` & `nixos_compose-0.5.5/nix/flavours/docker/systemd.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/g5k-image.nix` & `nixos_compose-0.5.5/nix/flavours/g5k-image.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/g5k-nfs-store.nix` & `nixos_compose-0.5.5/nix/flavours/g5k-nfs-store.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/base-hardware.nix` & `nixos_compose-0.5.5/nix/flavours/shared/base-hardware.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/base-vm.nix` & `nixos_compose-0.5.5/nix/flavours/shared/base-vm.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/common.nix` & `nixos_compose-0.5.5/nix/flavours/shared/common.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/g5k-common.nix` & `nixos_compose-0.5.5/nix/flavours/shared/g5k-common.nix`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,19 @@
   boot.supportedFilesystems = [ "nfs" ];
   nxc.wait-online.enable = true;
 
   systemd.services.nxc-script = {
     after = [ "network.target" "network-online.target" ];
     wants = [ "network-online.target" ];
     wantedBy = [ "multi-user.target" ];
-    serviceConfig.Type = "oneshot";
+    serviceConfig = {
+      Type = "oneshot";
+      Restart = "on-failure";
+      RestartSec=1;
+    };
     #path = [ pkgs.hostname pkgs.iproute pkgs.jq ];
     script = ''
-      user=$( ${pkgs.jq}/bin/jq -r '."user" // empty' etc/nxc/deployment.json)
+      user=$( ${pkgs.jq}/bin/jq -r '."user" // empty' /etc/nxc/deployment.json)
       mkdir -p /home/$user
       ${pkgs.util-linux}/bin/mount -t nfs nfs:/export/home/$user /home/$user'';
   };
 }
```

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/g5k-ssh-host-keys.nix` & `nixos_compose-0.5.5/nix/flavours/shared/g5k-ssh-host-keys.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/installation-device.nix` & `nixos_compose-0.5.5/nix/flavours/shared/installation-device.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/netboot.nix` & `nixos_compose-0.5.5/nix/flavours/shared/netboot.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/nxc-shared-dirs-nfs.nix` & `nixos_compose-0.5.5/nix/flavours/shared/nxc-shared-dirs-nfs.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/nxc.nix` & `nixos_compose-0.5.5/nix/flavours/shared/nxc.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/ssh-keys.nix` & `nixos_compose-0.5.5/nix/flavours/shared/ssh-keys.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/stage-1-cmds.nix` & `nixos_compose-0.5.5/nix/flavours/shared/stage-1-cmds.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/shared/vm-stage-1-cmds.nix` & `nixos_compose-0.5.5/nix/flavours/shared/vm-stage-1-cmds.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours/vm.nix` & `nixos_compose-0.5.5/nix/flavours/vm.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/flavours.json` & `nixos_compose-0.5.5/nix/flavours.json`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/generate_one_composition_info.nix` & `nixos_compose-0.5.5/nix/generate_one_composition_info.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/helpers.nix` & `nixos_compose-0.5.5/nix/helpers.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/make-system-tarball.nix` & `nixos_compose-0.5.5/nix/make-system-tarball.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/make-system-tarball.sh` & `nixos_compose-0.5.5/nix/make-system-tarball.sh`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/multiple_compositions.nix` & `nixos_compose-0.5.5/nix/multiple_compositions.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/nur.nix` & `nixos_compose-0.5.5/nix/nur.nix`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 #    { nixpkgs.overlays = [ nur.overlay ]; }
 #    # add wanted NUR's modules
 #    nur.repos.kapack.modules.oar
 #  ];
 #
 { nixpkgs, system, NUR, repoOverrides ? { } }:
 let nurpkgs = import nixpkgs { inherit system; };
-in {
+in
+{
   overlay = (final: prev: {
     nur = import NUR {
       nurpkgs = prev;
       pkgs = prev;
       repoOverrides =
         builtins.mapAttrs (name: value: import value { pkgs = prev; })
-        repoOverrides;
+          repoOverrides;
     };
   });
   repos = (import NUR {
     inherit nurpkgs;
     repoOverrides =
-      builtins.mapAttrs (name: value: import value { }) repoOverrides;
+      builtins.mapAttrs (name: value: import value { pkgs = nurpkgs; }) repoOverrides;
   }).repos;
 
 }
```

### Comparing `nixos_compose-0.5.4/nix/one_composition.nix` & `nixos_compose-0.5.5/nix/one_composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nix/setup.nix` & `nixos_compose-0.5.5/nix/setup.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/actions.py` & `nixos_compose-0.5.5/nixos_compose/actions.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/cli.py` & `nixos_compose-0.5.5/nixos_compose/cli.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/commands/cmd_build.py` & `nixos_compose-0.5.5/nixos_compose/commands/cmd_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,19 @@
 )
 @click.option(
     "-u",
     "--update-flake",
     is_flag=True,
     help="Update flake.lock equivalent to: nix flake update",
 )
+@click.option(
+    "--monitor",
+    is_flag=True,
+    help="Build with nix-output-monitor",
+)
 @pass_context
 @on_finished(lambda ctx: ctx.show_elapsed_time())
 @on_started(lambda ctx: ctx.assert_valid_env())
 def cli(
     ctx,
     composition_file,
     nix_flags,
@@ -92,14 +97,15 @@
     dry_run,
     dry_build,
     composition_flavour,
     list_compositions_flavours,
     update_flake,
     setup,
     setup_param,
+    monitor,
 ):
     """Build multi Nixos composition.
     Typically it performs the kind of following command:
       nix build
     """
 
     def determine_flavour(ctx):
@@ -133,15 +139,18 @@
     build_cmd = []
 
     # Do we are in flake context
     if not op.exists(op.join(ctx.envdir, "flake.nix")):
         ctx.elog("Not Found flake.nix file")
         sys.exit(1)
 
-    nix_cmd_base = get_nix_command(ctx)
+    if monitor:
+        nix_cmd_base = ["nom"]
+    else:
+        nix_cmd_base = get_nix_command(ctx)
 
     if update_flake:
         cmd = nix_cmd_base + ["flake", "update"]
         if ctx.show_spinner:
             ctx.spinner.start("Updating flake.lock")
             ret = subprocess.call(
                 cmd,
```

### Comparing `nixos_compose-0.5.4/nixos_compose/commands/cmd_clean.py` & `nixos_compose-0.5.5/nixos_compose/commands/cmd_clean.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/commands/cmd_connect.py` & `nixos_compose-0.5.5/nixos_compose/commands/cmd_connect.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/commands/cmd_driver.py` & `nixos_compose-0.5.5/nixos_compose/commands/cmd_driver.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/commands/cmd_helper.py` & `nixos_compose-0.5.5/nixos_compose/commands/cmd_helper.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/commands/cmd_init.py` & `nixos_compose-0.5.5/nixos_compose/commands/cmd_init.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/commands/cmd_start.py` & `nixos_compose-0.5.5/nixos_compose/commands/cmd_start.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,20 @@
 )
 @click.option(
     "--remote-deployment-info",
     is_flag=True,
     help="deployement info is served by http (in place of kernel parameters)",
 )
 @click.option(
+    "--port",
+    type=click.INT,
+    default=0,
+    help="Port to use for the HTTP server",
+)
+@click.option(
     "-c",
     "-C",
     "--composition",
     type=click.STRING,
     help="specify composition, can specify flavour e.g. composition::flavour",
 )
 @click.option(
@@ -150,14 +156,15 @@
     ssh,
     sudo,
     push_path,
     reuse,
     composition,
     flavour,
     remote_deployment_info,
+    port,
     test_script,
     file_test_script,
     sigwait,
     kernel_params,
     role_distribution,
     roles_distribution_file,
     compose_info,
@@ -346,27 +353,28 @@
     if (
         ctx.ip_addresses
         and (ctx.flavour.name != "vm-ramdisk")
         and (ctx.flavour.name != "vm")
     ):
         if ctx.use_httpd:
             ctx.vlog("Launch: httpd to distribute deployment.json")
-            ctx.httpd = HTTPDaemon(ctx=ctx)
+            ctx.httpd = HTTPDaemon(ctx=ctx, port=port)
+
 
         if hasattr(ctx.flavour, "generate_kexec_scripts"):
             ctx.flavour.generate_kexec_scripts()
 
         if ctx.push_path:
             push_on_machines(ctx)
 
         if ctx.use_httpd:
             ctx.httpd.start(directory=ctx.envdir)
 
         if not interactive:
-            ctx.flavour.launch()
+            ctx.flavour.launch(machines_file)
             sys.exit(0)
 
     test_script = read_test_script(ctx, ctx.compose_info)
 
     if not interactive and not execute_test_script:
         test_script = "start_all()"
```

### Comparing `nixos_compose-0.5.4/nixos_compose/commands/cmd_stop.py` & `nixos_compose-0.5.5/nixos_compose/commands/cmd_stop.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/context.py` & `nixos_compose-0.5.5/nixos_compose/context.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/driver/__init__.py` & `nixos_compose-0.5.5/nixos_compose/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/driver/driver.py` & `nixos_compose-0.5.5/nixos_compose/driver/driver.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/driver/logger.py` & `nixos_compose-0.5.5/nixos_compose/driver/logger.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/driver/machine.py` & `nixos_compose-0.5.5/nixos_compose/driver/machine.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/driver/vlan.py` & `nixos_compose-0.5.5/nixos_compose/driver/vlan.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/flavour.py` & `nixos_compose-0.5.5/nixos_compose/flavour.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/flavours/__init__.py` & `nixos_compose-0.5.5/nixos_compose/flavours/__init__.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/flavours/docker.py` & `nixos_compose-0.5.5/nixos_compose/flavours/docker.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/flavours/grid5000.py` & `nixos_compose-0.5.5/nixos_compose/flavours/grid5000.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,45 +47,48 @@
         kernel_params: $kernel_params
       filesystem: ext4
       partition_type: 131
       multipart: false
 """
 
 
-def generate_kadeploy_envfile(ctx, deploy=None, kernel_params=""):
+def generate_kadeploy_envfile(ctx, deploy=None, kernel_params="", kaenv_path=None, deploy_image_path=None):
     if not ctx.compose_info:
         read_compose_info(ctx)
 
     base_path = op.join(
         ctx.envdir, f"artifact/{ctx.composition_name}/{ctx.flavour.name}"
     )
     os.makedirs(base_path, mode=0o700, exist_ok=True)
-    kaenv_path = op.join(base_path, "nixos.yaml")
+    if kaenv_path is None:
+        kaenv_path = op.join(base_path, "nixos.yaml")
 
     if not deploy:
         if ctx.use_httpd:
             base_url = f"http://{ctx.httpd.ip}:{ctx.httpd.port}"
             deploy = f"{base_url}/deploy/{ctx.composition_flavour_prefix}.json"
         else:
             generate_deploy_info_b64(ctx)
             deploy = ctx.deployment_info_b64
 
     user = os.environ["USER"]
+    g5k_frontend = socket.gethostname()
+    g5k_site = g5k_frontend[1:]
     system = ctx.compositions_info["system"]
     additional_kernel_params = ""
     if ctx.kernel_params:
         additional_kernel_params = ctx.kernel_params
     with open(kaenv_path, "w") as kaenv_file:
         t = Template(KADEPOY_ENV_DESC)
         kaenv = t.substitute(
             image_name="NixOS",
             author=user,
             system=KADEPOY_ARCH[system],
-            file_image_url=f"http://public.grenoble.grid5000.fr/~{user}/nixos.tar.xz",
-            kernel_params=f"boot.shell_on_fail console=tty0 console=ttyS0,115200 deploy={deploy} {additional_kernel_params} {ctx.kernel_params}",
+            file_image_url=f"local://{deploy_image_path}" if deploy_image_path else f"http://public.{g5k_site}.grid5000.fr/~{user}/nixos.tar.xz",
+            kernel_params=f"boot.shell_on_fail console=tty0 console=ttyS0,115200 deploy={deploy} {additional_kernel_params} {kernel_params}",
         )
         kaenv_file.write(kaenv)
 
 
 class G5kKexecBasedFlavour(Flavour):
     def __init__(self, ctx):
         super().__init__(ctx)
@@ -183,40 +186,46 @@
         super().__init__(ctx)
 
         self.name = "g5k-image"
 
     def generate_deployment_info(self):
         generate_deployment_info(self.ctx)
 
-    def launch(self, machine_file=None):
-        generate_kadeploy_envfile(self.ctx)
+    def launch(self, machine_file=None, kaenv_path=None, deploy_image_path=None):
+        generate_kadeploy_envfile(self.ctx, kaenv_path=kaenv_path, deploy_image_path=deploy_image_path)
         image_path = realpath_from_store(
             self.ctx, self.ctx.deployment_info["all"]["image"]
         )
-        cmd_copy_image = f'cp {image_path} ~{os.environ["USER"]}/public/nixos.tar.xz && chmod 644 ~{os.environ["USER"]}/public/nixos.tar.xz'
+        if deploy_image_path is None:
+            user = os.environ["USER"]
+            deploy_image_path = f"~{user}/public/nixos.tar.xz"
+            
+        cmd_copy_image = f'cp {image_path} {deploy_image_path} && chmod 644 {deploy_image_path}'
         if machine_file or click.confirm(
-            f'Do you want to copy image to ~{os.environ["USER"]}/public/nixos.tar.xz ?'
+            f'Do you want to copy image to {deploy_image_path} ?'
         ):
             try:
                 subprocess.call(cmd_copy_image, shell=True)
             except Exception as ex:
                 raise click.ClickException(f"Failed to copy image: {ex}")
         else:
             print(f"You can copy image with: {cmd_copy_image}")
         base_path = op.join(
             self.ctx.envdir,
             f"artifact/{self.ctx.composition_name}/{self.ctx.flavour.name}",
         )
+        if kaenv_path is None:
+            kaenv_path = op.join(base_path, "nixos.yaml") 
         if machine_file:
             cmd_kadeploy = (
-                f'kadeploy3 -a {op.join(base_path, "nixos.yaml")} -f {machine_file}'
+                f'kadeploy3 -a {kaenv_path} -f {machine_file}'
             )
         else:
             cmd_kadeploy = (
-                f'kadeploy3 -a {op.join(base_path, "nixos.yaml")} -f $OAR_NODEFILE'
+                f'kadeploy3 -a {kaenv_path} -f $OAR_NODEFILE'
             )
 
         if machine_file or click.confirm(
             "Do you want to kadeploy nixos.tar.xz image on nodes from $OAR_NODEFILE"
         ):
             try:
                 subprocess.call(cmd_kadeploy, shell=True)
```

### Comparing `nixos_compose-0.5.4/nixos_compose/flavours/vm.py` & `nixos_compose-0.5.5/nixos_compose/flavours/vm.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/g5k.py` & `nixos_compose-0.5.5/nixos_compose/g5k.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/httpd.py` & `nixos_compose-0.5.5/nixos_compose/httpd.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/platform.py` & `nixos_compose-0.5.5/nixos_compose/platform.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/setup.py` & `nixos_compose-0.5.5/nixos_compose/setup.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/state.py` & `nixos_compose-0.5.5/nixos_compose/state.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/tools/kataract.py` & `nixos_compose-0.5.5/nixos_compose/tools/kataract.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/nixos_compose/utils.py` & `nixos_compose-0.5.5/nixos_compose/utils.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.4/pyproject.toml` & `nixos_compose-0.5.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nixos-compose"
-version = "0.5.4"
+version = "0.5.5"
 description = ""
 authors = ["Olivier Richard <olivier.richard@imag.fr>"]
 license = "MIT"
 include = [
      { path = 'examples', format = 'wheel' },
      { path = 'nix', format = 'wheel' },
      #{ path = 'tools', format = 'wheel' }
```

### Comparing `nixos_compose-0.5.4/PKG-INFO` & `nixos_compose-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nixos-compose
-Version: 0.5.4
+Version: 0.5.5
 Summary: 
 License: MIT
 Author: Olivier Richard
 Author-email: olivier.richard@imag.fr
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

