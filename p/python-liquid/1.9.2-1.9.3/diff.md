# Comparing `tmp/python_liquid-1.9.2.tar.gz` & `tmp/python_liquid-1.9.3.tar.gz`

## Comparing `python_liquid-1.9.2.tar` & `python_liquid-1.9.3.tar`

### file list

```diff
@@ -1,182 +1,183 @@
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/__init__.py
--rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/analyze_tags.py
--rw-r--r--   0        0        0     8313 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/ast.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/chain_map.py
--rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/context.py
--rw-r--r--   0        0        0    30422 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/environment.py
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/exceptions.py
--rw-r--r--   0        0        0    34912 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expression.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/filter.py
--rw-r--r--   0        0        0    15137 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/lex.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/limits.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/loaders.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/mode.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/output.py
--rw-r--r--   0        0        0    27025 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/py.typed
--rw-r--r--   0        0        0    33438 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/static_analysis.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/stream.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/stringify.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/tag.py
--rw-r--r--   0        0        0    16970 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/template.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/token.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/undefined.py
--rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/illegal.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/literal.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/statement.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/drops/__init__.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/drops/drops.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/filters/__init__.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/filters/array.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/filters/extra.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/filters/math.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/filters/misc.py
--rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/filters/string.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/loaders/__init__.py
--rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/loaders/base_loader.py
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/loaders/caching_file_system_loader.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/loaders/choice_loader.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/loaders/file_system_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/__init__.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/assign_tag.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/capture_tag.py
--rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/case_tag.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/comment_tag.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/cycle_tag.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/decrement_tag.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/echo_tag.py
--rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/for_tag.py
--rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/if_tag.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/ifchanged_tag.py
--rw-r--r--   0        0        0     9238 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/include_tag.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/increment_tag.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/inline_comment_tag.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/liquid_tag.py
--rw-r--r--   0        0        0    11639 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/render_tag.py
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/tablerow_tag.py
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/builtin/tags/unless_tag.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/__init__.py
--rw-r--r--   0        0        0    11693 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/common.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/stream.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/arguments/__init__.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/arguments/lex.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/arguments/parse.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/boolean/__init__.py
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/boolean/lex.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/boolean/parse.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/conditional/__init__.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/conditional/lex.py
--rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/conditional/parse.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/filtered/__init__.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/filtered/lex.py
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/filtered/parse.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/include/__init__.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/include/lex.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/loop/__init__.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/loop/lex.py
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/expressions/loop/parse.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/__init__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/filters/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/filters/_json.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/filters/array.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/filters/html.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/tags/__init__.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/tags/_with.py
--rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/tags/extends.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/tags/if_expressions.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/tags/if_not.py
--rw-r--r--   0        0        0    10144 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/extra/tags/macro.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/future/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/future/environment.py
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/__init__.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/abs_filter.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/append_filter.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/assign_tag.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/at_least_filter.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/at_most_filter.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/base64_decode_filter.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/base64_encode_filter.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/base64_url_safe_decode_filter.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/base64_url_safe_encode_filter.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/capitalize_filter.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/capture_tag.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/case.py
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/case_tag.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/ceil_filter.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/comment_tag.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/compact_filter.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/concat_filter.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/cycle_tag.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/date_filter.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/decrement_tag.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/default_filter.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/divided_by_filter.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/downcase_filter.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/echo_tag.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/escape_filter.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/escape_once_filter.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/first_filter.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/floor_filter.py
--rw-r--r--   0        0        0    20459 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/for_tag.py
--rw-r--r--   0        0        0     7364 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/identifiers.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/if_tag.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/ifchanged_tag.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/illegal.py
--rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/include_tag.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/increment_tag.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/inline_comment_tag.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/join_filter.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/last_filter.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/liquid_tag.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/lstrip_filter.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/map_filter.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/minus_filter.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/modulo_filter.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/newline_to_br_filter.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/not_liquid.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/output_statement.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/plus_filter.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/prepend_filter.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/range_objects.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/raw_tag.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/remove_filter.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/remove_first_filter.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/remove_last_filter.py
--rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/render_tag.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/replace_filter.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/replace_first_filter.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/replace_last_filter.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/reverse_filter.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/round_filter.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/rstrip_filter.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/size_filter.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/slice_filter.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/sort_filter.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/sort_natural_filter.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/special.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/split_filter.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/strip_filter.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/strip_html_filter.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/strip_newlines_filter.py
--rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/tablerow_tag.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/times_filter.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/truncate_filter.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/truncatewords_filter.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/uniq_filter.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/unless_tag.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/upcase_filter.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/url_decode_filter.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/url_encode_filter.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/where_filter.py
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/golden/whitespace_control.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/utils/__init__.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/utils/cache.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/utils/cache.pyi
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/utils/html.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 python_liquid-1.9.2/liquid/utils/text.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 python_liquid-1.9.2/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 python_liquid-1.9.2/LICENSE
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 python_liquid-1.9.2/README.md
--rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 python_liquid-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 python_liquid-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/__init__.py
+-rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/analyze_tags.py
+-rw-r--r--   0        0        0     8313 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/ast.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/chain_map.py
+-rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/context.py
+-rw-r--r--   0        0        0    30571 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/environment.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/exceptions.py
+-rw-r--r--   0        0        0    34912 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expression.py
+-rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/filter.py
+-rw-r--r--   0        0        0    15137 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/lex.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/limits.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/loaders.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/mode.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/output.py
+-rw-r--r--   0        0        0    27025 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/py.typed
+-rw-r--r--   0        0        0    33438 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/static_analysis.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/stream.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/stringify.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/tag.py
+-rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/template.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/token.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/undefined.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/illegal.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/literal.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/statement.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/drops/__init__.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/drops/drops.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/filters/__init__.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/filters/array.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/filters/extra.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/filters/math.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/filters/misc.py
+-rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/filters/string.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/loaders/__init__.py
+-rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/loaders/base_loader.py
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/loaders/caching_file_system_loader.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/loaders/choice_loader.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/loaders/file_system_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/__init__.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/assign_tag.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/capture_tag.py
+-rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/case_tag.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/comment_tag.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/cycle_tag.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/decrement_tag.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/echo_tag.py
+-rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/for_tag.py
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/if_tag.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/ifchanged_tag.py
+-rw-r--r--   0        0        0     9238 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/include_tag.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/increment_tag.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/inline_comment_tag.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/liquid_tag.py
+-rw-r--r--   0        0        0    11639 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/render_tag.py
+-rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/tablerow_tag.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/builtin/tags/unless_tag.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/__init__.py
+-rw-r--r--   0        0        0    11693 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/common.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/stream.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/arguments/__init__.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/arguments/lex.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/arguments/parse.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/boolean/__init__.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/boolean/lex.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/boolean/parse.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/conditional/__init__.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/conditional/lex.py
+-rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/conditional/parse.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/filtered/__init__.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/filtered/lex.py
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/filtered/parse.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/include/__init__.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/include/lex.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/loop/__init__.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/loop/lex.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/expressions/loop/parse.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/__init__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/filters/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/filters/_json.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/filters/array.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/filters/html.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/tags/__init__.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/tags/_with.py
+-rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/tags/extends.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/tags/if_expressions.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/tags/if_not.py
+-rw-r--r--   0        0        0    10144 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/extra/tags/macro.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/future/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/future/environment.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/__init__.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/abs_filter.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/append_filter.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/assign_tag.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/at_least_filter.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/at_most_filter.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/base64_decode_filter.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/base64_encode_filter.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/base64_url_safe_decode_filter.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/base64_url_safe_encode_filter.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/capitalize_filter.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/capture_tag.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/case.py
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/case_tag.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/ceil_filter.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/comment_tag.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/compact_filter.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/concat_filter.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/cycle_tag.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/date_filter.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/decrement_tag.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/default_filter.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/divided_by_filter.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/downcase_filter.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/echo_tag.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/escape_filter.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/escape_once_filter.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/first_filter.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/floor_filter.py
+-rw-r--r--   0        0        0    20459 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/for_tag.py
+-rw-r--r--   0        0        0     7364 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/identifiers.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/if_tag.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/ifchanged_tag.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/illegal.py
+-rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/include_tag.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/increment_tag.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/inline_comment_tag.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/join_filter.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/last_filter.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/liquid_tag.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/lstrip_filter.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/map_filter.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/minus_filter.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/modulo_filter.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/newline_to_br_filter.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/not_liquid.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/output_statement.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/plus_filter.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/prepend_filter.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/range_objects.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/raw_tag.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/remove_filter.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/remove_first_filter.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/remove_last_filter.py
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/render_tag.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/replace_filter.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/replace_first_filter.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/replace_last_filter.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/reverse_filter.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/round_filter.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/rstrip_filter.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/size_filter.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/slice_filter.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/sort_filter.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/sort_natural_filter.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/special.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/split_filter.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/strip_filter.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/strip_html_filter.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/strip_newlines_filter.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/sum_filter.py
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/tablerow_tag.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/times_filter.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/truncate_filter.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/truncatewords_filter.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/uniq_filter.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/unless_tag.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/upcase_filter.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/url_decode_filter.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/url_encode_filter.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/where_filter.py
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/golden/whitespace_control.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/utils/__init__.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/utils/cache.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/utils/cache.pyi
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/utils/html.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 python_liquid-1.9.3/liquid/utils/text.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 python_liquid-1.9.3/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 python_liquid-1.9.3/LICENSE
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 python_liquid-1.9.3/README.md
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 python_liquid-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 python_liquid-1.9.3/PKG-INFO
```

### Comparing `python_liquid-1.9.2/liquid/__init__.py` & `python_liquid-1.9.3/liquid/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from .analyze_tags import DEFAULT_INNER_TAG_MAP
 
 from .static_analysis import TemplateAnalysis
 from .static_analysis import ContextualTemplateAnalysis
 
 from . import future
 
-__version__ = "1.9.2"
+__version__ = "1.9.3"
 
 __all__ = (
     "AwareBoundTemplate",
     "BoundTemplate",
     "CachingFileSystemLoader",
     "ChoiceLoader",
     "Context",
```

### Comparing `python_liquid-1.9.2/liquid/analyze_tags.py` & `python_liquid-1.9.3/liquid/analyze_tags.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/ast.py` & `python_liquid-1.9.3/liquid/ast.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/chain_map.py` & `python_liquid-1.9.3/liquid/chain_map.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/context.py` & `python_liquid-1.9.3/liquid/context.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/environment.py` & `python_liquid-1.9.3/liquid/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
             self.parse_boolean_expression_value_with_parens,
             self.parse_conditional_expression_value,
             self.parse_conditional_expression_value_with_parens,
             self.parse_filtered_expression_value,
             self.parse_loop_expression_value,
         ) = self._get_expression_parsers(self.expression_cache_size)
 
-        builtin.register(self)
+        self.setup_tags_and_filters()
 
     def __hash__(self) -> int:
         return hash(
             (
                 self.statement_start_string,
                 self.statement_end_string,
                 self.tag_start_string,
@@ -286,14 +286,18 @@
                 expression the filter is applied to. If the filter needs access to the
                 environment or render context, you probably want to make `func` a class
                 that inherits from `liquid.filter.Filter`, and override the
                 `__call__` method. All builtin filters are implemented in this way.
         """
         self.filters[name] = func
 
+    def setup_tags_and_filters(self) -> None:
+        """Add default tags and filters to this environment."""
+        builtin.register(self)
+
     def parse(self, source: str) -> ast.ParseTree:
         """Parse `source` as a liquid template.
 
         More often than not you'll want to use `Environment.from_string` instead.
         """
         parser = get_parser(self)
         token_iter = self.tokenizer()(source)
```

### Comparing `python_liquid-1.9.2/liquid/exceptions.py` & `python_liquid-1.9.3/liquid/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,16 +124,15 @@
 
 
 class TemplateNotFound(Error):
     """Exception raised when a template could not be found."""
 
     def __str__(self) -> str:
         msg = super().__str__()
-        msg = f"template not found {msg}"
-        return msg
+        return f"template not found {msg}"
 
 
 class ResourceLimitError(Error):
     """Base class for exceptions relating to resource limits."""
 
 
 class ContextDepthError(ResourceLimitError):
```

### Comparing `python_liquid-1.9.2/liquid/expression.py` & `python_liquid-1.9.3/liquid/expression.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/filter.py` & `python_liquid-1.9.3/liquid/filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Filter function helpers."""
 
 from __future__ import annotations
 
+from decimal import Decimal
 from functools import wraps
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 from typing import Iterable
 from typing import Iterator
 from typing import List
@@ -145,14 +146,49 @@
         except ValueError as err:
             if default is not None:
                 return default
             raise FilterArgumentError(
                 f"could not cast string '{val}' to a number"
             ) from err
 
+    elif default is not None:
+        return default
+
+    raise FilterArgumentError(
+        f"expected an int, float or string, found {type(val).__name__}"
+    )
+
+
+def decimal_arg(
+    val: Any, default: Union[int, Decimal, None] = None
+) -> Union[int, Decimal]:
+    """Return `val` as an int or decimal.
+
+    If `val` can't be cast to an int or decimal, return `default`.
+    """
+    if isinstance(val, int):
+        return val
+    if isinstance(val, float):
+        return Decimal(str(val))
+
+    if isinstance(val, str):
+        try:
+            return to_int(val)
+        except ValueError:
+            pass
+
+        try:
+            return Decimal(val)
+        except ValueError as err:
+            if default is not None:
+                return default
+            raise FilterArgumentError(
+                f"could not cast string '{val}' to a number"
+            ) from err
+
     elif default is not None:
         return default
 
     raise FilterArgumentError(
         f"expected an int, float or string, found {type(val).__name__}"
     )
```

### Comparing `python_liquid-1.9.2/liquid/lex.py` & `python_liquid-1.9.3/liquid/lex.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/limits.py` & `python_liquid-1.9.3/liquid/limits.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/loaders.py` & `python_liquid-1.9.3/liquid/loaders.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/output.py` & `python_liquid-1.9.3/liquid/output.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/parse.py` & `python_liquid-1.9.3/liquid/parse.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/static_analysis.py` & `python_liquid-1.9.3/liquid/static_analysis.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/stream.py` & `python_liquid-1.9.3/liquid/stream.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/stringify.py` & `python_liquid-1.9.3/liquid/stringify.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/tag.py` & `python_liquid-1.9.3/liquid/tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/template.py` & `python_liquid-1.9.3/liquid/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,18 +255,15 @@
         """Return a namespace dictionary.
 
         This is used by `render_with_context` to extend an existing context.
         """
         return {**render_args, "partial": partial}
 
     def __repr__(self) -> str:
-        return (
-            f"Template(name='{self.name}', "
-            f"path='{self.path}', uptodate={self.is_up_to_date})"
-        )  # pragma: no cover
+        return f"Template(name='{self.name}', path='{self.path}')"  # pragma: no cover
 
     def analyze(
         self, follow_partials: bool = True, raise_for_failures: bool = True
     ) -> TemplateAnalysis:
         """Statically analyze this template and any included/rendered templates.
 
         Args:
```

### Comparing `python_liquid-1.9.2/liquid/token.py` & `python_liquid-1.9.3/liquid/token.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/undefined.py` & `python_liquid-1.9.3/liquid/undefined.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/__init__.py` & `python_liquid-1.9.3/liquid/builtin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .filters.array import first
 from .filters.array import join
 from .filters.array import last
 from .filters.array import map_
 from .filters.array import reverse
 from .filters.array import sort
 from .filters.array import sort_natural
+from .filters.array import sum_
 from .filters.array import uniq
 from .filters.array import where
 from .filters.extra import safe
 from .filters.math import abs_
 from .filters.math import at_least
 from .filters.math import at_most
 from .filters.math import ceil
@@ -153,14 +154,15 @@
     env.add_filter("first", first)
     env.add_filter("last", last)
     env.add_filter("concat", concat)
     env.add_filter("map", map_)
     env.add_filter("reverse", reverse)
     env.add_filter("sort", sort)
     env.add_filter("sort_natural", sort_natural)
+    env.add_filter("sum", sum_)
     env.add_filter("where", where)
     env.add_filter("uniq", uniq)
     env.add_filter("compact", compact)
 
     env.add_filter("size", size)
     env.add_filter("default", default)
     env.add_filter("date", date)
```

### Comparing `python_liquid-1.9.2/liquid/builtin/illegal.py` & `python_liquid-1.9.3/liquid/builtin/illegal.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/literal.py` & `python_liquid-1.9.3/liquid/builtin/literal.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/statement.py` & `python_liquid-1.9.3/liquid/builtin/statement.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/filters/array.py` & `python_liquid-1.9.3/liquid/builtin/filters/array.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Filter functions that operate on arrays."""
 from __future__ import annotations
 
+from decimal import Decimal
 from functools import partial
 from itertools import chain
 from itertools import islice
 from operator import getitem
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Iterable
@@ -18,14 +19,15 @@
 except ImportError:
     from liquid.exceptions import Markup  # type: ignore
 
 from liquid.exceptions import FilterArgumentError
 from liquid.exceptions import FilterError
 from liquid.expression import NIL
 from liquid.filter import array_filter
+from liquid.filter import decimal_arg
 from liquid.filter import liquid_filter
 from liquid.filter import sequence_filter
 from liquid.filter import with_environment
 from liquid.undefined import is_undefined
 
 if TYPE_CHECKING:
     from liquid import Environment
@@ -121,15 +123,15 @@
 
     if is_undefined(sequence):
         return second_array
 
     return list(chain(sequence, second_array))
 
 
-@liquid_filter
+@sequence_filter
 def map_(sequence: ArrayT, key: object) -> List[object]:
     """Create an array of values from a map."""
     try:
         return [_getitem(itm, str(key), default=NIL) for itm in sequence]
     except TypeError as err:
         raise FilterError("can't map sequence") from err
 
@@ -210,7 +212,23 @@
     """Removes any nil values from an array."""
     if key is not None:
         try:
             return [itm for itm in sequence if itm[key] is not None]
         except TypeError as err:
             raise FilterArgumentError(f"can't read property '{key}'") from err
     return [itm for itm in sequence if itm is not None]
+
+
+@sequence_filter
+def sum_(sequence: ArrayT, key: object = None) -> Union[float, int, Decimal]:
+    """Return the sum of all numeric elements in an array.
+
+    If _key_ is given, it is assumed that sequence items are mapping-like,
+    and the values at _item[key]_ will be summed instead.
+    """
+    if key is not None and not is_undefined(key):
+        rv = sum(decimal_arg(_getitem(elem, key, 0), 0) for elem in sequence)
+    else:
+        rv = sum(decimal_arg(elem, 0) for elem in sequence)
+    if isinstance(rv, Decimal):
+        return float(rv)
+    return rv
```

### Comparing `python_liquid-1.9.2/liquid/builtin/filters/extra.py` & `python_liquid-1.9.3/liquid/builtin/filters/extra.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/filters/math.py` & `python_liquid-1.9.3/liquid/builtin/filters/math.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/filters/misc.py` & `python_liquid-1.9.3/liquid/builtin/filters/misc.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/filters/string.py` & `python_liquid-1.9.3/liquid/builtin/filters/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,16 +172,15 @@
         rv = to_int(val)
     except (ValueError, TypeError) as err:
         raise FilterArgumentError(
             f"slice expected an integer start, found {type(val).__name__}"
         ) from err
 
     rv = min(rv, MAX_SLICE_ARG)
-    rv = max(rv, MIN_SLICE_ARG)
-    return rv
+    return max(rv, MIN_SLICE_ARG)
 
 
 @liquid_filter
 def slice_(val: Any, start: Any, length: Any = 1) -> Union[str, List[object]]:
     """Return the subsequence of _val_ starting at _start_ with up to _length_ chars.
 
     Array-like objects return a list, strings return a substring, all other objects are
```

### Comparing `python_liquid-1.9.2/liquid/builtin/loaders/__init__.py` & `python_liquid-1.9.3/liquid/builtin/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/loaders/base_loader.py` & `python_liquid-1.9.3/liquid/builtin/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/loaders/caching_file_system_loader.py` & `python_liquid-1.9.3/liquid/builtin/loaders/caching_file_system_loader.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/loaders/choice_loader.py` & `python_liquid-1.9.3/liquid/builtin/loaders/choice_loader.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/loaders/file_system_loader.py` & `python_liquid-1.9.3/liquid/builtin/loaders/file_system_loader.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/assign_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/assign_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/capture_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/capture_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/case_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/case_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/comment_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/comment_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/cycle_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/cycle_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/decrement_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/decrement_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/echo_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/echo_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/for_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/for_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/if_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/if_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/ifchanged_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/ifchanged_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/include_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/include_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/increment_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/increment_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/inline_comment_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/inline_comment_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/liquid_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/liquid_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,17 @@
         expect(stream, TOKEN_TAG, value=TAG_LIQUID)
         tok = stream.current
         stream.next_token()
 
         if stream.current.type == TOKEN_EOF:
             # Empty liquid tag. Empty block.
             block = BlockNode(tok, [])
+        elif stream.current.type == TOKEN_TAG:
+            parser = get_parser(self.env)
+            block = parser.parse_block(stream, end=())
         else:
             expect(stream, TOKEN_EXPRESSION)
             expr_stream = TokenStream(
                 self.tokenize_liquid_expression(
                     stream.current.value, line_count=stream.current.linenum
                 )
             )
```

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/render_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/render_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/tablerow_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/tablerow_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/builtin/tags/unless_tag.py` & `python_liquid-1.9.3/liquid/builtin/tags/unless_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/__init__.py` & `python_liquid-1.9.3/liquid/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/common.py` & `python_liquid-1.9.3/liquid/expressions/common.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/stream.py` & `python_liquid-1.9.3/liquid/expressions/stream.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/arguments/lex.py` & `python_liquid-1.9.3/liquid/expressions/arguments/lex.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/arguments/parse.py` & `python_liquid-1.9.3/liquid/expressions/arguments/parse.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/boolean/lex.py` & `python_liquid-1.9.3/liquid/expressions/boolean/lex.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/boolean/parse.py` & `python_liquid-1.9.3/liquid/expressions/boolean/parse.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/conditional/lex.py` & `python_liquid-1.9.3/liquid/expressions/conditional/lex.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/conditional/parse.py` & `python_liquid-1.9.3/liquid/expressions/conditional/parse.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/filtered/lex.py` & `python_liquid-1.9.3/liquid/expressions/filtered/lex.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/filtered/parse.py` & `python_liquid-1.9.3/liquid/expressions/filtered/parse.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/include/lex.py` & `python_liquid-1.9.3/liquid/expressions/include/lex.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/loop/lex.py` & `python_liquid-1.9.3/liquid/expressions/loop/lex.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/expressions/loop/parse.py` & `python_liquid-1.9.3/liquid/expressions/loop/parse.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/extra/__init__.py` & `python_liquid-1.9.3/liquid/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/extra/filters/_json.py` & `python_liquid-1.9.3/liquid/extra/filters/_json.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/extra/filters/array.py` & `python_liquid-1.9.3/liquid/extra/filters/array.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/extra/filters/html.py` & `python_liquid-1.9.3/liquid/extra/filters/html.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/extra/tags/__init__.py` & `python_liquid-1.9.3/liquid/extra/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/extra/tags/_with.py` & `python_liquid-1.9.3/liquid/extra/tags/_with.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/extra/tags/extends.py` & `python_liquid-1.9.3/liquid/extra/tags/extends.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/extra/tags/if_expressions.py` & `python_liquid-1.9.3/liquid/extra/tags/if_expressions.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/extra/tags/if_not.py` & `python_liquid-1.9.3/liquid/extra/tags/if_not.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/extra/tags/macro.py` & `python_liquid-1.9.3/liquid/extra/tags/macro.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/future/environment.py` & `python_liquid-1.9.3/liquid/future/environment.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/__init__.py` & `python_liquid-1.9.3/liquid/golden/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,100 +62,102 @@
 from . import sort_filter
 from . import sort_natural_filter
 from . import special
 from . import split_filter
 from . import strip_filter
 from . import strip_html_filter
 from . import strip_newlines_filter
+from . import sum_filter
 from . import tablerow_tag
 from . import times_filter
 from . import truncate_filter
 from . import truncatewords_filter
 from . import uniq_filter
 from . import unless_tag
 from . import upcase_filter
 from . import url_decode_filter
 from . import url_encode_filter
 from . import where_filter
 from . import whitespace_control
 
 test_cases = [
+    abs_filter,
+    append_filter,
     assign_tag,
+    at_least_filter,
+    at_most_filter,
+    base64_decode_filter,
+    base64_encode_filter,
+    base64_url_safe_decode_filter,
+    base64_url_safe_encode_filter,
+    capitalize_filter,
     capture_tag,
     case_tag,
+    ceil_filter,
     comment_tag,
+    compact_filter,
+    concat_filter,
     cycle_tag,
+    date_filter,
     decrement_tag,
+    default_filter,
+    divided_by_filter,
+    downcase_filter,
     echo_tag,
+    escape_filter,
+    escape_once_filter,
+    first_filter,
+    floor_filter,
     for_tag,
+    identifiers,
     if_tag,
     ifchanged_tag,
     illegal,
     include_tag,
     increment_tag,
-    liquid_tag,
-    not_liquid,
-    output_statement,
-    raw_tag,
-    render_tag,
-    tablerow_tag,
-    unless_tag,
-    whitespace_control,
-    concat_filter,
-    first_filter,
+    inline_comment_tag,
     join_filter,
     last_filter,
+    liquid_tag,
+    lstrip_filter,
     map_filter,
-    reverse_filter,
-    sort_filter,
-    sort_natural_filter,
-    where_filter,
-    uniq_filter,
-    compact_filter,
-    abs_filter,
-    at_most_filter,
-    at_least_filter,
-    ceil_filter,
-    floor_filter,
-    divided_by_filter,
     minus_filter,
-    plus_filter,
-    round_filter,
-    times_filter,
     modulo_filter,
-    size_filter,
-    default_filter,
-    date_filter,
-    capitalize_filter,
-    append_filter,
-    downcase_filter,
-    escape_filter,
-    escape_once_filter,
-    lstrip_filter,
     newline_to_br_filter,
+    not_liquid,
+    output_statement,
+    plus_filter,
     prepend_filter,
+    range_objects,
+    raw_tag,
     remove_filter,
     remove_first_filter,
     remove_last_filter,
+    render_tag,
     replace_filter,
     replace_first_filter,
     replace_last_filter,
+    reverse_filter,
+    round_filter,
+    rstrip_filter,
+    size_filter,
     slice_filter,
+    sort_filter,
+    sort_natural_filter,
+    special,
     split_filter,
-    upcase_filter,
     strip_filter,
-    rstrip_filter,
     strip_html_filter,
     strip_newlines_filter,
+    sum_filter,
+    tablerow_tag,
+    times_filter,
     truncate_filter,
     truncatewords_filter,
-    url_encode_filter,
+    uniq_filter,
+    unless_tag,
+    upcase_filter,
     url_decode_filter,
-    base64_encode_filter,
-    base64_decode_filter,
-    base64_url_safe_encode_filter,
-    base64_url_safe_decode_filter,
-    range_objects,
-    special,
-    inline_comment_tag,
-    identifiers,
+    url_encode_filter,
+    where_filter,
+    whitespace_control,
 ]
```

### Comparing `python_liquid-1.9.2/liquid/golden/abs_filter.py` & `python_liquid-1.9.3/liquid/golden/abs_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/append_filter.py` & `python_liquid-1.9.3/liquid/golden/append_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/assign_tag.py` & `python_liquid-1.9.3/liquid/golden/assign_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/at_least_filter.py` & `python_liquid-1.9.3/liquid/golden/at_least_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/at_most_filter.py` & `python_liquid-1.9.3/liquid/golden/at_most_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/base64_decode_filter.py` & `python_liquid-1.9.3/liquid/golden/base64_decode_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/base64_encode_filter.py` & `python_liquid-1.9.3/liquid/golden/base64_encode_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/base64_url_safe_decode_filter.py` & `python_liquid-1.9.3/liquid/golden/base64_url_safe_decode_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/base64_url_safe_encode_filter.py` & `python_liquid-1.9.3/liquid/golden/base64_url_safe_encode_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/capitalize_filter.py` & `python_liquid-1.9.3/liquid/golden/capitalize_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/capture_tag.py` & `python_liquid-1.9.3/liquid/golden/capture_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/case.py` & `python_liquid-1.9.3/liquid/golden/case.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/case_tag.py` & `python_liquid-1.9.3/liquid/golden/case_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/ceil_filter.py` & `python_liquid-1.9.3/liquid/golden/ceil_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/comment_tag.py` & `python_liquid-1.9.3/liquid/golden/comment_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/compact_filter.py` & `python_liquid-1.9.3/liquid/golden/compact_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/concat_filter.py` & `python_liquid-1.9.3/liquid/golden/concat_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/cycle_tag.py` & `python_liquid-1.9.3/liquid/golden/cycle_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/date_filter.py` & `python_liquid-1.9.3/liquid/golden/date_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/default_filter.py` & `python_liquid-1.9.3/liquid/golden/default_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/divided_by_filter.py` & `python_liquid-1.9.3/liquid/golden/divided_by_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/downcase_filter.py` & `python_liquid-1.9.3/liquid/golden/downcase_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/echo_tag.py` & `python_liquid-1.9.3/liquid/golden/echo_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/escape_filter.py` & `python_liquid-1.9.3/liquid/golden/escape_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/escape_once_filter.py` & `python_liquid-1.9.3/liquid/golden/escape_once_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/first_filter.py` & `python_liquid-1.9.3/liquid/golden/first_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/floor_filter.py` & `python_liquid-1.9.3/liquid/golden/floor_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/for_tag.py` & `python_liquid-1.9.3/liquid/golden/for_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/identifiers.py` & `python_liquid-1.9.3/liquid/golden/identifiers.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/if_tag.py` & `python_liquid-1.9.3/liquid/golden/if_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/ifchanged_tag.py` & `python_liquid-1.9.3/liquid/golden/ifchanged_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/illegal.py` & `python_liquid-1.9.3/liquid/golden/illegal.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/include_tag.py` & `python_liquid-1.9.3/liquid/golden/include_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/increment_tag.py` & `python_liquid-1.9.3/liquid/golden/increment_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/inline_comment_tag.py` & `python_liquid-1.9.3/liquid/golden/minus_filter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,58 @@
-"""Golden tests cases for testing liquid's `#` tag."""
+"""Golden tests cases for testing liquid's built-in `minus` filter."""
 
 from liquid.golden.case import Case
 
 cases = [
     Case(
-        description="with whitespace control and padding",
-        template=r"{%- # some comment -%}",
-        expect="",
+        description="integer value and integer arg",
+        template=r"{{ 10 | minus: 2 }}",
+        expect="8",
     ),
     Case(
-        description="with whitespace control no padding",
-        template=r"{%-# some comment -%}",
-        expect="",
+        description="integer value and float arg",
+        template=r"{{ 10 | minus: 2.0 }}",
+        expect="8.0",
     ),
     Case(
-        description="no whitespace control with padding",
-        template=r"{% # some comment %}",
-        expect="",
+        description="float value and float arg",
+        template=r"{{ 10.1 | minus: 2.2 }}",
+        expect="7.9",
     ),
     Case(
-        description="no whitespace control no padding",
-        template=r"{%# some comment %}",
-        expect="",
+        description="string value and string arg",
+        template=r'{{ "10.1" | minus: "2.2" }}',
+        expect="7.9",
     ),
     Case(
-        description="no padding after the hash",
-        template=r"{%#some comment %}",
-        expect="",
+        description="string not a number",
+        template=r'{{ "foo" | minus: "2.0" }}',
+        expect="-2.0",
     ),
     Case(
-        description="empty",
-        template=r"{%#%}",
-        expect="",
+        description="arg string not a number",
+        template=r'{{ "10" | minus: "foo" }}',
+        expect="10",
     ),
     Case(
-        description="liquid tag",
-        template="\n".join(
-            [
-                r"{% liquid ",
-                r"  # first comment line",
-                r"  # second comment line",
-                r"",
-                r"  # another comment line",
-                r"  echo 'Hello '",
-                r"",
-                r"  # more comments",
-                r"  echo 'goodbye'",
-                r"-%}",
-            ]
-        ),
-        expect="Hello goodbye",
-    ),
-    Case(
-        description="multiple lines",
-        template="\n".join(
-            [
-                "{%-",
-                "  # spread inline comments",
-                "  # over multiple lines",
-                "-%}",
-            ]
-        ),
+        description="too many args",
+        template=r"{{ 5 | minus: 1, '5' }}",
         expect="",
+        error=True,
     ),
     Case(
-        description="lots of hashes in a liquid tag",
-        template="\n".join(
-            [
-                r"{% liquid",
-                r"  ##########################",
-                r"  # spread inline comments #",
-                r"  ##########################",
-                r"-%}",
-            ]
-        ),
-        expect="",
+        description="not a string, int or float",
+        template=r"{{ a | minus: 1 }}",
+        expect="-1",
+        globals={"a": {}},
     ),
     Case(
-        description="enforce leading hash",
-        template="\n".join(
-            [
-                "{%-",
-                "  # spread inline comments",
-                "  over multiple lines",
-                "-%}",
-            ]
-        ),
-        expect="",
-        error=True,
+        description="undefined left value",
+        template=r"{{ nosuchthing | minus: 2 }}",
+        expect="-2",
     ),
     Case(
-        description="can't comment tags",
-        template="{%- # {% echo 'hello world' %} -%}",
-        expect=" -%}",
+        description="undefined argument",
+        template=r"{{ 10 | minus: nosuchthing }}",
+        expect="10",
     ),
 ]
```

### Comparing `python_liquid-1.9.2/liquid/golden/join_filter.py` & `python_liquid-1.9.3/liquid/golden/join_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/last_filter.py` & `python_liquid-1.9.3/liquid/golden/last_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/liquid_tag.py` & `python_liquid-1.9.3/liquid/golden/liquid_tag.py`

 * *Files 13% similar despite different names*

```diff
@@ -179,8 +179,37 @@
                 r"42",
                 r"{%- liquid endif -%}",
             ]
         ),
         expect="",
         error=True,
     ),
+    Case(
+        description="bare liquid tag in liquid tag",
+        template="\n".join(
+            [
+                r"{%- liquid",
+                r"  liquid",
+                r'  echo "foo"',
+                r"-%}",
+            ]
+        ),
+        expect="foo",
+    ),
+    Case(
+        description="liquid tag in liquid tag",
+        template="\n".join(
+            [
+                r"{%- liquid",
+                r"  liquid echo 'bar'",
+                r'  echo "foo"',
+                r"-%}",
+            ]
+        ),
+        expect="barfoo",
+    ),
+    Case(
+        description="nested liquid in liquid tag",
+        template='{%- liquid liquid liquid echo "foo" -%}',
+        expect="foo",
+    ),
 ]
```

### Comparing `python_liquid-1.9.2/liquid/golden/lstrip_filter.py` & `python_liquid-1.9.3/liquid/golden/lstrip_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/map_filter.py` & `python_liquid-1.9.3/liquid/golden/map_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,8 +31,20 @@
     ),
     Case(
         description="undefined argument",
         template=r"{{ a | map: nosuchthing | join: '#' }}",
         expect="#",
         globals={"a": [{"title": "foo"}, {"title": "bar"}]},
     ),
+    Case(
+        description="nested arrays get flattened",
+        template=r"{{ a | map: 'title' | join: '#' }}",
+        expect="foo#bar#baz",
+        globals={"a": [{"title": "foo"}, [{"title": "bar"}, {"title": "baz"}]]},
+    ),
+    Case(
+        description="input is a hash",
+        template=r"{{ a | map: 'title' | join: '#' }}",
+        expect="foo",
+        globals={"a": {"title": "foo", "some": "thing"}},
+    ),
 ]
```

### Comparing `python_liquid-1.9.2/liquid/golden/minus_filter.py` & `python_liquid-1.9.3/liquid/golden/modulo_filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-"""Golden tests cases for testing liquid's built-in `minus` filter."""
+"""Golden tests cases for testing liquid's built-in `modulo` filter."""
 
 from liquid.golden.case import Case
 
 cases = [
     Case(
         description="integer value and integer arg",
-        template=r"{{ 10 | minus: 2 }}",
-        expect="8",
+        template=r"{{ 10 | modulo: 2 }}",
+        expect="0",
     ),
     Case(
         description="integer value and float arg",
-        template=r"{{ 10 | minus: 2.0 }}",
-        expect="8.0",
+        template=r"{{ 10 | modulo: 2.0 }}",
+        expect="0.0",
     ),
     Case(
         description="float value and float arg",
-        template=r"{{ 10.1 | minus: 2.2 }}",
-        expect="7.9",
+        template=r"{{ 10.1 | modulo: 7.0 }}",
+        expect="3.1",
     ),
     Case(
-        description="string value and string arg",
-        template=r'{{ "10.1" | minus: "2.2" }}',
-        expect="7.9",
+        description="string value and argument",
+        template=r'{{ "10" | modulo: "2.0" }}',
+        expect="0.0",
     ),
     Case(
         description="string not a number",
-        template=r'{{ "foo" | minus: "2.0" }}',
-        expect="-2.0",
+        template=r'{{ "foo" | modulo: "2.0" }}',
+        expect="0.0",
     ),
     Case(
         description="arg string not a number",
-        template=r'{{ "10" | minus: "foo" }}',
-        expect="10",
+        template=r'{{ "10" | modulo: "foo" }}',
+        expect="",
+        error=True,
     ),
     Case(
         description="too many args",
-        template=r"{{ 5 | minus: 1, '5' }}",
+        template=r"{{ 5 | modulo: 1, '5' }}",
         expect="",
         error=True,
     ),
     Case(
         description="not a string, int or float",
-        template=r"{{ a | minus: 1 }}",
-        expect="-1",
+        template=r"{{ a | modulo: 1 }}",
+        expect="0",
         globals={"a": {}},
     ),
     Case(
         description="undefined left value",
-        template=r"{{ nosuchthing | minus: 2 }}",
-        expect="-2",
+        template=r"{{ nosuchthing | modulo: 2 }}",
+        expect="0",
     ),
     Case(
         description="undefined argument",
-        template=r"{{ 10 | minus: nosuchthing }}",
-        expect="10",
+        template=r"{{ 5 | modulo: nosuchthing }}",
+        expect="",
+        error=True,
     ),
 ]
```

### Comparing `python_liquid-1.9.2/liquid/golden/modulo_filter.py` & `python_liquid-1.9.3/liquid/golden/plus_filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-"""Golden tests cases for testing liquid's built-in `modulo` filter."""
+"""Golden tests cases for testing liquid's built-in `plus` filter."""
 
 from liquid.golden.case import Case
 
 cases = [
     Case(
         description="integer value and integer arg",
-        template=r"{{ 10 | modulo: 2 }}",
-        expect="0",
+        template=r"{{ 10 | plus: 2 }}",
+        expect="12",
     ),
     Case(
         description="integer value and float arg",
-        template=r"{{ 10 | modulo: 2.0 }}",
-        expect="0.0",
+        template=r"{{ 10 | plus: 2.0 }}",
+        expect="12.0",
     ),
     Case(
         description="float value and float arg",
-        template=r"{{ 10.1 | modulo: 7.0 }}",
-        expect="3.1",
+        template=r"{{ 10.1 | plus: 2.2 }}",
+        expect="12.3",
     ),
     Case(
-        description="string value and argument",
-        template=r'{{ "10" | modulo: "2.0" }}',
-        expect="0.0",
+        description="string value and string arg",
+        template=r'{{ "10.1" | plus: "2.2" }}',
+        expect="12.3",
     ),
     Case(
         description="string not a number",
-        template=r'{{ "foo" | modulo: "2.0" }}',
-        expect="0.0",
+        template=r'{{ "foo" | plus: "2.0" }}',
+        expect="2.0",
     ),
     Case(
         description="arg string not a number",
-        template=r'{{ "10" | modulo: "foo" }}',
-        expect="",
-        error=True,
+        template=r'{{ "10" | plus: "foo" }}',
+        expect="10",
     ),
     Case(
         description="too many args",
-        template=r"{{ 5 | modulo: 1, '5' }}",
+        template=r"{{ 5 | plus: 1, '5' }}",
         expect="",
         error=True,
     ),
     Case(
         description="not a string, int or float",
-        template=r"{{ a | modulo: 1 }}",
-        expect="0",
+        template=r"{{ a | plus: 1 }}",
+        expect="1",
         globals={"a": {}},
     ),
     Case(
         description="undefined left value",
-        template=r"{{ nosuchthing | modulo: 2 }}",
-        expect="0",
+        template=r"{{ nosuchthing | plus: 2 }}",
+        expect="2",
     ),
     Case(
         description="undefined argument",
-        template=r"{{ 5 | modulo: nosuchthing }}",
-        expect="",
-        error=True,
+        template=r"{{ 10 | plus: nosuchthing }}",
+        expect="10",
+    ),
+    Case(
+        description="integer value and negative integer arg",
+        template=r"{{ 10 | plus: -2 }}",
+        expect="8",
     ),
 ]
```

### Comparing `python_liquid-1.9.2/liquid/golden/newline_to_br_filter.py` & `python_liquid-1.9.3/liquid/golden/newline_to_br_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/output_statement.py` & `python_liquid-1.9.3/liquid/golden/output_statement.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/plus_filter.py` & `python_liquid-1.9.3/liquid/golden/times_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,53 @@
-"""Golden tests cases for testing liquid's built-in `plus` filter."""
+"""Golden tests cases for testing liquid's built-in `times` filter."""
 
 from liquid.golden.case import Case
 
 cases = [
     Case(
-        description="integer value and integer arg",
-        template=r"{{ 10 | plus: 2 }}",
-        expect="12",
+        description="int times int",
+        template=r"{{ 5 | times: 2 }}",
+        expect="10",
     ),
     Case(
-        description="integer value and float arg",
-        template=r"{{ 10 | plus: 2.0 }}",
-        expect="12.0",
+        description="int times float",
+        template=r"{{ 5 | times: 2.1 }}",
+        expect="10.5",
     ),
     Case(
-        description="float value and float arg",
-        template=r"{{ 10.1 | plus: 2.2 }}",
-        expect="12.3",
+        description="float times float",
+        template=r"{{ 5.0 | times: 2.1 }}",
+        expect="10.5",
     ),
     Case(
-        description="string value and string arg",
-        template=r'{{ "10.1" | plus: "2.2" }}',
-        expect="12.3",
+        description="string times string",
+        template=r'{{ "5.0" | times: "2.1" }}',
+        expect="10.5",
     ),
     Case(
-        description="string not a number",
-        template=r'{{ "foo" | plus: "2.0" }}',
-        expect="2.0",
+        description="negative multiplication",
+        template=r"{{ -5 | times: 2 }}",
+        expect="-10",
     ),
     Case(
-        description="arg string not a number",
-        template=r'{{ "10" | plus: "foo" }}',
-        expect="10",
+        description="missing arg",
+        template=r"{{ 5 | times }}",
+        expect="",
+        error=True,
     ),
     Case(
         description="too many args",
-        template=r"{{ 5 | plus: 1, '5' }}",
+        template=r"{{ 5 | times: 1, 2 }}",
         expect="",
         error=True,
     ),
     Case(
-        description="not a string, int or float",
-        template=r"{{ a | plus: 1 }}",
-        expect="1",
-        globals={"a": {}},
-    ),
-    Case(
         description="undefined left value",
-        template=r"{{ nosuchthing | plus: 2 }}",
-        expect="2",
+        template=r"{{ nosuchthing | times: 2 }}",
+        expect="0",
     ),
     Case(
         description="undefined argument",
-        template=r"{{ 10 | plus: nosuchthing }}",
-        expect="10",
+        template=r"{{ 5 | times: nosuchthing }}",
+        expect="0",
     ),
 ]
```

### Comparing `python_liquid-1.9.2/liquid/golden/prepend_filter.py` & `python_liquid-1.9.3/liquid/golden/prepend_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/range_objects.py` & `python_liquid-1.9.3/liquid/golden/range_objects.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/raw_tag.py` & `python_liquid-1.9.3/liquid/golden/raw_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/remove_filter.py` & `python_liquid-1.9.3/liquid/golden/remove_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/remove_first_filter.py` & `python_liquid-1.9.3/liquid/golden/remove_first_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/remove_last_filter.py` & `python_liquid-1.9.3/liquid/golden/remove_last_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/render_tag.py` & `python_liquid-1.9.3/liquid/golden/render_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/replace_filter.py` & `python_liquid-1.9.3/liquid/golden/replace_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/replace_first_filter.py` & `python_liquid-1.9.3/liquid/golden/replace_first_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/replace_last_filter.py` & `python_liquid-1.9.3/liquid/golden/replace_last_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/reverse_filter.py` & `python_liquid-1.9.3/liquid/golden/reverse_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/round_filter.py` & `python_liquid-1.9.3/liquid/golden/round_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/rstrip_filter.py` & `python_liquid-1.9.3/liquid/golden/rstrip_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/size_filter.py` & `python_liquid-1.9.3/liquid/golden/size_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/slice_filter.py` & `python_liquid-1.9.3/liquid/golden/slice_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/sort_filter.py` & `python_liquid-1.9.3/liquid/golden/sort_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/sort_natural_filter.py` & `python_liquid-1.9.3/liquid/golden/sort_natural_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/special.py` & `python_liquid-1.9.3/liquid/golden/special.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/split_filter.py` & `python_liquid-1.9.3/liquid/golden/split_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/strip_filter.py` & `python_liquid-1.9.3/liquid/golden/strip_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/strip_html_filter.py` & `python_liquid-1.9.3/liquid/golden/strip_html_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/strip_newlines_filter.py` & `python_liquid-1.9.3/liquid/golden/strip_newlines_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/tablerow_tag.py` & `python_liquid-1.9.3/liquid/golden/tablerow_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/truncate_filter.py` & `python_liquid-1.9.3/liquid/golden/truncate_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/truncatewords_filter.py` & `python_liquid-1.9.3/liquid/golden/truncatewords_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/uniq_filter.py` & `python_liquid-1.9.3/liquid/golden/uniq_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/unless_tag.py` & `python_liquid-1.9.3/liquid/golden/unless_tag.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/upcase_filter.py` & `python_liquid-1.9.3/liquid/golden/upcase_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/url_decode_filter.py` & `python_liquid-1.9.3/liquid/golden/url_decode_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/url_encode_filter.py` & `python_liquid-1.9.3/liquid/golden/url_encode_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/where_filter.py` & `python_liquid-1.9.3/liquid/golden/where_filter.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/golden/whitespace_control.py` & `python_liquid-1.9.3/liquid/golden/whitespace_control.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/utils/cache.py` & `python_liquid-1.9.3/liquid/utils/cache.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/utils/cache.pyi` & `python_liquid-1.9.3/liquid/utils/cache.pyi`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/utils/html.py` & `python_liquid-1.9.3/liquid/utils/html.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/liquid/utils/text.py` & `python_liquid-1.9.3/liquid/utils/text.py`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/.gitignore` & `python_liquid-1.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/LICENSE` & `python_liquid-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/README.md` & `python_liquid-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `python_liquid-1.9.2/pyproject.toml` & `python_liquid-1.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     "pytest-cov",
     "black",
     "mypy",
     "pyyaml",
     "types-pyyaml",
     "twine",
     "ruff",
-    "sphinx",
     "mock",
     "types-python-dateutil",
+    "MarkupSafe",
 ]
 
 [tool.hatch.envs.default.scripts]
 cov = [
     "hatch run noescape:cov",
     "pytest --cov-append --cov-report= --cov-fail-under=97 --cov-config=pyproject.toml --cov=liquid --cov=tests {args}",
 ]
```

### Comparing `python_liquid-1.9.2/PKG-INFO` & `python_liquid-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-liquid
-Version: 1.9.2
+Version: 1.9.3
 Summary: A Python engine for the Liquid template language.
 Project-URL: Change Log, https://github.com/jg-rp/liquid/blob/main/CHANGES.md
 Project-URL: Documentation, https://jg-rp.github.io/liquid/
 Project-URL: Homepage, https://jg-rp.github.io/liquid/
 Project-URL: Issue Tracker, https://github.com/jg-rp/liquid/issues
 Project-URL: Source Code, https://github.com/jg-rp/liquid
 Author-email: James Prior <jamesgr.prior@gmail.com>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-liquid Version: 1.9.2 Summary: A Python
+Metadata-Version: 2.1 Name: python-liquid Version: 1.9.3 Summary: A Python
 engine for the Liquid template language. Project-URL: Change Log, https://
 github.com/jg-rp/liquid/blob/main/CHANGES.md Project-URL: Documentation, https:
 //jg-rp.github.io/liquid/ Project-URL: Homepage, https://jg-rp.github.io/
 liquid/ Project-URL: Issue Tracker, https://github.com/jg-rp/liquid/issues
 Project-URL: Source Code, https://github.com/jg-rp/liquid Author-email: James
 Prior
 prior@gmail.com> License-Expression: MIT License-File: LICENSE Classifier:
```

