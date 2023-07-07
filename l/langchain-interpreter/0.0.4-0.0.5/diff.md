# Comparing `tmp/langchain_interpreter-0.0.4.tar.gz` & `tmp/langchain_interpreter-0.0.5.tar.gz`

## Comparing `langchain_interpreter-0.0.4.tar` & `langchain_interpreter-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,25 @@
--rw-r--r--   0        0        0    19257 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/src/examples/chains_from_json.ipynb
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/src/examples/json_from_chains.ipynb
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/src/json/conv_buffer_memory.json
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/src/json/llmchain.json
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/src/json/seq_chain.json
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/src/json/seq_chain_memory.json
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/src/json/simple_seq_chain.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/src/langchain_interpreter/__init__.py
--rwxr-xr-x   0        0        0     4140 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/src/langchain_interpreter/main.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/LICENSE
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/README.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/conf.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/index.rst
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/langchain_interpreter.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/modules.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/docs/requirements.txt
+-rw-r--r--   0        0        0    17907 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/examples/chains_from_json.ipynb
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/examples/json_from_chains.ipynb
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/examples/validation.ipynb
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/json/conv_buffer_memory.json
+-rwxr-xr-x   0        0        0      403 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/json/llmchain.json
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/json/seq_chain.json
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/json/seq_chain_memory.json
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/json/simple_seq_chain.json
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/langchain_interpreter/__init__.py
+-rwxr-xr-x   0        0        0     4767 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/langchain_interpreter/main.py
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/src/langchain_interpreter/validation.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/LICENSE
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/README.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.5/PKG-INFO
```

### Comparing `langchain_interpreter-0.0.4/src/examples/chains_from_json.ipynb` & `langchain_interpreter-0.0.5/src/examples/chains_from_json.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9771593915343915%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'outputs': {0: {'output_type': 'execute_result', 'data': "*

 * *            "OrderedDict([('text/plain', ['True'])]), 'execution_count': 1, 'metadata': "*

 * *            "OrderedDict(), delete: ['name', 'text']}}, 'source': {delete: [5, 4, 3, 2]}}, 1: "*

 * *            "{'execution_count': 2, 'outputs': {0: {'output_type': 'execute_result', 'data': "*

 * *            'OrderedDict([(\'text/plain\', ["{\'product\': \'colorful socks\', \'text\': '*

 * *            '\'\\\\n\\\\nSocktastic!\'}"] […]*

```diff
@@ -1,51 +1,48 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/home/oriont/miniconda3/envs/langchain/lib/python3.11/site-packages/deeplake/util/check_latest_version.py:32: UserWarning: A newer version of deeplake (3.6.7) is available. It's recommended that you update to the latest version using `pip install -U deeplake`.\n",
-                        "  warnings.warn(\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "True"
+                        ]
+                    },
+                    "execution_count": 1,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from dotenv import load_dotenv\n",
-                "load_dotenv()\n",
-                "\n",
-                "import sys\n",
-                "sys.path.insert(1, '../langchain_interpreter/')\n",
-                "from main import chain_from_file"
+                "load_dotenv()\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
-                    "ename": "ImportError",
-                    "evalue": "attempted relative import with no known parent package",
-                    "output_type": "error",
-                    "traceback": [
-                        "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
-                        "\u001b[0;31mImportError\u001b[0m                               Traceback (most recent call last)",
-                        "Cell \u001b[0;32mIn[5], line 1\u001b[0m\n\u001b[0;32m----> 1\u001b[0m \u001b[39mfrom\u001b[39;00m \u001b[39m.\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mlangchain_interpreter\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mmain\u001b[39;00m \u001b[39mimport\u001b[39;00m chain_from_file\n\u001b[1;32m      3\u001b[0m mychain \u001b[39m=\u001b[39m chain_from_file(\u001b[39m\"\u001b[39m\u001b[39m../json/llmchain.json\u001b[39m\u001b[39m\"\u001b[39m)\n\u001b[1;32m      4\u001b[0m mychain({\u001b[39m\"\u001b[39m\u001b[39mproduct\u001b[39m\u001b[39m\"\u001b[39m: \u001b[39m\"\u001b[39m\u001b[39mcolorful socks\u001b[39m\u001b[39m\"\u001b[39m})\n",
-                        "\u001b[0;31mImportError\u001b[0m: attempted relative import with no known parent package"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "{'product': 'colorful socks', 'text': '\\n\\nSocktastic!'}"
+                        ]
+                    },
+                    "execution_count": 2,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from ..langchain_interpreter.main import chain_from_file\n",
+                "from langchain_interpreter.main import chain_from_file\n",
                 "\n",
                 "mychain = chain_from_file(\"../json/llmchain.json\")\n",
                 "mychain({\"product\": \"colorful socks\"})"
             ]
         },
         {
             "cell_type": "code",
@@ -86,15 +83,15 @@
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from ..langchain_interpreter.main import chain_from_file\n",
+                "from langchain_interpreter import chain_from_file\n",
                 "\n",
                 "sschain = chain_from_file(\"../json/simple_seq_chain.json\")\n",
                 "sschain(\"Tragedy at sunset on the beach\")"
             ]
         },
         {
             "cell_type": "code",
@@ -123,15 +120,15 @@
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from main import chain_from_file\n",
+                "from langchain_interpreter import chain_from_file\n",
                 "\n",
                 "seq_chain = chain_from_file(\"json/seq_chain.json\")\n",
                 "seq_chain({\"title\": \"Tragedy at sunset on the beach\", \"era\": \"Victorian England\"})"
             ]
         },
         {
             "cell_type": "code",
@@ -161,15 +158,15 @@
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from main import chain_from_file\n",
+                "from langchain_interpreter import chain_from_file\n",
                 "\n",
                 "seq_chain = chain_from_file(\"json/seq_chain_memory.json\")\n",
                 "seq_chain({\"title\": \"Tragedy at sunset on the beach\", \"era\": \"Victorian England\"})"
             ]
         },
         {
             "cell_type": "code",
@@ -192,15 +189,15 @@
                         "File \u001b[0;32m~/langchain_interpreter/src/examples/../langchain_interpreter/main.py:118\u001b[0m, in \u001b[0;36mget_conversation_buffer_memory\u001b[0;34m(cfg, **kwargs)\u001b[0m\n\u001b[1;32m    116\u001b[0m \u001b[39mif\u001b[39;00m \u001b[39m\"\u001b[39m\u001b[39mhistory\u001b[39m\u001b[39m\"\u001b[39m \u001b[39min\u001b[39;00m kwargs:\n\u001b[1;32m    117\u001b[0m     history \u001b[39m=\u001b[39m kwargs\u001b[39m.\u001b[39mget(\u001b[39m\"\u001b[39m\u001b[39mhistory\u001b[39m\u001b[39m\"\u001b[39m)\n\u001b[0;32m--> 118\u001b[0m     context \u001b[39m+\u001b[39m\u001b[39m=\u001b[39m parse_history(history)\n\u001b[1;32m    120\u001b[0m \u001b[39m# Save context\u001b[39;00m\n\u001b[1;32m    121\u001b[0m \u001b[39mfor\u001b[39;00m pos \u001b[39min\u001b[39;00m \u001b[39mrange\u001b[39m(\u001b[39m0\u001b[39m, \u001b[39mlen\u001b[39m(context), \u001b[39m2\u001b[39m):\n",
                         "File \u001b[0;32m~/langchain_interpreter/src/examples/../langchain_interpreter/main.py:137\u001b[0m, in \u001b[0;36mparse_history\u001b[0;34m(history)\u001b[0m\n\u001b[1;32m    135\u001b[0m         ctx\u001b[39m.\u001b[39mappend({\u001b[39m\"\u001b[39m\u001b[39moutput\u001b[39m\u001b[39m\"\u001b[39m: l\u001b[39m.\u001b[39mlstrip(\u001b[39m\"\u001b[39m\u001b[39mAI: \u001b[39m\u001b[39m\"\u001b[39m)})\n\u001b[1;32m    136\u001b[0m     \u001b[39melse\u001b[39;00m:\n\u001b[0;32m--> 137\u001b[0m         \u001b[39mraise\u001b[39;00m \u001b[39mValueError\u001b[39;00m(\u001b[39m\"\u001b[39m\u001b[39meach line in history must be from AI or human\u001b[39m\u001b[39m\"\u001b[39m)\n\u001b[1;32m    139\u001b[0m \u001b[39mreturn\u001b[39;00m ctx\n",
                         "\u001b[0;31mValueError\u001b[0m: each line in history must be from AI or human"
                     ]
                 }
             ],
             "source": [
-                "\n",
+                "from langchain_interpreter import chain_from_file\n",
                 "\n",
                 "# conv_chain = chain_from_file(\"../json/conv_buffer_memory.json\", history=\"Human: hi\\nAI: whats up\\nHuman: not much. what about you?\\nAI: I've been learning about linear algebra recently. It's really interesting!\")\n",
                 "conv_chain = chain_from_file(\"../json/conv_buffer_memory.json\", history=\"\")\n",
                 "conv_chain(\"Hello!\")"
             ]
         },
         {
@@ -257,23 +254,14 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "conversation.predict(input=\"not much. what about you?\")"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from main import chain_from_file\n"
-            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "langchain",
             "language": "python",
             "name": "python3"
```

### Comparing `langchain_interpreter-0.0.4/src/json/seq_chain.json` & `langchain_interpreter-0.0.5/src/json/seq_chain.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('name', 'Sequential Chain'), ('description', 'An example sequential "*

 * *            "chain.'), ('template_version', '0.0.5'), ('chain', OrderedDict([('type', "*

 * *            "'SequentialChain'), ('input_variables', ['era', 'title']), ('output_variables', "*

 * *            "['synopsis', 'review']), ('chains', [OrderedDict([('type', 'LLMChain'), ('llm', "*

 * *            "OrderedDict([('type', 'openai'), ('args', OrderedDict([('temperature', 0.7)]))])), "*

 * *            "('prompt', OrderedDict([(' […]*

```diff
@@ -1,46 +1,51 @@
 {
-    "chains": [
-        {
-            "llm": {
-                "args": {
-                    "temperature": 0.7
+    "chain": {
+        "chains": [
+            {
+                "llm": {
+                    "args": {
+                        "temperature": 0.7
+                    },
+                    "type": "openai"
                 },
-                "name": "openai"
-            },
-            "output_key": "synopsis",
-            "prompt": {
-                "input_variables": [
-                    "title",
-                    "era"
-                ],
-                "template": "You are a playwright. Given the title of play and the era it is set in, it is your job to write a synopsis for that title.\n\nTitle: {title}\nEra: {era}\nPlaywright: This is a synopsis for the above play:"
-            },
-            "type": "LLMChain"
-        },
-        {
-            "llm": {
-                "args": {
-                    "temperature": 0.7
+                "output_key": "synopsis",
+                "prompt": {
+                    "input_variables": [
+                        "title",
+                        "era"
+                    ],
+                    "template": "You are a playwright. Given the title of play and the era it is set in, it is your job to write a synopsis for that title.\n\nTitle: {title}\nEra: {era}\nPlaywright: This is a synopsis for the above play:"
                 },
-                "name": "openai"
-            },
-            "output_key": "review",
-            "prompt": {
-                "input_variables": [
-                    "synopsis"
-                ],
-                "template": "You are a play critic from the New York Times. Given the synopsis of play, it is your job to write a review for that play.\n\nPlay Synopsis:\n{synopsis}\nReview from a New York Times play critic of the above play:"
+                "type": "LLMChain"
             },
-            "type": "LLMChain"
-        }
-    ],
-    "input_variables": [
-        "era",
-        "title"
-    ],
-    "output_variables": [
-        "synopsis",
-        "review"
-    ],
-    "type": "SequentialChain"
+            {
+                "llm": {
+                    "args": {
+                        "temperature": 0.7
+                    },
+                    "type": "openai"
+                },
+                "output_key": "review",
+                "prompt": {
+                    "input_variables": [
+                        "synopsis"
+                    ],
+                    "template": "You are a play critic from the New York Times. Given the synopsis of play, it is your job to write a review for that play.\n\nPlay Synopsis:\n{synopsis}\nReview from a New York Times play critic of the above play:"
+                },
+                "type": "LLMChain"
+            }
+        ],
+        "input_variables": [
+            "era",
+            "title"
+        ],
+        "output_variables": [
+            "synopsis",
+            "review"
+        ],
+        "type": "SequentialChain"
+    },
+    "description": "An example sequential chain.",
+    "name": "Sequential Chain",
+    "template_version": "0.0.5"
 }
```

### Comparing `langchain_interpreter-0.0.4/src/json/seq_chain_memory.json` & `langchain_interpreter-0.0.5/src/json/seq_chain_memory.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('name', 'Sequential Chain with Simple Memory'), ('description', 'An "*

 * *            "example sequential chain with simple memory.'), ('template_version', '0.0.5'), "*

 * *            "('chain', OrderedDict([('type', 'SequentialChain'), ('input_variables', ['era', "*

 * *            "'title']), ('output_variables', ['social_post_text']), ('memory', "*

 * *            "OrderedDict([('type', 'SimpleMemory'), ('memories', OrderedDict([('time', 'December "*

 * *            "25th, 8pm PST'), ('location', 'Th […]*

```diff
@@ -1,71 +1,76 @@
 {
-    "chains": [
-        {
-            "llm": {
-                "args": {
-                    "temperature": 0.7
+    "chain": {
+        "chains": [
+            {
+                "llm": {
+                    "args": {
+                        "temperature": 0.7
+                    },
+                    "type": "openai"
                 },
-                "name": "openai"
-            },
-            "output_key": "synopsis",
-            "prompt": {
-                "input_variables": [
-                    "title",
-                    "era"
-                ],
-                "template": "You are a playwright. Given the title of play and the era it is set in, it is your job to write a synopsis for that title.\n\nTitle: {title}\nEra: {era}\nPlaywright: This is a synopsis for the above play:"
-            },
-            "type": "LLMChain"
-        },
-        {
-            "llm": {
-                "args": {
-                    "temperature": 0.7
+                "output_key": "synopsis",
+                "prompt": {
+                    "input_variables": [
+                        "title",
+                        "era"
+                    ],
+                    "template": "You are a playwright. Given the title of play and the era it is set in, it is your job to write a synopsis for that title.\n\nTitle: {title}\nEra: {era}\nPlaywright: This is a synopsis for the above play:"
                 },
-                "name": "openai"
-            },
-            "output_key": "review",
-            "prompt": {
-                "input_variables": [
-                    "synopsis"
-                ],
-                "template": "You are a play critic from the New York Times. Given the synopsis of play, it is your job to write a review for that play.\n\nPlay Synopsis:\n{synopsis}\nReview from a New York Times play critic of the above play:"
+                "type": "LLMChain"
             },
-            "type": "LLMChain"
-        },
-        {
-            "llm": {
-                "args": {
-                    "temperature": 0.7
+            {
+                "llm": {
+                    "args": {
+                        "temperature": 0.7
+                    },
+                    "type": "openai"
+                },
+                "output_key": "review",
+                "prompt": {
+                    "input_variables": [
+                        "synopsis"
+                    ],
+                    "template": "You are a play critic from the New York Times. Given the synopsis of play, it is your job to write a review for that play.\n\nPlay Synopsis:\n{synopsis}\nReview from a New York Times play critic of the above play:"
                 },
-                "name": "openai"
+                "type": "LLMChain"
             },
-            "output_key": "social_post_text",
-            "prompt": {
-                "input_variables": [
-                    "synopsis",
-                    "review",
-                    "time",
-                    "location"
-                ],
-                "template": "You are a social media manager for a theater company.  Given the title of play, the era it is set in, the date,time and location, the synopsis of the play, and the review of the play, it is your job to write a social media post for that play.\n\nHere is some context about the time and location of the play:\nDate and Time: {time}\nLocation: {location}\n\nPlay Synopsis:\n{synopsis}\nReview from a New York Times play critic of the above play:\n{review}\n\nSocial Media Post:"
+            {
+                "llm": {
+                    "args": {
+                        "temperature": 0.7
+                    },
+                    "type": "openai"
+                },
+                "output_key": "social_post_text",
+                "prompt": {
+                    "input_variables": [
+                        "synopsis",
+                        "review",
+                        "time",
+                        "location"
+                    ],
+                    "template": "You are a social media manager for a theater company.  Given the title of play, the era it is set in, the date,time and location, the synopsis of the play, and the review of the play, it is your job to write a social media post for that play.\n\nHere is some context about the time and location of the play:\nDate and Time: {time}\nLocation: {location}\n\nPlay Synopsis:\n{synopsis}\nReview from a New York Times play critic of the above play:\n{review}\n\nSocial Media Post:"
+                },
+                "type": "LLMChain"
+            }
+        ],
+        "input_variables": [
+            "era",
+            "title"
+        ],
+        "memory": {
+            "memories": {
+                "location": "Theater in the Park",
+                "time": "December 25th, 8pm PST"
             },
-            "type": "LLMChain"
-        }
-    ],
-    "input_variables": [
-        "era",
-        "title"
-    ],
-    "memory": {
-        "memories": {
-            "location": "Theater in the Park",
-            "time": "December 25th, 8pm PST"
+            "type": "SimpleMemory"
         },
-        "type": "SimpleMemory"
+        "output_variables": [
+            "social_post_text"
+        ],
+        "type": "SequentialChain"
     },
-    "output_variables": [
-        "social_post_text"
-    ],
-    "type": "SequentialChain"
+    "description": "An example sequential chain with simple memory.",
+    "name": "Sequential Chain with Simple Memory",
+    "template_version": "0.0.5"
 }
```

### Comparing `langchain_interpreter-0.0.4/src/json/simple_seq_chain.json` & `langchain_interpreter-0.0.5/src/json/simple_seq_chain.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('name', 'Simple Sequential Chain'), ('description', 'An example simple "*

 * *            "sequential chain'), ('template_version', '0.0.5'), ('chain', OrderedDict([('type', "*

 * *            "'SimpleSequentialChain'), ('chains', [OrderedDict([('type', 'LLMChain'), ('llm', "*

 * *            "OrderedDict([('type', 'openai'), ('args', OrderedDict([('temperature', 0)]))])), "*

 * *            "('prompt', OrderedDict([('template', 'You are a playwright. Given the title of play, "*

 * *            'it is you […]*

```diff
@@ -1,35 +1,40 @@
 {
-    "chains": [
-        {
-            "llm": {
-                "args": {
-                    "temperature": 0
+    "chain": {
+        "chains": [
+            {
+                "llm": {
+                    "args": {
+                        "temperature": 0
+                    },
+                    "type": "openai"
                 },
-                "name": "openai"
-            },
-            "prompt": {
-                "input_variables": [
-                    "title"
-                ],
-                "template": "You are a playwright. Given the title of play, it is your job to write a synopsis for that title. \n\nTitle: {title}\nPlaywright: This is a synopsis for the above play:"
-            },
-            "type": "LLMChain"
-        },
-        {
-            "llm": {
-                "args": {
-                    "temperature": 0
+                "prompt": {
+                    "input_variables": [
+                        "title"
+                    ],
+                    "template": "You are a playwright. Given the title of play, it is your job to write a synopsis for that title. \n\nTitle: {title}\nPlaywright: This is a synopsis for the above play:"
                 },
-                "name": "openai"
-            },
-            "prompt": {
-                "input_variables": [
-                    "synopsis"
-                ],
-                "template": "You are a play critic from the New York Times. Given the synopsis of play, it is your job to write a review for that play.\n\nPlay Synopsis:\n{synopsis}\nReview from a New York Times play critic of the above play:"
+                "type": "LLMChain"
             },
-            "type": "LLMChain"
-        }
-    ],
-    "type": "SimpleSequentialChain"
+            {
+                "llm": {
+                    "args": {
+                        "temperature": 0
+                    },
+                    "type": "openai"
+                },
+                "prompt": {
+                    "input_variables": [
+                        "synopsis"
+                    ],
+                    "template": "You are a play critic from the New York Times. Given the synopsis of play, it is your job to write a review for that play.\n\nPlay Synopsis:\n{synopsis}\nReview from a New York Times play critic of the above play:"
+                },
+                "type": "LLMChain"
+            }
+        ],
+        "type": "SimpleSequentialChain"
+    },
+    "description": "An example simple sequential chain",
+    "name": "Simple Sequential Chain",
+    "template_version": "0.0.5"
 }
```

### Comparing `langchain_interpreter-0.0.4/src/langchain_interpreter/main.py` & `langchain_interpreter-0.0.5/src/langchain_interpreter/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,50 @@
     SimpleSequentialChain,
     SequentialChain,
     ConversationChain,
 )
 from langchain import PromptTemplate, OpenAI, LLMChain
 from langchain.memory import SimpleMemory, ConversationBufferMemory
 from langchain.llms import type_to_cls_dict
+from langchain_interpreter import validate_chain
 import json
 
 
 def chain_from_file(filename, **kwargs):
+    """Generate a LangChain Chain from a json file.
+
+    Args:
+        filename (str): the path to the file containing json template.
+
+    Returns:
+        chain: the chain specified by the json template.
+
+    Raises:
+        ValidationError:
+    """
+
     with open(filename) as f:
         cfg = json.load(f)
+    validate_chain(cfg)
     return get_chain(cfg, **kwargs)
 
 
 def chain_from_str(s, **kwargs):
-    return get_chain(json.loads(s), **kwargs)
+    """Generate a LangChain Chain from a json string.
+
+    Args:
+        s (str): the json string to turn into a chain
+
+    Returns:
+        chain: the chain specified by the json template.
+    """
+
+    cfg = json.loads(s)
+    validate_chain(cfg)
+    return get_chain(cfg, **kwargs)
 
 
 def get_chain(cfg, **kwargs):
     if cfg["type"] == "LLMChain":
         return get_llm_chain(cfg, **kwargs)
     if cfg["type"] == "SimpleSequentialChain":
         return get_simple_sequential_chain(cfg, **kwargs)
@@ -36,15 +61,16 @@
     memory = try_memory(cfg, **kwargs)
 
     conv_chain = ConversationChain(llm=llm, memory=memory)
     return conv_chain
 
 
 def get_llm(cfg, **kwargs):
-    llm_type = type_to_cls_dict[cfg["name"]]
+    # TODO: restrict types you can use
+    llm_type = type_to_cls_dict[cfg["type"]]
     llm = llm_type(**cfg["args"], openai_api_key=kwargs.get("openai_api_key"))
     return llm
 
 
 def get_llm_chain(cfg, **kwargs):
     llm = get_llm(cfg["llm"], **kwargs)
     prompt = get_prompt(cfg["prompt"])
```

### Comparing `langchain_interpreter-0.0.4/.gitignore` & `langchain_interpreter-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.4/LICENSE` & `langchain_interpreter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.4/pyproject.toml` & `langchain_interpreter-0.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "langchain_interpreter"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Elijah Tarr", email="elijahotarr@gmail.com" },
 ]
 description = "A way to turn json into langchain pipelines."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

