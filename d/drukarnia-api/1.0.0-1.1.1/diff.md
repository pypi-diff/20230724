# Comparing `tmp/drukarnia-api-1.0.0.tar.gz` & `tmp/drukarnia-api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drukarnia-api-1.0.0.tar", last modified: Sat Jun 24 15:57:15 2023, max compression
+gzip compressed data, was "drukarnia-api-1.1.1.tar", last modified: Mon Jul 24 13:13:17 2023, max compression
```

## Comparing `drukarnia-api-1.0.0.tar` & `drukarnia-api-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/drukarnia_api/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/article.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/author.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/drukarnia_api/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/shortcuts/class_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/drukarnia_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-24 15:57:15.000000 drukarnia-api-1.0.0/drukarnia_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-24 15:57:15.000000 drukarnia-api-1.0.0/drukarnia_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:57:15.000000 drukarnia-api-1.0.0/drukarnia_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-24 15:57:15.000000 drukarnia-api-1.0.0/drukarnia_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 15:57:15.000000 drukarnia-api-1.0.0/drukarnia_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.520018 drukarnia-api-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-24 13:13:17.520018 drukarnia-api-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.512018 drukarnia-api-1.1.1/drukarnia_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.516018 drukarnia-api-1.1.1/drukarnia_api/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.520018 drukarnia-api-1.1.1/drukarnia_api/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/article.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18934 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.520018 drukarnia-api-1.1.1/drukarnia_api/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/shortcuts/class_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.512018 drukarnia-api-1.1.1/drukarnia_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-24 13:13:17.000000 drukarnia-api-1.1.1/drukarnia_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-24 13:13:17.000000 drukarnia-api-1.1.1/drukarnia_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:13:17.000000 drukarnia-api-1.1.1/drukarnia_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 13:13:17.000000 drukarnia-api-1.1.1/drukarnia_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 13:13:17.000000 drukarnia-api-1.1.1/drukarnia_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:13:17.520018 drukarnia-api-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/setup.py
```

### Comparing `drukarnia-api-1.0.0/LICENSE` & `drukarnia-api-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drukarnia-api-1.0.0/PKG-INFO` & `drukarnia-api-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 1.0.0
+Version: 1.1.1
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -19,50 +19,52 @@
 
 # drukarnia-api
 
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/main/LICENSE)
 
 ## Overview
-`drukarnia-api` is a Python library designed as a wrapper for the ***Drukarnia API***, providing various functionalities for interacting with the Drukarnia platform. It simplifies the process of accessing and manipulating data from the Drukarnia API, enabling users to seamlessly integrate Drukarnia's features into their applications. The library is actively being developed and already includes almost all of the necessary features. We are working diligently to implement the remaining features as quickly as possible.
+`drukarnia-api` is a Python library designed as a wrapper for the <a href="https://drukarnia.com.ua">***Drukarnia API***</a>, providing various functionalities for interacting with the platform. It simplifies the process of accessing and manipulating data from the web, enabling users to seamlessly work with Drukarnia. The library is actively being developed and already includes almost all of the necessary features. We are working diligently to implement the remaining features as quickly as possible.
 
 
 ## Simple Usage
 ```python
 from drukarnia_api import Search
 
 
 async def get_author_article_titles():
-    async with Search() as search_engine:
-        authors = await search_engine.find_author('cupomanka') 
-        # Get the first search result
-        author = authors[0]
+    search = Search()
+    
+    async with search:
+        cupomanka, *_ = await search.find_author('cupomanka') 
 
         # Collect all data about the user
-        await author.collect_data()
+        await cupomanka.collect_data()
 
         # Get user articles
-        articles = await author.articles
+        articles = await cupomanka.articles
 
         # Print all titles
         for article in articles:
-            print(article.title)
+            print(await article.title)
 
 
 if __name__ == '__main__':
     import asyncio
 
     loop = asyncio.get_event_loop()
     loop.run_until_complete(get_author_article_titles())
 ```
 
+###### Advance Examples: <a href="https://github.com/androu-sys/drukarnia-api/blob/main/usage.ipynb">usage.ipynb</a>
+
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
 pip install drukarnia-api
 ```
 
 ## Contributing
 
-Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository: https://github.com/androu-sys/drukarnia-api.
+Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please <a href="https://github.com/androu-sys/drukarnia-api/issues/new">open an issue</a> or <a href="https://t.me/U1F615">contact me</a>.
```

### Comparing `drukarnia-api-1.0.0/README.md` & `drukarnia-api-1.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 # drukarnia-api
 
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/main/LICENSE)
 
 ## Overview
-`drukarnia-api` is a Python library designed as a wrapper for the ***Drukarnia API***, providing various functionalities for interacting with the Drukarnia platform. It simplifies the process of accessing and manipulating data from the Drukarnia API, enabling users to seamlessly integrate Drukarnia's features into their applications. The library is actively being developed and already includes almost all of the necessary features. We are working diligently to implement the remaining features as quickly as possible.
+`drukarnia-api` is a Python library designed as a wrapper for the <a href="https://drukarnia.com.ua">***Drukarnia API***</a>, providing various functionalities for interacting with the platform. It simplifies the process of accessing and manipulating data from the web, enabling users to seamlessly work with Drukarnia. The library is actively being developed and already includes almost all of the necessary features. We are working diligently to implement the remaining features as quickly as possible.
 
 
 ## Simple Usage
 ```python
 from drukarnia_api import Search
 
 
 async def get_author_article_titles():
-    async with Search() as search_engine:
-        authors = await search_engine.find_author('cupomanka') 
-        # Get the first search result
-        author = authors[0]
+    search = Search()
+    
+    async with search:
+        cupomanka, *_ = await search.find_author('cupomanka') 
 
         # Collect all data about the user
-        await author.collect_data()
+        await cupomanka.collect_data()
 
         # Get user articles
-        articles = await author.articles
+        articles = await cupomanka.articles
 
         # Print all titles
         for article in articles:
-            print(article.title)
+            print(await article.title)
 
 
 if __name__ == '__main__':
     import asyncio
 
     loop = asyncio.get_event_loop()
     loop.run_until_complete(get_author_article_titles())
 ```
 
+###### Advance Examples: <a href="https://github.com/androu-sys/drukarnia-api/blob/main/usage.ipynb">usage.ipynb</a>
+
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
 pip install drukarnia-api
 ```
 
 ## Contributing
 
-Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository: https://github.com/androu-sys/drukarnia-api.
+Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please <a href="https://github.com/androu-sys/drukarnia-api/issues/new">open an issue</a> or <a href="https://t.me/U1F615">contact me</a>.
```

### Comparing `drukarnia-api-1.0.0/drukarnia_api/article.py` & `drukarnia-api-1.1.1/drukarnia_api/objects/comment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,282 +1,224 @@
-from datetime import datetime
-from warnings import warn
 from aiohttp import ClientSession
 
-from drukarnia_api.drukarnia_base import DrukarniaElement
-from drukarnia_api.shortcuts import data2authors, data2articles, data2tags, data2comments
+from drukarnia_api.objects.base_object import DrukarniaElement
+from drukarnia_api.shortcuts import data2authors, data2comments
 
-from typing import TYPE_CHECKING, Tuple, Dict, List
+from datetime import datetime
+from typing import TYPE_CHECKING, Tuple, Dict
 
 if TYPE_CHECKING:  # always False, used for type hints
-    from drukarnia_api.author import Author
-    from drukarnia_api.tag import Tag
-    from drukarnia_api.comment import Comment
-
-
-class Article(DrukarniaElement):
-    def __init__(self, slug: str = None, article_id: str = None, *args, **kwargs):
-        """
-        Initializes an Article object with the given slug and article ID.
-        """
-        super().__init__(*args, **kwargs)
+    from drukarnia_api.objects.author import Author
 
-        self._update_data({'slug': slug, '_id': article_id})
 
-    @DrukarniaElement._control_attr('article_id')
-    @DrukarniaElement._is_authenticated
-    async def post_comment(self, comment_text: str) -> str:
-        """
-        Posts a comment on the article and returns the ID of the posted comment.
+class Comment(DrukarniaElement):
+    async def reply(self, comment_text: str) -> str:
         """
+        Posts a reply to a comment and returns the ID of the new comment.
 
-        posted_comment_id = await self.request('post', '/api/articles/{_id}/comments'.format(_id=self.article_id),
-                                               data={'comment': comment_text}, output='read')
-        return str(posted_comment_id)
+        Parameters:
+            comment_text (str): The text of the comment to be posted as a reply.
 
-    @DrukarniaElement._control_attr('article_id')
-    @DrukarniaElement._is_authenticated
-    async def like_article(self, n_likes: int) -> None:
-        """
-        Likes the article with the specified number of likes.
+        Returns:
+            str: The ID of the new comment.
         """
 
-        if not (0 <= n_likes <= 10):
-            raise ValueError('Number of likes must be greater or equal to zero and lower or equal to ten')
+        new_comment_id = await self.request(
+            'post',
+            f'/api/articles/{await self.article_id}/comments/{await self.comment_id}/replies',
+            data={
+                "comment": comment_text,
+                "replyToComment": await self.comment_id,
+                "rootComment": await self.comment_id,   # not sure
+                "rootCommentOwner": await self.owner_id,
+                "replyToUser": await self.owner_id,
+            },
+            output='read'
+        )
 
-        await self.request('post', f'/api/articles/{self.article_id}/like', data={'likes': n_likes})
+        return new_comment_id.decode('utf-8')
 
-    @DrukarniaElement._control_attr('article_id')
-    @DrukarniaElement._is_authenticated
-    async def bookmark(self, section_id: str = '', unbookmark: bool = False) -> None:
+    async def delete(self) -> None:
         """
-        Adds or removes the article from bookmarks based on the 'unbookmark' parameter.
+        Deletes a comment from the article.
         """
 
-        if unbookmark:
-            await self.request('delete', f'/api/articles/{self.article_id}/bookmarks')
+        await self.request(
+            'delete',
+            f'/api/articles/{await self.article_id}/comments/{await self.comment_id}')
 
-        elif not section_id:
-            raise ValueError('section_id must be passed for bookmarking')
-
-        else:
-            await self.request('post', '/api/articles/bookmarks',
-                               data={"article": self.article_id, "list": section_id})
-
-    @DrukarniaElement._control_attr('slug')
-    async def collect_data(self, return_: bool = False) -> Dict or None:
+    @DrukarniaElement.requires_attributes(['article_id', 'comment_id'])
+    async def get_replies(self,
+                          create_comments: bool = True) -> Tuple['Comment'] or Tuple[Dict]:
         """
-        Collects the article's data and updates the object's attributes.
-        If 'return_' is True, returns the collected data.
+        Deletes a comment from the article.
         """
 
-        data = await self.request('get', f'/api/articles/{self.slug}', output='json')
+        replies = await self.request(
+            'get',
+            f'/api/articles/{await self.article_id}/comments/{await self.comment_id}/replies',
+            output='json'
+        )
 
-        self._update_data(data)
+        if create_comments:
+            replies = await data2comments(replies, session=self.session)
 
-        if return_:
-            return data
+        return replies
 
-    @property
-    async def owner(self) -> 'Author' or None:
+    @DrukarniaElement.requires_attributes(['article_id'])
+    async def like_comment(self, unlike: bool = False) -> None:
         """
-        Retrieves the owner of the article.
+        Likes or unlikes a comment based on the 'delete' parameter.
+
+        Parameters:
+            unlike (bool, optional): If True, the comment will be unliked.
+            If False, the comment will be liked. Default is False.
         """
-        owner = self._access_data('owner', None)
-        if owner is None:
-            return None
 
-        return await data2authors([owner], self.session)
+        if unlike:
+            await self.request(
+                'delete',
+                f'/api/articles/{await self.article_id}/comments/{await self.comment_id}/likes')
 
-    @property
-    async def comments(self) -> Tuple['Comment']:
-        """
-        Retrieves the comments of the article.
-        """
-        return await data2comments(self._access_data('comments', []), self.session)
+        else:
+            await self.request(
+                'post',
+                f'/api/articles/{await self.article_id}/comments/{await self.comment_id}/likes')
 
     @property
-    async def recommended_articles(self) -> Tuple['Article']:
-        """
-        Retrieves the recommended articles related to the article.
+    @DrukarniaElement.type_decorator(datetime)
+    async def created_at(self) -> datetime:
         """
-        return await data2articles(self._access_data('recommendedArticles', []), self.session)
+        Property to access the creation date of the comment.
 
-    @property
-    def relationships(self) -> Dict:
-        """
-        Retrieves the relationships of the article.
+        Returns:
+            datetime: The creation date of the comment.
         """
-        return self._get_basetype_from_data('relationships', dict)
 
-    @property
-    def is_bookmarked(self) -> bool:
-        """
-        Checks if the article is bookmarked.
-        """
-        return self._get_basetype_from_data('isBookmarked', bool)
+        return self._access_data('createdAt')
 
     @property
-    def is_liked(self) -> bool:
-        """
-        Checks if the article is liked.
+    @DrukarniaElement.type_decorator(bool)
+    async def hidden(self) -> bool:
         """
-        return self._get_basetype_from_data('isLiked', bool)
+        Property to check if the comment is hidden by the author.
 
-    @property
-    def sensitive(self) -> bool:
-        """
-        Checks if the article is sensitive.
+        Returns:
+            bool: True if the comment is hidden, False otherwise.
         """
-        return self._get_basetype_from_data('sensitive', bool)
+        return self._access_data('hiddenByAuthor')
 
     @property
-    def content(self) -> Dict:
+    @DrukarniaElement.type_decorator(bool)
+    async def is_blocked(self) -> bool:
         """
-        Retrieves the content of the article.
-        """
-        return self._get_basetype_from_data('content', dict)
+        Property to check if the comment is blocked.
 
-    @property
-    async def author_articles(self) -> Tuple['Article']:
+        Returns:
+            bool: True if the comment is blocked, False otherwise.
         """
-        Retrieves the articles written by the author of the article.
-        """
-        return await data2articles(self._access_data('authorArticles', []), self.session)
+        return self._access_data('isBlocked')
 
     @property
-    def thumb_picture(self) -> str:
-        """
-        Retrieves the thumbnail picture of the article.
+    @DrukarniaElement.type_decorator(bool)
+    async def is_liked(self) -> bool:
         """
-        return self._get_basetype_from_data('thumbPicture', str)
+        Property to check if the comment is liked by you.
 
-    @property
-    def picture(self) -> str:
+        Returns:
+            bool: True if the comment is liked, False otherwise.
         """
-        Retrieves the picture of the article.
-        """
-        return self._get_basetype_from_data('picture', str)
+        return self._access_data('isLiked')
 
     @property
-    def ads(self) -> str:
-        """
-        Retrieves the ads of the article.
+    @DrukarniaElement.type_decorator(int)
+    async def number_of_replies(self) -> int:
         """
-        return self._get_basetype_from_data('ads', str)
+        Property to get the number of replies to the comment.
 
-    @property
-    def index(self) -> str:
-        """
-        Retrieves the index of the article.
+        Returns:
+            int: The number of replies to the comment.
         """
-        return self._get_basetype_from_data('index', str)
+        return self._access_data('replyNum')
 
     @property
-    def created_at(self) -> datetime:
+    @DrukarniaElement.type_decorator(int)
+    async def number_of_likes(self) -> int:
         """
-        Retrieves the creation date of the article.
-        """
-        return self._get_datetime_from_author_data('createdAt')
+        Property to get the number of likes on the comment.
 
-    @property
-    def read_time(self) -> float:
+        Returns:
+            int: The number of likes on the comment.
         """
-        Retrieves the read time of the article.
-        """
-        return self._get_basetype_from_data('readTime', float)
+        return self._access_data('likesNum')
 
     @property
-    def number_of_like(self) -> int:
-        """
-        Retrieves the number of likes of the article.
+    @DrukarniaElement.type_decorator(str)
+    async def article_id(self) -> str or None:
         """
-        return self._get_basetype_from_data('description', int)
+        Property to get the ID of the associated article.
 
-    @property
-    def number_of_comment(self) -> int:
-        """
-        Retrieves the number of comments of the article.
+        Returns:
+            str or None: The ID of the associated article if available, otherwise None.
         """
-        return self._get_basetype_from_data('commentNum', int)
+        return self._access_data('article')
 
     @property
-    async def article_tags(self) -> Tuple['Tag']:
+    async def owner(self) -> 'Author':
         """
-        Retrieves the tags of the article.
-        """
-
-        tags = self._access_data('tags', [])
+        Property to get the owner (author) of the comment.
 
-        if any(map(lambda el: isinstance(el, str), tags)):
-            warn("Tag's data is incomplete, use collect_data method before in order to obtain whole data.")
-            tags = map(lambda el: {'_id': el}, tags)
-
-        return await data2tags(tags, self.session)
-
-    @property
-    async def main_article_tag(self) -> 'Tag' or None:
+        Returns:
+            Author: The Author object representing the owner of the comment.
         """
-        Retrieves the main tag of the article.
-        """
-
-        main_id = self._get_basetype_from_data('mainTagId', str)
-        main_name = self._get_basetype_from_data('mainTag', str)
-        main_slug = self._get_basetype_from_data('mainTagSlug', str)
-
-        if not (main_id and main_name and main_slug):
-            return None
-
-        main_tag, = await data2tags([{'_id': main_id, 'name': main_name, 'slug': main_slug}], self.session)
-
-        return main_tag
+        author = await data2authors([self._access_data('owner', [])], self.session)
+        return author[0] if author else None
 
     @property
-    def description(self) -> str:
-        """
-        Retrieves the description of the article.
+    @DrukarniaElement.type_decorator(str)
+    async def text(self) -> str:
         """
-        return self._get_basetype_from_data('description', str)
+        Property to get the text of the comment.
 
-    @property
-    def seo_title(self) -> str:
-        """
-        Retrieves the SEO title of the article.
+        Returns:
+            str: The text of the comment.
         """
-        return self._get_basetype_from_data('seoTitle', str)
+        return self._access_data('comment')
 
     @property
-    def title(self) -> str:
+    @DrukarniaElement.type_decorator(str)
+    async def owner_id(self) -> str or None:
         """
-        Retrieves the title of the article.
-        """
-        return self._get_basetype_from_data('title', str)
+        Property to get the ID of the owner (author) of the comment.
 
-    @property
-    def article_id(self) -> str:
+        Returns:
+            str or None: The ID of the owner (author) of the comment if available, otherwise None.
         """
-        Retrieves the ID of the article.
-        """
-        return self._get_basetype_from_data('_id', str)
+        return self._access_data('owner', {}).get('_id', None)
 
     @property
-    def slug(self) -> str:
+    @DrukarniaElement.type_decorator(str)
+    async def comment_id(self) -> str:
         """
-        Retrieves the slug of the article.
+        Retrieves the ID of the comment.
+
+        Returns:
+            str: The ID of the comment.
         """
-        return self._get_basetype_from_data('slug', str)
+        return self._access_data('_id')
 
     @staticmethod
-    async def from_records(session: ClientSession, new_data: dict) -> 'Article':
+    async def from_records(session: ClientSession, new_data: dict) -> 'Comment':
         """
-        Creates an Article instance from records.
-        """
-        new_article = Article(session=session)
-        new_article._update_data(new_data)
+        Creates a Comment instance from records.
 
-        return new_article
+        Parameters:
+            session (ClientSession): The aiohttp ClientSession object to use for API requests.
+            new_data (dict): A dictionary containing the data for the new comment.
 
-    def __hash__(self) -> int:
-        """
-        Returns the hash value of the Article object.
+        Returns:
+            Comment: The newly created Comment instance.
         """
-        return hash(self.article_id or self.slug)
+        new_comment = Comment(session=session)
+        new_comment._update_data(new_data)
+
+        return new_comment
```

### Comparing `drukarnia-api-1.0.0/drukarnia_api/shortcuts/class_generator.py` & `drukarnia-api-1.1.1/drukarnia_api/shortcuts/class_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,94 @@
 from typing import Tuple
 from aiohttp import ClientSession
 import asyncio
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:  # always False, used for type hints
-    from drukarnia_api.author import Author
-    from drukarnia_api.article import Article
-    from drukarnia_api.tag import Tag
-    from drukarnia_api.comment import Comment
+    from drukarnia_api.objects.author import Author
+    from drukarnia_api.objects.article import Article
+    from drukarnia_api.objects.tag import Tag
+    from drukarnia_api.objects.comment import Comment
 
 
 async def data2tags(tags_data: list or None, session: ClientSession) -> Tuple['Tag'] or Tuple:
     """
     Converts a list of tag data into Tag objects asynchronously.
 
     Args:
-        tags_data (list or None): List of tag data.
+        tags_data (list or None): List of tag data. If None, an empty tuple will be returned.
         session (ClientSession): aiohttp ClientSession object.
 
     Returns:
-        Tuple: Tuple of Tag objects.
+        Tuple[Tag] or Tuple: Tuple of Tag objects or an empty tuple if tags_data is None.
     """
     if not tags_data:
         return ()
 
-    from drukarnia_api.tag import Tag
+    from drukarnia_api.objects.tag import Tag
 
     tasks = [Tag.from_records(session, tag) for tag in tags_data]
 
     return await asyncio.gather(*tasks)
 
 
 async def data2authors(authors_data: list or None, session: ClientSession) -> Tuple['Author'] or Tuple:
     """
     Converts a list of author data into Author objects asynchronously.
 
     Args:
-        authors_data (list or None): List of author data.
+        authors_data (list or None): List of author data. If None, an empty tuple will be returned.
         session (ClientSession): aiohttp ClientSession object.
 
     Returns:
-        Tuple: Tuple of Author objects.
+        Tuple[Author] or Tuple: Tuple of Author objects or an empty tuple if authors_data is None.
     """
     if not authors_data:
         return ()
 
-    from drukarnia_api.author import Author
+    from drukarnia_api.objects.author import Author
 
     tasks = [Author.from_records(session, author) for author in authors_data]
 
     return await asyncio.gather(*tasks)
 
 
 async def data2articles(articles_data: list or None, session: ClientSession) -> Tuple['Article'] or Tuple:
     """
     Converts a list of article data into Article objects asynchronously.
 
     Args:
-        articles_data (list or None): List of article data.
+        articles_data (list or None): List of article data. If None, an empty tuple will be returned.
         session (ClientSession): aiohttp ClientSession object.
 
     Returns:
-        Tuple: Tuple of Article objects.
+        Tuple[Article] or Tuple: Tuple of Article objects or an empty tuple if articles_data is None.
     """
     if not articles_data:
         return ()
 
-    from drukarnia_api.article import Article
+    from drukarnia_api.objects.article import Article
 
     tasks = [Article.from_records(session, article) for article in articles_data]
 
     return await asyncio.gather(*tasks)
 
 
 async def data2comments(comment_data: list or None, session: ClientSession) -> Tuple['Comment'] or Tuple:
+    """
+    Converts a list of comment data into Comment objects asynchronously.
+
+    Args:
+        comment_data (list or None): List of comment data. If None, an empty tuple will be returned.
+        session (ClientSession): aiohttp ClientSession object.
+
+    Returns:
+        Tuple[Comment] or Tuple: Tuple of Comment objects or an empty tuple if comment_data is None.
+    """
     if not comment_data:
         return ()
 
-    from drukarnia_api.comment import Comment
+    from drukarnia_api.objects.comment import Comment
 
     tasks = [Comment.from_records(session, comment) for comment in comment_data]
 
     return await asyncio.gather(*tasks)
```

### Comparing `drukarnia-api-1.0.0/drukarnia_api.egg-info/PKG-INFO` & `drukarnia-api-1.1.1/drukarnia_api.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 1.0.0
+Version: 1.1.1
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -19,50 +19,52 @@
 
 # drukarnia-api
 
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/main/LICENSE)
 
 ## Overview
-`drukarnia-api` is a Python library designed as a wrapper for the ***Drukarnia API***, providing various functionalities for interacting with the Drukarnia platform. It simplifies the process of accessing and manipulating data from the Drukarnia API, enabling users to seamlessly integrate Drukarnia's features into their applications. The library is actively being developed and already includes almost all of the necessary features. We are working diligently to implement the remaining features as quickly as possible.
+`drukarnia-api` is a Python library designed as a wrapper for the <a href="https://drukarnia.com.ua">***Drukarnia API***</a>, providing various functionalities for interacting with the platform. It simplifies the process of accessing and manipulating data from the web, enabling users to seamlessly work with Drukarnia. The library is actively being developed and already includes almost all of the necessary features. We are working diligently to implement the remaining features as quickly as possible.
 
 
 ## Simple Usage
 ```python
 from drukarnia_api import Search
 
 
 async def get_author_article_titles():
-    async with Search() as search_engine:
-        authors = await search_engine.find_author('cupomanka') 
-        # Get the first search result
-        author = authors[0]
+    search = Search()
+    
+    async with search:
+        cupomanka, *_ = await search.find_author('cupomanka') 
 
         # Collect all data about the user
-        await author.collect_data()
+        await cupomanka.collect_data()
 
         # Get user articles
-        articles = await author.articles
+        articles = await cupomanka.articles
 
         # Print all titles
         for article in articles:
-            print(article.title)
+            print(await article.title)
 
 
 if __name__ == '__main__':
     import asyncio
 
     loop = asyncio.get_event_loop()
     loop.run_until_complete(get_author_article_titles())
 ```
 
+###### Advance Examples: <a href="https://github.com/androu-sys/drukarnia-api/blob/main/usage.ipynb">usage.ipynb</a>
+
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
 pip install drukarnia-api
 ```
 
 ## Contributing
 
-Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository: https://github.com/androu-sys/drukarnia-api.
+Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please <a href="https://github.com/androu-sys/drukarnia-api/issues/new">open an issue</a> or <a href="https://t.me/U1F615">contact me</a>.
```

### Comparing `drukarnia-api-1.0.0/drukarnia_api.egg-info/SOURCES.txt` & `drukarnia-api-1.1.1/drukarnia_api.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 LICENSE
 README.md
 setup.py
 drukarnia_api/__init__.py
-drukarnia_api/article.py
-drukarnia_api/author.py
-drukarnia_api/comment.py
-drukarnia_api/search.py
-drukarnia_api/tag.py
 drukarnia_api.egg-info/PKG-INFO
 drukarnia_api.egg-info/SOURCES.txt
 drukarnia_api.egg-info/dependency_links.txt
 drukarnia_api.egg-info/requires.txt
 drukarnia_api.egg-info/top_level.txt
-drukarnia_api/drukarnia_base/__init__.py
-drukarnia_api/drukarnia_base/connection.py
-drukarnia_api/drukarnia_base/element.py
-drukarnia_api/drukarnia_base/exceptions.py
+drukarnia_api/network/__init__.py
+drukarnia_api/network/connection.py
+drukarnia_api/network/cookie.py
+drukarnia_api/network/exceptions.py
+drukarnia_api/network/headers.py
+drukarnia_api/network/utils.py
+drukarnia_api/objects/__init__.py
+drukarnia_api/objects/article.py
+drukarnia_api/objects/author.py
+drukarnia_api/objects/base_object.py
+drukarnia_api/objects/comment.py
+drukarnia_api/objects/search.py
+drukarnia_api/objects/tag.py
 drukarnia_api/shortcuts/__init__.py
 drukarnia_api/shortcuts/class_generator.py
```

### Comparing `drukarnia-api-1.0.0/setup.py` & `drukarnia-api-1.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get requirements
 with open(path.join(HERE, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="drukarnia-api",
-    version="1.0.0",
+    version="1.1.1",
     description="wrapper for the Drukarnia API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/androu-sys/drukarnia-api",
     author="Andrii Herts",
     license="MIT",
     classifiers=[
@@ -33,11 +33,11 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
-    packages=["drukarnia_api", "drukarnia_api.drukarnia_base", "drukarnia_api.shortcuts"],
+    packages=["drukarnia_api", "drukarnia_api.network", "drukarnia_api.shortcuts", "drukarnia_api.objects"],
     include_package_data=True,
     install_requires=requirements
 )
```

