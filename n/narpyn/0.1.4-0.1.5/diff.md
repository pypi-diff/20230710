# Comparing `tmp/narpyn-0.1.4.tar.gz` & `tmp/narpyn-0.1.5.tar.gz`

## Comparing `narpyn-0.1.4.tar` & `narpyn-0.1.5.tar`

### file list

```diff
@@ -1,166 +1,166 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 narpyn-0.1.4/.gitattributes
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 narpyn-0.1.4/.gitmodules
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 narpyn-0.1.4/build_ona.sh
--rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 narpyn-0.1.4/build_package.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narpyn-0.1.4/narpyn/ona/__init__.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 narpyn-0.1.4/narpyn/ona/nar.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 narpyn-0.1.4/narpyn/ona/narsese.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/.git
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/.gitignore
--rwxr-xr-x   0        0        0     3350 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/Dockerfile
--rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/LICENSE
--rwxr-xr-x   0        0        0     8257 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/README.md
--rwxr-xr-x   0        0        0      755 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/build.sh
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/docker-compose.yml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/install_python_dependencies.sh
--rwxr-xr-x   0        0        0     1701 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/libbuild.sh
--rwxr-xr-x   0        0        0      704 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/english/babi1.english
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/english/dialog.english
--rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/english/disambiguate.english
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/english/grammar.english
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/english/prepositions.english
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/english/robotQA.english
--rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/english/story1.english
--rwxr-xr-x   0        0        0      422 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/english/story2.english
--rwxr-xr-x   0        0        0      371 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/english/story3.english
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/english/story4.english
--rwxr-xr-x   0        0        0      941 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/activequestion.nal
--rwxr-xr-x   0        0        0     1288 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/asthma.nal
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/asthma2.nal
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/avoid.nal
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/avoid2.nal
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/avoid3.nal
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/catCAT.nal
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/categoryformationanddetection.nal
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/circus.nal
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/clapwave0.nal
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/clapwave1.nal
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/clapwave2.nal
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/clapwave3.nal
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/clapwave4.nal
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/clapwave5.nal
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/diagnostic.nal
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/door.nal
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/door2.nal
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/door3.nal
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/duck.nal
--rwxr-xr-x   0        0        0    14725 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/example1.nal
--rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/example2.nal
--rwxr-xr-x   0        0        0      869 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/example3.nal
--rwxr-xr-x   0        0        0      803 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/example4.nal
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/greenplant.nal
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/latch.nal
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/map.nal
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/map2.nal
--rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/marshmallow.nal
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/numbers.nal
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/pickbrighter.nal
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/plandeep.nal
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/prefergeneral.nal
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/prefernext.nal
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/preferspecific.nal
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/propertymatching.nal
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/relationalnetwork.nal
--rwxr-xr-x   0        0        0     3820 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/school.nal
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/self.nal
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/self2.nal
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/self3.nal
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/similarities.nal
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/spatial.nal
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/spatial3.nal
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/spatial4.nal
--rwxr-xr-x   0        0        0     1371 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/symmetry.nal
--rwxr-xr-x   0        0        0     1774 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/toothbrush.nal
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/examples/nal/whatwarmer.nal
--rwxr-xr-x   0        0        0     2403 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Concept.h
--rwxr-xr-x   0        0        0     7741 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Config.h
--rwxr-xr-x   0        0        0    35264 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Cycle.c
--rwxr-xr-x   0        0        0     1799 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Cycle.h
--rwxr-xr-x   0        0        0    26640 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Decision.c
--rwxr-xr-x   0        0        0     3336 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Decision.h
--rwxr-xr-x   0        0        0     2753 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Event.c
--rwxr-xr-x   0        0        0     2603 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Event.h
--rwxr-xr-x   0        0        0     2150 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Globals.c
--rwxr-xr-x   0        0        0     2673 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Globals.h
--rwxr-xr-x   0        0        0     4760 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/HashTable.c
--rwxr-xr-x   0        0        0     2640 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/HashTable.h
--rwxr-xr-x   0        0        0     2044 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Implication.h
--rwxr-xr-x   0        0        0     9629 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Inference.c
--rwxr-xr-x   0        0        0     2972 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Inference.h
--rwxr-xr-x   0        0        0     5349 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/InvertedAtomIndex.c
--rwxr-xr-x   0        0        0     2334 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/InvertedAtomIndex.h
--rwxr-xr-x   0        0        0    18958 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Memory.c
--rwxr-xr-x   0        0        0     4219 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Memory.h
--rwxr-xr-x   0        0        0    20399 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/NAL.c
--rwxr-xr-x   0        0        0    14959 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/NAL.h
--rwxr-xr-x   0        0        0    11792 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/NAR.c
--rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/NAR.h
--rwxr-xr-x   0        0        0    28145 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Narsese.c
--rwxr-xr-x   0        0        0     4422 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Narsese.h
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/OccurrenceTimeIndex.c
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/OccurrenceTimeIndex.h
--rwxr-xr-x   0        0        0     6777 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/PriorityQueue.c
--rwxr-xr-x   0        0        0     3264 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/PriorityQueue.h
--rwxr-xr-x   0        0        0     1922 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/RuleTable.h
--rwxr-xr-x   0        0        0    14924 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Shell.c
--rwxr-xr-x   0        0        0     1888 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Shell.h
--rwxr-xr-x   0        0        0     1774 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Stack.c
--rwxr-xr-x   0        0        0     1814 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Stack.h
--rwxr-xr-x   0        0        0     3850 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Stamp.c
--rwxr-xr-x   0        0        0     2253 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Stamp.h
--rwxr-xr-x   0        0        0     3835 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Stats.c
--rwxr-xr-x   0        0        0     1668 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Stats.h
--rwxr-xr-x   0        0        0     4506 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Table.c
--rwxr-xr-x   0        0        0     2530 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Table.h
--rwxr-xr-x   0        0        0     3651 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Term.c
--rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Term.h
--rwxr-xr-x   0        0        0     7595 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Truth.c
--rwxr-xr-x   0        0        0     3383 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Truth.h
--rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Usage.c
--rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Usage.h
--rwxr-xr-x   0        0        0    18602 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Variable.c
--rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/Variable.h
--rwxr-xr-x   0        0        0     5197 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/main.c
--rwxr-xr-x   0        0        0     1888 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/NetworkNAR/Metric.c
--rwxr-xr-x   0        0        0     1655 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/NetworkNAR/Metric.h
--rwxr-xr-x   0        0        0     2300 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/NetworkNAR/UDP.c
--rwxr-xr-x   0        0        0     1938 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/NetworkNAR/UDP.h
--rwxr-xr-x   0        0        0     3997 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/NetworkNAR/UDPNAR.c
--rwxr-xr-x   0        0        0     1667 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/NetworkNAR/UDPNAR.h
--rwxr-xr-x   0        0        0     4565 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Alien_Test.h
--rwxr-xr-x   0        0        0     1645 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Alphabet_Test.h
--rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Bandrobot_Test.h
--rwxr-xr-x   0        0        0     2938 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Cartpole_Test.h
--rwxr-xr-x   0        0        0     3458 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Follow_Test.h
--rwxr-xr-x   0        0        0     2767 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Multistep2_Test.h
--rwxr-xr-x   0        0        0     3034 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Multistep_Test.h
--rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Pong2_Test.h
--rwxr-xr-x   0        0        0     4272 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Pong_Test.h
--rwxr-xr-x   0        0        0     2084 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Procedure_Test.h
--rwxr-xr-x   0        0        0    16593 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Robot_Test.h
--rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Sequence_Test.h
--rwxr-xr-x   0        0        0    17000 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/Testchamber_Test.h
--rwxr-xr-x   0        0        0     2193 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/UDPNAR_Test.h
--rwxr-xr-x   0        0        0     2594 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/system_tests/system_tests.h
--rwxr-xr-x   0        0        0     5377 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/HashTable_Test.h
--rwxr-xr-x   0        0        0     4433 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/InvertedAtomIndex_Test.h
--rwxr-xr-x   0        0        0     2080 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/Memory_Test.h
--rwxr-xr-x   0        0        0     1973 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/Narsese_Test.h
--rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/OccurrenceTimeIndex_Test.h
--rwxr-xr-x   0        0        0     2280 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/PriorityQueue_Test.h
--rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/RuleTable_Test.h
--rwxr-xr-x   0        0        0     2426 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/Stack_Test.h
--rwxr-xr-x   0        0        0     1571 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/Stamp_Test.h
--rwxr-xr-x   0        0        0     2464 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/Table_Test.h
--rwxr-xr-x   0        0        0     2161 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/UDP_Test.h
--rwxr-xr-x   0        0        0     1721 2020-02-02 00:00:00.000000 narpyn-0.1.4/ona/src/unit_tests/unit_tests.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narpyn-0.1.4/tests/ona/__init__.py
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 narpyn-0.1.4/tests/ona/test_nar.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 narpyn-0.1.4/tests/ona/test_narsese.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 narpyn-0.1.4/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 narpyn-0.1.4/LICENSE
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 narpyn-0.1.4/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 narpyn-0.1.4/hatch.toml
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 narpyn-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 narpyn-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 narpyn-0.1.5/.gitattributes
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 narpyn-0.1.5/.gitmodules
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 narpyn-0.1.5/build_ona.sh
+-rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 narpyn-0.1.5/build_package.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narpyn-0.1.5/narpyn/ona/__init__.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 narpyn-0.1.5/narpyn/ona/nar.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 narpyn-0.1.5/narpyn/ona/narsese.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/.git
+-rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/.gitignore
+-rwxr-xr-x   0        0        0     3350 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/Dockerfile
+-rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/LICENSE
+-rwxr-xr-x   0        0        0     8257 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/README.md
+-rwxr-xr-x   0        0        0      755 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/build.sh
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/docker-compose.yml
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/install_python_dependencies.sh
+-rwxr-xr-x   0        0        0     1701 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/libbuild.sh
+-rwxr-xr-x   0        0        0      704 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/english/babi1.english
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/english/dialog.english
+-rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/english/disambiguate.english
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/english/grammar.english
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/english/prepositions.english
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/english/robotQA.english
+-rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/english/story1.english
+-rwxr-xr-x   0        0        0      422 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/english/story2.english
+-rwxr-xr-x   0        0        0      371 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/english/story3.english
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/english/story4.english
+-rwxr-xr-x   0        0        0      941 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/activequestion.nal
+-rwxr-xr-x   0        0        0     1288 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/asthma.nal
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/asthma2.nal
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/avoid.nal
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/avoid2.nal
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/avoid3.nal
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/catCAT.nal
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/categoryformationanddetection.nal
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/circus.nal
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/clapwave0.nal
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/clapwave1.nal
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/clapwave2.nal
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/clapwave3.nal
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/clapwave4.nal
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/clapwave5.nal
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/diagnostic.nal
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/door.nal
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/door2.nal
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/door3.nal
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/duck.nal
+-rwxr-xr-x   0        0        0    14725 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/example1.nal
+-rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/example2.nal
+-rwxr-xr-x   0        0        0      869 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/example3.nal
+-rwxr-xr-x   0        0        0      803 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/example4.nal
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/greenplant.nal
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/latch.nal
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/map.nal
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/map2.nal
+-rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/marshmallow.nal
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/numbers.nal
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/pickbrighter.nal
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/plandeep.nal
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/prefergeneral.nal
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/prefernext.nal
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/preferspecific.nal
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/propertymatching.nal
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/relationalnetwork.nal
+-rwxr-xr-x   0        0        0     3820 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/school.nal
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/self.nal
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/self2.nal
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/self3.nal
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/similarities.nal
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/spatial.nal
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/spatial3.nal
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/spatial4.nal
+-rwxr-xr-x   0        0        0     1371 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/symmetry.nal
+-rwxr-xr-x   0        0        0     1774 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/toothbrush.nal
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/examples/nal/whatwarmer.nal
+-rwxr-xr-x   0        0        0     2403 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Concept.h
+-rwxr-xr-x   0        0        0     7741 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Config.h
+-rwxr-xr-x   0        0        0    35264 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Cycle.c
+-rwxr-xr-x   0        0        0     1799 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Cycle.h
+-rwxr-xr-x   0        0        0    26640 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Decision.c
+-rwxr-xr-x   0        0        0     3336 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Decision.h
+-rwxr-xr-x   0        0        0     2753 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Event.c
+-rwxr-xr-x   0        0        0     2603 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Event.h
+-rwxr-xr-x   0        0        0     2150 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Globals.c
+-rwxr-xr-x   0        0        0     2673 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Globals.h
+-rwxr-xr-x   0        0        0     4760 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/HashTable.c
+-rwxr-xr-x   0        0        0     2640 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/HashTable.h
+-rwxr-xr-x   0        0        0     2044 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Implication.h
+-rwxr-xr-x   0        0        0     9629 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Inference.c
+-rwxr-xr-x   0        0        0     2972 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Inference.h
+-rwxr-xr-x   0        0        0     5349 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/InvertedAtomIndex.c
+-rwxr-xr-x   0        0        0     2334 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/InvertedAtomIndex.h
+-rwxr-xr-x   0        0        0    18958 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Memory.c
+-rwxr-xr-x   0        0        0     4219 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Memory.h
+-rwxr-xr-x   0        0        0    20399 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/NAL.c
+-rwxr-xr-x   0        0        0    14959 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/NAL.h
+-rwxr-xr-x   0        0        0    11792 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/NAR.c
+-rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/NAR.h
+-rwxr-xr-x   0        0        0    28145 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Narsese.c
+-rwxr-xr-x   0        0        0     4422 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Narsese.h
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/OccurrenceTimeIndex.c
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/OccurrenceTimeIndex.h
+-rwxr-xr-x   0        0        0     6777 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/PriorityQueue.c
+-rwxr-xr-x   0        0        0     3264 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/PriorityQueue.h
+-rwxr-xr-x   0        0        0     1922 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/RuleTable.h
+-rwxr-xr-x   0        0        0    14924 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Shell.c
+-rwxr-xr-x   0        0        0     1888 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Shell.h
+-rwxr-xr-x   0        0        0     1774 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Stack.c
+-rwxr-xr-x   0        0        0     1814 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Stack.h
+-rwxr-xr-x   0        0        0     3850 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Stamp.c
+-rwxr-xr-x   0        0        0     2253 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Stamp.h
+-rwxr-xr-x   0        0        0     3835 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Stats.c
+-rwxr-xr-x   0        0        0     1668 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Stats.h
+-rwxr-xr-x   0        0        0     4506 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Table.c
+-rwxr-xr-x   0        0        0     2530 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Table.h
+-rwxr-xr-x   0        0        0     3651 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Term.c
+-rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Term.h
+-rwxr-xr-x   0        0        0     7595 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Truth.c
+-rwxr-xr-x   0        0        0     3383 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Truth.h
+-rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Usage.c
+-rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Usage.h
+-rwxr-xr-x   0        0        0    18602 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Variable.c
+-rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/Variable.h
+-rwxr-xr-x   0        0        0     5197 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/main.c
+-rwxr-xr-x   0        0        0     1888 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/NetworkNAR/Metric.c
+-rwxr-xr-x   0        0        0     1655 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/NetworkNAR/Metric.h
+-rwxr-xr-x   0        0        0     2300 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/NetworkNAR/UDP.c
+-rwxr-xr-x   0        0        0     1938 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/NetworkNAR/UDP.h
+-rwxr-xr-x   0        0        0     3997 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/NetworkNAR/UDPNAR.c
+-rwxr-xr-x   0        0        0     1667 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/NetworkNAR/UDPNAR.h
+-rwxr-xr-x   0        0        0     4565 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Alien_Test.h
+-rwxr-xr-x   0        0        0     1645 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Alphabet_Test.h
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Bandrobot_Test.h
+-rwxr-xr-x   0        0        0     2938 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Cartpole_Test.h
+-rwxr-xr-x   0        0        0     3458 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Follow_Test.h
+-rwxr-xr-x   0        0        0     2767 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Multistep2_Test.h
+-rwxr-xr-x   0        0        0     3034 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Multistep_Test.h
+-rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Pong2_Test.h
+-rwxr-xr-x   0        0        0     4272 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Pong_Test.h
+-rwxr-xr-x   0        0        0     2084 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Procedure_Test.h
+-rwxr-xr-x   0        0        0    16593 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Robot_Test.h
+-rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Sequence_Test.h
+-rwxr-xr-x   0        0        0    17000 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/Testchamber_Test.h
+-rwxr-xr-x   0        0        0     2193 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/UDPNAR_Test.h
+-rwxr-xr-x   0        0        0     2594 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/system_tests/system_tests.h
+-rwxr-xr-x   0        0        0     5377 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/HashTable_Test.h
+-rwxr-xr-x   0        0        0     4433 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/InvertedAtomIndex_Test.h
+-rwxr-xr-x   0        0        0     2080 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/Memory_Test.h
+-rwxr-xr-x   0        0        0     1973 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/Narsese_Test.h
+-rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/OccurrenceTimeIndex_Test.h
+-rwxr-xr-x   0        0        0     2280 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/PriorityQueue_Test.h
+-rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/RuleTable_Test.h
+-rwxr-xr-x   0        0        0     2426 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/Stack_Test.h
+-rwxr-xr-x   0        0        0     1571 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/Stamp_Test.h
+-rwxr-xr-x   0        0        0     2464 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/Table_Test.h
+-rwxr-xr-x   0        0        0     2161 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/UDP_Test.h
+-rwxr-xr-x   0        0        0     1721 2020-02-02 00:00:00.000000 narpyn-0.1.5/ona/src/unit_tests/unit_tests.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narpyn-0.1.5/tests/ona/__init__.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 narpyn-0.1.5/tests/ona/test_nar.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 narpyn-0.1.5/tests/ona/test_narsese.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 narpyn-0.1.5/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 narpyn-0.1.5/LICENSE
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 narpyn-0.1.5/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 narpyn-0.1.5/hatch.toml
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 narpyn-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 narpyn-0.1.5/PKG-INFO
```

### Comparing `narpyn-0.1.4/narpyn/ona/nar.py` & `narpyn-0.1.5/narpyn/ona/nar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
+import os
 import subprocess
+from pathlib import Path
 
 from .narsese import *
 
 logger = logging.getLogger(__name__)
 
 
 def send_input(process: subprocess.Popen, input_: str) -> None:
@@ -83,15 +85,15 @@
         output = get_output(process)
     # ic("Got a matching output.")
     return output
 
 
 def setup_nars_ops(
     process: subprocess.Popen, ops: list[str], babblingops: Optional[int] = None
-):
+) -> None:
     """Setup NARS operations"""
     for i, op in enumerate(ops):
         send_input(process, f"*setopname {i+1} {op}")
     if babblingops is None:
         send_input(process, f"*babblingops={len(ops)}")
     else:
         send_input(process, f"*babblingops={babblingops}")
@@ -100,17 +102,46 @@
 def setup_nars(
     process: subprocess.Popen,
     ops: list[str],
     motor_babbling: Optional[float] = None,
     babblingops: Optional[int] = None,
     volume: Optional[int] = None,
     decision_threshold: Optional[float] = None,
-):
+) -> None:
     """Send NARS settings"""
     send_input(process, "*reset")
     setup_nars_ops(process, ops, babblingops=babblingops)
     if motor_babbling is not None:
         send_input(process, f"*motorbabbling={motor_babbling}")
     if volume is not None:
         send_input(process, f"*volume={volume}")
     if decision_threshold is not None:
         send_input(process, f"*decisionthreshold={decision_threshold}")
+
+
+def start_nars(
+    ops: list[str],
+    motor_babbling: Optional[float] = None,
+    babblingops: Optional[int] = None,
+    volume: Optional[int] = None,
+    decision_threshold: Optional[float] = None,
+) -> subprocess.Popen:
+    """Start an ONA process and set it up
+
+    Returns: process: subprocess.Popen: the object of the spawned subprocess.
+    """
+    # Start the ONA process
+    narspath = Path(os.environ["NARS_HOME"])
+    process_cmd = [
+        (narspath / "NAR").as_posix(),
+        "shell",
+    ]
+    process: subprocess.Popen = subprocess.Popen(
+        process_cmd,
+        stdin=subprocess.PIPE,
+        stdout=subprocess.PIPE,
+        universal_newlines=True,
+    )
+
+    # Configure ONA and return the process
+    setup_nars(process, ops, motor_babbling, babblingops, volume, decision_threshold)
+    return process
```

### Comparing `narpyn-0.1.4/narpyn/ona/narsese.py` & `narpyn-0.1.5/narpyn/ona/narsese.py`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/CODE_OF_CONDUCT.md` & `narpyn-0.1.5/ona/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/Dockerfile` & `narpyn-0.1.5/ona/Dockerfile`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/LICENSE` & `narpyn-0.1.5/ona/LICENSE`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/README.md` & `narpyn-0.1.5/ona/README.md`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/build.sh` & `narpyn-0.1.5/ona/build.sh`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/libbuild.sh` & `narpyn-0.1.5/ona/libbuild.sh`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/english/babi1.english` & `narpyn-0.1.5/ona/examples/english/babi1.english`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/english/dialog.english` & `narpyn-0.1.5/ona/examples/english/dialog.english`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/english/disambiguate.english` & `narpyn-0.1.5/ona/examples/english/disambiguate.english`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/english/grammar.english` & `narpyn-0.1.5/ona/examples/english/grammar.english`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/english/robotQA.english` & `narpyn-0.1.5/ona/examples/english/robotQA.english`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/english/story4.english` & `narpyn-0.1.5/ona/examples/english/story4.english`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/activequestion.nal` & `narpyn-0.1.5/ona/examples/nal/activequestion.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/asthma.nal` & `narpyn-0.1.5/ona/examples/nal/asthma.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/asthma2.nal` & `narpyn-0.1.5/ona/examples/nal/asthma2.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/catCAT.nal` & `narpyn-0.1.5/ona/examples/nal/catCAT.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/categoryformationanddetection.nal` & `narpyn-0.1.5/ona/examples/nal/categoryformationanddetection.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/circus.nal` & `narpyn-0.1.5/ona/examples/nal/circus.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/clapwave2.nal` & `narpyn-0.1.5/ona/examples/nal/clapwave2.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/clapwave3.nal` & `narpyn-0.1.5/ona/examples/nal/clapwave3.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/clapwave4.nal` & `narpyn-0.1.5/ona/examples/nal/clapwave4.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/clapwave5.nal` & `narpyn-0.1.5/ona/examples/nal/clapwave5.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/diagnostic.nal` & `narpyn-0.1.5/ona/examples/nal/diagnostic.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/example1.nal` & `narpyn-0.1.5/ona/examples/nal/example1.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/example2.nal` & `narpyn-0.1.5/ona/examples/nal/example2.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/example3.nal` & `narpyn-0.1.5/ona/examples/nal/example3.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/example4.nal` & `narpyn-0.1.5/ona/examples/nal/example4.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/map.nal` & `narpyn-0.1.5/ona/examples/nal/map.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/map2.nal` & `narpyn-0.1.5/ona/examples/nal/map2.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/marshmallow.nal` & `narpyn-0.1.5/ona/examples/nal/marshmallow.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/numbers.nal` & `narpyn-0.1.5/ona/examples/nal/numbers.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/prefergeneral.nal` & `narpyn-0.1.5/ona/examples/nal/prefergeneral.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/prefernext.nal` & `narpyn-0.1.5/ona/examples/nal/prefernext.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/preferspecific.nal` & `narpyn-0.1.5/ona/examples/nal/preferspecific.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/propertymatching.nal` & `narpyn-0.1.5/ona/examples/nal/propertymatching.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/relationalnetwork.nal` & `narpyn-0.1.5/ona/examples/nal/relationalnetwork.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/school.nal` & `narpyn-0.1.5/ona/examples/nal/school.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/similarities.nal` & `narpyn-0.1.5/ona/examples/nal/similarities.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/symmetry.nal` & `narpyn-0.1.5/ona/examples/nal/symmetry.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/examples/nal/toothbrush.nal` & `narpyn-0.1.5/ona/examples/nal/toothbrush.nal`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Concept.h` & `narpyn-0.1.5/ona/src/Concept.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Config.h` & `narpyn-0.1.5/ona/src/Config.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Cycle.c` & `narpyn-0.1.5/ona/src/Cycle.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Cycle.h` & `narpyn-0.1.5/ona/src/Cycle.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Decision.c` & `narpyn-0.1.5/ona/src/Decision.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Decision.h` & `narpyn-0.1.5/ona/src/Decision.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Event.c` & `narpyn-0.1.5/ona/src/Event.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Event.h` & `narpyn-0.1.5/ona/src/Event.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Globals.c` & `narpyn-0.1.5/ona/src/Globals.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Globals.h` & `narpyn-0.1.5/ona/src/Globals.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/HashTable.c` & `narpyn-0.1.5/ona/src/HashTable.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/HashTable.h` & `narpyn-0.1.5/ona/src/HashTable.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Implication.h` & `narpyn-0.1.5/ona/src/Implication.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Inference.c` & `narpyn-0.1.5/ona/src/Inference.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Inference.h` & `narpyn-0.1.5/ona/src/Inference.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/InvertedAtomIndex.c` & `narpyn-0.1.5/ona/src/InvertedAtomIndex.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/InvertedAtomIndex.h` & `narpyn-0.1.5/ona/src/InvertedAtomIndex.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Memory.c` & `narpyn-0.1.5/ona/src/Memory.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Memory.h` & `narpyn-0.1.5/ona/src/Memory.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/NAL.c` & `narpyn-0.1.5/ona/src/NAL.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/NAL.h` & `narpyn-0.1.5/ona/src/NAL.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/NAR.c` & `narpyn-0.1.5/ona/src/NAR.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/NAR.h` & `narpyn-0.1.5/ona/src/NAR.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Narsese.c` & `narpyn-0.1.5/ona/src/Narsese.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Narsese.h` & `narpyn-0.1.5/ona/src/Narsese.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/OccurrenceTimeIndex.c` & `narpyn-0.1.5/ona/src/OccurrenceTimeIndex.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/OccurrenceTimeIndex.h` & `narpyn-0.1.5/ona/src/OccurrenceTimeIndex.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/PriorityQueue.c` & `narpyn-0.1.5/ona/src/PriorityQueue.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/PriorityQueue.h` & `narpyn-0.1.5/ona/src/PriorityQueue.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/RuleTable.h` & `narpyn-0.1.5/ona/src/RuleTable.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Shell.c` & `narpyn-0.1.5/ona/src/Shell.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Shell.h` & `narpyn-0.1.5/ona/src/Shell.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Stack.c` & `narpyn-0.1.5/ona/src/Stack.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Stack.h` & `narpyn-0.1.5/ona/src/Stack.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Stamp.c` & `narpyn-0.1.5/ona/src/Stamp.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Stamp.h` & `narpyn-0.1.5/ona/src/Stamp.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Stats.c` & `narpyn-0.1.5/ona/src/Stats.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Stats.h` & `narpyn-0.1.5/ona/src/Stats.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Table.c` & `narpyn-0.1.5/ona/src/Table.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Table.h` & `narpyn-0.1.5/ona/src/Table.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Term.c` & `narpyn-0.1.5/ona/src/Term.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Term.h` & `narpyn-0.1.5/ona/src/Term.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Truth.c` & `narpyn-0.1.5/ona/src/Truth.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Truth.h` & `narpyn-0.1.5/ona/src/Truth.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Usage.c` & `narpyn-0.1.5/ona/src/Usage.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Usage.h` & `narpyn-0.1.5/ona/src/Usage.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Variable.c` & `narpyn-0.1.5/ona/src/Variable.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/Variable.h` & `narpyn-0.1.5/ona/src/Variable.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/main.c` & `narpyn-0.1.5/ona/src/main.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/NetworkNAR/Metric.c` & `narpyn-0.1.5/ona/src/NetworkNAR/Metric.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/NetworkNAR/Metric.h` & `narpyn-0.1.5/ona/src/NetworkNAR/Metric.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/NetworkNAR/UDP.c` & `narpyn-0.1.5/ona/src/NetworkNAR/UDP.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/NetworkNAR/UDP.h` & `narpyn-0.1.5/ona/src/NetworkNAR/UDP.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/NetworkNAR/UDPNAR.c` & `narpyn-0.1.5/ona/src/NetworkNAR/UDPNAR.c`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/NetworkNAR/UDPNAR.h` & `narpyn-0.1.5/ona/src/NetworkNAR/UDPNAR.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Alien_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Alien_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Alphabet_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Alphabet_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Bandrobot_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Bandrobot_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Cartpole_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Cartpole_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Follow_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Follow_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Multistep2_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Multistep2_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Multistep_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Multistep_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Pong2_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Pong2_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Pong_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Pong_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Procedure_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Procedure_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Robot_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Robot_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Sequence_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Sequence_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/Testchamber_Test.h` & `narpyn-0.1.5/ona/src/system_tests/Testchamber_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/UDPNAR_Test.h` & `narpyn-0.1.5/ona/src/system_tests/UDPNAR_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/system_tests/system_tests.h` & `narpyn-0.1.5/ona/src/system_tests/system_tests.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/HashTable_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/HashTable_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/InvertedAtomIndex_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/InvertedAtomIndex_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/Memory_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/Memory_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/Narsese_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/Narsese_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/OccurrenceTimeIndex_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/OccurrenceTimeIndex_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/PriorityQueue_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/PriorityQueue_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/RuleTable_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/RuleTable_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/Stack_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/Stack_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/Stamp_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/Stamp_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/Table_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/Table_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/UDP_Test.h` & `narpyn-0.1.5/ona/src/unit_tests/UDP_Test.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/ona/src/unit_tests/unit_tests.h` & `narpyn-0.1.5/ona/src/unit_tests/unit_tests.h`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/tests/ona/test_nar.py` & `narpyn-0.1.5/tests/ona/test_nar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from unittest.mock import Mock, patch, call
+from unittest.mock import Mock, call, patch
 
 from narpyn.ona.nar import (
     expect_output,
     get_output,
     get_raw_output,
     send_input,
     setup_nars,
@@ -68,15 +68,18 @@
     assert len(output["answers"]) == 1
     assert output["answers"][0] == {
         "occurrenceTime": "5",
         "punctuation": "!",
         "term": "^op1 ({SELF} * arg)",
     }
     assert len(output["executions"]) == 1
-    assert output["executions"][0] == {"operator": "^op1", "arguments": ["{SELF}", "arg"]}
+    assert output["executions"][0] == {
+        "operator": "^op1",
+        "arguments": ["{SELF}", "arg"],
+    }
     assert (
         output["raw"]
         == "Input: task1! :|: occurrenceTime=5\nDerived: task2! :|: occurrenceTime=5\nRevised: sent. :|: occurrenceTime=2\nAnswer: ^op1 ({SELF} * arg)! :|: occurrenceTime=5\n^op1 executed with args ({SELF} * arg)"
     )
 
 
 @patch("subprocess.Popen")
@@ -129,22 +132,30 @@
 def test_setup_nars_ops(mock_popen):
     mock_stdin = Mock()
     mock_stdout = Mock()
     mock_popen.return_value = Mock(stdin=mock_stdin, stdout=mock_stdout)
     ops = ["op1", "op2"]
     setup_nars_ops(mock_popen(), ops)
     mock_stdin.write.assert_has_calls(
-        [call("*setopname 1 op1\n"), call("*setopname 2 op2\n"), call(f"*babblingops={len(ops)}\n")]
+        [
+            call("*setopname 1 op1\n"),
+            call("*setopname 2 op2\n"),
+            call(f"*babblingops={len(ops)}\n"),
+        ]
     )
     mock_stdin.flush.assert_has_calls([call()] * 3)
     send_input_calls = [call(mock_popen(), f"*babblingops={len(ops)}")]
     setup_nars_ops(mock_popen(), ops, babblingops=5)
     send_input_calls.append(call(mock_popen(), "*babblingops=5"))
     mock_stdin.write.assert_has_calls(
-        [call("*setopname 1 op1\n"), call("*setopname 2 op2\n"), call("*babblingops=5\n")]
+        [
+            call("*setopname 1 op1\n"),
+            call("*setopname 2 op2\n"),
+            call("*babblingops=5\n"),
+        ]
     )
     mock_stdin.flush.assert_has_calls([call()] * 3)
     assert mock_stdin.write.call_count == 6
 
 
 @patch("subprocess.Popen")
 def test_setup_nars(mock_popen):
```

### Comparing `narpyn-0.1.4/tests/ona/test_narsese.py` & `narpyn-0.1.5/tests/ona/test_narsese.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 # Test parse_task function
 def test_parse_task():
     assert parse_task("task! :|: occurrenceTime=3 Truth: f=0.7 c=0.89") == {
         "occurrenceTime": "3",
         "punctuation": "!",
         "term": "task",
-        'truth': {'frequency': 0.7, 'confidence': 0.89},
+        "truth": {"frequency": 0.7, "confidence": 0.89},
     }
     assert parse_task(
         "task! occurrenceTime=eternal Priority=1.0 Truth: f=0.5 c=0.9"
     ) == {
         "occurrenceTime": "eternal",
         "punctuation": "!",
         "term": "task",
```

### Comparing `narpyn-0.1.4/.gitignore` & `narpyn-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/LICENSE` & `narpyn-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/hatch.toml` & `narpyn-0.1.5/hatch.toml`

 * *Files identical despite different names*

### Comparing `narpyn-0.1.4/pyproject.toml` & `narpyn-0.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -16,19 +16,34 @@
 pytest = "^7.3.1"
 ipython = "^8.14.0"
 
 [project]
 name = "narpyn"
 dynamic = ["version"]
 description = "A Python API library for NARS"
+keywords = [
+  "nars",
+  "ai",
+]
 authors = [{name = "Adrian Borucki", email = "ab@synthillect.ai"}]
+classifiers = [
+  "Development Status :: 3 - Alpha",
+  "License :: OSI Approved :: Apache Software License",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: Implementation :: CPython",
+]
 license = "Apache-2.0"
 readme = "README.md"
 requires-python = ">=3.10"
 
+#[project.scripts]
+#NAR = "NAR:NAR"
+
 [build-system]
 requires = ["hatchling>=1.17.0", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 source = "vcs"
 
@@ -53,15 +68,15 @@
   "/ona/*.py",
   "/tests",
 ]
 
 [tool.hatch.build.targets.wheel.hooks.autorun]
 dependencies = ["hatch-autorun"]
 code = """
-os.environ["NARS_HOME"] = os.path.dirname(os.path.abspath(__file__)) + "/ona"
+from pathlib import Path; os.environ["NARS_HOME"] = (Path(sys.path[0]) / ".." / "lib" / f"python{sys.version_info.major}.{sys.version_info.minor}" / "site-packages" / "ona").as_posix()
 """
 
 [tool.hatch.build.targets.wheel.hooks.mypyc]
 enable-by-default = false
 dependencies = ["hatch-mypyc>=0.14.1"]
 require-runtime-dependencies = true
 mypy-args = [
```

