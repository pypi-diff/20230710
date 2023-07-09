# Comparing `tmp/ofscraper-2.6.4.tar.gz` & `tmp/ofscraper-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.6.4.tar", max compression
+gzip compressed data, was "ofscraper-2.7.tar", max compression
```

## Comparing `ofscraper-2.6.4.tar` & `ofscraper-2.7.tar`

### file list

```diff
@@ -1,51 +1,57 @@
--rw-r--r--   0        0        0     1067 2023-07-01 20:38:09.278774 ofscraper-2.6.4/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-01 20:38:09.278774 ofscraper-2.6.4/README.md
--rw-r--r--   0        0        0      607 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     8526 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/archive.py
--rw-r--r--   0        0        0     5019 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1067 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/init.py
--rw-r--r--   0        0        0     2859 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/me.py
--rw-r--r--   0        0        0     9222 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/messages.py
--rw-r--r--   0        0        0    10084 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5672 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/pinned.py
--rw-r--r--   0        0        0    11976 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/posts.py
--rw-r--r--   0        0        0     3909 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3408 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     8918 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/timeline.py
--rw-r--r--   0        0        0    14531 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/commands/check.py
--rw-r--r--   0        0        0     4942 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    13967 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     6339 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     8581 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3253 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     5037 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      696 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7683 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    27832 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     1209 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    11211 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8986 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    10803 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    20240 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     3376 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     6486 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     9615 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/of.py
--rw-r--r--   0        0        0    11732 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4263 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1358 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0    29248 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/table.py
--rw-r--r--   0        0        0     5818 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1759 2023-07-01 20:38:42.271109 ofscraper-2.6.4/pyproject.toml
--rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 ofscraper-2.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-09 23:08:33.766147 ofscraper-2.7/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-09 23:08:33.766147 ofscraper-2.7/README.md
+-rw-r--r--   0        0        0      607 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/__init__.py
+-rw-r--r--   0        0        0     1007 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     9002 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     9866 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/init.py
+-rw-r--r--   0        0        0     8238 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2859 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9763 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    10276 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     6012 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     3999 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3408 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     9480 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0        0 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/classes/__init__.py
+-rw-r--r--   0        0        0      804 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0     8861 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     7274 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     3603 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0    14535 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     4946 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    14111 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     6818 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    10059 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3576 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     5037 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      696 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7683 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    29826 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     1583 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    12152 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     9703 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    13073 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    24710 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     5435 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     7193 2023-07-09 23:08:33.774147 ofscraper-2.7/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0    10696 2023-07-09 23:08:33.778147 ofscraper-2.7/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7013 2023-07-09 23:08:33.778147 ofscraper-2.7/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4263 2023-07-09 23:08:33.778147 ofscraper-2.7/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-07-09 23:08:33.778147 ofscraper-2.7/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1211 2023-07-09 23:08:33.778147 ofscraper-2.7/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-07-09 23:08:33.778147 ofscraper-2.7/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0    29248 2023-07-09 23:08:33.778147 ofscraper-2.7/ofscraper/utils/table.py
+-rw-r--r--   0        0        0     5818 2023-07-09 23:08:33.778147 ofscraper-2.7/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1926 2023-07-09 23:09:11.726244 ofscraper-2.7/pyproject.toml
+-rw-r--r--   0        0        0     4546 1970-01-01 00:00:00.000000 ofscraper-2.7/PKG-INFO
```

### Comparing `ofscraper-2.6.4/LICENSE` & `ofscraper-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/README.md` & `ofscraper-2.7/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/__init__.py` & `ofscraper-2.7/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/__version__.py` & `ofscraper-2.7/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/api/archive.py` & `ofscraper-2.7/ofscraper/api/archive.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,16 @@
                 if len(posts)==0:
                     log.debug(f" {log_id} -> number of post found 0")
                 elif len(posts)>0:
                     log.debug(f"{log_id} -> number of archived post found {len(posts)}")
                     log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
                     log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
                     log.debug(f"{log_id} -> found archived post IDs {list(map(lambda x:x.get('id'),posts))}")
+                    log.trace("{log_id} -> archive raw {posts}".format(log_id=log_id,posts=  "\n\n".join(list(map(lambda x:f"scrapeinfo archive: {str(x)}",posts)))))
+
        
                     if required_ids==None:
                         attempt.set(0)
                         tasks.append(asyncio.create_task(scrape_archived_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
                     else:
                         [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
 
@@ -112,14 +114,15 @@
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
         
         async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
                             sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.AlT_SEM)) as c: 
 
             oldarchived=cache.get(f"archived_{model_id}",default=[])
+            log.trace("oldarchive {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"oldarchive: {str(x)}",oldarchived)))))
             oldtimeset=set(map(lambda x:x.get("id"),oldarchived))
             log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
             oldarchived=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldarchived))
             postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldarchived)))
             filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
             
         
@@ -151,14 +154,16 @@
     log.debug(f"[bold]Archived Count with Dupes[/bold] {len(responseArray)} found")
     for post in responseArray:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         oldtimeset.discard(post["id"])
         unduped.append(post)
+    log.trace(f"archive dupeset {dupeSet}")
+    log.trace("archived raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo archive: {str(x)}",unduped)))))
     log.debug(f"[bold]Archived Count without Dupes[/bold] {len(unduped)} found")
     if len(oldtimeset)==0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"archived_{model_id}",list(map(lambda x:{"id":x.get("id"),"postedAtPrecise":x.get("postedAtPrecise")},unduped)),expire=constants.RESPONSE_EXPIRY)
         cache.set(f"archived_check_{model_id}{model_id}",unduped,expire=constants.CHECK_EXPIRY)
 
         cache.close()
     elif len(oldtimeset)>0 and not (args_.getargs().before or args_.getargs().after):
```

### Comparing `ofscraper-2.6.4/ofscraper/api/init.py` & `ofscraper-2.7/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/api/me.py` & `ofscraper-2.7/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/api/messages.py` & `ofscraper-2.7/ofscraper/api/messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     page_count=0
     #require a min num of posts to be returned
     min_posts=50
     with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console): 
         async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
                       sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
             oldmessages=cache.get(f"messages_{model_id}",default=[]) if not args_.getargs().no_cache else []
+            log.trace("oldamessage {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"oldtimeline: {str(x)}",oldmessages)))))
+
             oldmsgset=set(map(lambda x:x.get("id"),oldmessages))
             log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
             oldmessages=list(filter(lambda x:(x.get("createdAt") or x.get("postedAt"))!=None,oldmessages))
             startdex=0 if len(oldmessages)==0 else \
             max(([i for i in range(len(oldmessages)) if arrow.get(oldmessages[i].get("createdAt") or oldmessages[i].get("postedAt")) <=(args_.getargs().before or arrow.now())] or [len(oldmessages)])[0]-1,0)
             log.debug(f"Setting Start Index at {startdex}")
             postedAtArray=list(map(lambda x:x["id"],sorted(oldmessages,key=lambda x:arrow.get(x.get("createdAt") or x.get("postedAt") ).float_timestamp,reverse=True)))
@@ -107,14 +109,16 @@
     log.debug(f"[bold]Messages Count with Dupes[/bold] {len(responseArray)} found")
     for message in responseArray:
         if message["id"] in dupeSet:
             continue
         dupeSet.add(message["id"])
         oldmsgset.discard(message["id"])       
         unduped.append(message)
+    log.trace(f"messages dupeset {dupeSet}")
+    log.trace("messages raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo message: {str(x)}",unduped)))))
     if len(oldmsgset)==0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"messages_{model_id}",list(map(lambda x:{"id":x.get("id"),"createdAt":x.get("createdAt") or x.get("postedAt") },unduped)),expire=constants.RESPONSE_EXPIRY)
         cache.set(f"message_check_{model_id}",oldmessages,expire=constants.CHECK_EXPIRY)
 
         cache.close()
     elif len(oldmsgset)>0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"messages_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
@@ -150,14 +154,15 @@
                 if len(messages)==0:
                     log.debug(f"{log_id} -> number of messages found 0")
                 elif len(messages)>0:
                     log.debug(f"{log_id} -> number of messages found {len(messages)}")
                     log.debug(f"{log_id} -> first date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
                     log.debug(f"{log_id} -> last date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
                     log.debug(f"{log_id} -> found message ids {list(map(lambda x:x.get('id'),messages))}")
+                    log.trace("{log_id} -> messages raw {posts}".format(log_id=log_id,posts=  "\n\n".join(list(map(lambda x:f" messages scrapeinfo: {str(x)}",messages)))))
 
 
                     if (arrow.get( messages[-1].get("createdAt") or messages[-1].get("postedAt")).float_timestamp<(args_.getargs().after or arrow.get(0)).float_timestamp):
                         attempt.set(0)
                     elif required_ids==None:
                         attempt.set(0)
                         tasks.append(asyncio.create_task(scrape_messages(c, model_id,progress,message_id=messages[-1]['id'])))
@@ -187,13 +192,14 @@
     headers = auth.make_headers(auth.read_auth())
     url=constants.messageSPECIFIC.format(model_id,postid)
 
     auth.add_cookies(client)
     client.headers.update(auth.create_sign(url, headers))
     r=client.get(url)
     if not r.is_error:
+        log.trace(f"message raw individual {r.json()}")
         return r.json()['list'][0]
     log.debug(f"{r.status_code}")
     log.debug(f"{r.content.decode()}")
```

### Comparing `ofscraper-2.6.4/ofscraper/api/paid.py` & `ofscraper-2.7/ofscraper/api/paid.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,16 @@
                     page_count=page_count+1
                     overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
                     output.extend(result)
                 tasks=list(filter(lambda x:x.done()==False,tasks))
             overall_progress.remove_task(page_task)  
     log.debug(f"[bold]Paid Post count without Dupes[/bold] {len(output)} found")
     # set purchash check values during scan
+    log.trace("paid raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo paid: {str(x)}",output)))))
+
     cache.set(f"purchased_check_{model_id}",output,expire=constants.CHECK_EXPIRY)
     cache.close()
     return output
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_paid(c,username,job_progress,offset=0):
@@ -100,14 +102,15 @@
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
     headers=auth.make_headers(auth.read_auth())
     headers=auth.create_sign(url, headers)
     async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
         sem.release()
         if r.ok:
             data=await r.json()
+            log.trace("paid raw {posts}".format(posts=  data))
             attempt.set(0)
             media=list(filter(lambda x:isinstance(x,list),data.values()))[0]
             log.debug(f"offset:{offset} -> media found {len(media)}")
             log.debug(f"offset:{offset} -> hasmore value in json {data.get('hasMore','undefined') }")
             log.debug(f"offset:{offset} -> found paid content ids {list(map(lambda x:x.get('id'),media))}")
             if  data.get("hasMore"):
                 offset += len(media)
```

### Comparing `ofscraper-2.6.4/ofscraper/api/pinned.py` & `ofscraper-2.7/ofscraper/api/pinned.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,14 +67,15 @@
                 if len(posts)==0:
                     log.debug(f"{log_id} -> number of pinned post f found 0")
                 else:
                     log.debug(f"{log_id} -> number of pinned post found {len(posts)}")
                     log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
                     log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
                     log.debug(f"{log_id} -> found pinned post IDs {list(map(lambda x:x.get('id'),posts))}")
+                    log.trace("{log_id} -> pinned raw {posts}".format(log_id=log_id,posts=  "\n\n".join(list(map(lambda x:f"scrapeinfo pinned: {str(x)}",posts)))))
 
   
                 #post infinite loops            
                 # elif required_ids==None:
                 #     attempt.set(0)
                     # tasks.append(asyncio.create_task(scrape_pinned_posts(headers, model_id,progress,timestamp=posts[0]['postedAtPrecise'])))
             else:
@@ -117,9 +118,11 @@
     dupeSet=set()
     log.debug(f"[bold]Pinned Count with Dupes[/bold] {len(responseArray)} found")
     for post in responseArray:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         unduped.append(post)
+    log.trace(f"pinned dupeset {dupeSet}")
+    log.trace("pinned raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo pinned: {str(x)}",unduped)))))
     log.debug(f"[bold]Pinned Count without Dupes[/bold] {len(unduped)} found")
     return unduped
```

### Comparing `ofscraper-2.6.4/ofscraper/api/profile.py` & `ofscraper-2.7/ofscraper/api/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 
 
 # can get profile from username or id
 @retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def scrape_profile(username:Union[int, str]) -> dict:
     id=cache.get(f"username_{username}",None)
+    log.trace(f"username date: {id}")
     if id:
         return id
     headers = auth.make_headers(auth.read_auth())
 
     attempt.set(attempt.get(0) + 1)
     log.info(f"Attempt {attempt.get()}/{constants.NUM_TRIES} to get profile {username}")
     with httpx.Client(http2=True, headers=headers) as c:
@@ -46,14 +47,15 @@
         c.headers.update(auth.create_sign(url, headers))
 
         r = c.get(profileEP.format(username), timeout=None)
         if not r.is_error:
             attempt.set(0)
             cache.set(f"username_{username}",r.json(),int(HOURLY_EXPIRY*2))
             cache.close()
+            log.trace(f"username date: {r.json()}")
             return r.json()
         elif r.status_code==404:
             return {"username":"modeldeleted"}
         r.raise_for_status()
 
 
 def parse_profile(profile: dict) -> tuple:
```

### Comparing `ofscraper-2.6.4/ofscraper/api/subscriptions.py` & `ofscraper-2.7/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/api/timeline.py` & `ofscraper-2.7/ofscraper/api/timeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,17 +71,17 @@
                     log.debug(f"{log_id} -> number of post found 0")
 
 
                 elif len(posts)>0:
                     log.debug(f"{log_id} -> number of post found {len(posts)}")
                     log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
                     log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
-
                     log.debug(f"{log_id} -> found postids {list(map(lambda x:x.get('id'),posts))}")
-
+                    log.trace("{log_id} -> post raw {posts}".format(log_id=log_id,posts=  "\n\n".join(list(map(lambda x:f"scrapeinfo timeline: {str(x)}",posts)))))
+                               
                     if required_ids==None:
                         attempt.set(0)
                         tasks.append(asyncio.create_task(scrape_timeline_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
                     else:
                         [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
                         #try once more to get id if only 1 left
                         if len(required_ids)==1:
@@ -114,14 +114,16 @@
     page_count=0
     
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
         async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
                       sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
 
             oldtimeline=cache.get(f"timeline_{model_id}",default=[]) if not args_.getargs().no_cache else []
+            log.trace("oldtimeline {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"oldtimeline: {str(x)}",oldtimeline)))))
+
             oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
             log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
             oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
             postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
             filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
             
         
@@ -153,14 +155,16 @@
     log.debug(f"[bold]Timeline Count with Dupes[/bold] {len(responseArray)} found")
     for post in responseArray:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         oldtimeset.discard(post["id"])
         unduped.append(post)
+    log.trace(f"timeline dupeset {dupeSet}")
+    log.trace("post raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo timeline: {str(x)}",unduped)))))
     log.debug(f"[bold]Timeline Count without Dupes[/bold] {len(unduped)} found")
     if len(oldtimeset)==0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"timeline_{model_id}",list(map(lambda x:{"id":x.get("id"),"postedAtPrecise":x.get("postedAtPrecise")},unduped)),expire=constants.RESPONSE_EXPIRY)
         cache.set(f"timeline_check_{model_id}",unduped,expire=constants.CHECK_EXPIRY)
         cache.close()
     elif len(oldtimeset)>0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"timeline_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
@@ -174,11 +178,13 @@
 def get_individual_post(id,client=None):
     headers = auth.make_headers(auth.read_auth())
     url=f"https://onlyfans.com/api2/v2/posts/{id}?skip_users=all"
     auth.add_cookies(client)
     client.headers.update(auth.create_sign(url, headers))
     r=client.get(url)
     if not r.is_error:
+        log.trace(f"post raw individual {r.json()}")
         return r.json()
     log.debug(f"{r.status_code}")
     log.debug(f"{r.content.decode()}")
+
```

### Comparing `ofscraper-2.6.4/ofscraper/commands/check.py` & `ofscraper-2.7/ofscraper/commands/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import arrow
 import ofscraper.utils.args as args_
 import ofscraper.db.operations as operations
 import ofscraper.api.profile as profile
 import ofscraper.utils.auth as auth
 import ofscraper.api.timeline as timeline
 import ofscraper.api.messages as messages_
-import ofscraper.api.posts as posts_
+import ofscraper.classes.posts as posts_
 import ofscraper.constants as constants
 import ofscraper.api.paid as paid_
 import ofscraper.api.archive as archive
 import ofscraper.api.pinned as pinned
 import ofscraper.api.highlights as highlights_
 import ofscraper.utils.console as console_
 import ofscraper.utils.table as table
```

### Comparing `ofscraper-2.6.4/ofscraper/commands/manual.py` & `ofscraper-2.7/ofscraper/commands/manual.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import httpx
 import ofscraper.utils.args as args_
 import ofscraper.api.timeline as timeline
 import ofscraper.api.profile as profile
 import ofscraper.api.timeline as timeline
 import ofscraper.utils.auth as auth
-import ofscraper.api.posts as posts_
+import ofscraper.classes.posts as posts_
 import ofscraper.db.operations as operations
 import ofscraper.utils.download as download
 import ofscraper.api.messages as messages_
 import ofscraper.api.highlights as highlights_
 import ofscraper.constants as constants
```

### Comparing `ofscraper-2.6.4/ofscraper/commands/scraper.py` & `ofscraper-2.7/ofscraper/commands/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,17 +76,21 @@
             # Edit `auth.json` file
             auth.edit_auth()
         
         elif result_main_prompt == 4:
             # Edit `config.json` file
             config.edit_config()
 
+        elif result_main_prompt == 5:
+            # Edit `config.json` file
+            config.edit_config_advanced()
+
         
     
-        elif result_main_prompt == 5:
+        elif result_main_prompt == 6:
             # Display  `Profiles` menu
             result_profiles_prompt = prompts.profiles_prompt()
 
             if result_profiles_prompt == 0:
                 # Change profiles
                 profiles.change_profile()
 
@@ -189,14 +193,15 @@
                 [user_dict.update({ele.post.model_id:user_dict.get(ele.post.model_id,[])+[ele]}) for ele in OF.process_all_paid()]
                 for value in user_dict.values():
                     model_id =value[0].post.model_id
                     username=value[0].post.username
                     operations.create_tables(model_id,username)
                     operations.write_profile_table(model_id,username)
                     asyncio.run(download.process_dicts(
+                        
                     username,
                     model_id,
                     value,
                     ))
             except Exception as e:
                 log.traceback(f"failed with exception: {e}")
                 log.traceback(traceback.format_exc())
```

### Comparing `ofscraper-2.6.4/ofscraper/constants.py` & `ofscraper-2.7/ofscraper/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,43 +33,49 @@
 timelineEP = 'https://onlyfans.com/api2/v2/users/{}/posts?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&pinned=0&format=infinite'
 timelineNextEP = 'https://onlyfans.com/api2/v2/users/{}/posts?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&afterPublishTime={}&pinned=0&format=infinite'
 timelinePinnedEP = 'https://onlyfans.com/api2/v2/users/{}/posts?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&pinnedf=1&format=infinite'
 timelinePinnedNextEP = 'https://onlyfans.com/api2/v2/users/{}/posts?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&pinned=1&afterPublishTime={}&format=infinite'
 archivedEP = 'https://onlyfans.com/api2/v2/users/{}/posts/archived?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&format=infinite'
 archivedNextEP = 'https://onlyfans.com/api2/v2/users/{}/posts/archived?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&afterPublishTime={}&format=infinite'
 
-highlightsWithStoriesEP = 'https://onlyfans.com/api2/v2/users/{}/stories/highlights?limit=5&offset=0&unf=1'
+highlightsWithStoriesEP = 'https://onlyfans.com/api2/v2/users/{}/stories/highlights?limit=5&offset={}&unf=1'
 highlightsWithAStoryEP = 'https://onlyfans.com/api2/v2/users/{}/stories?unf=1'
 storyEP = 'https://onlyfans.com/api2/v2/stories/highlights/{}?unf=1'
 
 messagesEP = 'https://onlyfans.com/api2/v2/chats/{}/messages?limit=100&offset=0&order=desc&skip_users=all&skip_users_dups=1'
 messagesNextEP = 'https://onlyfans.com/api2/v2/chats/{}/messages?limit=100&offset=0&id={}&order=desc&skip_users=all&skip_users_dups=1'
 
 favoriteEP = 'https://onlyfans.com/api2/v2/posts/{}/favorites/{}'
 postURL = 'https://onlyfans.com/{}/{}'
 
-DYNAMIC = 'https://raw.githubusercontent.com/deviint/onlyfans-dynamic-rules/main/dynamicRules.json'
+DIGITALCRIMINALS = 'https://raw.githubusercontent.com/DIGITALCRIMINALS/dynamic-rules/main/onlyfans.json'
 
+DEVIINT = 'https://raw.githubusercontent.com/deviint/onlyfans-dynamic-rules/main/dynamicRules.json'
 donateEP = "https://www.buymeacoffee.com/excludedBittern"
 
 purchased_contentEP = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}&user_id={}"
 purchased_contentALL = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}"
 
 messageSPECIFIC="https://onlyfans.com/my/chats/chat/{}/?firstId={}"
 highlightSPECIFIC="https://onlyfans.com/api2/v2/stories/highlights/{}"
 storiesSPECIFIC="https://onlyfans.com/api2/v2/stories/{}"
 messageSPECIFIC= "https://onlyfans.com/api2/v2/chats/{}/messages?limit=10&order=desc&skip_users=all&firstId={}"
 
+labelsEP = "https://onlyfans.com/api2/v2/users/{}/labels?limit=100&offset={}&order=desc&non-empty=1"
+labelledPostsEP = "https://onlyfans.com/api2/v2/users/{}/posts?limit=100&offset={}&order=publish_date_desc&skip_users=all&counters=0&format=infinite&label={}"
+
+
 mainPromptChoices = {
     'Download content from a user': 0,
     'Like all of a user\'s posts': 1,
     'Unlike all of a user\'s posts': 2,
     'Edit auth.json file': 3,
     'Edit config.json file': 4,
-    'Edit Profile': 5,
+    'Edit advanced config.json settings': 5,
+    'Edit Profile': 6,
 
 }
 usernameOrListChoices = {
     'Select from accounts on profile': 0,
     'Enter a username': 1,
     'Scrape all users that I\'m subscribed to': 2
 }
@@ -96,14 +102,15 @@
 SAVE_PATH_DEFAULT=str(pathlib.Path.home()/'Data/ofscraper')
 DATE_DEFAULT="MM-DD-YYYY"
 PROFILE_DEFAULT="main_profile"
 PREMIUM_DEFAULT="Premium"
 MP4DECRYPT_DEFAULT=""
 FFMPEG_DEFAULT =""
 DISCORD_DEFAULT =""
+DYNAMIC_DEFAULT="deviint"
 SUPPRESS_LOG_LEVEL=21
 RESPONSE_TYPE_DEFAULT= {
             "message":"Messages",
             "timeline":"Posts",
             "archived":"Archived",
             "paid":"Messages",
             "stories":"Stories",
@@ -114,14 +121,16 @@
 NUM_TRIES=10
 
 
 RESPONSE_EXPIRY=5000000
 CHECK_EXPIRY=86400
 DAILY_EXPIRY=86400
 HOURLY_EXPIRY=3600
+SIZE_TIMEOUT=1209600
+KEY_EXPIRY=2592000
 DISCORDWAIT=5
 OF_MIN=15
 OF_MAX=50
 LICENCE_URL="https://onlyfans.com/api2/v2/users/media/{}/drm/{}/{}?type=widevine"
 logname="ofscraper"
 PATH_STR_MAX=200
 TABLE_STR_MAX=100
```

### Comparing `ofscraper-2.6.4/ofscraper/db/operations.py` & `ofscraper-2.7/ofscraper/db/operations.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,20 +7,22 @@
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import contextlib
 import pathlib
 import sqlite3
+import aiosqlite
 import traceback
 import math
 import logging
 from rich.console import Console
 from ..db import queries
-from ..utils.paths import createDir,databasePathHelper
+from ..utils.paths import createDir
+import ofscraper.classes.placeholder as placeholder
 
 console=Console()
 log=logging.getLogger(__package__)
 #print error 
 def operation_wrapper(func): 
     def inner(*args,**kwargs): 
         try:
@@ -30,166 +32,188 @@
             raise E    
     return inner
 
 
 
 @operation_wrapper
 def create_message_table(model_id,username):
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.messagesCreate)
             conn.commit()
 
 @operation_wrapper
 def write_messages_table(message: dict):
-    datebase_path =databasePathHelper(message.model_id,message.username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(message.model_id,message.username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             if len(cur.execute(queries.messageDupeCheck,(message.id,)).fetchall())==0:
                 insertData=(message.id,message.text,message.price,message.paid,message.archived,message.date,message.model_id)
                 cur.execute(queries.messagesInsert,insertData)
                 conn.commit()
 
 
 
             
   
 @operation_wrapper
 def write_post_table(data: dict, model_id,username):
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             if len(cur.execute(queries.postDupeCheck,(data.id,)).fetchall())==0:
                 insertData=(data.id,data.text,data.price,data.paid ,data.archived,data.date)
                 cur.execute(queries.postInsert,insertData)
                 conn.commit()
 @operation_wrapper
 def create_post_table(model_id,username):
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.postCreate)
             conn.commit()
 @operation_wrapper
 def create_stories_table(model_id,username):
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.storiesCreate)
             conn.commit()
 @operation_wrapper
 def write_stories_table(data: dict, model_id,username):
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             if len(cur.execute(queries.storiesDupeCheck,(data.id,)).fetchall())==0:
                 insertData=(data.id,data.text or data.title or "",data.price,data.paid ,data.archived,data.date)
                 cur.execute(queries.storiesInsert,insertData)
                 conn.commit()
 @operation_wrapper
 def create_media_table(model_id,username):
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.mediaCreate)
             conn.commit()
 @operation_wrapper
 def get_media_ids(model_id,username) -> list:
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.allIDCheck)
             conn.commit()
             return list(map(lambda x:x[0],cur.fetchall()))
 @operation_wrapper
 def get_post_ids(model_id,username) -> list:
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.allPOSTCheck)
             conn.commit()
             return list(map(lambda x:x[0],cur.fetchall()))
 
 @operation_wrapper
 def get_profile_info(model_id,username) -> list:
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     if not pathlib.Path(datebase_path).exists():
         return None
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
-            modelinfo=cur.execute(queries.profileDupeCheck,(model_id,)).fetchall() or [(None,)]
+            modelinfo=cur.execute(queries.prorfileDupeCheck,(model_id,)).fetchall() or [(None,)]
             conn.commit()
             return modelinfo[0][-1]
 
 
 @operation_wrapper
-def write_media_table(media,filename,model_id,username) -> list:
-    datebase_path =databasePathHelper(model_id,username)
-    with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
-        with contextlib.closing(conn.cursor()) as cur:
-            insertData=[media.id,media.postid,media.url,str(pathlib.Path(filename).parent),pathlib.Path(filename).name,
-            math.ceil(pathlib.Path(filename).stat().st_size),media.responsetype_.capitalize(),media.mediatype.capitalize() ,
-            media.preview,media.linked, 1,media.date]
-            if len(cur.execute(queries.mediaDupeCheck,(media.id,)).fetchall())==0:
-                cur.execute(queries.mediaInsert,insertData)
-            else:
-                insertData.append(media.id)
-                cur.execute(queries.mediaUpdate,insertData)
-            conn.commit()
+async def write_media_table(media,filename,model_id,username) -> list:
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
+    async with aiosqlite.connect(datebase_path) as conn:
+        insertData=[media.id,media.postid,media.url,str(pathlib.Path(filename).parent),pathlib.Path(filename).name,
+        math.ceil(pathlib.Path(filename).stat().st_size),media.responsetype_.capitalize(),media.mediatype.capitalize() ,
+        media.preview,media.linked, 1,media.date]
+        if len((await (await conn.execute(queries.mediaDupeCheck,(media.id,))).fetchall()))==0:
+            await conn.execute(queries.mediaInsert,insertData)
+        else:
+            insertData.append(media.id)
+            await conn.execute(queries.mediaUpdate,insertData)
+        await conn.commit()
 
-            
+
+   
    
 @operation_wrapper
 def create_products_table(model_id,username):
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.productCreate)
             conn.commit()
 @operation_wrapper
 def create_others_table(model_id,username):
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.otherCreate)
             conn.commit()
 @operation_wrapper
 def create_profile_table(model_id,username):
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.profilesCreate)
             conn.commit()
 
 @operation_wrapper
 def write_profile_table(model_id,username) -> list:
-    datebase_path =databasePathHelper(model_id,username)
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             insertData=[model_id,username]
             if len(cur.execute(queries.profileDupeCheck,(model_id,)).fetchall())==0:
                 cur.execute(queries.profileInsert,insertData)
             else:
                 insertData.append(model_id)
                 cur.execute(queries.profileUpdate,insertData)
             conn.commit()
 
+@operation_wrapper
+def create_labels_table(model_id, username):
+    datebase_path = placeholder.Placeholders().databasePathHelper(model_id, username)
+    createDir(datebase_path.parent)
+    with contextlib.closing(sqlite3.connect(datebase_path, check_same_thread=False)) as conn:
+        with contextlib.closing(conn.cursor()) as cur:
+            cur.execute(queries.labelsCreate)
+            conn.commit()
+
+@operation_wrapper
+def write_labels_table(label: dict, model_id, username):
+    datebase_path =placeholder.Placeholders().databasePathHelper(model_id, username)
+    createDir(datebase_path.parent)
+    with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
+        with contextlib.closing(conn.cursor()) as cur:
+            for post in label.posts:
+                if len(cur.execute(queries.labelDupeCheck,(label.label_id, post.id)).fetchall())==0:
+                    insertData=(label.label_id, label.name,label.type, post.id)
+                    cur.execute(queries.labelInsert,insertData)
+                    conn.commit()
+
 
 def create_tables(model_id,username):
     create_post_table(model_id,username)
     create_message_table(model_id,username)
     create_media_table(model_id,username)
     create_products_table(model_id,username)
     create_others_table(model_id,username)
     create_profile_table(model_id,username)
     create_stories_table(model_id,username)
+    create_labels_table(model_id, username)
```

### Comparing `ofscraper-2.6.4/ofscraper/db/queries.py` & `ofscraper-2.7/ofscraper/db/queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -178,8 +178,29 @@
 
 profileUpdate=\
 f"""Update 'profiles'
 SET
 user_id=?,username=?
 WHERE user_id=(?);"""
 
+labelsCreate=\
+"""
+CREATE TABLE IF NOT EXISTS labels (
+	id INTEGER NOT NULL, 
+	name VARCHAR, 
+	type VARCHAR, 
+	post_id INTEGER, 
+	PRIMARY KEY (id, post_id)
+)
+"""
+
+labelDupeCheck=\
+"""
+SELECT * FROM labels WHERE id=? AND post_id=?
+"""
+
+labelInsert=\
+f"""INSERT INTO 'labels'(
+id, name, type, post_id)
+VALUES (?, ?,?,?);"""
+
```

### Comparing `ofscraper-2.6.4/ofscraper/interaction/like.py` & `ofscraper-2.7/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.7/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.7/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/prompts/prompts.py` & `ofscraper-2.7/ofscraper/prompts/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,16 @@
                 Choice("Profile"),
                 Choice('Timeline'),
                 Choice('Pinned'),
                 Choice('Archived'),
                 Choice('Highlights'),
                 Choice('Stories'),
                 Choice('Messages'),
-                Choice("Purchased")
+                Choice("Purchased"),
+                Choice("Labels")
             ]
             ,"instruction":prompt_strings.CHECKLISTINSTRUCTIONS,
 
         }
     ]
     answers = prompt(questions)
     return answers[name]
@@ -336,14 +337,68 @@
         }
     ]
     answer = prompt(questions)
     profile = answer[name]
     return profile
 
 
+def config_prompt_advanced(config_) -> dict:
+    questions = [
+        {
+            'type': 'list',
+            'name': 'dynamic-mode-default',
+            'message': 'What would you like to use for dynamic rules',
+            'default': config.get_dynamic(config_),
+            'choices':["deviint","digitalcriminals"],
+        },
+        {
+            'type': 'list',
+            'name': 'key-mode-default',
+            'message': 'Make selection for how to retrive keys',
+            'default': config.get_key_mode(config_),
+            'choices':["auto","manual"],
+
+        },
+
+        {
+            'type': 'filepath',
+            'name': 'client-id',
+            'message': 'Enter path to client id file',
+            'default': config.get_client_id(config_) or "",
+            "validate":prompt_validators.MultiValidator(EmptyInputValidator(),PathValidator(is_file=True)),
+        },
+         {
+            'type': 'filepath',
+            'name': 'private-key',
+            'message': 'Enter path to private-key',
+            'default': config.get_private_key(config_)  or "",
+            "validate":prompt_validators.MultiValidator(EmptyInputValidator(),PathValidator(is_file=True)),
+        },
+        {
+            'type': 'list',
+            'name': 'partfileclean',
+            'message': 'auto clean .part files',
+            "long_instruction":"You won't be able to resume downloads if you select 'Yes'",
+            'default': config.get_part_file_clean(config_),
+            'choices':[Choice(True,"Yes"),Choice(False,"No")],
+        },
+            {
+            'type': 'input',
+            'name': 'custom',
+            'message': 'edit custom value:\n',
+            "long_instruction":"This is a helper value for remapping placeholder values",
+            'default': config.get_custom(config_) or "",
+        },
+    ]
+
+    new_settings=prompt(questions)
+    config_.update(new_settings)
+    return config_
+    
+
 def config_prompt(config_) -> dict:
 
     questions = [
         {
             'type': 'input',
             'name': 'main_profile',
             'message': 'What would you like your main profile to be?',
@@ -574,15 +629,16 @@
             'default': config.get_profile_responsetype(config_),
             'message':"profile responsetype mapping: "
         }
      ]
     answers = prompt(questions)
     console.print("Set mapping for {responsetype} placeholder\n\n")
     answers["responsetype"]=prompt(questions2)
-    return answers
+    config_.update(answers)
+    return config_
 def reset_username_prompt() -> bool:
     name = 'reset username'
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': "Do you want to reset username selection",
```

### Comparing `ofscraper-2.6.4/ofscraper/start.py` & `ofscraper-2.7/ofscraper/start.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,28 +3,25 @@
 import ofscraper.utils.args as args_
 import ofscraper.commands.scraper as scraper
 import ofscraper.commands.check as check
 import ofscraper.commands.manual as manual
 import ofscraper.utils.config as config_
 import ofscraper.utils.profiles as profiles_
 import ofscraper.utils.paths as paths_
-
+import ssl
+import platform
+import certifi
 
 
 def main():
-    log=logger.init_logger(logging.getLogger(__package__))
+    startvalues()
     args=args_.getargs()
-    #print info
-    log.debug(args)
-
     if vars(args).get("help"):
         quit()
-    log.info(f"config path: {str(paths_.get_config_path())}")
-    log.info(f"profile path: {str(paths_.get_profile_path())}")
-    log.info(f"log folder: {str(paths_.get_config_home()/'logging')}")
+  
 
     make_folders()
     if args.command=="post_check":
         check.post_checker()
     elif args.command=="msg_check":
         check.message_checker()
     elif args.command=="paid_check":
@@ -35,8 +32,22 @@
         manual.manual_download()
     else:
         scraper.main()
 
 def make_folders():
     config_.get_config_folder()
     profiles_.create_profile_path()
+
+def startvalues():
+    args=args_.getargs()
+    log=logger.init_logger(logging.getLogger(__package__))
+    logger.updateSenstiveDict(paths_.get_username(),"your_username")
+    #print info
+    log.debug(args)
+    log.debug(config_.read_config())
+    log.info(f"config path: {str(paths_.get_config_path())}")
+    log.info(f"profile path: {str(paths_.get_profile_path())}")
+    log.info(f"log folder: {str(paths_.get_config_home()/'logging')}")
+    log.debug(f"ssl {ssl.get_default_verify_paths()}")
+    log.debug(f"python version {platform. python_version()}" )
+    log.debug(f"certifi {certifi.where()}")
```

### Comparing `ofscraper-2.6.4/ofscraper/utils/args.py` & `ofscraper-2.7/ofscraper/utils/args.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     )
     general.add_argument(
         '-r', '--profile', help="Change which profile you want to use\nIf not set then the config file is used\nProfiles are always within the config file parent directory",default=None,type=lambda x:f"{re.sub('_profile','', x)}_profile"
     )
     output=parent_parser.add_argument_group("Logging",description="Arguments for output controls")  
 
     output.add_argument(
-        '-l', '--log', help = 'set log file level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG"]
+        '-l', '--log', help = 'set log file level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG","TRACE"]
     ),
     output.add_argument(
-        '-dc', '--discord', help = 'set discord log level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG"]
+        '-dc', '--discord', help = 'set discord log level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG","TRACE"]
     )
 
     output.add_argument(
-        '-p', '--output', help = 'set console output log level', type=str.upper,default="NORMAL",choices=["PROMPT","STATS","LOW","NORMAL","DEBUG"]
+        '-p', '--output', help = 'set console output log level', type=str.upper,default="NORMAL",choices=["PROMPT","STATS","LOW","NORMAL","DEBUG","TRACE"]
     )
   
 
 
     parser = argparse.ArgumentParser(add_help=False,parents=[parent_parser],prog="OF-Scraper")  
     parser.add_argument( '-h', '--help', action='help')
     scraper=parser.add_argument_group("scraper",description="General Arguments for scraper")                                
@@ -68,14 +68,18 @@
     post.add_argument(
         '-sp', '--scrape-paid', help = 'scrape the entire paid page for content. This can take a very long time',default=False,required=False,action="store_true"
     )
 
     post.add_argument(
         '-dt', '--download-type', help = 'Filter to what type of download you want None==Both, protected=Files that need mp4decrpyt',default=None,required=False,type=str.lower,choices=["protected","normal"]
     )
+
+    post.add_argument(
+        '-lb', '--label', help = 'Filter by label',default=None,required=False,type=label_helper,action="extend"
+    )
    
 
      #Filters for accounts
     filters=parser.add_argument_group("filters",description="Filters out usernames based on selected parameters")
     
     filters.add_argument(
         '-at', '--account-type', help = 'Filter Free or paid accounts\npaid and free correspond to your original price, and not the renewal price',default=None,required=False,type = str.lower,choices=["paid","free"]
@@ -91,26 +95,37 @@
  
     filters.add_argument(
         '-af', '--after', help = 'Process post at or after the given date Month/Day/Year\nnWorks for like,unlike, and downloading posts',type=arrow_helper)
     
     
     sort=parser.add_argument_group("sort",description="Options on how to sort list")
     sort.add_argument(
-        '-st', '--sort', help = 'What to sort the model list by',default="Name",choices=["Name","Subscribed","Expiring","Price"],type=str.lower)
+        '-st', '--sort', help = 'What to sort the model list by',default="Name",choices=["name","subscribed","expiring","price"],type=str.lower)
     sort.add_argument(
         '-ds', '--desc', help = 'Sort the model list in descending order',action="store_true",default=False) 
     
     advanced=parser.add_argument_group("Advanced",description="Advanced Args")  
     advanced.add_argument(
         '-uf', '--users-first', help = 'Scrape all users first rather then one at a time. This only effects downloading posts',default=False,required=False,action="store_true"
     )
     advanced.add_argument(
         '-nc', '--no-cache', help = 'disable cache',default=False,required=False,action="store_true"
     )
+    advanced.add_argument(
+        '-k', '--key-mode', help = 'key mode override',default=None,required=False,choices=["auto","manual"],type=str.lower)
+    advanced.add_argument(
+        '-dr', '--dynamic-rules', help = 'Dynamic signing',default=None,required=False,choices=["dc","deviint"],type=str.lower)
+    advanced.add_argument(
+        '-pc', '--part-cleanup', help = 'Cleanup temp .part files\nNote this removes the ability to resume from downloads',default=False,action="store_true")
 
+    
+    
+    
+    
+    
     subparser=parser.add_subparsers(help="commands",dest="command")
     post_check=subparser.add_parser("post_check",help="Display a generated table of data with information about models post(s)\nCache lasts for 24 hours",parents=[parent_parser])
 
 
     post_check.add_argument("-u","--url",
     help = 'Scan posts via url',default=None,required=False,type = check_strhelper,action='extend'
     )
@@ -185,14 +200,16 @@
         input=sys.argv[1:]
     parser=create_parser(input)
     args=parser.parse_args(input)
     #deduplicate posts
     args.posts=list(set(args.posts or []))
     args.username=set(args.username or [])
     args.excluded_username=set( args.excluded_username or [])
+    args.label=set(args.label) if args.label else args.label
+
 
     if args.command in set(["post_check","msg_check"])and not (args.url or args.file):
         raise argparse.ArgumentTypeError("error: argument missing --url or --file must be specified )")
     if args.command in set(["story_check","paid_check"])and not (args.username or args.file):
         raise argparse.ArgumentTypeError("error: argument missing --username or --file must be specified )")
     return args
 
@@ -211,34 +228,41 @@
     if isinstance(x,str) and pathlib.Path(x).exists():
         with open(x,"r") as _:
            return _.readlines()
 
    
     
 def posttype_helper(x):
-    choices=set(["Highlights","All","Archived","Messages","Timeline","Pinned","Stories","Purchased","Profile","Skip"])
+    choices=set(["Highlights","All","Archived","Messages","Timeline","Pinned","Stories","Purchased","Profile","Labels","Skip"])
     if isinstance(x,str):
         x=x.split(',')
         x=list(map(lambda x:x.capitalize() ,x))
     if len(list(filter(lambda y: y not in choices,x)))>0:
-        raise argparse.ArgumentTypeError("error: argument -o/--posts: invalid choice: (choose from 'highlights', 'all', 'archived', 'messages', 'timeline', 'pinned', 'stories', 'purchased','profile')")
+        raise argparse.ArgumentTypeError("error: argument -o/--posts: invalid choice: (choose from 'highlights', 'all', 'archived', 'messages', 'timeline', 'pinned', 'stories', 'purchased','profile','labels')")
     return x
 
 def changeargs(newargs):
     global args
     args=newargs
 
 
 def username_helper(x):
     temp=None
     if isinstance(x,list):
         temp=x
     elif isinstance(x,str):
         temp=x.split(",")
     return temp
+def label_helper(x):
+    temp=None
+    if isinstance(x,list):
+        temp=x
+    elif isinstance(x,str):
+        temp=x.split(",")
+    return list(map(lambda x:x.lower(),temp))
 
 def arrow_helper(x):
     print(x)
     try:
         return arrow.get(x)
     except arrow.parser.ParserError as E:
         try:
```

### Comparing `ofscraper-2.6.4/ofscraper/utils/auth.py` & `ofscraper-2.7/ofscraper/utils/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from urllib.parse import urlparse
 import requests
 from rich.console import Console
 import httpx
 import browser_cookie3
 from .profiles import get_active_profile
 from ..prompts.prompts import *
-from ..constants import configPath, DYNAMIC, requestAuth
+from ..constants import configPath, DIGITALCRIMINALS, requestAuth,DEVIINT
 import ofscraper.utils.paths as paths
 
 
 console=Console()
 log=logging.getLogger(__package__)
 
 def read_auth():
@@ -258,19 +258,41 @@
         if not p.is_dir():
             p.mkdir(parents=True, exist_ok=True)
 
         with open(p / requestAuth, 'w') as f:
             f.write(json.dumps(request_auth, indent=4))
 
 
+
+
+
 def get_request_auth():
+    if (args_.getargs().dynamic_rules or config.get_dynamic(config.read_config()) or "deviint")=="deviint":
+        return get_request_auth_deviint()
+    else:
+        return get_request_digitalcriminals()
+
+def get_request_auth_deviint():
     with httpx.Client(http2=True) as c:
-        r = c.get(DYNAMIC)
+        r = c.get(DEVIINT)
     if not r.is_error:
         content = r.json()
         static_param = content['static_param']
         fmt = f"{content['start']}:{{}}:{{:x}}:{content['end']}" 
         checksum_indexes = content['checksum_indexes']
         checksum_constant = content['checksum_constant']
         return (static_param, fmt, checksum_indexes, checksum_constant)
     else:
         return []
+    
+def get_request_digitalcriminals():
+    with httpx.Client(http2=True) as c:
+        r = c.get(DIGITALCRIMINALS)
+    if not r.is_error:
+        content = r.json()
+        static_param = content['static_param']
+        fmt = content['format']
+        checksum_indexes = content['checksum_indexes']
+        checksum_constant = content['checksum_constant']
+        return (static_param, fmt, checksum_indexes, checksum_constant)
+    else:
+        return []
```

### Comparing `ofscraper-2.6.4/ofscraper/utils/binaries.py` & `ofscraper-2.7/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/utils/config.py` & `ofscraper-2.7/ofscraper/utils/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,20 +75,24 @@
             'file_format':get_fileformat(config),
             'textlength':get_textlength(config),
             'space-replacer':get_spacereplacer(config),
             'date': get_date(config),
             "metadata": get_metadata(config),
             "filter":get_filter(config),
             "threads":get_threads(config),
-                "code-execution":get_allow_code_execution(config),
-
+            "code-execution":get_allow_code_execution(config),
+            "custom":get_custom(config),
             "mp4decrypt":get_mp4decrypt(config),
             "ffmpeg":get_ffmpeg(config),
              "discord":get_discord(config),
-
+             "private-key":get_private_key(config),
+             "client-id":get_client_id(config),
+            "key-mode-default":get_key_mode(config),
+            "dynamic-mode-default":get_dynamic(config),
+            "partfileclean":get_part_file_clean(config),
             "responsetype":{
            "timeline":get_timeline_responsetype(config),
          "message":get_messages_responsetype(config),
             "archived":get_archived_responsetype(config),
             "paid":get_paid_responsetype(config),
             "stories":get_stories_responsetype(config),
             "highlights":get_highlights_responsetype(config),
@@ -160,14 +164,47 @@
                     with open(p, 'r') as f:
                         configText=f.read()
                         config = json.loads(configText)
                     break
                 except:
                     continue
 
+def edit_config_advanced():
+    try:
+        p = paths_.get_config_path()
+        log.info(f"config path: {p}")
+        with open(p, 'r') as f:
+            configText=f.read()
+            config = json.loads(configText)
+
+        updated_config = {
+            'config': prompts.config_prompt_advanced(config['config'])
+        }
+
+        with open(p, 'w') as f:
+            f.write(json.dumps(updated_config, indent=4))
+
+        console.print('`config.json` has been successfully edited.')
+    except FileNotFoundError:
+        make_config(p)
+    except json.JSONDecodeError as e:
+            while True:
+                try:
+                    print("You config.json has a syntax error")
+                    print(f"{e}\n\n")
+                    with open(p,"w") as f:
+                        f.write(prompts.manual_config_prompt(configText))
+                    with open(p, 'r') as f:
+                        configText=f.read()
+                        config = json.loads(configText)
+                    break
+                except:
+                    continue
+
+
 def update_mp4decrypt():
     config={"config":read_config()}
     if prompts.auto_download_mp4_decrypt()=="Yes":
         config["config"]["mp4decrypt"]=binaries.mp4decrypt_download()
     else:
         config["config"]["mp4decrypt"]=prompts.mp4_prompt(config["config"])
     p = paths_.get_config_path() 
@@ -302,8 +339,38 @@
 def get_pinned_responsetype(config=None):
     if config==None:
         return constants.RESPONSE_TYPE_DEFAULT["pinned"]       
     return config.get('responsetype',{}).get("pinned") or constants.RESPONSE_TYPE_DEFAULT["pinned"]
 def get_spacereplacer(config=None):
     if config==None:
         return " "      
-    return config.get('space-replacer'," ") or " "
+    return config.get('space-replacer'," ") or " "
+
+def get_custom(config=None):
+    if config==None:
+        return None 
+    return config.get('custom')
+def get_private_key(config=None):
+    if config==None:
+        return None 
+    return config.get('private-key')
+
+def get_client_id(config=None):
+    if config==None:
+        return None 
+    return config.get('client-id')
+
+def get_key_mode(config=None):
+    if config==None:
+        return "auto" 
+    value=config.get("key-mode-default")
+    return value.lower() if value and value.lower() in set(["auto","manual"]) else "auto"
+
+def get_dynamic(config=None):
+    if config==None:
+        return constants.DYNAMIC_DEFAULT
+    value=config.get("dynamic-mode-default")
+    return value.lower() if value and value.lower() in set(["deviint","dc"]) else "deviint"
+def get_part_file_clean(config=None):
+    if config==None:
+        return False
+    return config.get("partfileclean",False) or False
```

### Comparing `ofscraper-2.6.4/ofscraper/utils/dates.py` & `ofscraper-2.7/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/utils/download.py` & `ofscraper-2.7/ofscraper/utils/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,17 @@
         _____                                               
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
-
 import asyncio
 import math
 import pathlib
-from random import randint
 import platform
 import shutil
 import ssl
 import certifi
 import traceback
 import re
 import logging
@@ -34,40 +32,45 @@
     BarColumn,
     TimeRemainingColumn
 )
 from rich.live import Live
 from rich.panel import Panel
 from rich.console import Group
 from rich.table import Column
+from pywidevine.cdm import Cdm
+from pywidevine.device import Device
+from pywidevine.pssh import PSSH
 import arrow
 from bs4 import BeautifulSoup
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
     pass
-from tenacity import retry,stop_after_attempt,wait_random,retry_if_result
+from tenacity import retry,stop_after_attempt,wait_random
 
 import ofscraper.utils.config as config_
 import ofscraper.utils.separate as seperate
 import ofscraper.db.operations as operations
 import ofscraper.utils.paths as paths
 import ofscraper.utils.auth as auth
 import ofscraper.constants as constants
 import ofscraper.utils.dates as dates
 import ofscraper.utils.logger as logger
 import ofscraper.utils.console as console
 import ofscraper.utils.stdout as stdout
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args_
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
+import ofscraper.classes.placeholder as placeholder
 from diskcache import Cache
-import ofscraper.api.me as me
 cache = Cache(paths.getcachepath())
 attempt = contextvars.ContextVar("attempt")
 log=logging.getLogger(__package__)
+log_trace=True if "TRACE" in set([args_.getargs().log,args_.getargs().output,args_.getargs().discord]) else False
+
 
 
 async def process_dicts(username, model_id, medialist):
     with stdout.lowstdout():
         overall_progress=Progress(  TextColumn("{task.description}"),
         BarColumn(),TaskProgressColumn(),TimeElapsedColumn())
         job_progress=Progress(TextColumn("{task.description}",table_column=Column(ratio=2)),BarColumn(),
@@ -79,17 +82,20 @@
         global sem
         sem = semaphoreDelayed(config_.get_threads(config_.read_config()))
      
 
         with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console):    
                 if not args_.getargs().dupe:
                     media_ids = set(operations.get_media_ids(model_id,username))
+                    log.debug(f"number of unique media ids in database for {username}: {len(media_ids)}")
                     medialist = seperate.separate_by_id(medialist, media_ids)
+                    log.debug(f"Number of new mediaids to download: {len(medialist)}")  
                     medialist=seperate.seperate_avatars(medialist)
-                    log.info(f"Skipping previously downloaded\nMedia left for download {len(medialist)}")
+                    log.debug(f"Remove avatar and return final number of new mediaids to download: {len(medialist)}")
+
                 else:
                     log.info(f"forcing all downloads media count {len(medialist)}")
                 file_size_limit = config_.get_filesize()
                   
                 aws=[]
                 photo_count = 0
                 video_count = 0
@@ -134,34 +140,30 @@
     return photo_count+video_count+audio_count,skipped
 def retry_required(value):
     return value == ('skipped', 1)
 
 async def download(c,ele,model_id,username,file_size_limit,progress):
     attempt.set(attempt.get(0) + 1)  
     try:
-            with paths.set_directory(paths.getmediadir(ele,username,model_id)):
+            with paths.set_directory(placeholder.Placeholders().getmediadir(ele,username,model_id)):
                 if ele.url:
                     return await main_download_helper(c,ele,pathlib.Path(".").absolute(),file_size_limit,username,model_id,progress)
                 elif ele.mpd:
                     return await alt_download_helper(c,ele,pathlib.Path(".").absolute(),file_size_limit,username,model_id,progress)
                 else:
                     return None
     except Exception as e:
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {e}")   
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {traceback.format_exc()}")   
         return 'skipped', 1
 async def main_download_helper(c,ele,path,file_size_limit,username,model_id,progress):
     path_to_file=None
-    async with sem:
-            log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with normal downloader")
-            total ,temp,path_to_file=await main_download_downloader(c,ele,path,file_size_limit,username,model_id,progress)
-            if int(file_size_limit)>0 and total > int(file_size_limit): 
-                return "skipped",1
 
-    
+    log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with normal downloader")
+    total ,temp,path_to_file=await main_download_downloader(c,ele,path,file_size_limit,username,model_id,progress)
 
     if not pathlib.Path(temp).exists():
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {temp} was not created") 
         return "skipped",1
     elif abs(total-pathlib.Path(temp).absolute().stat().st_size)>500:
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename_} size mixmatch target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
         return "skipped",1 
@@ -172,71 +174,100 @@
         if ele.postdate:
             newDate=dates.convert_local_time(ele.postdate)
             log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
             set_time(path_to_file,newDate )
             log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
 
         if ele.id:
-            operations.write_media_table(ele,path_to_file,model_id,username)
+            await operations.write_media_table(ele,path_to_file,model_id,username)
         set_cache_helper(ele)
         return ele.mediatype,total
-
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
 async def main_download_downloader(c,ele,path,file_size_limit,username,model_id,progress):
-    url=ele.url
-    log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {url}")
-    async with c.request("get",url,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=None) as r:
-            if r.ok:
-                rheaders=r.headers
-                total = int(rheaders['Content-Length'])
-                if file_size_limit>0 and total > int(file_size_limit): 
-                        return total ,None,None    
-                content_type = rheaders.get("content-type").split('/')[-1]
-                filename=paths.createfilename(ele,username,model_id,content_type)
-                path_to_file = paths.truncate(pathlib.Path(path,f"{filename}"))                 
-                pathstr=str(path_to_file)
-                temp=paths.truncate(f"{path_to_file}.part")
-                pathlib.Path(temp).unlink(missing_ok=True)
-                task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
-                with open(temp, 'wb') as f:                           
-                    progress.update(task1,visible=True )
-                    async for chunk in r.content.iter_chunked(1024):
-                        f.write(chunk)
-                        progress.update(task1, advance=len(chunk))
-                    progress.remove_task(task1)  
-                return total ,temp,path_to_file
-            else:
-                r.raise_for_status()  
+    try:
+        url=ele.url
+        log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {url}")
+        await sem.acquire()
+        pathlib.Path(temp).unlink(missing_ok=True) if (args_.getargs().part_cleanup or config_.get_part_file_clean(config_.read_config()) or False) else None
+        temp=paths.truncate(pathlib.Path(path,f"{ele.filename}_{ele.id}.part"))
+        resume_size=0 if not pathlib.Path(temp).exists() else pathlib.Path(temp).absolute().stat().st_size
+        cache.close()
+        headers=None
+        total=None
+        path_to_file=None
+       
+
+      
+        async with c.request("get",url,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=None,headers=None) as r:
+                if r.ok:
+                    rheaders=r.headers
+                    total = int(rheaders['Content-Length'])
+                    if file_size_limit>0 and total > int(file_size_limit): 
+                            return total ,"skipped",None 
+                       
+                    content_type = rheaders.get("content-type").split('/')[-1]
+                    filename=placeholder.Placeholders().createfilename(ele,username,model_id,content_type)
+                    path_to_file = paths.truncate(pathlib.Path(path,f"{filename}")) 
+                else:
+                    r.raise_for_status()          
+                                   
+        if total!=resume_size:
+            headers={"Range":f"bytes={resume_size}-{total}"}
+            async with c.request("get",url,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=None,headers=headers) as r:
+                if r.ok:
+                    pathstr=str(path_to_file)
+                    if not total or (resume_size!=total):
+                        task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
+                        size=0
+                        with open(temp, 'ab') as f: 
+                            progress.update(task1,visible=True )
+                            async for chunk in r.content.iter_chunked(1024):
+                                size=size+len(chunk) if log_trace else size
+                                log.trace(f"Media:{ele.id} Post:{ele.postid} Download:{size}/{total}")
+                                f.write(chunk)
+                                progress.update(task1, advance=len(chunk))
+                            progress.remove_task(task1)  
+                else:
+                    r.raise_for_status() 
+                                  
+        return total ,temp,path_to_file
+
+    except Exception as E:
+        log.traceback(traceback.format_exc())
+        log.traceback(E)
+        raise E
+    finally:
+        sem.release()
 
 
 
 
 async def alt_download_helper(c,ele,path,file_size_limit,username,model_id,progress):
-    async with sem:
-        log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with protected media downloader")      
-        log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {ele.mpd}")
-        path_to_file = paths.truncate(pathlib.Path(path,f'{paths.createfilename(ele,username,model_id,"mp4")}'))
-        temp_path=paths.truncate(pathlib.Path(path,f"temp_{ele.id or ele.filename_}_{randint(100,999)}.mp4"))
-        audio,video=await alt_download_preparer(ele)
-        audio=await alt_download_downloader(audio,c,ele,path,file_size_limit,progress)
-        if file_size_limit>0 and int(audio["total"]) > int(file_size_limit): 
-            return 'skipped', 1
-        video=await alt_download_downloader(video,c,ele,path,file_size_limit,progress)
-        if int(file_size_limit)>0 and int(video["total"]) > int(file_size_limit): 
-            return 'skipped', 1       
-          
+    log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with protected media downloader")      
+    log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {ele.mpd}")
+    path_to_file = paths.truncate(pathlib.Path(path,f'{placeholder.Placeholders().createfilename(ele,username,model_id,"mp4")}'))
+    temp_path=paths.truncate(pathlib.Path(path,f"temp_{ele.id or ele.filename_}.mp4"))
+    audio,video=await alt_download_preparer(ele)
+    audio=await alt_download_downloader(audio,c,ele,path,file_size_limit,progress)
+    video=await alt_download_downloader(video,c,ele,path,file_size_limit,progress)
+    if int(file_size_limit)>0 and int(video["total"])+int(audio["total"]) > int(file_size_limit): 
+        return 'skipped', 1       
+        
     for item in [audio,video]:
         if not pathlib.Path(item["path"]).exists():
                 log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['path']} was not created") 
                 return "skipped",1
         elif abs(item["total"]-pathlib.Path(item['path']).absolute().stat().st_size)>500:
             log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['name']} size mixmatch target: {item['total']} vs actual: {pathlib.Path(item['path']).absolute().stat().st_size}")   
             return "skipped",1 
                 
     for item in [audio,video]:
-        key=await key_helper(c,item["pssh"],ele.license,ele.id)
+
+        key=await key_helper_manual(c,item["pssh"],ele.license,ele.id)  if (args_.getargs().key_mode or config_.get_key_mode(config_.read_config()) or "auto") == "manual" \
+        else await key_helper(c,item["pssh"],ele.license,ele.id)
         if key==None:
             log.debug(f"Media:{ele.id} Post:{ele.postid} Could not get key")
             return "skipped",1 
         log.debug(f"Media:{ele.id} Post:{ele.postid} got key")
         newpath=pathlib.Path(re.sub("\.part$","",str(item["path"]),re.IGNORECASE))
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(item['path']).absolute()} -> {newpath}")   
         r=subprocess.run([config_.get_mp4decrypt(config_.read_config()),"--key",key,str(item["path"]),str(newpath)],stdout=subprocess.PIPE,stderr=subprocess.PIPE)
@@ -263,108 +294,178 @@
     shutil.move(temp_path,path_to_file)
     if ele.postdate:
         newDate=dates.convert_local_time(ele.postdate)
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
         set_time(path_to_file,newDate )
         log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
     if ele.id:
-        operations.write_media_table(ele,path_to_file,model_id,username)
+        await operations.write_media_table(ele,path_to_file,model_id,username)
     return ele.mediatype,audio["total"]+video["total"]
 
 async def alt_download_preparer(ele):
     mpd=await ele.parse_mpd
     for period in mpd.periods:
                 for adapt_set in filter(lambda x:x.mime_type=="video/mp4",period.adaptation_sets):             
                     kId=None
                     for prot in adapt_set.content_protections:
                         if prot.value==None:
                             kId = prot.pssh[0].pssh 
                             break
                     maxquality=max(map(lambda x:x.height,adapt_set.representations))
                     for repr in adapt_set.representations:
-                        name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
+                        origname=f"{repr.base_urls[0].base_url_value}"
                         if repr.height==maxquality:
-                            video={"origname":repr.base_urls[0].base_url_value,"pssh":kId,"type":"video","name":name}
+                            video={"origname":origname,"pssh":kId,"type":"video","name":f"tempvid_{origname}"}
                             break
                 for adapt_set in filter(lambda x:x.mime_type=="audio/mp4",period.adaptation_sets):             
                     kId=None
-                    name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
                     for prot in adapt_set.content_protections:
                         if prot.value==None:
                             kId = prot.pssh[0].pssh 
                             logger.updateSenstiveDict(kId,"pssh_code")
                             break
                     for repr in adapt_set.representations:
-                        name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
-                        audio={"origname":repr.base_urls[0].base_url_value,"pssh":kId,"type":"audio","name":name}
+                        origname=f"{repr.base_urls[0].base_url_value}"
+                        audio={"origname":origname,"pssh":kId,"type":"audio","name":f"tempaudio_{origname}"}
                         break
     return audio,video
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
 async def alt_download_downloader(item,c,ele,path,file_size_limit,progress):
-    base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
-    url=f"{base_url}{item['origname']}"
-    log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['origname']} with {url}")
-    params={"Policy":ele.policy,"Key-Pair-Id":ele.keypair,"Signature":ele.signature}   
-    async with c.request("get",url,params=params,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=auth.make_headers(auth.read_auth())) as r:
-        if r.ok:
-            rheaders=r.headers
-            total = int(rheaders['Content-Length'])
-            item["total"]=total
-            temp= paths.truncate(pathlib.Path(path,f"{item['name']}.part"))
-            temp.unlink(missing_ok=True)
-            item["path"]=temp
-            if file_size_limit>0 and total > int(file_size_limit): 
-                    return  item
-            pathstr=str(temp)
-            task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
-            with open(temp, 'wb') as f:                           
-                progress.update(task1,visible=True )
-                async for chunk in r.content.iter_chunked(1024):
-                    f.write(chunk)
-                    progress.update(task1, advance=len(chunk))
-                progress.remove_task(task1)
-            return item
-        else:
-            r.raise_for_status()
+    try:
+        base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
+        url=f"{base_url}{item['origname']}"
+        log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['origname']} with {url}")
+        await sem.acquire()
+        params={"Policy":ele.policy,"Key-Pair-Id":ele.keypair,"Signature":ele.signature}   
+        temp= paths.truncate(pathlib.Path(path,f"{item['name']}.part"))
+        headers=auth.make_headers(auth.read_auth())
+        pathlib.Path(temp).unlink(missing_ok=True) if (args_.getargs().part_cleanup or config_.get_part_file_clean(config_.read_config()) or False) else None
+        resume_size=0 if not pathlib.Path(temp).exists() else pathlib.Path(temp).absolute().stat().st_size
+        total=None
+        
+        async with c.request("get",url,params=params,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
+            if r.ok:
+                rheaders=r.headers
+                total = int(rheaders['Content-Length'])
+                if file_size_limit>0 and total > int(file_size_limit): 
+                        return total ,None,None 
+                r.raise_for_status()  
+        if total!=resume_size:
+            headers={"Range":f"bytes={resume_size}-{total}"}  
+            async with c.request("get",url,params=params,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as l:
+                if l.ok:
+                    pathstr=str(temp)
+                    task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
+                    progress.update(task1, advance=resume_size)
+                    with open(temp, 'ab') as f:                           
+                        progress.update(task1,visible=True )
+                        size=0
+                        async for chunk in l.content.iter_chunked(1024):
+                            size=size+len(chunk) if log_trace else size
+                            log.trace(f"Media:{ele.id} Post:{ele.postid} Download:{size}/{total}")
+                            f.write(chunk)
+                            progress.update(task1, advance=len(chunk))
+                        progress.remove_task(task1)
+                else:
+                    l.raise_for_status()
+                    return item
+        item["total"]=total
+        item["path"]=temp
+        return item
+              
+    except Exception as E:
+        log.traceback(traceback.format_exc())
+        log.traceback(E)
+        raise E
+    finally:
+        sem.release()
 
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
 async def key_helper(c,pssh,licence_url,id):
+    log.debug("using auto key helper")
+    try:
+        out=cache.get(licence_url)
+        log.debug(f"ID:{id} pssh: {pssh!=None}")
+        log.debug(f"ID:{id} licence: {licence_url}")
+        if not out:
+            headers=auth.make_headers(auth.read_auth())
+            headers["cookie"]=auth.get_cookies()
+            auth.create_sign(licence_url,headers)
+            json_data = {
+                'license': licence_url,
+                'headers': json.dumps(headers),
+                'pssh': pssh,
+                'buildInfo': '',
+                'proxy': '',
+                'cache': True,
+            }
+
+
+            async with c.request("post",'https://cdrm-project.com/wv',json=json_data,ssl=ssl.create_default_context(cafile=certifi.where()),allow_redirects=True,cookies=None) as r:
+                httpcontent=await r.text()
+                log.debug(f"ID:{id} key_response: {httpcontent}")
+                soup = BeautifulSoup(httpcontent, 'html.parser')
+                out=soup.find("li").contents[0]
+                cache.set(licence_url,out, expire=constants.KEY_EXPIRY)
+                cache.close()
+        return out
+    except Exception as E:
+        log.traceback(E)
+        log.traceback(traceback.format_exc())
+        raise E
+        
+
+async def key_helper_manual(c,pssh,licence_url,id):
+    log.debug("using manual keyhelper")
     out=cache.get(licence_url)
+    if out!=None:
+        return out
     log.debug(f"ID:{id} pssh: {pssh!=None}")
     log.debug(f"ID:{id} licence: {licence_url}")
-    if not out:
-        headers=auth.make_headers(auth.read_auth())
-        headers["cookie"]=auth.get_cookies()
-        auth.create_sign(licence_url,headers)
-        json_data = {
-            'license': licence_url,
-            'headers': json.dumps(headers),
-            'pssh': pssh,
-            'buildInfo': '',
-            'proxy': '',
-            'cache': True,
-        }
-
-
-                 
-
-        async with c.request("post",'https://cdrm-project.com/wv',json=json_data,ssl=ssl.create_default_context(cafile=certifi.where()),allow_redirects=True,cookies=None) as r:
-            httpcontent=await r.text()
-            log.debug(f"ID:{id} key_response: {httpcontent}")
-            soup = BeautifulSoup(httpcontent, 'html.parser')
-            out=soup.find("li").contents[0]
-            cache.set(licence_url,out, expire=2592000)
-            cache.close()
-    return out
-        
+
+    # prepare pssh
+    pssh = PSSH(pssh)
+
+
+    # load device
+    private_key=pathlib.Path(config_.get_private_key(config_.read_config())).read_bytes()
+    client_id=pathlib.Path(config_.get_client_id(config_.read_config())).read_bytes()
+    device = Device(security_level=3,private_key=private_key,client_id=client_id,type_="ANDROID",flags=None)
+
+
+    # load cdm
+    cdm = Cdm.from_device(device)
+
+    # open cdm session
+    session_id = cdm.open()
+
+    
+    
+    
+    # get license challenge
+    challenge = cdm.get_license_challenge(session_id, pssh)
+    headers=auth.make_headers(auth.read_auth())
+    headers=auth.create_sign(licence_url, headers)
+    keys=None
+    async with c.request("post",licence_url,data=challenge,ssl=ssl.create_default_context(cafile=certifi.where()),allow_redirects=True, headers=headers,cookies=auth.add_cookies_aio()) as r:
+        cdm.parse_license(session_id, await r.content.read())
+        keys = cdm.get_keys(session_id)
+        cdm.close(session_id)
+    keyobject=list(filter(lambda x:x.type=="CONTENT",keys))[0]
+    key="{}:{}".format(keyobject.kid.hex,keyobject.key.hex())
+    cache.set(licence_url,key, expire=constants.KEY_EXPIRY)
+    return key
+
+                
+
+    
 
 
-  
 def convert_num_bytes(num_bytes: int) -> str:
     if num_bytes == 0:
       return '0 B'
     num_digits = int(math.log10(num_bytes)) + 1
 
     if num_digits >= 10:
         return f'{round(num_bytes / 10**9, 2)} GB'
@@ -385,10 +486,9 @@
         return error_content
 
 
 def set_cache_helper(ele):
     if  ele.postid and ele.responsetype_=="profile":
         cache.set(ele.postid ,True)
         cache.close()
-    elif  ele.filename_ and ele.responsetype_=="highlights":
-        cache.set(ele.filename_,True)
-        cache.close()
+
+
```

### Comparing `ofscraper-2.6.4/ofscraper/utils/encoding.py` & `ofscraper-2.7/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/utils/exit.py` & `ofscraper-2.7/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/utils/logger.py` & `ofscraper-2.7/ofscraper/utils/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,20 +16,28 @@
 import ofscraper.constants as constants
 senstiveDict={}
 discord_queue=queue.Queue()
 
 
 class DebugOnly(logging.Filter):
     def filter(self, record):
-        if record.levelname=="DEBUG" or record.levelname=="TRACEBACK":
+
+        if record.levelno==10 or record.levelno==11:
+            return True
+        return False
+
+class TraceOnly(logging.Filter):
+    def filter(self, record):
+        if record.levelno<=11:
             return True
         return False
+
 class NoDebug(logging.Filter):
     def filter(self, record):
-        if record.levelname=="DEBUG" or record.levelname=="TRACEBACK":
+        if record.levelno<=11:
             return False
         return True
 class DiscordHandler(logging.Handler):
     def __init__(self):
         logging.Handler.__init__(self)
     def emit(self, record):
         log_entry = self.format(record)
@@ -95,17 +103,17 @@
 class SensitiveFormatter(logging.Formatter):
     """Formatter that removes sensitive information in logs."""
     @staticmethod
     def _filter(s):
         if s.find("Avatar :")!=-1:
             None
         else:
-            s=re.sub("&Policy=[^&\"]+", "&Policy={hidden}", s)
-            s=re.sub("&Signature=[^&\"]+", "&Signature={hidden}", s)
-            s=re.sub("&Key-Pair-Id=[^&\"]+", "&Key-Pair-Id={hidden}", s)
+            s=re.sub("&Policy=[^&\"\']+", "&Policy={hidden}", s)
+            s=re.sub("&Signature=[^&\"\']+", "&Signature={hidden}", s)
+            s=re.sub("&Key-Pair-Id=[^&\"\']+", "&Key-Pair-Id={hidden}", s)
             for ele in senstiveDict.items():
                 s=re.sub(re.escape(str(ele[0])),str(ele[1]),s)
         return s
 
     def format(self, record):
         original = logging.Formatter.format(self, record)  # call parent method
         return self._filter(original)
@@ -118,51 +126,74 @@
     def _filter(s):
         s=SensitiveFormatter._filter(s)
         s=re.sub("\[bold\]|\[/bold\]","",s)
         return s
     
 
 
-def logForLevel(self, message, *args, **kwargs):
-        if self.isEnabledFor(logging.DEBUG+5):
-            self._log(logging.DEBUG+5, message, args, **kwargs)
-def logToRoot(message, *args, **kwargs):
-        logging.log(logging.DEBUG+5, message, *args, **kwargs)   
-
-def addtrackback():
-
-    logging.addLevelName(logging.DEBUG+5, "TRACEBACK")
-    logging.TRACEBACK = logging.DEBUG+5
-    setattr(logging.getLoggerClass(),"traceback", logForLevel)
-    setattr(logging, "traceback",logToRoot)
+def logForLevel(level):
+    def inner(self, message, *args, **kwargs):
+        if self.isEnabledFor(level):
+            self._log(level, message, args, **kwargs)
+    return inner
+
+def  logToRoot(level):
+    def inner(message, *args, **kwargs):
+            logging.log(level, message, *args, **kwargs)  
+    return inner 
+
+def addtraceback():
+    level=logging.DEBUG+1
+
+    logging.addLevelName(level ,"TRACEBACK")
+    logging.TRACEBACK = level
+    setattr(logging, "TRACEBACK", level)
+    setattr(logging.getLoggerClass(),"traceback", logForLevel(level))
+    setattr(logging, "traceback",logToRoot(level))
+
+def addtrace():
+    level=logging.DEBUG-5
+
+    logging.addLevelName( level,"TRACE")
+    logging.TRACE = level
+    setattr(logging, "TRACE", level)
+    setattr(logging.getLoggerClass(),"trace", logForLevel(level))
+    setattr(logging, "trace",logToRoot(level))
+
+
 
 def updateSenstiveDict(word,replacement):
      global senstiveDict
      senstiveDict[word]=replacement
 
 
 def getLevel(input):
     """
     CRITICAL 50
     ERROR 40
     WARNING 30
     INFO 20
     DEBUG 10
+    TRACE 5 
     """
     return {"OFF":100,
             "PROMPT":"CRITICAL",
             "STATS":"ERROR",
             "LOW":"WARNING",
             "NORMAL":"INFO",
-            "DEBUG":"DEBUG"}.get(input,100)
+            "DEBUG":"DEBUG",
+            "TRACE":"TRACE"
+            
+            }.get(input,100)
 
 def init_logger(log):
     format=' \[%(module)s.%(funcName)s:%(lineno)d]  %(message)s'
     log.setLevel(1)
-    addtrackback()
+    addtraceback()
+    addtrace()
     # # #log file
       # #discord
     cord=DiscordHandler()
     cord.setLevel(getLevel(args.getargs().discord))
     cord.setFormatter(SensitiveFormatter('%(message)s'))
     #console
     sh=RichHandler(rich_tracebacks=True,markup=True,tracebacks_show_locals=True,show_time=False,show_level=False,console=console.shared_console)
@@ -180,26 +211,26 @@
         fh=logging.StreamHandler(stream)
         fh.setLevel(getLevel(args.getargs().log))
         fh.setFormatter(LogFileFormatter('%(asctime)s - %(message)s',"%Y-%m-%d %H:%M:%S"))
         fh.addFilter(NoDebug())
         log.addHandler(fh)
 
     
-    if args.getargs().output=="DEBUG":
+    if args.getargs().output in {"TRACE","DEBUG"}:
+        funct=DebugOnly if args.getargs().output=="DEBUG" else TraceOnly
         sh2=RichHandler(rich_tracebacks=True, console=console.shared_console,markup=True,tracebacks_show_locals=True,show_time=False)
         sh2.setLevel(args.getargs().output)
         sh2.setFormatter(SensitiveFormatter(format))
-        sh2.addFilter(DebugOnly())
+        sh2.addFilter(funct())
         log.addHandler(sh2)
-    if args.getargs().log=="DEBUG":
+    if args.getargs().log in {"TRACE","DEBUG"}:
+        funct=DebugOnly if args.getargs().output=="DEBUG" else TraceOnly
         fh2=logging.StreamHandler(stream)
         fh2.setLevel(getLevel(args.getargs().log))
         fh2.setFormatter(LogFileFormatter('%(asctime)s - %(levelname)s - %(message)s',"%Y-%m-%d %H:%M:%S"))
-        fh2.addFilter(DebugOnly())
+        fh2.addFilter(funct())
         log.addHandler(fh2)
-    
-
     return log
 
 
 def add_widget(widget):
     [setattr(ele,"widget",widget) for ele in list(filter(lambda x:isinstance(x,TextHandler),logging.getLogger("ofscraper").handlers))]
```

### Comparing `ofscraper-2.6.4/ofscraper/utils/of.py` & `ofscraper-2.7/ofscraper/utils/of.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,28 @@
 import asyncio
 import time
 import logging
 from itertools import chain
 import ofscraper.prompts.prompts as prompts
 import ofscraper.api.messages as messages
 import ofscraper.db.operations as operations
-import ofscraper.api.posts as posts_
+import ofscraper.classes.posts as posts_
+import ofscraper.classes.media as media
 import ofscraper.utils.args as args_
 import ofscraper.api.paid as paid
 import ofscraper.api.highlights as highlights
 import ofscraper.api.timeline as timeline
 import ofscraper.api.profile as profile
 import ofscraper.utils.args as args_
 import ofscraper.utils.filters as filters
 import ofscraper.utils.stdout as stdout
 import ofscraper.api.archive as archive
 import ofscraper.api.pinned as pinned
+import ofscraper.api.labels as labels_api
+import ofscraper.classes.labels as labels
 
 log=logging.getLogger(__package__)
 args=args_.getargs()
 log.debug(args)
 
 def process_messages(model_id,username):
     with stdout.lowstdout():
@@ -37,45 +40,46 @@
         messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
         log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),messages_))}")
         log.debug("Removing locked messages media")
         for message in messages_:
             operations.write_messages_table(message)
         output=[]
         [ output.extend(message.media) for message in messages_]
-        return list(filter(lambda x:isinstance(x,posts_.Media),output))
+        return list(filter(lambda x:isinstance(x,media.Media),output))
 
 def process_paid_post(model_id,username):
     with stdout.lowstdout():
         paid_content=asyncio.run(paid.get_paid_posts(username,model_id))
         paid_content=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="paid"),paid_content))
         log.debug(f"[bold]Paid Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),paid_content))}")
         log.debug("Removing locked paid media")
         for post in paid_content:
             operations.write_post_table(post,model_id,username)
         output=[]
         [output.extend(post.media) for post in paid_content]
-        return list(filter(lambda x:isinstance(x,posts_.Media),output))
+        return list(filter(lambda x:isinstance(x,media.Media),output))
 
          
 
 def process_highlights( model_id,username):
     with stdout.lowstdout():
-        highlights_, stories = asyncio.run(highlights.get_highlight_post( model_id))
-        highlights_, stories=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="highlights"),highlights_)),\
-        list(map(lambda x:posts_.Post(x,model_id,username,responsetype="stories"),stories))
-        log.debug(f"[bold]Combined Story and Highlight Media count[/bold] {sum(map(lambda x:len(x.post_media), highlights_))+sum(map(lambda x:len(x.post_media), stories))}")
+        stories = asyncio.run(highlights.get_stories_post( model_id))
+        highlights_=asyncio.run(highlights.get_highlight_post( model_id))
+        highlights_=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="highlights"),highlights_))
+        stories=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="stories"),stories))
         for post in highlights_:
             operations.write_stories_table(post,model_id,username)
         for post in stories:
             operations.write_stories_table(post,model_id,username)   
+        log.debug(f"[bold]Combined Story and Highlight Media count[/bold] {sum(map(lambda x:len(x.post_media), highlights_))+sum(map(lambda x:len(x.post_media), stories))}")
         output=[]
         output2=[]
         [ output.extend(highlight.media) for highlight in highlights_]
         [ output2.extend(stories.media) for stories in stories]
-        return list(filter(lambda x:isinstance(x,posts_.Media),output)),list(filter(lambda x:isinstance(x,posts_.Media),output2))
+        return list(filter(lambda x:isinstance(x,media.Media),output)),list(filter(lambda x:isinstance(x,media.Media),output2))
 
         
 
 
 
 
 
@@ -86,54 +90,54 @@
         timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
         log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),timeline_posts))}")
         log.debug("Removing locked timeline media")
         for post in timeline_posts:
             operations.write_post_table(post,model_id,username)
         output=[]
         [output.extend(post.media) for post in  timeline_posts ]
-        return list(filter(lambda x:isinstance(x,posts_.Media),output))
+        return list(filter(lambda x:isinstance(x,media.Media),output))
 
 def process_archived_posts( model_id,username):
     with stdout.lowstdout():
         archived_posts = asyncio.run(archive.get_archived_post(model_id))
         archived_posts =list(map(lambda x:posts_.Post(x,model_id,username),archived_posts ))
         log.debug(f"[bold]Archived Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),archived_posts))}")
         log.debug("Removing locked archived media")
 
         for post in archived_posts:
             operations.write_post_table(post,model_id,username)
         output=[]
         [ output.extend(post.media) for post in archived_posts ]
-        return list(filter(lambda x:isinstance(x,posts_.Media),output))
+        return list(filter(lambda x:isinstance(x,media.Media),output))
 
 
 
 
 def process_pinned_posts( model_id,username):
     with stdout.lowstdout():
         pinned_posts = asyncio.run(pinned.get_pinned_post( model_id))
         pinned_posts =list(map(lambda x:posts_.Post(x,model_id,username,"pinned"),pinned_posts ))
         log.debug(f"[bold]Pinned Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),pinned_posts))}")
         log.debug("Removing locked pinned media")
         for post in  pinned_posts:
             operations.write_post_table(post,model_id,username)
         output=[]
         [ output.extend(post.media) for post in pinned_posts ]
-        return list(filter(lambda x:isinstance(x,posts_.Media),output))
+        return list(filter(lambda x:isinstance(x,media.Media),output))
 
 def process_profile( username) -> list:
     with stdout.lowstdout():
         user_profile = profile.scrape_profile( username)
         urls, info = profile.parse_profile(user_profile)
         profile.print_profile_info(info)       
         output=[]
         for ele in enumerate(urls):
             count=ele[0]
             data=ele[1]
-            output.append(posts_.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
+            output.append(media.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
         avatars=list(filter(lambda x:x.filename.find('avatar')!=-1,output))
         if len(avatars)>0:
             log.warning(f"Avatar : {avatars[0].url}")
         return output
 
 def process_all_paid():
     with stdout.lowstdout():
@@ -156,14 +160,26 @@
 
                      
         log.debug(f"[bold]Paid Media for all models[/bold] {sum(map(lambda x:len(x.media),post_array))}")
         output=[]
         [output.extend(post.media) for post in post_array]
         return output
 
+def process_labels(model_id, username):
+    with stdout.lowstdout():
+        labels_ = asyncio.run(labels_api.get_labels(model_id))
+
+        labels_=labels_ if not args_.getargs().label else list(filter(lambda x:x.get("name").lower() in args_.getargs().label ,labels_))
+        labelled_posts_ = asyncio.run(labels_api.get_labelled_posts(labels_, model_id))
+        labelled_posts_= list(map(lambda x:labels.Label(x,model_id,username),labelled_posts_))
+        for labelled_post in labelled_posts_:
+            operations.write_labels_table(labelled_post, model_id, username)
+
+        output = [post.media for labelled_post in labelled_posts_ for post in labelled_post.posts]
+        return [item for sublist in output for item in sublist]
 
 def select_areas():
     if not args.scrape_paid and len( args.posts or [])==0:
           args.scrape_paid=prompts.scrape_paid_prompt()
     args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.areas_prompt())
 ))
 
@@ -176,15 +192,15 @@
     archived_posts_dicts  = []
     highlights_dicts  = []
     messages_dicts  = []
     stories_dicts=[]
     purchased_dict=[]
     pinned_post_dict=[]
     profile_dicts=[]
-
+    labels_dicts=[]
 
     username=ele['name']
     if "Skip" in args.posts:
         return []
   
     if ('Profile' in args.posts or 'All' in args.posts):
         profile_dicts  = process_profile(username)
@@ -202,13 +218,15 @@
             highlights_tuple = process_highlights( model_id,username)  
             if 'Highlights'  in args.posts:
                 highlights_dicts=highlights_tuple[0]
             if 'Stories'  in args.posts:
                 stories_dicts=highlights_tuple[1]   
             if 'All' in args.posts:
                 highlights_dicts=highlights_tuple[0]
-                stories_dicts=highlights_tuple[1]               
+                stories_dicts=highlights_tuple[1]   
+    if ("Labels" in args.posts or "All" in args.posts) and ele["active"]:
+        labels_dicts = process_labels(model_id,username)             
     return filters.filterMedia(list(chain(*[profile_dicts  , timeline_posts_dicts ,pinned_post_dict,purchased_dict,
-            archived_posts_dicts , highlights_dicts , messages_dicts,stories_dicts]))
+            archived_posts_dicts , highlights_dicts , messages_dicts,stories_dicts, labels_dicts]))
 
 )
```

### Comparing `ofscraper-2.6.4/ofscraper/utils/profiles.py` & `ofscraper-2.7/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/utils/separate.py` & `ofscraper-2.7/ofscraper/utils/separate.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,14 @@
 
 def seperate_avatar_helper(ele):
     #id for avatar comes from xxh32 of url
     if  ele.postid and ele.responsetype_=="profile":
         value=cache.get(ele.postid ,False)
         cache.close()
         return value
-    elif  ele.filename and ele.responsetype_=="highlights":
-        value=cache.get(ele.filename,False)
-        cache.close()
-        return value
     return False
 
     
   
 
 
 # def separate_database_results_by_id(results: list, media_ids: list) -> list:
```

### Comparing `ofscraper-2.6.4/ofscraper/utils/stdout.py` & `ofscraper-2.7/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/utils/table.py` & `ofscraper-2.7/ofscraper/utils/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/ofscraper/utils/userselector.py` & `ofscraper-2.7/ofscraper/utils/userselector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.4/pyproject.toml` & `ofscraper-2.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.6.4"
+version = "2.7"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.7.0,<4"
+python = ">=3.7.0,<3.12"
 httpx = {extras = ["http2"], version = "^0.23.3"}
 inquirerpy = "^0.3.4"
 setuptools = "^67.6.0"
 schedule = "^1.1.0"
 browser-cookie3 = "^0.17.1"
 requests = "^2.28.2"
 bs4 = "^0.0.1"
@@ -24,14 +24,18 @@
 diskcache = "^5.6.1"
 ffmpeg-python = "^0.2.0"
 dunamai = "^1.17.0"
 poetry-dynamic-versioning = "^0.22.0"
 textual = "^0.27.0"
 aiohttp = {extras = ["speedups"], version = "^3.8.4"}
 faust-cchardet = "^2.1.18"
+certifi = "^2023.5.7"
+aiosqlite = "^0.19.0"
+pycryptodome = "^3.18.0"
+pywidevine = "^1.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.test]
@@ -53,14 +57,18 @@
 [tool.poetry.group.docs.dependencies]
 sphinx-argparse = "^0.4.0"
 
 
 [tool.poetry.group.testing.dependencies]
 coverage = "^7.2.7"
 
+
+[tool.poetry.group.build.dependencies]
+pyinstaller = "^5.13.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.scripts]
 ofscraper = "ofscraper.start:main"
 
@@ -79,8 +87,8 @@
 ]
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs="git"
 metadata=true
 format="{base}"
-pattern = "default-unprefixed"
+pattern = "(?P<base>\\d+\\.\\d+\\.\\d+)"
```

### Comparing `ofscraper-2.6.4/PKG-INFO` & `ofscraper-2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.6.4
+Version: 2.7
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
-Requires-Python: >=3.7.0,<4
+Requires-Python: >=3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
+Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: browser-cookie3 (>=0.17.1,<0.18.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: dunamai (>=1.17.0,<2.0.0)
 Requires-Dist: faust-cchardet (>=2.1.18,<3.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: httpx[http2] (>=0.23.3,<0.24.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: mpegdash (>=0.3.1,<0.4.0)
 Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: poetry-dynamic-versioning (>=0.22.0,<0.23.0)
+Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
+Requires-Dist: pywidevine (>=1.6.0,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: textual (>=0.27.0,<0.28.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0)
```

