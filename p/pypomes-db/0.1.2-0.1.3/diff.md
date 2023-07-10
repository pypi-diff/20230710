# Comparing `tmp/pypomes_db-0.1.2.tar.gz` & `tmp/pypomes_db-0.1.3.tar.gz`

## Comparing `pypomes_db-0.1.2.tar` & `pypomes_db-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pypomes_db-0.1.2/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12107 2020-02-02 00:00:00.000000 pypomes_db-0.1.2/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.2/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/PKG-INFO
```

### Comparing `pypomes_db-0.1.2/src/pypomes_db/db_pomes.py` & `pypomes_db-0.1.3/src/pypomes_db/db_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # noinspection PyProtectedMember
-from pyodbc import connect, Connection, Row
+from pyodbc import connect, Connection
 from typing import Final
 from pypomes_core.env_pomes import APP_PREFIX, env_get_int, env_get_str
 
 # dados para acesso ao BD
 DB_DRIVER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_DRIVER")
 DB_NAME: Final[str] = env_get_str(f"{APP_PREFIX}_DB_NAME")
 DB_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_DB_HOST")
@@ -89,68 +89,70 @@
     if required and not exc and result is None:
         # sim, reporte o erro
         errors.append(__db_required_msg(sel_stmt, where_vals))
 
     return result
 
 
-def db_exec_stored_procedure(errors: list[str], nm_proced: str, param_vals: tuple) -> list[Row]:
+def db_exec_stored_procedure(errors: list[str], nm_procedure: str, proc_vals: tuple) -> list[tuple]:
     """
     Executa o stored procedure no banco de dados com os parâmetros informados e retorna os erros que ocorrerem
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
-    :param nm_proced: nome do stored procedure
-    :param param_vals: lista de valores dos parâmetros
+    :param nm_procedure: nome do stored procedure
+    :param proc_vals: lista de valores para a sotred procedure
     :return: lista de tuplas contendo o resultado da busca, ou [] se a busca resultar vazia
     """
     # inicializa a variável de retorno
-    result: list[Row] = []
+    result: list[tuple] = []
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # obtém o cursor e executa a operação
             with conn.cursor() as cursor:
-                sql = f"SET NOCOUNT ON; EXEC {nm_proced} {','.join(('?',) * len(param_vals))}"
-                cursor.execute(sql, param_vals)
+                stmt = f"SET NOCOUNT ON; EXEC {nm_procedure} {','.join(('?',) * len(proc_vals))}"
+                cursor.execute(stmt, proc_vals)
                 # obtem as tuplas retornadas
                 for record in cursor:
-                    result.append(record)
+                    values: list = [rec[0] for rec in record]
+                    result.append(tuple(values))
 
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def db_select_all(errors: list[str], sel_stmt: str,
-                  where_vals: tuple, required: bool = False) -> list[Row]:
+                  where_vals: tuple, required: bool = False) -> list[tuple]:
     """
     Busca no banco de dados e retorna todas as tuplas que satisfaçam o comando de busca *sele_stmt*.
     O comando pode opcionalmente conter critérios de busca, com valores respectivos fornecidos
     em *where_vals*. A lista de valores para um atributo com a cláusula *IN* deve estar contida
     em tupla específica. Se a busca resultar vazia, uma lista vazia é retornado.
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :param sel_stmt: comando SELECT para a busca
     :param where_vals: lista de valores a serem associados aos critérios de busca
     :param required: define se busca vazia deve ser considerada erro
     :return: lista de tuplas contendo o resultado da busca, ou [] se a busca resultar vazia
     """
     # inicializa a variável de retorno
-    result: list[Row] = []
+    result: list[tuple] = []
 
     exc: bool = False
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # obtem o cursor e executa a operação
             with conn.cursor() as cursor:
                 cursor.execute(sel_stmt, where_vals)
                 # obtem as tuplas retornadas
                 for record in cursor:
-                    result.append(record)
+                    values: list = [rec[0] for rec in record]
+                    result.append(tuple(values))
     except Exception as e:
         exc = True
         errors.append(__db_except_msg(e))
 
     # o parâmetro 'required' foi definido, não houve erros, e nenhum registro foi obtido ?
     if required and not exc and len(result) == 0:
         # sim, reporte o erro
@@ -209,24 +211,14 @@
     :param delete_stmt: comando DELETE
     :param where_vals: lista de valores para os critérios de seleção de tuplas
     :return: o número de tuplas excluídas
     """
     return __db_modify(errors, delete_stmt, where_vals)
 
 
-def db_row_to_dict(row):
-    """
-    Converts a pyodbc.Row object to a dictionary.
-
-    :param row: A pyodbc.Row object.
-    :return: A dictionary where keys are column names and values are the corresponding values in the row.
-    """
-    return {description[0]: row[i] for i, description in enumerate(row.cursor_description)}
-
-
 def __db_modify(errors: list[str], modify_stmt: str, bind_vals: tuple) -> int:
     """
     Modifica o banco de dados, inserindo, atualizando ou excluindo tuplas, segundo as
     definições do comando *modify_stmt*. Os valores para essa modificação, seguidos dos
     valores para a seleção das tuplas, estão em *bind_vals*.
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
```

### Comparing `pypomes_db-0.1.2/LICENSE` & `pypomes_db-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.1.2/pyproject.toml` & `pypomes_db-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (DB modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.1.2/PKG-INFO` & `pypomes_db-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_db
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of Python pomes, pennyeach (DB modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

