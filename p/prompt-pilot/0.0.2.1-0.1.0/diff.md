# Comparing `tmp/prompt_pilot-0.0.2.1.tar.gz` & `tmp/prompt_pilot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_pilot-0.0.2.1.tar", max compression
+gzip compressed data, was "prompt_pilot-0.1.0.tar", max compression
```

## Comparing `prompt_pilot-0.0.2.1.tar` & `prompt_pilot-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,11 @@
--rwxr-xr-x   0        0        0      715 2023-07-04 06:16:26.306751 prompt_pilot-0.0.2.1/README.md
--rwxr-xr-x   0        0        0      178 2023-06-10 13:32:54.211564 prompt_pilot-0.0.2.1/prompt_pilot/__init__.py
--rwxr-xr-x   0        0        0       46 2023-06-10 13:30:06.476133 prompt_pilot-0.0.2.1/prompt_pilot/api/__init__.py
--rwxr-xr-x   0        0        0        0 2023-06-10 13:29:37.491549 prompt_pilot-0.0.2.1/prompt_pilot/api/openai.py
--rwxr-xr-x   0        0        0        0 2023-06-10 13:29:45.080510 prompt_pilot-0.0.2.1/prompt_pilot/api/replicate.py
--rwxr-xr-x   0        0        0       77 2023-06-23 03:48:57.037511 prompt_pilot-0.0.2.1/prompt_pilot/database/__init__.py
--rwxr-xr-x   0        0        0        0 2023-06-23 03:47:20.502300 prompt_pilot-0.0.2.1/prompt_pilot/database/pinecone.py
--rwxr-xr-x   0        0        0        0 2023-06-23 03:47:25.180198 prompt_pilot-0.0.2.1/prompt_pilot/database/vectorvault.py
--rwxr-xr-x   0        0        0        0 2023-06-23 03:49:43.426746 prompt_pilot-0.0.2.1/prompt_pilot/database/weaviate.py
--rwxr-xr-x   0        0        0       77 2023-06-22 08:39:57.594475 prompt_pilot-0.0.2.1/prompt_pilot/hello.py
--rwxr-xr-x   0        0        0       52 2023-06-30 06:20:29.554760 prompt_pilot-0.0.2.1/prompt_pilot/language/__init__.py
--rwxr-xr-x   0        0        0    17131 2023-07-04 06:16:35.412877 prompt_pilot-0.0.2.1/prompt_pilot/language/assistants.py
--rwxr-xr-x   0        0        0     4030 2023-07-03 23:22:47.647291 prompt_pilot-0.0.2.1/prompt_pilot/language/characters.py
--rwxr-xr-x   0        0        0      552 2023-07-03 22:33:27.616353 prompt_pilot-0.0.2.1/prompt_pilot/language/others.py
--rwxr-xr-x   0        0        0     3228 2023-07-03 22:03:48.206564 prompt_pilot-0.0.2.1/prompt_pilot/language/psychology.py
--rwxr-xr-x   0        0        0      103 2023-06-30 06:20:22.612831 prompt_pilot-0.0.2.1/prompt_pilot/language/techniques/__init__.py
--rwxr-xr-x   0        0        0     1904 2023-06-30 06:15:19.304174 prompt_pilot-0.0.2.1/prompt_pilot/language/techniques/few_shot.py
--rwxr-xr-x   0        0        0      724 2023-05-30 08:28:53.337680 prompt_pilot-0.0.2.1/prompt_pilot/language/techniques/nlp_tasks.py
--rwxr-xr-x   0        0        0     1192 2023-06-23 03:37:17.453328 prompt_pilot-0.0.2.1/prompt_pilot/language/techniques/promptingtypes.py
--rwxr-xr-x   0        0        0     1238 2023-06-23 03:49:06.026906 prompt_pilot-0.0.2.1/prompt_pilot/language/techniques/zero_shot.py
--rwxr-xr-x   0        0        0       80 2023-06-10 13:25:50.199950 prompt_pilot-0.0.2.1/prompt_pilot/vision/__init__.py
--rwxr-xr-x   0        0        0    13904 2023-06-10 13:25:42.393016 prompt_pilot-0.0.2.1/prompt_pilot/vision/image_generation.py
--rwxr-xr-x   0        0        0      336 2023-05-30 12:25:46.080948 prompt_pilot-0.0.2.1/prompt_pilot/vision/img2img.py
--rwxr-xr-x   0        0        0      355 2023-06-30 06:15:16.320627 prompt_pilot-0.0.2.1/prompt_pilot/vision/inpainting.py
--rwxr-xr-x   0        0        0      502 2023-07-04 06:17:01.342011 prompt_pilot-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1398 1970-01-01 00:00:00.000000 prompt_pilot-0.0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1086 2023-07-07 16:16:32.241652 prompt_pilot-0.1.0/README.md
+-rwxr-xr-x   0        0        0      182 2023-07-07 16:04:29.401311 prompt_pilot-0.1.0/prompt_pilot/__init__.py
+-rwxr-xr-x   0        0        0      557 2023-07-07 10:04:14.663302 prompt_pilot-0.1.0/prompt_pilot/api.py
+-rwxr-xr-x   0        0        0    17144 2023-07-07 09:55:29.893218 prompt_pilot-0.1.0/prompt_pilot/assistants.py
+-rwxr-xr-x   0        0        0     4050 2023-07-06 13:47:26.824640 prompt_pilot-0.1.0/prompt_pilot/characters.py
+-rwxr-xr-x   0        0        0      969 2023-07-05 19:46:03.250001 prompt_pilot-0.1.0/prompt_pilot/data_science.py
+-rwxr-xr-x   0        0        0    13904 2023-06-10 13:25:42.393016 prompt_pilot-0.1.0/prompt_pilot/image_generation.py
+-rwxr-xr-x   0        0        0      336 2023-07-07 16:03:57.618810 prompt_pilot-0.1.0/prompt_pilot/img_to_img.py
+-rwxr-xr-x   0        0        0      355 2023-06-30 06:15:16.320627 prompt_pilot-0.1.0/prompt_pilot/inpainting.py
+-rwxr-xr-x   0        0        0      455 2023-07-07 15:34:55.648885 prompt_pilot-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1578 1970-01-01 00:00:00.000000 prompt_pilot-0.1.0/PKG-INFO
```

### Comparing `prompt_pilot-0.0.2.1/prompt_pilot/language/assistants.py` & `prompt_pilot-0.1.0/prompt_pilot/assistants.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     """
     
     return prompt
 
 def digital_marketing_analyst(name:str = "Alex", company_name:str = "XYZ Corp", company_industry:str = "E-commerce") -> str:
     
     prompt = f"""
-    I want you to behave as a Digital Marketing Analyst for {company_name} in the {company_industry} industry. Your role will involve analyzing digital marketing campaigns, optimizing online presence, and driving customer engagement.
+    I want you to behave as a Digital Marketing Analyst named {name} for {company_name} in the {company_industry} industry. Your role will involve analyzing digital marketing campaigns, optimizing online presence, and driving customer engagement.
 
     As a Digital Marketing Analyst, your responsibilities will include:
 
     1. Campaign Performance Analysis: You will analyze digital marketing campaigns, including search engine marketing (SEM), search engine optimization (SEO), social media marketing, and email marketing, to evaluate performance, identify trends, and provide actionable insights for campaign optimization.
 
     2. Web Analytics: You will work with web analytics tools to track website performance, user behavior, and conversion rates, leveraging data to identify areas of improvement and optimize the user experience.
```

### Comparing `prompt_pilot-0.0.2.1/prompt_pilot/language/characters.py` & `prompt_pilot-0.1.0/prompt_pilot/characters.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 def fictional_character(character: str = "Homer", series: str = "The simpsons") -> tuple[str,str]:
     
     prompt = f"I want you to behave like {character} from {series}. I want you to respond and answer like {character} using the tone, manner and vocabulary {character} would use. Do not write any explanations. Only answer like {character}. You must know all of the knowledge of {character}. My first sentence is 'Hi {character}.'"
     
     return prompt
 
-def magician(input: str = "") -> str:
+def magician(name: str = "Zathura") -> str:
     
-    prompt = "I want you to behave as a magician. I will provide you with an audience and some suggestions for tricks that can be performed. Your goal is to perform these tricks in the most entertaining way possible, using your skills of deception and misdirection to amaze and astound the spectators."
+    prompt = f"I want you to behave as a magician named {name}. I will provide you with an audience and some suggestions for tricks that can be performed. Your goal is to perform these tricks in the most entertaining way possible, using your skills of deception and misdirection to amaze and astound the spectators."
     
     return prompt
 
 def journalist(input: str = "") -> str:
     
     prompt = "I want you to behave as a journalist. You will report on breaking news, write feature stories and opinion pieces, develop research techniques for verifying information and uncovering sources, adhere to journalistic ethics, and deliver accurate reporting using your own distinct style."
```

### Comparing `prompt_pilot-0.0.2.1/prompt_pilot/vision/image_generation.py` & `prompt_pilot-0.1.0/prompt_pilot/image_generation.py`

 * *Files identical despite different names*

