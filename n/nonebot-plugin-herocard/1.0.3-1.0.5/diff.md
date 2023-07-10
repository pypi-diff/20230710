# Comparing `tmp/nonebot-plugin-herocard-1.0.3.tar.gz` & `tmp/nonebot-plugin-herocard-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-herocard-1.0.3.tar", last modified: Wed May 24 15:23:32 2023, max compression
+gzip compressed data, was "nonebot-plugin-herocard-1.0.5.tar", last modified: Mon Jul 10 09:27:17 2023, max compression
```

## Comparing `nonebot-plugin-herocard-1.0.3.tar` & `nonebot-plugin-herocard-1.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1707 2023-05-24 15:23:22.964186 nonebot-plugin-herocard-1.0.3/README.md
--rw-r--r--   0        0        0     2704 2023-05-24 15:23:22.964186 nonebot-plugin-herocard-1.0.3/nonebot_plugin_herocard/__init__.py
--rw-r--r--   0        0        0      588 2023-05-24 15:23:22.964186 nonebot-plugin-herocard-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 nonebot-plugin-herocard-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2305 2023-07-10 09:27:09.862390 nonebot-plugin-herocard-1.0.5/README.md
+-rw-r--r--   0        0        0     2747 2023-07-10 09:27:09.862390 nonebot-plugin-herocard-1.0.5/nonebot_plugin_herocard/__init__.py
+-rw-r--r--   0        0        0      588 2023-07-10 09:27:09.862390 nonebot-plugin-herocard-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 nonebot-plugin-herocard-1.0.5/PKG-INFO
```

### Comparing `nonebot-plugin-herocard-1.0.3/nonebot_plugin_herocard/__init__.py` & `nonebot-plugin-herocard-1.0.5/nonebot_plugin_herocard/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,18 @@
     if text := event.get_plaintext():
         text_list = []
         # 按照空白行分割文本成多个段落，排除包含空白字符的段落
         raw_text_list = text.split('\n')
         raw_text_list = [paragraph.strip() for paragraph in raw_text_list if paragraph.strip()]
         # 循环遍历 text_list 中的内容
         for text in raw_text_list:
-                edit_text = re.sub(r'#\((呵呵|哈哈|吐舌|啊|酷|怒|开心|汗|泪|黑线|鄙视|不高兴|真棒|钱|疑问|阴险|吐|咦|委屈|花心|呼~|笑眼|冷|太开心|滑稽|勉强|狂汗|乖|睡觉|惊哭|生气|惊讶|喷|爱心|心碎|玫瑰|礼物|彩虹|星星月亮|太阳|钱币|灯泡|茶杯|蛋糕|音乐|haha|胜利|大拇指|弱|OK|瓜|翔|吓|帅|小乖|捂嘴笑|你懂的|what|酸爽|呀咩爹|笑尿|挖鼻|犀利|小红脸|懒得理|沙发|手纸|香蕉|便便|药丸|红领巾|蜡烛|三道杠|暗中观察|吃瓜|喝酒|嘿嘿嘿|噗|困成狗|微微一笑|托腮|摊手|柯基暗中观察|欢呼|炸药|突然兴奋|紧张|黑头瞪眼|黑头高兴)\)', '', text)
+                edit_text = re.sub(r'#\((呵呵|哈哈|吐舌|啊|酷|怒|开心|汗|泪|黑线|鄙视|不高兴|真棒|钱|疑问|阴险|吐|咦|委屈|花心|呼~|笑眼|冷|太开心|滑稽|勉强|狂汗|乖|睡觉|惊哭|生气|惊讶|喷|爱心|心碎|玫瑰|礼物|彩虹|星星月亮|太阳|钱币|灯泡|茶杯|蛋糕|音乐|haha|胜利|大拇指|弱|OK|瓜|翔|吓|帅|小乖|捂嘴笑|你懂的|what|酸爽|呀咩爹|笑尿|挖鼻|犀利|小红脸|懒得理|沙发|手纸|香蕉|便便|药丸|红领巾|蜡烛|三道杠|暗中观察|吃瓜|喝酒|嘿嘿嘿|噗|困成狗|微微一笑|托腮|摊手|柯基暗中观察|欢呼|炸药|突然兴奋|紧张|黑头瞪眼|黑头高兴)\) ', '', text)
                 text_list.append(edit_text)
         for text in text_list:
             msg = hero(text)
-            # print(msg)
-            await hero_assistant.finish(str(msg))
+            if msg == None:
+                continue
+            else:
+                # print(msg)
+                await hero_assistant.send(str(msg))
     else:
-        await hero_assistant.finish("呜...出错了，前后加个'。'再试试？")
+        await hero_assistant.finish("结束进程")
```

### Comparing `nonebot-plugin-herocard-1.0.3/pyproject.toml` & `nonebot-plugin-herocard-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-herocard"
-version = "1.0.3"
+version = "1.0.5"
 description = "用于提取本子🥵标题关键词的 NoneBot2 插件"
 authors = [
     { name = "Xie-Tiao", email = "1183004468@qq.com" },
 ]
 license = "MIT"
 dependencies = [
     "nonebot2>=2.0.0b2",
```

