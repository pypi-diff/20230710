# Comparing `tmp/llmreflect-0.0.4.tar.gz` & `tmp/llmreflect-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreflect-0.0.4.tar", max compression
+gzip compressed data, was "llmreflect-0.0.5.tar", max compression
```

## Comparing `llmreflect-0.0.4.tar` & `llmreflect-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4061 2023-07-07 19:45:36.588014 llmreflect-0.0.4/README.md
--rw-r--r--   0        0        0     1235 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Agents/BasicAgent.py
--rw-r--r--   0        0        0     2522 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Agents/EvaluationAgent.py
--rw-r--r--   0        0        0     3204 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Agents/ModerateAgent.py
--rw-r--r--   0        0        0     9728 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Agents/PostgresqlAgent.py
--rw-r--r--   0        0        0     2429 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Agents/QuestionAgent.py
--rw-r--r--   0        0        0        0 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Agents/__init__.py
--rw-r--r--   0        0        0     1873 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Chains/BasicChain.py
--rw-r--r--   0        0        0    15317 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Chains/DatabaseChain.py
--rw-r--r--   0        0        0     1656 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Chains/ModerateChain.py
--rw-r--r--   0        0        0        0 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Chains/__init__.py
--rw-r--r--   0        0        0     8378 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Prompt/BasicPrompt.py
--rw-r--r--   0        0        0        0 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Prompt/__init__.py
--rw-r--r--   0        0        0     2807 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Prompt/promptbase/gradingpostgresql.json
--rw-r--r--   0        0        0     2366 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Prompt/promptbase/moderatepostgresql.json
--rw-r--r--   0        0        0     4951 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Prompt/promptbase/postgresql.json
--rw-r--r--   0        0        0     1119 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Prompt/promptbase/postgresqlfix.json
--rw-r--r--   0        0        0     2011 2023-07-07 19:45:36.588014 llmreflect-0.0.4/llmreflect/Prompt/promptbase/questionpostgresql.json
--rw-r--r--   0        0        0     1933 2023-07-07 19:45:36.592014 llmreflect-0.0.4/llmreflect/Retriever/BasicRetriever.py
--rw-r--r--   0        0        0     4219 2023-07-07 19:45:36.592014 llmreflect-0.0.4/llmreflect/Retriever/DatabaseRetriever.py
--rw-r--r--   0        0        0        0 2023-07-07 19:45:36.592014 llmreflect-0.0.4/llmreflect/Retriever/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 19:45:36.592014 llmreflect-0.0.4/llmreflect/Tests/__init__.py
--rw-r--r--   0        0        0     6217 2023-07-07 19:45:36.592014 llmreflect-0.0.4/llmreflect/Tests/test_chains.py
--rw-r--r--   0        0        0      442 2023-07-07 19:45:36.592014 llmreflect-0.0.4/llmreflect/Tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-07-07 19:45:36.592014 llmreflect-0.0.4/llmreflect/Utils/__init__.py
--rw-r--r--   0        0        0      690 2023-07-07 19:45:36.592014 llmreflect-0.0.4/llmreflect/Utils/database.py
--rw-r--r--   0        0        0      305 2023-07-07 19:45:36.592014 llmreflect-0.0.4/llmreflect/Utils/message.py
--rw-r--r--   0        0        0        0 2023-07-07 19:45:36.592014 llmreflect-0.0.4/llmreflect/__init__.py
--rw-r--r--   0        0        0      478 2023-07-07 19:45:36.592014 llmreflect-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 llmreflect-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     4061 2023-07-10 18:42:44.696518 llmreflect-0.0.5/README.md
+-rw-r--r--   0        0        0     3647 2023-07-10 18:42:44.696518 llmreflect-0.0.5/llmreflect/Agents/BasicAgent.py
+-rw-r--r--   0        0        0     2377 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Agents/EvaluationAgent.py
+-rw-r--r--   0        0        0     3059 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Agents/ModerateAgent.py
+-rw-r--r--   0        0        0     9597 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Agents/PostgresqlAgent.py
+-rw-r--r--   0        0        0     2284 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Agents/QuestionAgent.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Agents/__init__.py
+-rw-r--r--   0        0        0     1873 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Chains/BasicChain.py
+-rw-r--r--   0        0        0    21665 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Chains/DatabaseChain.py
+-rw-r--r--   0        0        0     1786 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Chains/ModerateChain.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Chains/__init__.py
+-rw-r--r--   0        0        0     8378 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/BasicPrompt.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/__init__.py
+-rw-r--r--   0        0        0     2807 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/promptbase/gradingpostgresql.json
+-rw-r--r--   0        0        0     2366 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/promptbase/moderatepostgresql.json
+-rw-r--r--   0        0        0     4951 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/promptbase/postgresql.json
+-rw-r--r--   0        0        0     1119 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/promptbase/postgresqlfix.json
+-rw-r--r--   0        0        0     2011 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Prompt/promptbase/questionpostgresql.json
+-rw-r--r--   0        0        0     1933 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Retriever/BasicRetriever.py
+-rw-r--r--   0        0        0     4219 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Retriever/DatabaseRetriever.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Retriever/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Tests/__init__.py
+-rw-r--r--   0        0        0     7686 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Tests/test_chains.py
+-rw-r--r--   0        0        0      442 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Utils/__init__.py
+-rw-r--r--   0        0        0      690 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Utils/database.py
+-rw-r--r--   0        0        0      305 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/Utils/message.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:42:44.700518 llmreflect-0.0.5/llmreflect/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-10 18:42:44.700518 llmreflect-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 llmreflect-0.0.5/PKG-INFO
```

### Comparing `llmreflect-0.0.4/README.md` & `llmreflect-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/llmreflect/Agents/EvaluationAgent.py` & `llmreflect-0.0.5/llmreflect/Agents/EvaluationAgent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from llmreflect.Agents.BasicAgent import Agent
-from llmreflect.Prompt.BasicPrompt import BasicPrompt
-from langchain.llms.openai import OpenAI
+from llmreflect.Agents.BasicAgent import OpenAIAgent
 from llmreflect.Utils.message import message
 from llmreflect.Retriever.BasicRetriever import BasicEvaluationRetriever
 
 
-class PostgressqlGradingAgent(Agent):
+class PostgressqlGradingAgent(OpenAIAgent):
     """
     This is the agent class use for grading postgresql generation.
     Args:
         Agent (_type_): _description_
     """
     def __init__(self, open_ai_key: str,
                  prompt_name: str = 'gradingpostgresql',
@@ -22,20 +20,18 @@
             prompt_name (str, optional): name for the prompt json file.
                 Defaults to 'gradingpostgresql'.
             max_output_tokens (int, optional): maximum completion length.
                 Defaults to 512.
             temperature (float, optional): how consistent the llm performs.
                 The lower the more consistent. Defaults to 0.0.
         """
-        prompt = BasicPrompt.\
-            load_prompt_from_json_file(prompt_name)
-        llm = OpenAI(temperature=temperature, openai_api_key=open_ai_key)
-        llm.max_tokens = max_output_tokens
-        super().__init__(prompt=prompt,
-                         llm=llm)
+        super().__init__(open_ai_key=open_ai_key,
+                         prompt_name=prompt_name,
+                         max_output_tokens=max_output_tokens,
+                         temperature=temperature)
 
     def equip_retriever(self, retriever: BasicEvaluationRetriever):
         object.__setattr__(self, 'retriever', retriever)
 
     def grade(self, request: str, sql_cmd: str, db_summary: str) -> dict:
         """
         Convert LLM output into a score and an explanation.
```

### Comparing `llmreflect-0.0.4/llmreflect/Agents/ModerateAgent.py` & `llmreflect-0.0.5/llmreflect/Agents/ModerateAgent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from llmreflect.Agents.BasicAgent import Agent
-from llmreflect.Prompt.BasicPrompt import BasicPrompt
-from langchain.llms.openai import OpenAI
+from llmreflect.Agents.BasicAgent import OpenAIAgent
 from llmreflect.Utils.message import message
 from llmreflect.Retriever.BasicRetriever import \
     BasicQuestionModerateRetriever
 
 
-class PostgresqlModerateAgent(Agent):
+class PostgresqlModerateAgent(OpenAIAgent):
     """
     Agent for filtering out illegal and malicious requests.
     Args:
         Agent (_type_): _description_
     """
     def __init__(self, open_ai_key: str,
                  prompt_name: str = 'moderatepostgresql',
@@ -25,20 +23,18 @@
             max_output_tokens (int, optional): maximum completion length.
                 Defaults to 512.
             temperature (float, optional): how consistent the llm performs.
                 The lower the more consistent. To obtain diverse questions,
                 a high temperature is recommended.
                 Defaults to 0.0.
         """
-        prompt = BasicPrompt.\
-            load_prompt_from_json_file(prompt_name)
-        llm = OpenAI(temperature=temperature, openai_api_key=open_ai_key)
-        llm.max_tokens = max_output_tokens
-        super().__init__(prompt=prompt,
-                         llm=llm)
+        super().__init__(open_ai_key=open_ai_key,
+                         prompt_name=prompt_name,
+                         max_output_tokens=max_output_tokens,
+                         temperature=temperature)
 
     def equip_retriever(self, retriever: BasicQuestionModerateRetriever):
         # notice it requires DatabaseQuestionModerateRetriever
         object.__setattr__(self, 'retriever', retriever)
 
     def predict_decision_only(self, user_input: str) -> bool:
         """
```

### Comparing `llmreflect-0.0.4/llmreflect/Agents/PostgresqlAgent.py` & `llmreflect-0.0.5/llmreflect/Agents/PostgresqlAgent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from llmreflect.Agents.BasicAgent import Agent
-from langchain.llms.openai import OpenAI
+from llmreflect.Agents.BasicAgent import OpenAIAgent
 from llmreflect.Utils.message import message
 from llmreflect.Retriever.DatabaseRetriever import DatabaseRetriever
-from llmreflect.Prompt.BasicPrompt import BasicPrompt
 from typing import Any
 
 
-class PostgresqlAgent(Agent):
+class PostgresqlAgent(OpenAIAgent):
     """
     Agent class for executing postgresql command
     Args:
         Agent (_type_): _description_
     """
     def __init__(self, open_ai_key: str,
                  prompt_name: str = 'postgresql',
@@ -24,19 +22,18 @@
             prompt_name (str, optional): name for the prompt json file.
                 Defaults to 'postgressql'.
             max_output_tokens (int, optional): maximum completion length.
                 Defaults to 512.
             temperature (float, optional): how consistent the llm performs.
                 The lower the more consistent. Defaults to 0.0.
         """
-        prompt = BasicPrompt.load_prompt_from_json_file(prompt_name)
-        llm = OpenAI(temperature=temperature, openai_api_key=open_ai_key)
-        llm.max_tokens = max_output_tokens
-        super().__init__(prompt=prompt,
-                         llm=llm)
+        super().__init__(open_ai_key=open_ai_key,
+                         prompt_name=prompt_name,
+                         max_output_tokens=max_output_tokens,
+                         temperature=temperature)
         object.__setattr__(self, 'split_symbol', split_symbol)
 
     def equip_retriever(self, retriever: DatabaseRetriever):
         """_summary_
 
         Args:
             retriever (DatabaseRetriever): use database retriever
```

### Comparing `llmreflect-0.0.4/llmreflect/Agents/QuestionAgent.py` & `llmreflect-0.0.5/llmreflect/Agents/QuestionAgent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from llmreflect.Agents.BasicAgent import Agent
-from llmreflect.Prompt.BasicPrompt import BasicPrompt
-from langchain.llms.openai import OpenAI
+from llmreflect.Agents.BasicAgent import OpenAIAgent
 from llmreflect.Utils.message import message
 from llmreflect.Retriever.DatabaseRetriever import DatabaseQuestionRetriever
 
 
-class PostgresqlQuestionAgent(Agent):
+class PostgresqlQuestionAgent(OpenAIAgent):
     """
     Agent for creating questions based on a given database
     Args:
         Agent (_type_): _description_
     """
     def __init__(self, open_ai_key: str,
                  prompt_name: str = 'questionpostgresql',
@@ -24,20 +22,18 @@
             max_output_tokens (int, optional): maximum completion length.
                 Defaults to 512.
             temperature (float, optional): how consistent the llm performs.
                 The lower the more consistent. To obtain diverse questions,
                 a high temperature is recommended.
                 Defaults to 0.0.
         """
-        prompt = BasicPrompt.\
-            load_prompt_from_json_file(prompt_name)
-        llm = OpenAI(temperature=temperature, openai_api_key=open_ai_key)
-        llm.max_tokens = max_output_tokens
-        super().__init__(prompt=prompt,
-                         llm=llm)
+        super().__init__(open_ai_key=open_ai_key,
+                         prompt_name=prompt_name,
+                         max_output_tokens=max_output_tokens,
+                         temperature=temperature)
 
     def equip_retriever(self, retriever: DatabaseQuestionRetriever):
         # notice it requires DatabaseQuestionRetriever
         object.__setattr__(self, 'retriever', retriever)
 
     def predict_n_questions(self, n_questions: int = 5) -> str:
         """
```

### Comparing `llmreflect-0.0.4/llmreflect/Chains/BasicChain.py` & `llmreflect-0.0.5/llmreflect/Chains/BasicChain.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/llmreflect/Chains/DatabaseChain.py` & `llmreflect-0.0.5/llmreflect/Chains/DatabaseChain.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from llmreflect.Agents.QuestionAgent import PostgresqlQuestionAgent
 from llmreflect.Agents.PostgresqlAgent import PostgresqlAgent, \
     PostgresqlSelfFixAgent
 from llmreflect.Agents.EvaluationAgent import PostgressqlGradingAgent
 from llmreflect.Retriever.DatabaseRetriever import DatabaseQuestionRetriever, \
     DatabaseRetriever
 from llmreflect.Retriever.BasicRetriever import BasicEvaluationRetriever
+from llmreflect.Chains.ModerateChain import ModerateChain
 from typing import List
 from llmreflect.Utils.message import message
 
 
 class DatabaseQuestionChain(BasicChain):
     def __init__(self, agent: PostgresqlQuestionAgent,
                  retriever: DatabaseQuestionRetriever):
@@ -111,84 +112,137 @@
         return self.agent.predict_db(
             user_input=user_input,
             get_cmd=get_cmd,
             get_summary=get_summary,
             get_db=get_db)
 
 
-class DatabaseQnAGradingChain(BasicChain):
+class DatabaseGradingChain(BasicChain):
     def __init__(self, agent: PostgressqlGradingAgent,
-                 retriever: BasicEvaluationRetriever,
-                 db_q_chain: DatabaseQuestionChain,
-                 db_a_chain: DatabaseAnswerChain,
-                 q_batch_size: int = 5):
-        """
+                 retriever: BasicEvaluationRetriever):
+        """_summary_
         A chain for the following workflow:
-        1. create questions based on the database
-        2. generate postgresql solutions for questions
-        3. evaluate the generated solutions
+        1. given by questions about a database and according
+            postgresql solutions for questions
+        2. evaluate the generated solutions
         Args:
             agent (PostgressqlGradingAgent): _description_
             retriever (BasicEvaluationRetriever): _description_
-            db_q_chain: chain for questioning
-            db_a_chain: chain for answering
-            q_batch_size: in each batch, ask how many questions
         """
         super().__init__(agent, retriever)
-        self.db_q_chain = db_q_chain
-        self.db_a_chain = db_a_chain
+
+    @classmethod
+    def from_config(cls,
+                    open_ai_key: str,
+                    max_output_tokens: int = 256,
+                    prompt_name: str = "gradingpostgresql",
+                    temperature: float = 0.7):
+        """_summary_
+
+        Args:
+            open_ai_key (str): _description_
+            max_output_tokens (int, optional): dont need to be long.
+                Defaults to 256.
+            prompt_name (str, optional): _description_.
+                Defaults to "gradingpostgresql".
+            temperature (float, optional): questions should be diverse.
+                Set this to a high value but lower than 1. Defaults to 0.7.
+
+        Returns:
+            _type_: _description_
+        """
+        agent = PostgressqlGradingAgent(
+            open_ai_key=open_ai_key,
+            prompt_name=prompt_name,
+            max_output_tokens=max_output_tokens,
+            temperature=temperature)
+
+        retriever = BasicEvaluationRetriever()
+        return cls(agent=agent, retriever=retriever)
+
+    def perform(self, question: str,
+                query: str,
+                db_summary: str) -> dict:
+        """_summary_
+
+        Args:
+            question (str): queries about a dataset
+            query (str): generated queries
+            db_summary (str): execution summary
+
+        Returns:
+            dict: {"grading": a float number between 0 to 10,
+                    "explanation": explanation for the score assigned}
+        """
+        grad_dict = self.agent.grade(request=question,
+                                     sql_cmd=query,
+                                     db_summary=db_summary)
+        return grad_dict
+
+
+class DatabaseQnAGradingChain(BasicCombinedChain):
+    def __init__(self, chains: List[BasicChain], q_batch_size: int = 5):
+        super().__init__(chains)
+        assert len(chains) == 3
+
+        for chain in self.chains:
+            if chain.__class__ == DatabaseAnswerChain:
+                self.db_a_chain = chain
+            elif chain.__class__ == DatabaseQuestionChain:
+                self.db_q_chain = chain
+            elif chain.__class__ == DatabaseGradingChain:
+                self.db_g_chain = chain
+            else:
+                raise Exception("Illegal chains!")
         self.q_batch_size = q_batch_size
 
     @classmethod
     def from_config(cls, uri: str,
                     include_tables: List,
                     open_ai_key: str,
-                    q_prompt_name: str = 'questionpostgresql',
-                    a_prompt_name: str = 'postgresql',
-                    g_prompt_name: str = 'gradingpostgresql',
-                    q_max_output_tokens: int = 512,
+                    question_chain_prompt_name: str = 'questionpostgresql',
+                    answer_chain_prompt_name: str = 'postgresql',
+                    grading_chain_prompt_name: str = 'gradingpostgresql',
+                    q_max_output_tokens: int = 256,
                     q_temperature: float = 0.7,
                     a_max_output_tokens: int = 512,
-                    g_max_output_tokens: int = 512,
+                    g_max_output_tokens: int = 256,
                     a_temperature: float = 0.0,
                     g_temperature: float = 0.0,
                     sample_rows: int = 0,
                     max_rows_return=500):
 
         db_q_chain = DatabaseQuestionChain.from_config(
             uri=uri,
             include_tables=include_tables,
             open_ai_key=open_ai_key,
-            prompt_name=q_prompt_name,
+            prompt_name=question_chain_prompt_name,
             max_output_tokens=q_max_output_tokens,
             temperature=q_temperature,
             sample_rows=sample_rows
         )
 
         db_a_chain = DatabaseAnswerChain.from_config(
             uri=uri,
             include_tables=include_tables,
             open_ai_key=open_ai_key,
-            prompt_name=a_prompt_name,
+            prompt_name=answer_chain_prompt_name,
             max_output_tokens=a_max_output_tokens,
             temperature=a_temperature,
             sample_rows=sample_rows,
             max_rows_return=max_rows_return
         )
 
-        agent = PostgressqlGradingAgent(
+        db_g_chain = DatabaseGradingChain.from_config(
             open_ai_key=open_ai_key,
-            prompt_name=g_prompt_name,
+            prompt_name=grading_chain_prompt_name,
             max_output_tokens=g_max_output_tokens,
             temperature=g_temperature)
 
-        retriever = BasicEvaluationRetriever()
-        return cls(agent=agent, retriever=retriever,
-                   db_a_chain=db_a_chain,
-                   db_q_chain=db_q_chain,
+        return cls(chains=[db_q_chain, db_a_chain, db_g_chain],
                    q_batch_size=5)
 
     def perform(self, n_question: int = 5) -> dict:
         """_summary_
 
         Args:
             n_question (int, optional): _description_. Defaults to 5.
@@ -217,95 +271,30 @@
         for q in t_questions:
             temp_dict = self.db_a_chain.perform(
                 user_input=q,
                 get_cmd=True,
                 get_summary=True,
                 get_db=False
             )
-            grad_dict = self.agent.grade(
-                request=q,
-                sql_cmd=temp_dict['cmd'],
+            grad_dict = self.db_g_chain.perform(
+                question=q,
+                query=temp_dict['cmd'],
                 db_summary=temp_dict['summary']
             )
             t_logs.append({
                 "question": q,
                 "cmd": temp_dict['cmd'],
                 "summary": temp_dict['summary'],
                 "grading": grad_dict['grading'],
                 "explanation": grad_dict['explanation']
             })
 
         return t_logs
 
 
-class DatabaseSelfFixChain(BasicChain):
-    """
-    A chain class for fixing sql errors
-    Args:
-        BasicChain (_type_): _description_
-    """
-    def __init__(self,
-                 agent: PostgresqlSelfFixAgent,
-                 retriever: DatabaseRetriever):
-        super().__init__(agent, retriever)
-
-    @classmethod
-    def from_config(cls, uri: str,
-                    include_tables: List,
-                    open_ai_key: str,
-                    prompt_name: str = 'postgresqlfix',
-                    max_output_tokens: int = 512,
-                    temperature: float = 0.0,
-                    sample_rows: int = 0,
-                    max_rows_return: int = 500):
-        agent = PostgresqlSelfFixAgent(
-            open_ai_key=open_ai_key,
-            prompt_name=prompt_name,
-            max_output_tokens=max_output_tokens,
-            temperature=temperature)
-
-        retriever = DatabaseRetriever(
-            uri=uri,
-            include_tables=include_tables,
-            max_rows_return=max_rows_return,
-            sample_rows=sample_rows
-        )
-        return cls(agent=agent, retriever=retriever)
-
-    def perform(self,
-                user_input: str,
-                history: str,
-                his_error: str,
-                get_cmd: bool = True,
-                get_db: bool = False,
-                get_summary: bool = True) -> dict:
-        """_summary_
-
-        Args:
-            user_input (str): user's description
-            history (str): history command used for query
-            his_error (str): the errors raised from executing the history cmd
-            get_cmd (bool, optional): if return cmd. Defaults to True.
-            get_db (bool, optional): if return queried db gross result.
-                Defaults to False.
-            get_summary (bool, optional): if return a summary of the result.
-                Defaults to True.
-
-        Returns:
-            dict: {'cmd': sql_cmd, 'summary': summary, 'db': gross db response}
-        """
-        return self.agent.predict_db(
-            user_input=user_input,
-            history=history,
-            his_error=his_error,
-            get_cmd=get_cmd,
-            get_summary=get_summary,
-            get_db=get_db)
-
-
 class DatabaseAnswerNFixChain(BasicCombinedChain):
     def __init__(self, chains: List[BasicChain], fix_patience: int = 3):
         super().__init__(chains)
         assert len(chains) == 2
         self.fix_patience = fix_patience
         for chain in self.chains:
             if chain.__class__ == DatabaseAnswerChain:
@@ -319,37 +308,39 @@
     def from_config(
             cls,
             uri: str,
             include_tables: list,
             open_ai_key: str,
             answer_chain_prompt_name: str,
             fix_chain_prompt_name: str,
-            max_output_tokens: int = 512,
-            temperature: float = 0.0,
+            max_output_tokens_a: int = 512,
+            max_output_tokens_f: int = 512,
+            temperature_a: float = 0.0,
+            temperature_f: float = 0.0,
             sample_row: int = 0,
             max_rows_return: int = 500,
             fix_patience: int = 3):
 
         db_a_chain = DatabaseAnswerChain.from_config(
             uri=uri,
             include_tables=include_tables,
             open_ai_key=open_ai_key,
             prompt_name=answer_chain_prompt_name,
-            max_output_tokens=max_output_tokens,
-            temperature=temperature,
+            max_output_tokens=max_output_tokens_a,
+            temperature=temperature_a,
             sample_rows=sample_row,
             max_rows_return=max_rows_return
         )
         db_fix_chain = DatabaseSelfFixChain.from_config(
             uri=uri,
             include_tables=include_tables,
             open_ai_key=open_ai_key,
             prompt_name=fix_chain_prompt_name,
-            max_output_tokens=max_output_tokens,
-            temperature=temperature,
+            max_output_tokens=max_output_tokens_f,
+            temperature=temperature_f,
             sample_rows=sample_row,
             max_rows_return=max_rows_return
         )
         return cls(chains=[db_a_chain, db_fix_chain],
                    fix_patience=fix_patience)
 
     def perform(self,
@@ -424,7 +415,185 @@
         if not get_summary:
             get_summary = ""
 
         return {'cmd': sql_cmd,
                 'summary': summary,
                 'db': db_result,
                 'error': error_logs}
+
+
+class DatabaseSelfFixChain(BasicChain):
+    """
+    A chain class for fixing sql errors
+    Args:
+        BasicChain (_type_): _description_
+    """
+    def __init__(self,
+                 agent: PostgresqlSelfFixAgent,
+                 retriever: DatabaseRetriever):
+        super().__init__(agent, retriever)
+
+    @classmethod
+    def from_config(cls, uri: str,
+                    include_tables: List,
+                    open_ai_key: str,
+                    prompt_name: str = 'postgresqlfix',
+                    max_output_tokens: int = 512,
+                    temperature: float = 0.0,
+                    sample_rows: int = 0,
+                    max_rows_return: int = 500):
+        agent = PostgresqlSelfFixAgent(
+            open_ai_key=open_ai_key,
+            prompt_name=prompt_name,
+            max_output_tokens=max_output_tokens,
+            temperature=temperature)
+
+        retriever = DatabaseRetriever(
+            uri=uri,
+            include_tables=include_tables,
+            max_rows_return=max_rows_return,
+            sample_rows=sample_rows
+        )
+        return cls(agent=agent, retriever=retriever)
+
+    def perform(self,
+                user_input: str,
+                history: str,
+                his_error: str,
+                get_cmd: bool = True,
+                get_db: bool = False,
+                get_summary: bool = True) -> dict:
+        """_summary_
+
+        Args:
+            user_input (str): user's description
+            history (str): history command used for query
+            his_error (str): the errors raised from executing the history cmd
+            get_cmd (bool, optional): if return cmd. Defaults to True.
+            get_db (bool, optional): if return queried db gross result.
+                Defaults to False.
+            get_summary (bool, optional): if return a summary of the result.
+                Defaults to True.
+
+        Returns:
+            dict: {'cmd': sql_cmd, 'summary': summary, 'db': gross db response}
+        """
+        return self.agent.predict_db(
+            user_input=user_input,
+            history=history,
+            his_error=his_error,
+            get_cmd=get_cmd,
+            get_summary=get_summary,
+            get_db=get_db)
+
+
+class DatabaseModerateNAnswerNFixChain(BasicCombinedChain):
+    def __init__(self, chains: List[BasicChain], fix_patience: int = 3):
+        super().__init__(chains)
+        assert len(chains) == 2
+        self.fix_patience = fix_patience
+        for chain in self.chains:
+            if chain.__class__ == ModerateChain:
+                self.moderate_chain = chain
+            elif chain.__class__ == DatabaseAnswerNFixChain:
+                self.a_n_f_chain = chain
+            else:
+                raise Exception("Illegal chains!")
+
+    @classmethod
+    def from_config(
+            cls,
+            uri: str,
+            include_tables: list,
+            open_ai_key: str,
+            answer_chain_prompt_name: str = "postgresql",
+            fix_chain_prompt_name: str = "postgresqlfix",
+            moderate_chain_prompt_name: str = "moderatepostgresql",
+            max_output_tokens_a: int = 512,
+            max_output_tokens_f: int = 512,
+            max_output_tokens_m: int = 256,
+            temperature_a: float = 0.0,
+            temperature_f: float = 0.0,
+            temperature_m: float = 0.0,
+            sample_row: int = 0,
+            max_rows_return: int = 500,
+            fix_patience: int = 3):
+
+        db_m_chain = ModerateChain.from_config(
+            open_ai_key=open_ai_key,
+            include_tables=include_tables,
+            prompt_name=moderate_chain_prompt_name,
+            max_output_tokens=max_output_tokens_m,
+            temperature=temperature_m
+        )
+        db_a_fix_chain = DatabaseAnswerNFixChain.from_config(
+            uri=uri,
+            include_tables=include_tables,
+            open_ai_key=open_ai_key,
+            answer_chain_prompt_name=answer_chain_prompt_name,
+            fix_chain_prompt_name=fix_chain_prompt_name,
+            max_output_tokens_a=max_output_tokens_a,
+            max_output_tokens_f=max_output_tokens_f,
+            temperature_a=temperature_a,
+            temperature_f=temperature_f,
+            sample_row=sample_row,
+            max_rows_return=max_rows_return,
+            fix_patience=fix_patience
+        )
+
+        return cls(chains=[db_m_chain, db_a_fix_chain],
+                   fix_patience=fix_patience)
+
+    def perform(self,
+                user_input: str,
+                get_cmd: bool = True,
+                get_db: bool = False,
+                get_summary: bool = True,
+                log_fix: bool = True,
+                explain_moderate: bool = True) -> dict:
+        """_summary_
+
+        Args:
+            user_input (str): _description_
+            get_cmd (bool, optional): _description_. Defaults to True.
+            get_db (bool, optional): _description_. Defaults to False.
+            get_summary (bool, optional): _description_. Defaults to True.
+            log_fix (bool, optional): _description_. Defaults to True.
+
+        Returns:
+            dict: 'cmd': str, sql_cmd,
+                'summary': str, summary,
+                'db': str, db_result,
+                'error': dict, error_logs: 'cmd', what sql cmd caused error,
+                                            'error', what is the error
+        """
+        assert get_cmd or get_db or get_summary
+
+        moderate_dict = self.moderate_chain.perform(
+            user_input=user_input,
+            with_explanation=explain_moderate
+        )
+        moderate_decision = moderate_dict['decision']
+        moderate_explanation = moderate_dict['explanation']
+        if not moderate_decision:
+            return_dict = {'cmd': "",
+                           'summary': "",
+                           'db': "",
+                           'error': "",
+                           'moderate_decision': moderate_decision,
+                           'moderate_explanation': moderate_explanation
+                           }
+            return return_dict
+
+        answer_dict = self.a_n_f_chain.perform(
+            user_input=user_input,
+            get_cmd=True,
+            get_db=get_db,
+            get_summary=True
+        )
+
+        return {'cmd': answer_dict['cmd'],
+                'summary': answer_dict['summary'],
+                'db': answer_dict['db'],
+                'error': answer_dict['error'],
+                'moderate_decision': moderate_decision,
+                'moderate_explanation': moderate_explanation}
```

### Comparing `llmreflect-0.0.4/llmreflect/Chains/ModerateChain.py` & `llmreflect-0.0.5/llmreflect/Chains/ModerateChain.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,20 +27,22 @@
             include_tables=include_tables)
         return cls(agent=agent, retriever=retriever)
 
     def perform(self, user_input: str,
                 with_explanation: bool = False) -> Any:
         """
         Overwrite perform function.
-        Generate n questions.
+        Sensor the questions if they are allowed
         Args:
-            n_questions (int, optional): _description_. Defaults to 5.
+            user_input (str): user's natural language request
+            with_explanation (bool): if add explanation
 
         Returns:
-            list: a list of questions, each question is a str object.
+            without explanation: return a boolean variable
+            with explanation: dict: {'decision': bool, 'explanation': str}
         """
         if with_explanation:
             result = self.agent.predict_decision_explained(
                 user_input=user_input)
         else:
             result = self.agent.predict_decision_only(user_input=user_input)
         return result
```

### Comparing `llmreflect-0.0.4/llmreflect/Prompt/BasicPrompt.py` & `llmreflect-0.0.5/llmreflect/Prompt/BasicPrompt.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/llmreflect/Prompt/promptbase/gradingpostgresql.json` & `llmreflect-0.0.5/llmreflect/Prompt/promptbase/gradingpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/llmreflect/Prompt/promptbase/moderatepostgresql.json` & `llmreflect-0.0.5/llmreflect/Prompt/promptbase/moderatepostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/llmreflect/Prompt/promptbase/postgresql.json` & `llmreflect-0.0.5/llmreflect/Prompt/promptbase/postgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/llmreflect/Prompt/promptbase/postgresqlfix.json` & `llmreflect-0.0.5/llmreflect/Prompt/promptbase/postgresqlfix.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/llmreflect/Prompt/promptbase/questionpostgresql.json` & `llmreflect-0.0.5/llmreflect/Prompt/promptbase/questionpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/llmreflect/Retriever/BasicRetriever.py` & `llmreflect-0.0.5/llmreflect/Retriever/BasicRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/llmreflect/Retriever/DatabaseRetriever.py` & `llmreflect-0.0.5/llmreflect/Retriever/DatabaseRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/llmreflect/Tests/test_chains.py` & `llmreflect-0.0.5/llmreflect/Tests/test_chains.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,48 @@
         or os.getenv("CIRCLECI") \
         or os.getenv("GITLAB_CI")
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
+def test_moderate_answer_fix_chain():
+    from llmreflect.Chains.DatabaseChain import \
+        DatabaseModerateNAnswerNFixChain
+    from decouple import config
+
+    uri = f"postgresql+psycopg2://{config('DBUSERNAME')}:\
+{config('DBPASSWORD')}@{config('DBHOST')}:{config('DBPORT')}/postgres"
+
+    ch = DatabaseModerateNAnswerNFixChain.from_config(
+        uri=uri,
+        include_tables=[
+            'tb_patient',
+            'tb_patients_allergies',
+            'tb_appointment_patients',
+            'tb_patient_mmse_and_moca_scores',
+            'tb_patient_medications'
+        ],
+        open_ai_key=config('OPENAI_API_KEY')
+    )
+    result = ch.perform(user_input="give me a list of patients",
+                        explain_moderate=True)
+    print(result)
+    assert result['moderate_decision']
+
+    result = ch.perform(user_input="Cats are the true rulers",
+                        explain_moderate=True)
+    assert not result['moderate_decision']
+    assert len(result['moderate_explanation']) > 0
+    print(result)
+
+
+@pytest.mark.skipif(bool(in_workflow()),
+                    reason="Only test database operations \
+                    in local env")
 def test_moderate_chain():
     from llmreflect.Chains.ModerateChain import ModerateChain
     from decouple import config
     ch = ModerateChain.from_config(
         open_ai_key=config('OPENAI_API_KEY'),
         include_tables=[
             'tb_patient',
@@ -40,44 +74,54 @@
     assert len(result['explanation']) > 0
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
 def test_grading_chain():
-
     from llmreflect.Chains.DatabaseChain import DatabaseQnAGradingChain
     from decouple import config
+    import pandas as pd
+
+    SAVE_LOG = False
+    N_QUESTIONS = 12
+
     uri = f"postgresql+psycopg2://{config('DBUSERNAME')}:\
 {config('DBPASSWORD')}@{config('DBHOST')}:{config('DBPORT')}/postgres"
 
     ch = DatabaseQnAGradingChain.from_config(
         uri=uri,
         include_tables=[
             'tb_patient',
             'tb_patients_allergies',
             'tb_appointment_patients',
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ],
+        a_max_output_tokens=512,
+        g_max_output_tokens=256,
         open_ai_key=config('OPENAI_API_KEY')
     )
-    logs = ch.perform(n_question=5)
-    for log in logs:
-        message("Question: " + log["question"], 'blue')
-        message("Query: " + log["cmd"], 'yellow')
-        message("Summary: " + log["summary"], "green")
-        message("Score: %.2f" % log["grading"], 'yellow')
-        message("Explain: " + log["explanation"], "green")
-        assert len(log["question"]) > 0
-        assert len(log["cmd"]) > 0
-        assert len(log["summary"]) > 0
-        assert len(log["explanation"]) > 0
-        assert log["grading"] > 0
-        print("=========================\n\n")
+    logs = ch.perform(n_question=N_QUESTIONS)
+    if SAVE_LOG:
+        df = pd.DataFrame.from_records(logs)
+        df.to_csv("self_grading.csv")
+    else:
+        for log in logs:
+            message("Question: " + log["question"], 'blue')
+            message("Query: " + log["cmd"], 'yellow')
+            message("Summary: " + log["summary"], "green")
+            message("Score: %.2f" % log["grading"], 'yellow')
+            message("Explain: " + log["explanation"], "green")
+            assert len(log["question"]) > 0
+            assert len(log["cmd"]) > 0
+            assert len(log["summary"]) > 0
+            assert len(log["explanation"]) > 0
+            assert log["grading"] > 0
+            print("=========================\n\n")
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
 def test_self_fix_chain():
     from llmreflect.Chains.DatabaseChain import DatabaseQuestionChain,\
```

### Comparing `llmreflect-0.0.4/llmreflect/Utils/database.py` & `llmreflect-0.0.5/llmreflect/Utils/database.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.4/PKG-INFO` & `llmreflect-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmreflect
-Version: 0.0.4
+Version: 0.0.5
 Summary: a package for llm self-reflection
 Author: alchemistwu
 Author-email: alchemistwu0521@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

