# Comparing `tmp/jax_lorax-0.1.2.tar.gz` & `tmp/jax_lorax-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_lorax-0.1.2.tar", max compression
+gzip compressed data, was "jax_lorax-0.2.0.tar", max compression
```

## Comparing `jax_lorax-0.1.2.tar` & `jax_lorax-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-03 04:00:32.027251 jax_lorax-0.1.2/LICENSE
--rw-r--r--   0        0        0     4396 2023-05-11 00:46:40.640430 jax_lorax-0.1.2/README.md
--rw-r--r--   0        0        0      132 2023-05-03 18:07:36.010823 jax_lorax-0.1.2/lorax/__init__.py
--rw-r--r--   0        0        0       31 2023-05-03 17:53:42.180819 jax_lorax-0.1.2/lorax/constants.py
--rw-r--r--   0        0        0     3466 2023-05-11 01:02:48.523768 jax_lorax-0.1.2/lorax/helpers.py
--rw-r--r--   0        0        0    10227 2023-05-08 20:14:22.096215 jax_lorax-0.1.2/lorax/transform.py
--rw-r--r--   0        0        0      479 2023-05-11 01:03:14.837101 jax_lorax-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 jax_lorax-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-03 04:00:32.027251 jax_lorax-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4464 2023-07-07 07:43:58.835320 jax_lorax-0.2.0/README.md
+-rw-r--r--   0        0        0      179 2023-07-03 05:29:09.277002 jax_lorax-0.2.0/lorax/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-03 17:53:42.180819 jax_lorax-0.2.0/lorax/constants.py
+-rw-r--r--   0        0        0     4365 2023-07-03 05:27:41.840335 jax_lorax-0.2.0/lorax/helpers.py
+-rw-r--r--   0        0        0     5399 2023-07-03 06:02:35.663678 jax_lorax-0.2.0/lorax/transform.py
+-rw-r--r--   0        0        0      494 2023-07-07 07:42:39.355320 jax_lorax-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5144 1970-01-01 00:00:00.000000 jax_lorax-0.2.0/PKG-INFO
```

### Comparing `jax_lorax-0.1.2/LICENSE` & `jax_lorax-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_lorax-0.1.2/PKG-INFO` & `jax_lorax-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,24 @@
-Metadata-Version: 2.1
-Name: jax-lorax
-Version: 0.1.2
-Summary: A JAX transform which applies LoRA to arbitrary JAX functions/models
-License: MIT
-Author: Davis Yoshida
-Author-email: dyoshida@ttic.edu
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: jax (>=0.4.6,<0.5.0)
-Requires-Dist: jaxlib (>=0.4.6,<0.5.0)
-Description-Content-Type: text/markdown
-
 # Lorax: LoRA for JAX functions
 This is a JAX transform which implements [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685). LoRA replaces operations like `Wx` with `(W + BA)x` where `A` and `B` are skinny rectangular matrices. You can then train only `A` and `B`, and leave `W` frozen, which dramatically reduces the amount of memory needed for things like optimizer states.
 
 Lorax should work on most JAX models. I did my testing with my models which use Haiku, and you can find an example of applying it to a HuggingFace Flax model in the [examples directory(examples/).
 
 ## Installation 
 
 ```bash
 pip install jax-lorax
 ```
 
+## Changelog
+
+### 0.2.0
+* Replaced backend with [Qax](https://github.com/davisyoshida/qax)
+* Overhauled API to simplify usage (No more need to separately handle frozen/tunable params)
+
 ### Running tests
 Install dev dependencies:
 ```bash
 git clone https://github.com/davisyoshida/lorax.git
 cd lorax
 pip install poetry
 poetry install
@@ -41,14 +29,15 @@
 pytest tests.py
 ```
 
 ## Minimal example
 Lorax makes it so you can take model code which wasn't written with LoRA in mind, and transform it so that it does! For example, consider the following MLP code:
 
 ```python
+
 import jax
 import jax.numpy as jnp
 
 import optax
 
 def model(params, x):
     """My model, written in the dark ages before LoRA, using gratuitous amounts of VRAM when trained"""
@@ -58,67 +47,69 @@
 
 dim = 5000
 
 # Initialize about 3 GB of params
 params = [jax.random.normal(jax.random.PRNGKey(i), (dim, dim)) / (dim ** 0.5) for i in range(30)]
 optimizer = optax.adam(learning_rate=3e-4)
 
+# OOM on 7GB GPU :(
 opt_state = optimizer.init(params)
-# OOM on 7 GB GPU :(
 ```
 
 The optimizer states are way too expensive, but applying Lorax lets you just train two `5000 x 64` matrices for each original weight.
 
 First import lorax and transform your model:
 ```python
-from lorax import lora
-lora_model = lora(model)
+import lorax
+
+# Transform the model code
+lora_model = lorax.lora(model)
 ```
 
 Next initialize the new LoRA parameters:
 ```python
-from lorax import init_lora
-
-# Tell LoRA what what you want the inner dimension of B and A to be for each parameter
+# Tell LoRA what to use as the small dimension of B and A
 rank_constraint = 64
 lora_spec = [rank_constraint for param in params]
 
 # Initialize a set of LoRA factors for each parameter
-frozen_params, tunable_params = init_lora(param_tree=params, spec=lora_spec, rng=jax.random.PRNGKey(0))
+lora_params = lorax.init_lora(param_tree=params, spec=lora_spec, rng=jax.random.PRNGKey(0))
+
+# The transformed model has the same call signature, but it can now handle parameters
+# of type lorax.LoraWeight
+lora_model(lora_params, jnp.ones((dim,)))
+
+# Wrap the optimizer so it will freeze parameters not marked as trainable by the spec
+optimizer = lorax.wrap_optimizer(optimizer, lora_spec)
+
+# Now the optimizer can be used just like normal
+opt_state = optimizer.init(lora_params)
 
-# The transformed model takes this tuple in place of the original params
-lora_model((frozen_params, tunable_params), jnp.ones((dim,)))
 ```
 
-That's it for the Lorax specific stuff. Training is just just like normal JAX training, but make sure to take your gradients with respect to `tunable_params` only
+That's it for the Lorax specific stuff. The wrapped `lora_model` function is just an ordinary
+JAX function, and the LoraWeight instances a pytrees.
 ```python
-# Define a loss function so we can differentiate with respect to only the tunable params
-def loss_fn(tunable_params, frozen_params, x):
-    combined_params = (frozen_params, tunable_params)
-    return lora_model(combined_params, x)
-
-# Standard taining setup
+# Normal update function:
 @jax.jit
-def update_fn(frozen_params, tunable_params, opt_state, x):
-    grad_fn = jax.value_and_grad(loss_fn)
-    loss, grad = grad_fn(tunable_params, frozen_params, x)
+def update_fn(lora_params, opt_state, x):
+    grad_fn = jax.value_and_grad(lora_model)
+    loss, grad = grad_fn(lora_params, x)
 
-    updates, new_opt_state = optimizer.update(grad, opt_state)
-    updated_params = optax.apply_updates(tunable_params, updates)
+    updates, new_opt_state = optimizer.update(grad, opt_state, params=lora_params)
+    updated_params = optax.apply_updates(lora_params, updates)
     return loss, new_opt_state, updated_params
-    
-opt_state = optimizer.init(tunable_params)
 ```
 
 Now for some dummy data and the training loop:
 ```python
 x = jax.random.normal(jax.random.PRNGKey(0), (dim,))
 for i in range(10):
-    loss, opt_state, tunable_params = update_fn(frozen_params, tunable_params, opt_state, x)
-    print(f'Step: {i} loss: {loss:.4e}')
+    loss, opt_state, lora_params = update_fn(lora_params, opt_state, x)
+    print(f'Step: {i} loss: {loss:.4e}') # Number goes down!
 # Step: 0 loss: 6.6614e-02
 # Step: 1 loss: 4.4402e-02
 # Step: 2 loss: 3.0241e-02
 # Step: 3 loss: 1.8457e-02
 # Step: 4 loss: 1.2326e-02
 # Step: 5 loss: 8.8878e-03
 # Step: 6 loss: 6.0599e-03
@@ -128,17 +119,16 @@
 ```
 
 Number goes down! We can now merge the trained LoRA params with the frozen params, and use them with the unmodified model:
 ```python
 lora_output = lora_model((frozen_params, tunable_params), x)
 
 # Now we merge the params to get params usable in the original model
-merged_params = merge_params(frozen_params, tunable_params)
+merged_params = lorax.merge_params(lora_params)
 orig_model_output = model(merged_params, x)
 
 # Verify that the model outputs are the same
 print(f'Difference between split and merged outputs: {orig_model_output - lora_output:.3e}')
 # Difference between split and merged params: 1.164e-10
 ```
 
 See [examples/huggingface_gpt2.py](examples/huggingface_gpt2.py) for an example applying Lorax to a realistic model.
-
```

