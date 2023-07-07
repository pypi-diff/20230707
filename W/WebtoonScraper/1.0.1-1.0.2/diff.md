# Comparing `tmp/WebtoonScraper-1.0.1.tar.gz` & `tmp/WebtoonScraper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-1.0.1.tar", last modified: Fri Jun 30 10:37:10 2023, max compression
+gzip compressed data, was "WebtoonScraper-1.0.2.tar", last modified: Fri Jul  7 14:00:15 2023, max compression
```

## Comparing `WebtoonScraper-1.0.1.tar` & `WebtoonScraper-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 10:37:10.974297 WebtoonScraper-1.0.1/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-06-30 07:37:22.000000 WebtoonScraper-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11977 2023-06-30 10:37:10.974297 WebtoonScraper-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    10558 2023-06-30 10:17:36.000000 WebtoonScraper-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 10:37:10.956553 WebtoonScraper-1.0.1/WebtoonScraper/
--rw-rw-rw-   0        0        0      522 2023-06-30 07:39:16.000000 WebtoonScraper-1.0.1/WebtoonScraper/BestChallengeScraper.py
--rw-rw-rw-   0        0        0     5602 2023-06-30 10:13:47.000000 WebtoonScraper-1.0.1/WebtoonScraper/BufftoonScraper.py
--rw-rw-rw-   0        0        0    10194 2023-06-29 13:08:21.000000 WebtoonScraper-1.0.1/WebtoonScraper/FolderManager.py
--rw-rw-rw-   0        0        0     4315 2023-06-30 07:49:56.000000 WebtoonScraper-1.0.1/WebtoonScraper/NaverGameScraper.py
--rw-rw-rw-   0        0        0     6909 2023-06-30 10:03:47.000000 WebtoonScraper-1.0.1/WebtoonScraper/NaverPostScraper.py
--rw-rw-rw-   0        0        0     3438 2023-06-30 09:56:21.000000 WebtoonScraper-1.0.1/WebtoonScraper/NaverWebtoonScraper.py
--rw-rw-rw-   0        0        0    16513 2023-06-30 09:37:13.000000 WebtoonScraper-1.0.1/WebtoonScraper/Scraper.py
--rw-rw-rw-   0        0        0     4258 2023-06-30 09:55:18.000000 WebtoonScraper-1.0.1/WebtoonScraper/TelescopeScraper.py
--rw-rw-rw-   0        0        0     7900 2023-06-30 03:51:13.000000 WebtoonScraper-1.0.1/WebtoonScraper/Webtoon.py
--rw-rw-rw-   0        0        0      501 2023-06-06 00:44:55.000000 WebtoonScraper-1.0.1/WebtoonScraper/WebtoonCanvasScraper.py
--rw-rw-rw-   0        0        0     4473 2023-06-30 09:58:27.000000 WebtoonScraper-1.0.1/WebtoonScraper/WebtoonOriginalsScraper.py
--rw-rw-rw-   0        0        0      679 2023-06-28 15:36:38.000000 WebtoonScraper-1.0.1/WebtoonScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 10:37:10.972275 WebtoonScraper-1.0.1/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0    11977 2023-06-30 10:37:10.000000 WebtoonScraper-1.0.1/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-06-30 10:37:10.000000 WebtoonScraper-1.0.1/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 10:37:10.000000 WebtoonScraper-1.0.1/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-1.0.1/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       37 2023-06-30 10:37:10.000000 WebtoonScraper-1.0.1/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-30 10:37:10.000000 WebtoonScraper-1.0.1/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 10:37:10.974297 WebtoonScraper-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1451 2023-06-30 07:38:15.000000 WebtoonScraper-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 10:37:10.972275 WebtoonScraper-1.0.1/test/
--rw-rw-rw-   0        0        0      859 2023-06-30 10:16:31.000000 WebtoonScraper-1.0.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:00:15.993418 WebtoonScraper-1.0.2/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-06-30 07:37:22.000000 WebtoonScraper-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    12160 2023-07-07 14:00:15.993418 WebtoonScraper-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10741 2023-07-07 13:56:07.000000 WebtoonScraper-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 14:00:15.977435 WebtoonScraper-1.0.2/WebtoonScraper/
+-rw-rw-rw-   0        0        0      645 2023-07-06 10:40:03.000000 WebtoonScraper-1.0.2/WebtoonScraper/BestChallengeScraper.py
+-rw-rw-rw-   0        0        0     5726 2023-07-06 10:39:23.000000 WebtoonScraper-1.0.2/WebtoonScraper/BufftoonScraper.py
+-rw-rw-rw-   0        0        0    10280 2023-07-07 13:59:29.000000 WebtoonScraper-1.0.2/WebtoonScraper/FolderManager.py
+-rw-rw-rw-   0        0        0     3766 2023-07-06 10:39:12.000000 WebtoonScraper-1.0.2/WebtoonScraper/NaverGameScraper.py
+-rw-rw-rw-   0        0        0     6756 2023-07-07 13:17:19.000000 WebtoonScraper-1.0.2/WebtoonScraper/NaverPostScraper.py
+-rw-rw-rw-   0        0        0     3653 2023-07-06 10:32:59.000000 WebtoonScraper-1.0.2/WebtoonScraper/NaverWebtoonScraper.py
+-rw-rw-rw-   0        0        0    16392 2023-07-07 13:56:04.000000 WebtoonScraper-1.0.2/WebtoonScraper/Scraper.py
+-rw-rw-rw-   0        0        0     4370 2023-07-06 10:33:22.000000 WebtoonScraper-1.0.2/WebtoonScraper/TelescopeScraper.py
+-rw-rw-rw-   0        0        0     9956 2023-07-06 10:35:05.000000 WebtoonScraper-1.0.2/WebtoonScraper/Webtoon.py
+-rw-rw-rw-   0        0        0      650 2023-07-06 10:29:39.000000 WebtoonScraper-1.0.2/WebtoonScraper/WebtoonCanvasScraper.py
+-rw-rw-rw-   0        0        0     4458 2023-07-06 10:40:46.000000 WebtoonScraper-1.0.2/WebtoonScraper/WebtoonOriginalsScraper.py
+-rw-rw-rw-   0        0        0     1124 2023-07-06 08:12:25.000000 WebtoonScraper-1.0.2/WebtoonScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:00:15.990225 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0    12160 2023-07-07 14:00:15.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      702 2023-07-07 14:00:15.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:00:15.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2023-07-07 14:00:15.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-07 14:00:15.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 14:00:15.993418 WebtoonScraper-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-07-07 13:56:29.000000 WebtoonScraper-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:00:15.992224 WebtoonScraper-1.0.2/test/
+-rw-rw-rw-   0        0        0      217 2023-07-06 11:06:58.000000 WebtoonScraper-1.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0     1502 2023-07-07 13:23:14.000000 WebtoonScraper-1.0.2/test/test.py
```

### Comparing `WebtoonScraper-1.0.1/LICENSE` & `WebtoonScraper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.0.1/PKG-INFO` & `WebtoonScraper-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: License :: OSI Approved :: MIT License
@@ -81,15 +81,15 @@
 로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
 
 1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BU) # 복사했던 수를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF) # 복사했던 수를 여기에다 붙여넣으세요.
    ```
 3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 로그인한 상태에서 웹툰 다운로드하기
 
 이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
@@ -202,15 +202,17 @@
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
 # Relese Note
 
-1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경
+1.0.2: 대형 리팩토링, get_webtoon_platform 비동기 방식으로 속도 개선, 상대경로로 변경, 테스트 추가
+
+1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경 (버그가 많기에 사용을 권장하지 않음)
 
 1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
 
 0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
 
 0.1.0: 버프툰 추가, 빠진 부분 재추가
```

### Comparing `WebtoonScraper-1.0.1/README.md` & `WebtoonScraper-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
 
 1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BU) # 복사했던 수를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF) # 복사했던 수를 여기에다 붙여넣으세요.
    ```
 3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 로그인한 상태에서 웹툰 다운로드하기
 
 이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
@@ -184,15 +184,17 @@
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
 # Relese Note
 
-1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경
+1.0.2: 대형 리팩토링, get_webtoon_platform 비동기 방식으로 속도 개선, 상대경로로 변경, 테스트 추가
+
+1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경 (버그가 많기에 사용을 권장하지 않음)
 
 1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
 
 0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
 
 0.1.0: 버프툰 추가, 빠진 부분 재추가
```

### Comparing `WebtoonScraper-1.0.1/WebtoonScraper/BestChallengeScraper.py` & `WebtoonScraper-1.0.2/WebtoonScraper/BestChallengeScraper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 '''Download Webtoons from Naver Webtoon Best Challenge.'''
-from WebtoonScraper.NaverWebtoonScraper import NaverWebtoonScraper
+if __name__ == "__main__":
+    from NaverWebtoonScraper import NaverWebtoonScraper
+else:
+    from .NaverWebtoonScraper import NaverWebtoonScraper
 
 
 class BestChallengeScraper(NaverWebtoonScraper):
     def __init__(self, pbar_independent=False, short_connection=False):
         super().__init__(pbar_independent, short_connection)
         self.BASE_URL = 'https://comic.naver.com/bestChallenge'
         self.EPISODE_IMAGES_URL_SELECTOR = '#comic_view_area > div > img'
 
 
 if __name__ == '__main__':
     wt = BestChallengeScraper()
+    wt.get_webtoon(763952)  # 과학고
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `WebtoonScraper-1.0.1/WebtoonScraper/BufftoonScraper.py` & `WebtoonScraper-1.0.2/WebtoonScraper/BufftoonScraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 '''Download Webtoons from Bufftoon.'''
 import re
 from pathlib import Path
 import time
 from async_lru import alru_cache
-from WebtoonScraper.Scraper import Scraper
+
+if __name__ == "__main__":
+    from WebtoonScraper.Scraper import Scraper
+else:
+    from .Scraper import Scraper
+
 
 class BufftoonScraper(Scraper):
     '''Scrape webtoons from Bufftoon.'''
-    def __init__(self, pbar_independent=False, short_connection=False, cookie: str=''):
+    def __init__(self, pbar_independent: bool = False, short_connection: bool = False, cookie: str = ''):
         super().__init__(pbar_independent, short_connection)
         self.BASE_URL = 'https://bufftoon.plaync.com'
         if not short_connection:
             self.IS_STABLE_CONNECTION = True
         self.COOKIE = cookie
-    
+
     @alru_cache(maxsize=4)
-    async def _get_webtoon_infomation(self, titleid, get_payment: bool=False, limit: int=500):
+    async def _get_webtoon_infomation(self, titleid, get_payment: bool = False, limit: int = 500):
         url = f'https://api-bufftoon.plaync.com/v2/series/{titleid}/episodes?sortType=2&offset=0&limit={limit}'
         raw_data = await self.get_internet('requests', url)
         raw_data = raw_data.json()
         subtitles = {}
         episode_ids = {}
         for raw_episode in raw_data['result']['episodes']:
             if not get_payment and raw_episode['isPaymentEpisode']:
@@ -63,16 +68,17 @@
         if sleep:
             time.sleep(1)
         subtitles, _ = await self._get_webtoon_infomation(titleid)
         subtitle = subtitles[episode_no]
         if file_acceptable:
             subtitle = self.get_acceptable_file_name(subtitle)
         return subtitle
-    
+
     async def get_episode_images_url(self, titleid, episode_no):
+        # sourcery skip: de-morgan
         HEADERS = {
             'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
             'Accept-Encoding': 'gzip, deflate, br',
             'Accept-Language': 'ko,en-US;q=0.9,en;q=0.8',
             'Cache-Control': 'max-age=0',
             'Connection': 'keep-alive',
             'Cookie': self.COOKIE,
@@ -86,22 +92,23 @@
             'Sec-Fetch-Dest': 'document',
             'Sec-Fetch-Mode': 'navigate',
             'Sec-Fetch-Site': 'same-origin',
             'Sec-Fetch-User': '?1',
             'Sec-Gpc': '1',
             'Upgrade-Insecure-Requests': '1',
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.43',
-            }
+        }
         _, episode_ids = await self._get_webtoon_infomation(titleid)
         url = f'{self.BASE_URL}/series/{titleid}/{episode_ids[episode_no]}'
         selector = '#content > div > div > div.viewer-wrapper > div > img'
         episode_images_url = await self.get_internet(get_type='soup_select', url=url,
-                                            selector=selector, headers=HEADERS)
-        
+                                                     selector=selector, headers=HEADERS)
+
         return [element['src'] for element in episode_images_url if not ('agerate' in element['src'] or 'ctguide' in element['src'])]
-    
+
     async def download_single_image(self, episode_dir: Path, url: str, image_no: int) -> None:
         super().download_single_image(episode_dir, url, image_no, 'png')
-    
+
+
 if __name__ == '__main__':
-    bt = BufftoonScraper()
-    bt.download_one_webtoon(1007888)
+    wt = BufftoonScraper()
+    wt.get_webtoon(1007888)  # 겜덕툰
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `WebtoonScraper-1.0.1/WebtoonScraper/FolderManager.py` & `WebtoonScraper-1.0.2/WebtoonScraper/FolderManager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+"""This module provides FolderManager class."""
+
 # 회차 묶기
 import os
 import shutil
 import re
 from collections import defaultdict
 from pathlib import Path
 import logging
 
 
 class FolderManager:
     def __init__(self):
-        
+
         self.BASE_DIR = 'webtoon'
         self.ALT_DIR = 'webtoon'
 
     @property
     def BASE_DIR(self):
         return self._BASE_DIR
 
@@ -30,69 +32,66 @@
         self._ALT_DIR = Path(ALT_DIR)
 
     ############### MAIN FUNCTIONALITY ###############
 
     def merge_webtoons_in_directory(self, merge_amount):
         webtoons = os.listdir(self.BASE_DIR)
         for webtoon in webtoons:
-            alt_webtoon_dir = self.ALT_DIR / webtoon
-            # base_dir와 alt_dir가 같은 경우를 대비해 이름을 달리함.
-            temp_alt_webtoon_dir = self.ALT_DIR / (webtoon + '(merged)') # why do I have to?
-            base_webtoon_dir = self.BASE_DIR / webtoon
-            self._merge_webtoon_episodes(base_webtoon_dir, temp_alt_webtoon_dir, merge_amount=merge_amount)
-            shutil.rmtree(base_webtoon_dir)
-            temp_alt_webtoon_dir.rename(alt_webtoon_dir)
-            # break
+            webtoon_dir = self.ALT_DIR / webtoon
+            self.merge_webtoon_episodes(webtoon_dir, merge_amount)
 
     def merge_webtoon_episodes(self,
                                webtoon_dir: Path,
                                merge_amount,
                                merge_last_bundle=True):
+        """
+        _merge_webtoon_episodes는 base_dir/alt_dir 두 가지 input을 받고 두 값이 같아서는 안 되지만,
+        merge_webtoon_episodes는 한 가지 input만 받고 한 폴더 내의 상태를 바꿔준다.
+        """
         # base_dir와 alt_dir가 같은 경우를 대비해 이름을 달리함.
-        # temp_alt_webtoon_dir = Path(str(webtoon_dir.parents)) / (webtoon_dir.name + '(merged)') # why do I have to?
-        temp_alt_webtoon_dir = Path(str(webtoon_dir) + '(merged)')
+        temp_alt_webtoon_dir = Path(f'{webtoon_dir}(merged)')
         self._merge_webtoon_episodes(webtoon_dir, temp_alt_webtoon_dir, merge_amount=merge_amount, merge_last_bundle=merge_last_bundle)
         os.rmdir(webtoon_dir)
         temp_alt_webtoon_dir.rename(webtoon_dir)
 
     def _merge_webtoon_episodes(self, base_webtoon_dir: Path, alt_webtoon_dir: Path, merge_amount, merge_last_bundle=True):
         # base_webtoon_dir와 alt_webtoon_dir가 같으면 안됨!
         if base_webtoon_dir == alt_webtoon_dir:
-            raise NotImplementedError('base_webtoon_dir and alt_webtoon_dir cannot be same.')
-        
+            raise NotImplementedError('base_webtoon_dir and alt_webtoon_dir cannot be same. Use merge_webtoon_episodes instead.')
+
         alt_webtoon_dir.mkdir(parents=True, exist_ok=True)
 
         # Thumbnail 옮기기 > alt_dir로 옮기는 것으로 변경
         self._move_thumbnail(base_webtoon_dir, alt_webtoon_dir)
-        
+
         # 에피소드를 분해해 base_webtoon_dir에 형식에 맞추어 넣음
         if not self._is_unified(base_webtoon_dir):
             self._unify_webtoon(base_webtoon_dir)
 
         # episode_bundle이 1인 경우 revert_to_original_download_state 수행
         if merge_amount == 1:
             print('Value of episode_bundle is 1, so autometically revert directory state to original.')
             self.restore_webtoon(base_webtoon_dir)
         episodes = os.listdir(base_webtoon_dir)
 
         # merge_last_bundle을 고려하지 않고 컬랙션을 제작함
-        merged_images: list[list[str]] = defaultdict(list)
+        merged_images = defaultdict(list)
         for episode in episodes:
             episode_no = int(episode.split('.')[0])
-            merged_images[(episode_no - 1)//merge_amount].append(episode)
+            merged_images[(episode_no - 1) // merge_amount].append(episode)
 
         # merge_last_bundle을 적용함
-        merged_images = sorted(merged_images.items())
-        _, last_images = merged_images[-1]
-        if merge_last_bundle and len(self._find_episode_id(last_images)) != merge_amount:
-            merged_second_last_list = merged_images[-2][1]
-            merged_second_last_list += merged_images.pop()[1]
+        merged_images_list: list[tuple[int, list[str]]] = sorted(merged_images.items())
+        _, last_images = merged_images_list[-1]
+        if merge_last_bundle and len(self._find_episode_id(last_images)) > merge_amount:
+            merged_second_last_list = merged_images_list[-2][1]
+            merged_second_last_list += merged_images_list.pop()[1]
 
         # 폴더에 넣는 과정
-        for _, images in merged_images:
+        for _, images in merged_images_list:
             alt_dir_name = self._make_dir_name(images)
             images_dir = alt_webtoon_dir / alt_dir_name
             images_dir.mkdir(parents=True, exist_ok=True)
             for image in images:
                 image_dir = base_webtoon_dir / image
                 shutil.move(image_dir, images_dir)
 
@@ -102,73 +101,80 @@
             return
         for episode_or_thumbnail in os.listdir(base_webtoon_dir):
             if re.match(r'.+[.](jpg|jpeg|png)$', episode_or_thumbnail, re.I):
                 base_thumbnail_dir = base_webtoon_dir / episode_or_thumbnail
                 alt_thumbnail_dir = alt_webtoon_dir / episode_or_thumbnail
                 shutil.move(base_thumbnail_dir, alt_thumbnail_dir)
                 return
-            
+
     ############### SUB FUNCTIONALITY ###############
 
     def _make_dir_name(self, images):
         episode_id = self._find_episode_id(images)
         # episode_id = set(int(image.split('.')[0]) for image in images)
         return f'{min(episode_id):04d}~{max(episode_id):04d}'
-    
+
     @staticmethod
     def _find_episode_id(images):
         return {int(image.split('.')[0]) for image in images}
-    
-    def _move_images(self, base_episode_dir: Path, alt_webtoon_dir: Path,
-                     episode_name: str|None=None, ignore_folders: bool=False, rename: bool=False):
-        """이미지가 들어있는 폴더를 받아서 rename하거나 하지 않고 alt_webtoon_dir로 보내는 함수
+
+    def _transit_folder_insides(self, base_episode_dir: Path,
+                                alt_webtoon_dir: Path,
+                                episode_name: str | None = None,
+                                ignore_folders: bool = False,
+                                rename: bool = False
+                                ):
+        """base와 alt 두 종류의 폴더를 받아 base 안의 내용물을 alt로 보내는 함수
 
         Args:
             base_episode_dir (Path): 이미지가 들어있는 폴더
             alt_webtoon_dir (Path): 이미지를 보낼 폴더
             episode_name (str): 만약 rename을 할 경우, 이름을 정하기 위한 에피소드 이름.
             ignore_folders (bool, optional): 폴더를 무시할 지 여부. Defaults to False.
             rename (bool, optional): 이름을 바꿀 것인지 여부. Defaults to False.
         """
         images = os.listdir(base_episode_dir)
         if ignore_folders:
             # 디렉토리(확장자가 없는 경우, 맨 앞줄 '.'은 상관없음.)이면 제거
             images = (image for image in images if not re.match(r'^([.])*((?![.]).)+$', image))
+
         for image in images:
             base_image_name = base_episode_dir / image
-            # os.rename(base_image_name, alt_image_name)
             if rename:
                 alt_image_name = alt_webtoon_dir / self._rename_image(image, episode_name)
             else:
                 alt_image_name = alt_webtoon_dir / image
             shutil.move(base_image_name, alt_image_name)
 
     def _unify_webtoon(self, directory):
         episodes = os.listdir(directory)
         for episode in episodes:
             base_episode_dir = directory / episode
-            self._move_images(base_episode_dir, directory, episode, rename=True)
+            self._transit_folder_insides(base_episode_dir, directory, episode, rename=True)
             os.rmdir(base_episode_dir)
 
     def _rename_image(self, image_name, episode_name):
         episode_split = re.search(r'^(\d+)[.] (.+)', episode_name)
+        if not episode_split:
+            if re.search(r'^(\d+)~(\d+)', episode_name):
+                raise ValueError(
+                    'Episode name is not valid. It\'s because you tried merging already merged webtoon folder.'
+                )
+            raise ValueError('Episode name is not valid.')
         image_no, image_extension = image_name.split('.')[0], image_name.split('.')[-1]
         return f'{episode_split[1]}.{image_no}. {episode_split[2]}.{image_extension}'
-    
+
     def _is_unified(self, directory):
         episodes_or_images = os.listdir(directory)
-        number_of_images = 0
-        for episode_or_image in episodes_or_images:
-            number_of_images += 1 if re.match(r'.+[.](jpg|jpeg|png)$',
-                                              episode_or_image, re.I) else 0
-        if number_of_images == 1 or number_of_images == 0:
-            return False
-        else:
-            return True
-    
+        number_of_images = sum(
+            1 if re.match(r'.+[.](jpg|jpeg|png)$', episode_or_image, re.I) else 0
+            for episode_or_image in episodes_or_images
+        )
+        return number_of_images not in [1, 0]
+
     ############### RESTORE FUNCTIONALITY ###############
 
     def restore_webtoons_in_directory(self):
         webtoons = os.listdir(self.BASE_DIR)
         for webtoon in webtoons:
             webtoon_dir = self.BASE_DIR / webtoon
             self.restore_webtoon(webtoon_dir)
@@ -178,51 +184,56 @@
         temp_thumbnail_path = directory / 'thumbnail-TEMP'
         temp_thumbnail_path.mkdir(parents=True)
         self._move_thumbnail(directory, temp_thumbnail_path)
 
         if not self._is_unified(directory):
             # self._unify_webtoon(directory)
             directories = os.listdir(directory)
-            directories = (directory_ for directory_ in directories
-                           if not directory_ == 'thumbnail-TEMP')
+            directories = (
+                directory_
+                for directory_ in directories
+                if directory_ != 'thumbnail-TEMP'
+            )
 
             for directory_ in directories:
                 directory_ = directory / directory_
-                self._move_images(directory_, directory)
+                self._transit_folder_insides(directory_, directory)
                 directory_.rmdir()
 
         images = os.listdir(directory)
         images = (image for image in images if image != 'thumbnail-TEMP')
 
         for image in images:
             image_info = re.match(r'(\d+)\.(\d+)\. (.+?)\.(\w.+)', image)
-            episode_no, image_no = image_info.group(1), image_info.group(2)
-            episode_name, image_extension = image_info.group(3), image_info.group(4)
+            if not image_info:
+                raise ValueError('image name is not valid. Possibly trying not merged webtoon folder.')
+            episode_no, image_no = image_info[1], image_info[2]
+            episode_name, image_extension = image_info[3], image_info[4]
 
             episode_dir = directory / f'{episode_no}. {episode_name}'
             alt_image_name = f'{image_no}.{image_extension}'
             episode_dir.mkdir(parents=True, exist_ok=True)
             base_image_path = directory / image
             alt_image_path = episode_dir / alt_image_name
             shutil.move(base_image_path, alt_image_path)
 
         self._move_thumbnail(temp_thumbnail_path, directory)
         temp_thumbnail_path.rmdir()
 
+
 if __name__ == "__main__":
-    print(os.curdir)
     fm = FolderManager()
-    # fm.BASE_DIR = './(699830)'
-    # fm.BASE_DIR = 'webtoon/(699830)'
+
+    # # test setters of BASE_DIR/ALT_DIR
     # fm.BASE_DIR = 'webtoon'
-    # fm.ALT_DIR = './going_on'
-    # fm.ALT_DIR = 'webtoon/going_on'
     # fm.ALT_DIR = 'webtoon'
-    # print(fm.BASE_DIR, repr(fm.ALT_DIR))
-    # print(fm._BASE_DIR, repr(fm._ALT_DIR))
-    # fm.merge_webtoon_episodes(fm.ALT_DIR, fm.BASE_DIR, 5)
-    # fm.merge_webtoon_episodes(fm.BASE_DIR, fm.ALT_DIR, 5)
-    # fm.restore_webtoon(fm.ALT_DIR)
 
-    # fm.merge_webtoons_in_directory(10)
+    # # test getters of BASE_DIR/ALT_DIR
+    # print(fm.BASE_DIR, fm.ALT_DIR)
+
+    # # test main functions
+    fm.merge_webtoons_in_directory(5)
+    # fm.merge_webtoon_episodes(Path('webtoon/somewebtoon(webtoonid)'), 5)
+
+    # # test restore functions
     # fm.restore_webtoons_in_directory()
-    # fm.merge_webtoon_episodes(Path('webtoon/(699830)'), 5)
+    # fm.restore_webtoon(Path('webtoon/somewebtoon(webtoonid)'))
```

### Comparing `WebtoonScraper-1.0.1/WebtoonScraper/NaverGameScraper.py` & `WebtoonScraper-1.0.2/WebtoonScraper/WebtoonOriginalsScraper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,97 @@
-'''Download Webtoons from Naver Post.
+'''Download Webtoons from Webtoon Originals.
 '''
-
-import contextlib
-from pathlib import Path
-from itertools import count
-import json
+from bs4 import BeautifulSoup as bs
 from async_lru import alru_cache
 
-from WebtoonScraper.Scraper import Scraper
+if __name__ == "__main__":
+    from Scraper import Scraper
+else:
+    from .Scraper import Scraper
+
 
-class NaverGameScraper(Scraper):
-    '''Scrape webtoons from Naver Post.'''
+class WebtoonOriginalsScraper(Scraper):
+    '''Scrape webtoons from Webtoon Originals.'''
     def __init__(self, pbar_independent=False, short_connection=False):
         super().__init__(pbar_independent, short_connection)
-        self.BASE_URL = 'https://game.naver.com/original_series'
-        if not short_connection:
-            self.IS_STABLE_CONNECTION = True
+        self.BASE_URL = 'https://www.webtoons.com/en/fantasy/watermelon'
+        self.IS_STABLE_CONNECTION = False
+        self.USER_AGENT = {
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+            "Referer": "http://www.webtoons.com"
+        }
+
+    async def get_title(self, titleid, file_acceptable):
+        url = f'{self.BASE_URL}/list?title_no={titleid}'
+        title = await self.get_internet(get_type='soup_select_one', url=url,
+                                        selector='meta[property="og:title"]')
+        title = title['content']
+        if file_acceptable:
+            title = self.get_acceptable_file_name(title)
+        return title
 
     @alru_cache(maxsize=4)
     async def _get_webtoon_infomation(self, titleid):
-        url = f'https://apis.naver.com/nng_main/nng_main/original/series/{titleid}'
-        webtoon_raw_data = await self.get_internet(get_type='requests', url=url)
-        webtoon_raw_data = webtoon_raw_data.json()
-        title = webtoon_raw_data['content']['seriesName']
-        thumbnail = webtoon_raw_data['content']['seriesImage']['verticalLogoImageUrl']
-        return title, thumbnail
+        # getting title_no
+        url = f'{self.BASE_URL}/list?title_no={titleid}'
+        title_no = await self.get_internet('soup_select_one', url, '#_listUl > li')
+        title_no = int(title_no['data-episode-no'])
+
+        # getting list of titles
+        selector = '#_bottomEpisodeList > div.episode_cont > ul > li'
+        url = f'{self.BASE_URL}/prologue/viewer?title_no={titleid}&episode_no={title_no}'
+        selected = await self.get_internet(get_type='soup_select', url=url,
+                                           selector=selector)
+
+        subtitles = {}
+        for element in selected:
+            episode_no = int(element["data-episode-no"])
+            subtitles[episode_no] = element.select_one("span.subj").text
 
-    @alru_cache(maxsize=4)
-    async def _get_episode_infomation(self, titleid, episode_max_limit=500):
-        # 여러 시즌을 하나로 통합
-        content_raw_data = []
-        for season in count(1):
-            url = f'https://apis.naver.com/nng_main/nng_main/original/series/{titleid}/seasons/{season}/contents?direction=NEXT&pagingType=CURSOR&sort=FIRST&limit={episode_max_limit}'
-            res = await self.get_internet(get_type='requests', url=url)
-            res = res.json()
-            if not res['content']:
-                break
-            content_raw_data += res['content']['data']
-
-        # 부제목, 이미지 데이터 불러옴
-        episodes_data = {}
-        for i, episode in enumerate(content_raw_data, 1):
-            # print(episode['feedId'])
-            subtitle = episode['feed']['title']
-            # print(json.loads(episode['feed']['contents']))
-            content_json_data = json.loads(episode['feed']['contents'])
-            image_urls = []
-            for image_url in content_json_data['document']['components']:
-                with contextlib.suppress(KeyError):
-                    image_urls.append(image_url['src'])
-            episodes_data[i] = {'subtitle': subtitle, 'image_urls': image_urls}
-
-        return episodes_data
-
-    async def get_title(self, titleid, file_acceptable=True):
-        title, _ = await self._get_webtoon_infomation(titleid)
-        if file_acceptable:
-            title = self.get_acceptable_file_name(title)
-        return title
+        return subtitles
 
     async def save_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
-        _, image_url = await self._get_webtoon_infomation(titleid)
+        url = f'{self.BASE_URL}/list?title_no={titleid}'
+        image_url = await self.get_internet(get_type='soup_select_one', url=url,
+                                            selector='meta[property="og:image"]')
+        image_url = image_url['content']
+        image_extension = self.get_file_extension(image_url)
+        image_raw = await self.get_internet(get_type='requests', url=image_url)
+        image_raw = image_raw.content
+        thumbnail_file = thumbnail_dir / f'{title}.{image_extension}'
+        thumbnail_file.write_bytes(image_raw)
+
+    async def save_real_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
+        '''save another form of thumbnail.'''
+        url = f'{self.BASE_URL}/rss?title_no={titleid}'
+        response = await self.get_internet(get_type='requests', url=url)
+        soup = bs(response.text, 'xml')
+        image_url = soup.select_one('channel > image > url').text
         image_extension = self.get_file_extension(image_url)
         image_raw = await self.get_internet(get_type='requests', url=image_url)
         image_raw = image_raw.content
-        Path(f'{thumbnail_dir}/{title}.{image_extension}').write_bytes(image_raw)
+        thumbnail_path = thumbnail_dir / f'{title}.{image_extension}'
+        thumbnail_path.write_bytes(image_raw)
 
     async def get_all_episode_no(self, titleid):
-        episodes_data = await self._get_episode_infomation(titleid)
-        return list(episodes_data)
+        subtitles = await self._get_webtoon_infomation(titleid)
+        return list(subtitles)
 
     async def get_subtitle(self, titleid, episode_no, file_acceptable):
-        episodes_data = await self._get_episode_infomation(titleid)
-        subtitle = episodes_data[episode_no]['subtitle']
-        if file_acceptable:
-            subtitle = self.get_acceptable_file_name(subtitle)
-        return subtitle
+        subtitles = await self._get_webtoon_infomation(titleid)
+        subtitle = subtitles[episode_no]
 
-    async def get_episode_images_url(self, titleid, episode_no):
-        episodes_data = await self._get_episode_infomation(titleid)
-        return episodes_data[episode_no]['image_urls']
-    
-if __name__ == '__main__':
-    # np = NaverPost()
-    # np.download_one_webtoon(625402, 19803452)
+        return self.get_acceptable_file_name(subtitle) if file_acceptable else subtitle
 
-    # wt = NaverPost()
-    # asyncio.run(wt.get_data(625402, 19803452))
+    async def get_episode_images_url(self, titleid, episode_no):
+        url = f'{self.BASE_URL}/prologue/viewer?title_no={titleid}&episode_no={episode_no}'
+        episode_images_url = await self.get_internet(get_type='soup_select', url=url,
+                                                     selector='#_imageList > img')
+        return [
+            element['data-url']
+            for element in episode_images_url
+            if not ('agerate' in element['src'] or 'ctguide' in element['src'])
+        ]
 
-    # wt = NaverPost()
-    # wt.member_no = 19803452
-    # print(asyncio.run(wt.get_episode_images_url(577056, 2)))
-
-    # from NaverPost import NaverPostScraper
-    wt = NaverGameScraper()
-    # wt.download_one_webtoon(614921, 19803452)
-    # wt.download_one_webtoon(577056, 19803452)
-    # wt.download_one_webtoon(625402, 19803452)
-    # wt.set_folders('webtoon')
-    # wt.download_one_webtoon(31)
-    wt.download_one_webtoon(5)
+if __name__ == '__main__':
+    wt = WebtoonOriginalsScraper()
+    wt.download_one_webtoon(5291)  # Wumpus
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `WebtoonScraper-1.0.1/WebtoonScraper/NaverPostScraper.py` & `WebtoonScraper-1.0.2/WebtoonScraper/NaverPostScraper.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,55 +3,61 @@
 
 from pathlib import Path
 from itertools import count
 import asyncio
 from async_lru import alru_cache
 import demjson3
 from bs4 import BeautifulSoup
-from WebtoonScraper.Scraper import Scraper
+
+if __name__ == "__main__":
+    from Scraper import Scraper
+else:
+    from .Scraper import Scraper
+
 
 class NaverPostScraper(Scraper):
     '''Scrape webtoons from Naver Post.'''
     def __init__(self, pbar_independent=False, short_connection=False):
         super().__init__(pbar_independent, short_connection)
         self.BASE_URL = 'https://post.naver.com'
         if not short_connection:
             self.IS_STABLE_CONNECTION = True
 
-    def download_one_webtoon(self, titleid: int, member_no: int,  value_range: tuple|int|None=None) -> None:
+    def download_one_webtoon(self, titleid: int, member_no: int,  value_range: tuple | int | None = None) -> None:
         """async를 사용하지 않는 일반 상태일 경우 사용하는 함수이다. 사용법은 download_one_webtoon_async와 동일하다."""
         asyncio.run(self.download_one_webtoon_async(titleid, member_no,  value_range))
 
-    async def download_one_webtoon_async(self, titleid, member_no: int, episode_no_range: tuple|int|None=None) -> None:
+    async def download_one_webtoon_async(self, titleid, member_no: int, episode_no_range: tuple | int | None = None) -> None:
         """포스트는 member_no도 받아야 하기 때문에 불가피하게 수정이 필요."""
         self.member_no = member_no
         await super().download_one_webtoon_async(titleid, episode_no_range)
 
     @alru_cache(maxsize=4)
     async def _get_webtoon_infomation(self, titleid: int) -> list:
+        # sourcery skip: for-append-to-extend, list-comprehension, move-assign-in-block
         subtitle_list = []
         for i in count(1):
             subtitle_sublist = []
             # n번째 리스트 불러옴
             url = f'https://post.naver.com/my/series/detail/more.nhn?memberNo={self.member_no}&seriesNo={titleid}&lastSortOrder=49&prevVolumeNo=&fromNo={i}&totalCount=68'
             # print(url)
             response = await self.get_internet('requests', url)
 
             # 네이버는 기본적으로 json이 망가져 있기에 json이 망가져 있어도 parse를 해주는 demjson이 필요
             demres = demjson3.decode(response.text)['html']
             soup = BeautifulSoup(demres, 'html.parser')
-            
+
             # subtitle data만듦.
             for tag in soup.select('ul > li > a > div > span.ell'):
-                subtitle_sublist.append({'subtitle' : tag.text.strip()})
+                subtitle_sublist.append({'subtitle': tag.text.strip()})
             for j, tag in enumerate(soup.select('ul > li > a > div > span.spot_post_like')):
                 # 버려지는 값은 member_no/그냥 member_no라고 해도 되지만 혹시 모를 corruption을 막기 위한 조치
                 episode_id, _ = map(int, tag['data-cid'].split('_'))
                 subtitle_sublist[j].update({'episode_id': episode_id, 'member_no': self.member_no})
-            
+
             # 지금 받아온 데이터가 이전 데이터와 같은지 확인
             if subtitle_sublist == subtitle_list[-len(subtitle_sublist):]:
                 break
             else:
                 subtitle_list += subtitle_sublist
         # 1화부터로 변경
         return subtitle_list[::-1]
@@ -77,58 +83,50 @@
 
     async def get_all_episode_no(self, titleid):
         """1부터 시작하니 주의!!"""
         subtitle_list = await self._get_webtoon_infomation(titleid)
         return (i + 1 for i in range(len(subtitle_list)))
 
     async def get_subtitle(self, titleid, episode_no, file_acceptable):
-        # if sleep:
-        #     time.sleep(1)
         subtitle_list = await self._get_webtoon_infomation(titleid)
         subtitle_info = subtitle_list[episode_no - 1]
         subtitle = subtitle_info['subtitle']
         if file_acceptable:
             subtitle = self.get_acceptable_file_name(subtitle)
         return subtitle
 
     async def get_episode_images_url(self, titleid, episode_no, attempt=3):
         subtitle_list = await self._get_webtoon_infomation(titleid)
         episode_id = subtitle_list[episode_no - 1]['episode_id']
         url = f'https://post.naver.com/viewer/postView.naver?volumeNo={episode_id}&memberNo={self.member_no}&navigationType=push'
         for _ in range(attempt):
             content = await self.get_internet(get_type='soup_select_one', url=url,
-                                                    selector='#__clipContent')
+                                              selector='#__clipContent')
             if content is None:
                 # '존재하지 않는 포스트입니다'하는 경고가 뜬 후 사이트가 받아지지 않는 오류
                 # 아마 episode_id에 titleid가 잘못 들어가면 생기는 오류로 추정하지만
                 # 정확한 이유는 불명, 가끔씩 생기는 문제.
                 print(f'episode {episode_id} invalid. retrying...')
             else:
                 break
         else:
             raise ConnectionError('Unknown error occurred. Please try again later.')
         content = content.text
         soup_content = BeautifulSoup(content, 'html.parser')
-        
+
         # 문서 내에 있는 모든 이미지 링크를 불러옴
         selector = 'div.se_component_wrap.sect_dsc.__se_component_area > div > div > div > div > a > img'
         episode_images_url = [tag['data-src'] for tag in soup_content.select(selector)]
-        
-        return [url for url in episode_images_url 
+
+        return [url for url in episode_images_url
                 if not url.startswith('https://mail.naver.com/read/image/')]
-    
+
+
 if __name__ == '__main__':
-    # np = NaverPost()
-    # np.download_one_webtoon(625402, 19803452)
+    wt = NaverPostScraper()
+    wt.download_one_webtoon(597061, 19803452)  # 겜덕겜소
 
-    # wt = NaverPost()
     # asyncio.run(wt.get_data(625402, 19803452))
 
-    # wt = NaverPost()
+    # wt = NaverPostScraper()
     # wt.member_no = 19803452
     # print(asyncio.run(wt.get_episode_images_url(577056, 2)))
-
-    # from NaverPost import NaverPostScraper
-    wt = NaverPostScraper()
-    # wt.download_one_webtoon(614921, 19803452)
-    wt.download_one_webtoon(577056, 19803452)
-    wt.download_one_webtoon(625402, 19803452)
```

### Comparing `WebtoonScraper-1.0.1/WebtoonScraper/NaverWebtoonScraper.py` & `WebtoonScraper-1.0.2/WebtoonScraper/NaverWebtoonScraper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 '''Download Webtoons from Naver Webtoon.'''
 from itertools import count
 from async_lru import alru_cache
 
-from WebtoonScraper.Scraper import Scraper
+if __name__ == "__main__":
+    from Scraper import Scraper
+else:
+    from .Scraper import Scraper
+
+
 class NaverWebtoonScraper(Scraper):
     '''Scrape webtoons from Naver Webtoon.'''
     def __init__(self, pbar_independent=False, short_connection=False):
         super().__init__(pbar_independent, short_connection)
         self.BASE_URL = 'https://comic.naver.com/webtoon'
         if not short_connection:
             self.IS_STABLE_CONNECTION = True
-        self.EPISODE_IMAGES_URL_SELECTOR = '#sectionContWide > img' # for best challenge
+        self.EPISODE_IMAGES_URL_SELECTOR = '#sectionContWide > img'  # for best challenge
 
     @alru_cache(maxsize=4)
     async def _get_webtoon_data(self, titleid: int):
         prev_articleList = []
         subtitles = {}
         for i in count(1):
             url = f"https://comic.naver.com/api/article/list?titleId={titleid}&page={i}&sort=ASC"
             res = await self.get_internet('requests', url)
             res = res.json()
-            
+
             curr_articleList = res["articleList"]
             if prev_articleList == curr_articleList:
                 break
             for article in curr_articleList:
                 subtitles[article["no"]] = article["subtitle"]
 
             prev_articleList = curr_articleList
-            
+
         return subtitles
 
     async def get_title(self, titleid, file_acceptable):
         url = f'{self.BASE_URL}/list?titleId={titleid}'
         title = await self.get_internet(get_type='soup_select_one', url=url,
                                         selector='meta[property="og:title"]')
         title = title['content']
@@ -55,24 +60,25 @@
         subtitles = await self._get_webtoon_data(titleid)
         return list(subtitles)
 
     async def get_subtitle(self, titleid, episode_no, file_acceptable):
         subtitles = await self._get_webtoon_data(titleid)
         subtitle = subtitles[episode_no]
 
-        if file_acceptable:
-            subtitle = self.get_acceptable_file_name(subtitle)
-        else:
-            subtitle = subtitle
-
-        return subtitle
+        return self.get_acceptable_file_name(subtitle) if file_acceptable else subtitle
 
     async def get_episode_images_url(self, titleid, episode_no):
         # sourcery skip: de-morgan
         url = f'{self.BASE_URL}/detail?titleId={titleid}&no={episode_no}'
         episode_images_url = await self.get_internet(get_type='soup_select', url=url,
                                                      selector=self.EPISODE_IMAGES_URL_SELECTOR)
         return [element['src'] for element in episode_images_url if not ('agerate' in element['src'] or 'ctguide' in element['src'])]
 
+
 if __name__ == '__main__':
     wt = NaverWebtoonScraper()
-    wt.download_one_webtoon(809590)
+    wt.download_one_webtoon(809590)  # 이번 생
+
+    # # get_internet test(Scraper는 abstract class라 직접 실행이 불가해서 대신 사용)
+    # import asyncio
+    # wt.IS_STABLE_CONNECTION = False
+    # asyncio.run(wt.get_internet('requests', 'https://koifoiewofi.com'))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `WebtoonScraper-1.0.1/WebtoonScraper/Scraper.py` & `WebtoonScraper-1.0.2/WebtoonScraper/Scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 """Abstract Class of all scrapers."""
 # TODO: file_acceptable built-in으로 만들기
+# TODO: titleid tuple도 허용해서 NPScraper에서 이용할 수 있도록 하기
+# TODO: get_webtoon 리스트 형식으로 변경하기
 import re
 import os
 import asyncio
 import shutil
 import html
 from pathlib import Path
 from typing import Iterable, Literal
 from abc import abstractmethod, ABCMeta
 
 import requests
+from requests.exceptions import ConnectionError
 from bs4 import BeautifulSoup as bs
 from bs4.element import Tag
 from tqdm import tqdm
 
+
 class Scraper(metaclass=ABCMeta):
     """Abstract class of all scrapers.
-    
+
     init, get_internet, 전반적인 로직 등은 모두 이 페이지에서 관리하고, 구체적인 다운로드 방법은 각각의 scraper들에게 맡깁니다.
     따라서 썸네일을 받아오거나 한 회차의 이미지 URL을 불러오는 등의 역할은 각자 scraper들에 구현되어 있습니다.
     """
 
-    def __init__(self, pbar_independent: bool=False, short_connection=False) -> None:
+    def __init__(self, pbar_independent: bool = False, short_connection=False) -> None:
         """시작에 필요한 여러가지를 관여합니다.
-        
+
         header, timeout을 구성하고 set_folders()를 호출합니다.
-        
+
         Args:
             pbar_independent: 만약 True라면 tqdm을 이용해서 로그를 표시하고, False라면 print를 통해서 로그를 표시합니다.
             short_connection:
                 만약 True라면 timeout를 3초로 짧게 잡고 IS_STABLE_CONNECTION(거짓일 경우, 연결에 실패하면 재시도를 함.)을 False로 합니다.
                 False라면 기본 설정을 유지하고 timeout도 길게(120초) 유지합니다.
         """
-        # BASE_URL and IS_STABLE_CONNECTION have to defined!
+        # BASE_URL and IS_STABLE_CONNECTION have to be defined!
         self.HEADERS = {
-            'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 '
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 '
             '(KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36'
-            }
-        # self.set_folders()
+        }
         self.BASE_DIR = 'webtoon'
         self.TIMEOUT = 120
         self.PBAR_INDEPENDENT = pbar_independent
         if short_connection:
             self.TIMEOUT = 3
             self.IS_STABLE_CONNECTION = False
-    
-    # @profile
+
     async def get_internet(
-            self, get_type: Literal['requests', 'soup', 'soup_select', 'soup_select_one'], 
-            url: str, selector=None, 
-            is_run_in_executor=False, 
-            attempt: int=10, 
+            self,
+            get_type: Literal['requests', 'soup', 'soup_select', 'soup_select_one'],
+            url: str,
+            selector: str = None,
+            is_run_in_executor: bool = False,
+            attempt: int = 10,
             headers=None
-            ) -> requests.Response|bs|list|Tag|None:
+    ) -> requests.Response | bs | list | Tag | None:
         """Get response/beautifulsoup/beautifulsoup tag list/beautifulsoup tag from internet.
 
         Args:
             get_type:
                 인터넷에서 url로부터 받은 것으로부터 할 것이 무엇인지를 결정합니다.
 
                 'requests': reqests.get한 값을 그대로(.content나 .test, .json()이 붙지 않은 원본 그대로) 반환합니다.
@@ -66,15 +70,14 @@
             url: 가져올 URL을 결정합니다.
             attempt:
                 self.IS_STABLE_CONNECTION이 False일 때 몇 번 시도한 뒤 포기할지를 결정합니다. 기본값은 10입니다.
                 예를 들어 attempt가 10이라면 만약 해당 사이트에 연결을 10번 시도한 뒤에도 실패한다면 포기하고 ConnectionError를 raise합니다.'
             headers: requests.get을 보낼 때 사용할 header를 받습니다. 만약 없을 경우 self.HEADERS를 대신 사용합니다.
         Returns:
             반환값은 어떤 get_type을 사용했는가에 따라 다르다.
-            
             'requests': requests.Response
             'soup': BeautifulSoup
             'soup_select': list[bs4.element.Tag]
             'soup_select_one': bs4.element.Tag
         Raises:
             ConnectionError:
                 만약 연결 오류 횟수가 시도 횟수를 넘어서면 이 에러를 발생합니다.
@@ -102,20 +105,19 @@
         else:
             for _ in range(attempt):
                 is_success = False
                 try:
                     response = await send_get_request()
                     is_success = True
                     break
-                except Exception as e:
-                    print('An error occured. Retrying...')
-                    print(f'Error detail: {e}')
+                except ConnectionError:
+                    print('A connection error occured. But don\'t worry. It should be normal process. Retrying...')
             if not is_success:
                 raise ConnectionError('Trying hard but failed. Maybe low attempt or timeout settizng is reason.'
-                                      ' Trying increasing attempt time or timeout. Or sometimes it is caused by invaild titldid.')
+                                      ' Trying increasing attempt time or timeout. Or sometimes it is caused by invaild titleid.')
 
         if get_type in ('soup', 'soup_select', 'soup_select_one'):
             soup = bs(response.text, "html.parser")
             if get_type == 'soup':
                 return soup
             if get_type == 'soup_select':
                 return soup.select(selector)
@@ -143,72 +145,72 @@
         """
         if self.PBAR_INDEPENDENT:
             print(description)
         else:
             self.pbar.set_description(description)
 
     @staticmethod
-    def get_file_extension(filename_or_url: str) -> str:
+    def get_file_extension(filename_or_url: str) -> str | None:
         """Get file extionsion of filename_or_url.
-        
+
         only supports jpg/png/jpeg/gif file format. If URL has queries, this ignores it.
 
         Args:
             filename_or_url: 파일 확장자가 궁금한 파일명이나 URL. 이때 URL 쿼리는 무시됩니다.
-        
+
         Returns:
             파일 확장자를 반환합니다.
         """
-        serch_result: re.Match|None = re.search(r'(?<=[.])(jpg|png|jpeg|gif)(?=[?].+$|$)', filename_or_url, re.I)
+        serch_result: re.Match | None = re.search(r'(?<=[.])(jpg|png|jpeg|gif)(?=[?].+$|$)', filename_or_url, re.I)
 
-        return None if serch_result is None else serch_result.group()
+        return None if serch_result is None else serch_result[0]
         # return filename_or_url.split('.')[-1].lower()
 
     @staticmethod
-    def get_acceptable_file_name(file_or_diretory_name: str, strict_checking: bool=False) -> str:
+    def get_acceptable_file_name(file_or_diretory_name: str, strict_checking: bool = False) -> str:
         """Translate file or diretory name to accaptable name.
 
         Caution: Don't put here diretory path beacause it will translate slash and backslash to acceptable(and cannot be used for going directory) name.
         """
         table = str.maketrans('\\/:*?"<>|\t\n', '⧵／：＊？＂＜＞∣   ')
 
-        processed = html.unescape(file_or_diretory_name) # change things like "&amp;" to "'".
-        
+        processed = html.unescape(file_or_diretory_name)  # change things like "&amp;" to "'".
+
         processed = processed.translate(table).strip()
 
         processed = re.sub(r'\.$', '．', processed)
 
         if strict_checking:
-            strict_checked_string = ''
-            for chractor in processed:
-                if ord(chractor) in (0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21,
-                                     22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 42, 58, 60, 62, 63, 124):
-                    strict_checked_string += ' '
-                else:
-                    strict_checked_string += chractor
-            return strict_checked_string
+            return ''.join(
+                ' '
+                if ord(chractor)
+                in {
+                    0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20,
+                    21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 42, 58, 60, 62, 63, 124,
+                }
+                else chractor
+                for chractor in processed
+            )
         return processed
 
     @property
     def BASE_DIR(self):
         return self._BASE_DIR
 
     @BASE_DIR.setter
     def BASE_DIR(self, BASE_DIR):
         self._BASE_DIR = Path(BASE_DIR)
 
 ################################## MAIN ACTION ##################################
 
-    def download_one_webtoon(self, titleid: int, value_range: tuple|int|None=None) -> None:
+    def download_one_webtoon(self, titleid: int, value_range: tuple | int | None = None) -> None:
         """async를 사용하지 않는 일반 상태일 경우 사용하는 함수이다. 사용법은 download_one_webtoon_async와 동일하다."""
         asyncio.run(self.download_one_webtoon_async(titleid, value_range))
-        # self.loop.run_until_complete(self.download_one_webtoon_async(titleid, value_range))
 
-    # @profile
-    async def download_one_webtoon_async(self, titleid, episode_no_range: tuple|int|None=None) -> None:
+    async def download_one_webtoon_async(self, titleid, episode_no_range: tuple | int | None = None) -> None:
         """웹툰 다운로드의 주죽이 되는 함수. 이 함수를 통해 웹툰을 다운로드한다.
 
         주의: 유료 회차는 다운로드받을 수 없다.
         :titleid: 다운로드할 웹툰의 titleid 혹은 title_no를 입력한다.
         :episode_no_range: 다운로드할 회차를 정한다.
                                 tuple일 경우: (처음, 끝) 순서로 값을 받는다. 이때 끝을 포함한다.
                                     예) (1,10): 1회차부터 10회차를 다운로드함
@@ -241,21 +243,20 @@
     @abstractmethod
     async def get_title(self, titleid: int, file_acceptable: bool) -> str:
         """웹툰의 title을 불러온다."""
 
     @abstractmethod
     async def save_webtoon_thumbnail(self, titleid: int, title: str, thumbnail_dir: Path) -> None:
         """웹툰의 썸네일을 불러오고 thumbnail_dir에 저장한다."""
-    
+
     @abstractmethod
     async def get_all_episode_no(self, titleid: int) -> Iterable:
         """웹툰에서 전체 에피소드를 가져온다."""
 
-    # @profile
-    def _check_validate_of_files(self, episode_dir: Path, episode_no: int, image_urls: list, subtitle: str) -> None|bool:
+    def _check_validate_of_files(self, episode_dir: Path, episode_no: int, image_urls: list, subtitle: str) -> None | bool:
         """episode_dir를 생성하고 이미 있다면 해당 폴더 내 내용물이 적합한지 조사한다.
 
         None를 return한다면 회차를 다운로드해야 한다는 의미이다.
         True를 return하면 해당 회차가 이미 완전히 다운로드되어 있으며, 따라서 다운로드를 지속할 이유가 없음을 의미한다.
         """
         try:
             episode_dir.mkdir()
@@ -266,15 +267,14 @@
                 self._set_pbar(f'{subtitle} is not vaild. Automatically restore files.')
                 shutil.rmtree(episode_dir)
                 episode_dir.mkdir()
             else:
                 self._set_pbar(f'skipping {subtitle}')
                 return True
 
-    # @profile
     async def download_one_episode(self, episode_no: int, titleid: int, webtoon_dir: Path) -> None:
         """한 회차를 다운로드받는다."""
         subtitle = await self.get_subtitle(titleid, episode_no, file_acceptable=True)
 
         if not subtitle:
             print(f'this episode is not free or not yet created. This episode won\'t be loaded. {episode_no=}')
             self._set_pbar('unknown episode')
@@ -294,28 +294,25 @@
     async def get_subtitle(self, titleid: int, episode_no: int, file_acceptable: bool) -> str:
         """부제목, 즉 회차의 제목을 불러온다."""
 
     @abstractmethod
     async def get_episode_images_url(self, titleid: int, episode_no: int) -> list:
         """해당 회차를 구성하는 이미지들을 불러온다."""
 
-    # @profile
-    async def download_single_image(self, episode_dir: Path, url: str, image_no: int, default_file_extension: str|None=None) -> None:
+    async def download_single_image(self, episode_dir: Path, url: str, image_no: int, default_file_extension: str | None = None) -> None:
         """Download image from url and returns to {episode_dir}/{file_name(translated to accactable name)}."""
-        # print(url)
         image_extension = self.get_file_extension(url)
-        
+
         # for Bufftoon
         if image_extension is None:
             if default_file_extension is not None:
                 raise ValueError('File extension not detected.')
             image_extension = default_file_extension
-        
+
         file_name = f'{image_no:03d}.{image_extension}'
 
         # self._set_pbar(f'{episode_dir}|{file_name}')
         image_raw = await self.get_internet(get_type='requests', url=url, is_run_in_executor=True)
         image_raw = image_raw.content
 
         file_dir = episode_dir / file_name
         file_dir.write_bytes(image_raw)
-
```

### Comparing `WebtoonScraper-1.0.1/WebtoonScraper/TelescopeScraper.py` & `WebtoonScraper-1.0.2/WebtoonScraper/TelescopeScraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """Download Webtoons from Manhwakyung."""
-from WebtoonScraper.Scraper import Scraper
+import time
+
 from async_lru import alru_cache
 
-import time
+if __name__ == "__main__":
+    from Scraper import Scraper
+else:
+    from .Scraper import Scraper
+
 
 class TelescopeScraper(Scraper):
     """Scrape webtoons from Manhwakyung."""
-    
+
     def __init__(self, pbar_independent=False, short_connection=False):
         super().__init__(pbar_independent, short_connection)
         self.BASE_URL = 'https://www.manhwakyung.com'
         self.IS_STABLE_CONNECTION = False
         self.TIMEOUT = 3
 
-    async def download_one_webtoon_async(self, titleid, episode_no_range: tuple|int|None=None):
+    async def download_one_webtoon_async(self, titleid, episode_no_range: tuple | int | None = None):
         self.title, self.list_thumbnail_url, self.grid_thumbnail_url, self.episode_infomation = await self._get_webtoon_infomation(titleid)
         await super().download_one_webtoon_async(titleid, episode_no_range)
 
     @alru_cache(maxsize=4)
     async def _get_webtoon_infomation(self, titleid):
         XHR_HEADER = {
             "authority": 'api.manhwakyung.com',
@@ -55,15 +60,15 @@
         # about episode
         episode_infomation = {}
         for episode in episodes:
             subtitle = episode['name']
             episode_no = episode['episodeNumber']
             episode_id = episode['id']
             episode_infomation[episode_no] = {'subtitle': subtitle, 'episode_id': episode_id}
-            
+
         return title, list_thumbnail_url, grid_thumbnail_url, episode_infomation
 
     async def get_title(self, titleid, file_acceptable):
         return self.title
 
     async def save_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
         image_url = self.grid_thumbnail_url
@@ -78,17 +83,18 @@
 
     async def get_subtitle(self, titleid, episode_no, file_acceptable):
         time.sleep(1)
         subtitle = self.episode_infomation[episode_no]['subtitle']
         if file_acceptable:
             subtitle = self.get_acceptable_file_name(subtitle)
         return subtitle
-    
+
     async def get_episode_images_url(self, titleid, episode_no):
         episode_id = self.episode_infomation[episode_no]['episode_id']
         elemetents = await self.get_internet('soup_select', f'https://www.manhwakyung.com/episode/{episode_id}',
                                              '#__next > div.css-0.euvlwci0 > div.css-0.ebi66ty0 > div > div > img')
         return [element.get('data-src') for element in elemetents]
 
+
 if __name__ == '__main__':
-    pass
-    
+    wt = TelescopeScraper()
+    wt.download_one_webtoon(137)  # 물망초
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `WebtoonScraper-1.0.1/WebtoonScraper.egg-info/PKG-INFO` & `WebtoonScraper-1.0.2/WebtoonScraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: License :: OSI Approved :: MIT License
@@ -81,15 +81,15 @@
 로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
 
 1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BU) # 복사했던 수를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF) # 복사했던 수를 여기에다 붙여넣으세요.
    ```
 3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 로그인한 상태에서 웹툰 다운로드하기
 
 이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
@@ -202,15 +202,17 @@
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
 # Relese Note
 
-1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경
+1.0.2: 대형 리팩토링, get_webtoon_platform 비동기 방식으로 속도 개선, 상대경로로 변경, 테스트 추가
+
+1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경 (버그가 많기에 사용을 권장하지 않음)
 
 1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
 
 0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
 
 0.1.0: 버프툰 추가, 빠진 부분 재추가
```

### Comparing `WebtoonScraper-1.0.1/WebtoonScraper.egg-info/SOURCES.txt` & `WebtoonScraper-1.0.2/WebtoonScraper.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 WebtoonScraper/__init__.py
 WebtoonScraper.egg-info/PKG-INFO
 WebtoonScraper.egg-info/SOURCES.txt
 WebtoonScraper.egg-info/dependency_links.txt
 WebtoonScraper.egg-info/not-zip-safe
 WebtoonScraper.egg-info/requires.txt
 WebtoonScraper.egg-info/top_level.txt
+test/__init__.py
 test/test.py
```

### Comparing `WebtoonScraper-1.0.1/setup.py` & `WebtoonScraper-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 import re
+from pathlib import Path
 
-with open('README.md', 'r', encoding='utf-8') as f:
-    long_description = '이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.\n'
-    long_description += f.read()
-    # 사진 대체
-    repl = r'![\g<1>](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/\g<2>)'
-    long_description = re.sub(r'!\[(.+?)\]\((images\/.+?)\)', repl, long_description)
+long_description = '이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.\n'
+long_description += Path('README.md').read_text(encoding='utf-8')
+# 사진 대체
+repl = r'![\g<1>](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/\g<2>)'
+long_description = re.sub(r'!\[(.+?)\]\((images\/.+?)\)', repl, long_description)
 
 setup(
     name='WebtoonScraper',
-    version='1.0.1',
+    version='1.0.2',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
-    install_requires=['tqdm', 'bs4', 'requests', 'async_lru', 'demjson3'],
+    install_requires=Path('requirements.txt').read_text().split(),
     packages=find_packages(exclude=[]),
     keywords=['Webtoon', 'Webtoon Scraper', 'Naver Webtoon', 'Webtoon Downloader', 'Download Webtoon'],
     python_requires='>=3.10',
     package_data={},
     zip_safe=False,
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

