# Comparing `tmp/qtgql-0.127.0.tar.gz` & `tmp/qtgql-0.128.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.127.0.tar", max compression
+gzip compressed data, was "qtgql-0.128.0.tar", max compression
```

## Comparing `qtgql-0.127.0.tar` & `qtgql-0.128.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1064 2023-07-09 18:31:46.802182 qtgql-0.127.0/LICENSE
--rw-r--r--   0        0        0     1055 2023-07-09 18:31:46.802182 qtgql-0.127.0/README.md
--rw-r--r--   0        0        0     4428 2023-07-09 18:32:06.498201 qtgql-0.127.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1939 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1685 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3091 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     3366 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    14721 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      864 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4237 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1699 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4353 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     2933 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0     1060 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4706 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     4041 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     5049 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     5220 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3237 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    18213 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1147 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.127.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-10 07:23:29.319740 qtgql-0.128.0/LICENSE
+-rw-r--r--   0        0        0     1055 2023-07-10 07:23:29.319740 qtgql-0.128.0/README.md
+-rw-r--r--   0        0        0     4428 2023-07-10 07:23:46.475887 qtgql-0.128.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1939 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1685 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3091 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3366 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    14789 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      864 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4237 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1699 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3629 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     2985 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1060 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4706 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     4137 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     5049 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     5220 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3237 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    18250 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1147 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.128.0/PKG-INFO
```

### Comparing `qtgql-0.127.0/LICENSE` & `qtgql-0.128.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/README.md` & `qtgql-0.128.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/pyproject.toml` & `qtgql-0.128.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.127.0"
+version = "0.128.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.127.0/qtgqlcodegen/cli.py` & `qtgql-0.128.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/config.py` & `qtgql-0.128.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.128.0/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.128.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/core/template.py` & `qtgql-0.128.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/generator.py` & `qtgql-0.128.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.128.0/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.128.0/qtgqlcodegen/operation/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,19 @@
                 name
             }
         }
     }
     :returns: all of the inline fragments as a flat list.
     """
     fields_for_concrete: list[gql_lang.FieldNode] = []
-    if not has_id_selection(selection_set) and not id_was_selected:
+    if (
+        parent_concrete.implements_node
+        and not has_id_selection(selection_set)
+        and not id_was_selected
+    ):
         id_was_selected = True
         inject_id_selection(selection_set)
     for field_or_frag in selection_set.selections:
         if inline_frag := is_inline_fragment(field_or_frag):
             type_name = inline_frag.type_condition.name.value
             # no need to validate inner types are implementation, graphql-core does this.
             concrete_choice = type_info.get_object_type(
```

### Comparing `qtgql-0.127.0/qtgqlcodegen/operation/template.py` & `qtgql-0.128.0/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.128.0/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.128.0/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/schema/template.py` & `qtgql-0.128.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.128.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.128.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -18,50 +18,33 @@
 {% for choice in proxy_field.type.choices -%}
 {% set do_on_meets -%}
 👉 setter_name 👈(👉choice.deserializer_name👈(👉proxy_field.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
 {% endset -%}
 👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
 {% endfor %}
 {% elif proxy_field.type.is_model -%}
-    {% if proxy_field.type.is_model.of_type.is_queried_object_type or proxy_field.type.is_model.of_type.is_queried_union -%}
-    👉proxy_field.concrete.type.member_type👈 obj_list;
+    👉proxy_field.concrete.type.member_type👈 👉proxy_field.name👈_init_list;
     for (const auto& node: data.value("👉proxy_field.name👈").toArray()){
     {% if proxy_field.type.is_model.of_type.is_queried_object_type %}
-        obj_list.append(👉 proxy_field.type.is_model.of_type.is_queried_object_type.deserializer_name 👈(node.toObject(), 👉operation_pointer👈));
-    {% elif proxy_field.type.is_model.of_type.is_queried_union %}
+        👉proxy_field.name👈_init_list.append(👉 proxy_field.type.is_model.of_type.is_queried_object_type.deserializer_name 👈(node.toObject(), 👉operation_pointer👈));
+    {% elif proxy_field.type.is_model.of_type.is_queried_union or proxy_field.type.is_model.of_type.is_queried_interface %}
         auto node_data = node.toObject();
         auto 👉proxy_field.name👈_typename = node_data.value("__typename").toString();
         {%set type_cond -%}👉proxy_field.name👈_typename{% endset -%}
         {% for choice in proxy_field.type.of_type.choices -%}
         {% set do_on_meets -%}
-        obj_list.append(👉choice.deserializer_name👈(node_data, 👉operation_pointer👈) 👉 setter_end 👈);
+        👉proxy_field.name👈_init_list.append(👉choice.deserializer_name👈(node_data, 👉operation_pointer👈) 👉 setter_end 👈);
         {% endset -%}
         👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
         {% endfor %}
-    {% endif %}
-    };
-    👉 setter_name 👈(obj_list👉 setter_end 👈);
-    {% elif proxy_field.type.is_model.is_interface -%}
-    👉 setter_name 👈(qtgql::ListModel(
-            parent=parent,
-            data=[👉proxy_field.type.is_model.is_interface.name👈.from_dict(parent, data=node, config=inner_config, metadata=👉operation_pointer👈) for
-    node in field_data],)👉 setter_end 👈);
-    {% elif proxy_field.type.is_model.is_union -%}
-    model_data = []
-    for node in field_data:
-    type_name = node['__typename']
-    choice = inner_👉config_name👈.choices[type_name]
-    model_data.append(
-            __TYPE_MAP__[type_name].from_dict(self, node,
-            choice, 👉operation_pointer👈)
-    )
-    👉 setter_name 👈(qtgql::ListModel(parent, data=model_data)👉 setter_end 👈);
     {% else %}
-    throw qtgql::exceptions::NotImplementedError({"can't update model of 👉proxy_field.type.of_type.__class__👈"});
+    throw qtgql::exceptions::NotImplementedError({"can't deserialize model of 👉proxy_field.type.of_type.__class__👈"});
     {% endif %}
+    };
+    👉 setter_name 👈(👉proxy_field.name👈_init_list👉 setter_end 👈);
 {% elif proxy_field.type.is_builtin_scalar -%}
     {% if proxy_field.type.is_void -%}
     /* deliberately empty */
     {% else -%}
     👉 setter_name 👈(data.value("👉proxy_field.name👈").👉 proxy_field.type.is_builtin_scalar.from_json_convertor 👈 👉 setter_end 👈);
     {% endif %}
     {% elif proxy_field.type.is_custom_scalar -%}
```

### Comparing `qtgql-0.127.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.128.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {% elif field.type.is_model  %}
     {% if  field.type.is_model.of_type.is_queried_object_type %}
     auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.type.of_type.name👈*>>();
     for (const auto & node: 👉 instance_of_concrete 👈){
     init_list_👉 field.name 👈->append(new 👉field.type.of_type.name👈(👉operation_pointer👈, node));
     }
     👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.name 👈>(this, std::move(init_list_👉 field.name 👈));
-    {% elif field.type.is_model.of_type.is_queried_union %}
+    {% elif field.type.is_model.of_type.is_queried_union or field.type.is_model.of_type.is_queried_interface %}
     auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.type.of_type.property_type👈>>();
     for (const auto & node: 👉 instance_of_concrete 👈){
         auto 👉field.name👈_typename = node->__typename();
         {%set type_cond -%}👉field.name👈_typename{% endset -%}
         {% for choice in field.type.of_type.choices -%}
         {% set do_on_meets -%}
         init_list_👉 field.name 👈->append(qobject_cast<👉 field.type.of_type.property_type 👈>(new 👉choice.type_name()👈(👉operation_pointer👈, std::static_pointer_cast<👉 choice.concrete.name 👈>(node))));
```

### Comparing `qtgql-0.127.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.128.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.128.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.128.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 proxy_to_update->qtgql_replace_concrete(concrete);
             }
             else{
                 👉field.private_name👈->insert(i, new 👉field.type.of_type.name👈(operation, concrete));
             }
         }
 
-    {% elif field.type.of_type.is_queried_union %}
+    {% elif field.type.of_type.is_queried_union or field.type.of_type.is_queried_interface %}
         auto 👉field.name👈_typename = concrete->__typename();
         {%set type_cond -%}👉field.name👈_typename{% endset -%}
         {% for choice in field.type.of_type.choices %}
         {% set do_on_meets -%}
         if (i > prev_len - 1){
             👉field.private_name👈->insert(i, new 👉choice.name👈(operation, std::static_pointer_cast<👉choice.concrete.name👈>(concrete)));
         }
@@ -47,15 +47,16 @@
 
         }
 
         {% endset %}
         👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
         {% endfor %}
     {% else %}
-    throw qtgql::exceptions::NotImplementedError({"can't update model of 👉field.type.of_type.__class__👈"});
+    throw qtgql::exceptions::NotImplementedError({""
+                                                  "can't update model of 👉field.type.of_type.__class__👈"});
     {% endif %}
     }
 {% elif field.type.is_queried_object_type -%}
 auto concrete = 👉new_concrete👈;
 if (👉field.private_name👈){
     👉field.private_name👈->qtgql_replace_concrete(concrete);
 }
```

### Comparing `qtgql-0.127.0/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.128.0/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.128.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.128.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/qtgqlcodegen/types.py` & `qtgql-0.128.0/qtgqlcodegen/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     def type_name(self) -> str:
         raise NotImplementedError(
             "models have no valid type for schema concretes, call member_type",
         )
 
     @property
     def property_type(self) -> str:
-        if self.of_type.is_queried_object_type:
+        if self.of_type.is_queried_object_type or self.of_type.is_queried_interface:
             return f"qtgql::bases::ListModelABC<{self.of_type.type_name()}> *"
         if self.of_type.is_queried_union:
             return f"qtgql::bases::ListModelABC<{self.of_type.is_queried_union.type_name()}> *"
         raise NotImplementedError
 
 
 @define
```

### Comparing `qtgql-0.127.0/qtgqlcodegen/utils.py` & `qtgql-0.128.0/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.127.0/PKG-INFO` & `qtgql-0.128.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.127.0
+Version: 0.128.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

