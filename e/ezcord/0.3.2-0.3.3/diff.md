# Comparing `tmp/ezcord-0.3.2.tar.gz` & `tmp/ezcord-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.3.2.tar", last modified: Sun Jul  2 10:05:59 2023, max compression
+gzip compressed data, was "ezcord-0.3.3.tar", last modified: Mon Jul 24 14:13:01 2023, max compression
```

## Comparing `ezcord-0.3.2.tar` & `ezcord-0.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.271898 ezcord-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 10:05:47.000000 ezcord-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-02 10:05:47.000000 ezcord-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-02 10:05:59.267897 ezcord-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-02 10:05:47.000000 ezcord-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 10:05:47.000000 ezcord-0.3.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-02 10:05:47.000000 ezcord-0.3.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/ezcord/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/ezcord/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/cogs/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/ezcord/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/embed_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/funcutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/ezcord/internal/language/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/language/de.json
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/language/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/language/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/ready_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/internal/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-02 10:05:47.000000 ezcord-0.3.2/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:05:59.267897 ezcord-0.3.2/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-02 10:05:59.000000 ezcord-0.3.2/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-02 10:05:59.000000 ezcord-0.3.2/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:05:59.000000 ezcord-0.3.2/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-02 10:05:59.000000 ezcord-0.3.2/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 10:05:59.000000 ezcord-0.3.2/ezcord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-02 10:05:47.000000 ezcord-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 10:05:47.000000 ezcord-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 10:05:59.271898 ezcord-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:13:01.503289 ezcord-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 14:12:47.000000 ezcord-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 14:12:47.000000 ezcord-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-24 14:13:01.503289 ezcord-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-24 14:12:47.000000 ezcord-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 14:12:47.000000 ezcord-0.3.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:13:01.499289 ezcord-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-24 14:12:47.000000 ezcord-0.3.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:13:01.499289 ezcord-0.3.3/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19286 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:13:01.499289 ezcord-0.3.3/ezcord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/cogs/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:13:01.503289 ezcord-0.3.3/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/internal/embed_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/internal/funcutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:13:01.503289 ezcord-0.3.3/ezcord/internal/language/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/internal/language/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/internal/language/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/internal/language/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/internal/ready_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-24 14:12:47.000000 ezcord-0.3.3/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:13:01.499289 ezcord-0.3.3/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-24 14:13:01.000000 ezcord-0.3.3/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-24 14:13:01.000000 ezcord-0.3.3/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:13:01.000000 ezcord-0.3.3/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-24 14:13:01.000000 ezcord-0.3.3/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 14:13:01.000000 ezcord-0.3.3/ezcord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-24 14:12:47.000000 ezcord-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 14:12:47.000000 ezcord-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:13:01.503289 ezcord-0.3.3/setup.cfg
```

### Comparing `ezcord-0.3.2/LICENSE` & `ezcord-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/PKG-INFO` & `ezcord-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.3.2
+Version: 0.3.3
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.3.2/README.md` & `ezcord-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/bot.py` & `ezcord-0.3.3/ezcord/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,17 +364,18 @@
             else:
                 error_msg = f"{error}"
 
             if self.error_handler:
                 error_txt = f"{t('error', f'```{error_msg}```')}"
                 try:
                     await error_emb(ctx, error_txt, title=t("error_title"))
-                except discord.HTTPException:
-                    # invalid interaction, probably took too long to respond
-                    pass
+                except discord.HTTPException as e:
+                    # ignore invalid interaction error, probably took too long to respond
+                    if e.code != 10062:
+                        self.logger.error("Could not send error message to user", exc_info=e)
 
             webhook_sent = False
             if self.error_webhook_url:
                 description = get_error_text(ctx, error)
                 webhook_sent = await self._send_error_webhook(description)
 
             self.logger.exception(
@@ -432,14 +433,15 @@
         style: HelpStyle = HelpStyle.embed_description,
         embed: discord.Embed | None = None,
         show_categories: bool = True,
         timeout: int = 500,
         ephemeral: bool = True,
         author_only: bool = True,
         guild_only: bool = True,
+        url_buttons: list[discord.Button] | None = None,
     ):
         """Add a help command that uses a select menu to group commands by cogs.
 
         If you use :class:`Cog`, you can pass in emojis to use for the select menu.
 
         Parameters
         ----------
@@ -455,23 +457,32 @@
         ephemeral:
             Whether the help command should be ephemeral. Defaults to ``True``.
         author_only:
             Whether the help command should only be visible to the author. Defaults to ``True``.
             This only works if ``ephemeral`` is ``False``.
         guild_only:
             Whether the help command should only be visible in guilds. Defaults to ``True``.
+        url_buttons:
+            A list of URL buttons to add to the help command. Defaults to ``None``.
         """
+        if url_buttons is None:
+            url_buttons = []
+        for button in url_buttons:
+            if not isinstance(button, discord.ui.Button):
+                raise TypeError(f"URL button must be of type 'Button', not {type(button)}.")
+
         self.help = {
             "style": style,
             "embed": embed,
             "show_categories": show_categories,
             "timeout": timeout,
             "ephemeral": ephemeral,
             "author_only": author_only,
             "guild_only": guild_only,
+            "url_buttons": url_buttons,
         }
         self.load_extension(f".cogs.help", package="ezcord")
 
 
 class PrefixBot(Bot, commands.Bot):
     """A subclass of :class:`discord.ext.commands.Bot` that implements the :class:`Bot` class.
```

### Comparing `ezcord-0.3.2/ezcord/cogs/help.py` & `ezcord-0.3.3/ezcord/cogs/help.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,16 @@
         if len(options) > 25 or len(embed.fields) > 25:
             log.error(
                 f"Help command category limit reached. Only 25 out of {len(options)} are shown."
             )
             options = options[:25]
             embed.fields = embed.fields[:25]
         view = CategoryView(options, self.bot, ctx.user, commands)
+        for button in self.bot.help["url_buttons"]:
+            view.add_item(button)
         await ctx.respond(view=view, embed=embed, ephemeral=self.bot.help["ephemeral"])
 
 
 def setup(bot: Bot):
     bot.add_cog(Help(bot))
 
 
@@ -168,17 +170,18 @@
             for command in commands:
                 if len(embed.description) <= 3500:
                     embed.description += f"### {command.mention}\n{command.description}\n"
                 else:
                     log.error("Help embed length limit reached. Some commands are not shown.")
                     break
 
-        await interaction.response.edit_message(
-            embed=embed, view=CategoryView(self.options, self.bot, self.member, self.commands)
-        )
+        view = CategoryView(self.options, self.bot, self.member, self.commands)
+        for button in self.bot.help["url_buttons"]:
+            view.add_item(button)
+        await interaction.response.edit_message(embed=embed, view=view)
 
 
 class CategoryView(discord.ui.View):
     def __init__(
         self,
         options: list[discord.SelectOption],
         bot: Bot,
```

### Comparing `ezcord-0.3.2/ezcord/components.py` & `ezcord-0.3.3/ezcord/components.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/emb.py` & `ezcord-0.3.3/ezcord/emb.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/enums.py` & `ezcord-0.3.3/ezcord/enums.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/internal/colors.py` & `ezcord-0.3.3/ezcord/internal/colors.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/internal/embed_templates.py` & `ezcord-0.3.3/ezcord/internal/embed_templates.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/internal/language/de.json` & `ezcord-0.3.3/ezcord/internal/language/de.json`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/internal/language/en.json` & `ezcord-0.3.3/ezcord/internal/language/en.json`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/internal/language/languages.py` & `ezcord-0.3.3/ezcord/internal/language/languages.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/internal/ready_style.py` & `ezcord-0.3.3/ezcord/internal/ready_style.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/internal/translation.py` & `ezcord-0.3.3/ezcord/internal/translation.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/logs.py` & `ezcord-0.3.3/ezcord/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,16 @@
         try:
             await webhook.send(
                 content=msg,
                 username=f"{name} Log",
             )
         except discord.HTTPException:
             log.error(
-                "Error while sending log message to webhook. Please check if the URL is correct."
+                "Error while sending log message to webhook. Please check if the URL is correct.",
+                extra={"webhook_sent": True},
             )
 
 
 def _discord_filter(record):
     """A filter that blocks logs that have already been sent to a Discord webhook."""
     if "webhook_sent" in record.__dict__:
         return not record.__dict__["webhook_sent"]
```

### Comparing `ezcord-0.3.2/ezcord/sql.py` & `ezcord-0.3.3/ezcord/sql.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,14 +69,18 @@
 
     async def close(self):
         """Close the current connection to the database."""
         if self.connection is not None:
             await self.connection.commit()
             await self.connection.close()
 
+    async def _close(self, db):
+        if not self.connection:
+            await db.close()
+
     async def one(self, sql: str, *args, **kwargs):
         """Returns one result row. If no row is found, ``None`` is returned.
 
         If the query returns only one column, the value of that column is returned.
 
         Parameters
         ----------
@@ -89,18 +93,22 @@
 
         Returns
         -------
         The result row or ``None``. A result row is either a tuple or a single value.
         """
         args = self._process_args(args)
         db = await self._connect(**kwargs)
-        async with db.execute(sql, args) as cursor:
-            result = await cursor.fetchone()
-        if not self.connection:
-            await db.close()
+        try:
+            async with db.execute(sql, args) as cursor:
+                result = await cursor.fetchone()
+        except Exception as e:
+            await self._close(db)
+            raise e
+
+        await self._close(db)
 
         if result is None:
             return None
         if len(result) == 1:
             return result[0]
 
         return result
@@ -121,18 +129,22 @@
 
         Returns
         -------
         A list of result rows. A result row is either a tuple or a single value.
         """
         args = self._process_args(args)
         db = await self._connect(**kwargs)
-        async with db.execute(sql, args) as cursor:
-            result = await cursor.fetchall()
-        if not self.connection:
-            await db.close()
+        try:
+            async with db.execute(sql, args) as cursor:
+                result = await cursor.fetchall()
+        except Exception as e:
+            await self._close(db)
+            raise e
+
+        await self._close(db)
         if len(result) == 0 or len(result[0]) == 1:
             return [row[0] for row in result]
 
         return result
 
     async def exec(self, sql: str, *args, end: bool = False, **kwargs) -> None:
         """Executes a SQL query.
@@ -147,11 +159,17 @@
         *args:
             Arguments for the query.
         **kwargs:
             Keyword arguments for the connection.
         """
         args = self._process_args(args)
         db = await self._connect(**kwargs)
-        await db.execute(sql, args)
+        try:
+            await db.execute(sql, args)
+        except Exception as e:
+            if end or not self.connection:
+                await db.commit()
+                await db.close()
+            raise e
         if end or not self.connection:
             await db.commit()
             await db.close()
```

### Comparing `ezcord-0.3.2/ezcord/times.py` & `ezcord-0.3.3/ezcord/times.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/ezcord/utils.py` & `ezcord-0.3.3/ezcord/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,7 +43,26 @@
         Keyword arguments for :class:`discord.File`.
 
     Returns
     -------
     :class:`discord.File`
     """
     return discord.File(io.BytesIO(text.encode()), filename=filename, **kwargs)
+
+
+def create_html_file(html: str, filename: str = "data.html", **kwargs) -> discord.File:
+    """Create a :class:`discord.File` object from an HTML string.
+
+    Parameters
+    ----------
+    html:
+        The HTML string to convert to an HTML file.
+    filename:
+        The filename to use for the HTML file.
+    **kwargs:
+        Keyword arguments for :class:`discord.File`.
+
+    Returns
+    -------
+    :class:`discord.File`
+    """
+    return create_text_file(html, filename, **kwargs)
```

### Comparing `ezcord-0.3.2/ezcord.egg-info/PKG-INFO` & `ezcord-0.3.3/ezcord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.3.2
+Version: 0.3.3
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.3.2/ezcord.egg-info/SOURCES.txt` & `ezcord-0.3.3/ezcord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.2/pyproject.toml` & `ezcord-0.3.3/pyproject.toml`

 * *Files identical despite different names*

