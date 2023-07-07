# Comparing `tmp/django-reactor-5.0.1b0.tar.gz` & `tmp/django-reactor-5.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-reactor-5.0.1b0.tar", last modified: Tue Jun 13 10:49:38 2023, max compression
+gzip compressed data, was "django-reactor-5.0.2b0.tar", last modified: Fri Jul  7 13:09:24 2023, max compression
```

## Comparing `django-reactor-5.0.1b0.tar` & `django-reactor-5.0.2b0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.695759 django-reactor-5.0.1b0/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)       65 2023-06-13 10:33:48.000000 django-reactor-5.0.1b0/MANIFEST.in
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16764 2023-06-13 10:49:38.695759 django-reactor-5.0.1b0/PKG-INFO
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    15905 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/README.md
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.692425 django-reactor-5.0.1b0/django_reactor.egg-info/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16764 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/django_reactor.egg-info/PKG-INFO
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      800 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/django_reactor.egg-info/SOURCES.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/django_reactor.egg-info/dependency_links.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-01 11:50:12.000000 django-reactor-5.0.1b0/django_reactor.egg-info/not-zip-safe
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      180 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/django_reactor.egg-info/requires.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        8 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/django_reactor.egg-info/top_level.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      451 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/pyproject.toml
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.692425 django-reactor-5.0.1b0/reactor/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2023-05-31 13:32:27.000000 django-reactor-5.0.1b0/reactor/__init__.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      291 2023-06-06 12:12:16.000000 django-reactor-5.0.1b0/reactor/apps.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     5661 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/auto_broadcast.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    13782 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/component.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     6125 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/consumer.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3990 2023-06-12 07:48:44.000000 django-reactor-5.0.1b0/reactor/event_transpiler.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      411 2023-05-31 13:32:27.000000 django-reactor-5.0.1b0/reactor/log.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3045 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/repository.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      874 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/schemas.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      765 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/serializer.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      590 2023-06-12 07:48:55.000000 django-reactor-5.0.1b0/reactor/settings.py
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.692425 django-reactor-5.0.1b0/reactor/static/
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.692425 django-reactor-5.0.1b0/reactor/static/reactor/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     4596 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/static/reactor/reactor-boost.js
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     9536 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/static/reactor/reactor.js
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    22594 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/reactor/static/reactor/reactor.min.js
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    87150 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/reactor/static/reactor/reactor.min.js.map
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.695759 django-reactor-5.0.1b0/reactor/templates/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      444 2022-07-30 12:06:00.000000 django-reactor-5.0.1b0/reactor/templates/reactor_header.html
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.695759 django-reactor-5.0.1b0/reactor/templatetags/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2022-07-30 12:06:00.000000 django-reactor-5.0.1b0/reactor/templatetags/__init__.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3524 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/templatetags/reactor.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      165 2022-07-30 12:06:00.000000 django-reactor-5.0.1b0/reactor/urls.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     2733 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/utils.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     1336 2023-06-13 10:49:38.695759 django-reactor-5.0.1b0/setup.cfg
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)       39 2023-06-01 09:29:36.000000 django-reactor-5.0.1b0/setup.py
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-07 13:09:24.416265 django-reactor-5.0.2b0/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)       65 2023-06-13 10:33:48.000000 django-reactor-5.0.2b0/MANIFEST.in
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16764 2023-07-07 13:09:24.416265 django-reactor-5.0.2b0/PKG-INFO
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    15905 2023-06-10 22:13:11.000000 django-reactor-5.0.2b0/README.md
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-07 13:09:24.412932 django-reactor-5.0.2b0/django_reactor.egg-info/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16764 2023-07-07 13:09:24.000000 django-reactor-5.0.2b0/django_reactor.egg-info/PKG-INFO
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      800 2023-07-07 13:09:24.000000 django-reactor-5.0.2b0/django_reactor.egg-info/SOURCES.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-07-07 13:09:24.000000 django-reactor-5.0.2b0/django_reactor.egg-info/dependency_links.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-01 11:50:12.000000 django-reactor-5.0.2b0/django_reactor.egg-info/not-zip-safe
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      180 2023-07-07 13:09:24.000000 django-reactor-5.0.2b0/django_reactor.egg-info/requires.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        8 2023-07-07 13:09:24.000000 django-reactor-5.0.2b0/django_reactor.egg-info/top_level.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      451 2023-06-10 22:13:11.000000 django-reactor-5.0.2b0/pyproject.toml
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-07 13:09:24.412932 django-reactor-5.0.2b0/reactor/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2023-05-31 13:32:27.000000 django-reactor-5.0.2b0/reactor/__init__.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      291 2023-06-06 12:12:16.000000 django-reactor-5.0.2b0/reactor/apps.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     5661 2023-06-10 22:13:11.000000 django-reactor-5.0.2b0/reactor/auto_broadcast.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    13782 2023-06-10 22:13:11.000000 django-reactor-5.0.2b0/reactor/component.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     6125 2023-06-10 22:13:11.000000 django-reactor-5.0.2b0/reactor/consumer.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3958 2023-07-07 13:06:43.000000 django-reactor-5.0.2b0/reactor/event_transpiler.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      411 2023-05-31 13:32:27.000000 django-reactor-5.0.2b0/reactor/log.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3045 2023-06-30 14:43:59.000000 django-reactor-5.0.2b0/reactor/repository.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      874 2023-06-10 22:13:11.000000 django-reactor-5.0.2b0/reactor/schemas.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      765 2023-06-30 09:52:16.000000 django-reactor-5.0.2b0/reactor/serializer.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      590 2023-06-12 07:48:55.000000 django-reactor-5.0.2b0/reactor/settings.py
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-07 13:09:24.412932 django-reactor-5.0.2b0/reactor/static/
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-07 13:09:24.416265 django-reactor-5.0.2b0/reactor/static/reactor/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3228 2023-07-07 12:51:54.000000 django-reactor-5.0.2b0/reactor/static/reactor/reactor-boost.js
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     9372 2023-07-07 13:07:27.000000 django-reactor-5.0.2b0/reactor/static/reactor/reactor.js
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    23666 2023-07-07 13:09:24.000000 django-reactor-5.0.2b0/reactor/static/reactor/reactor.min.js
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    94480 2023-07-07 13:09:24.000000 django-reactor-5.0.2b0/reactor/static/reactor/reactor.min.js.map
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-07 13:09:24.416265 django-reactor-5.0.2b0/reactor/templates/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      444 2022-07-30 12:06:00.000000 django-reactor-5.0.2b0/reactor/templates/reactor_header.html
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-07 13:09:24.416265 django-reactor-5.0.2b0/reactor/templatetags/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2022-07-30 12:06:00.000000 django-reactor-5.0.2b0/reactor/templatetags/__init__.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3524 2023-06-10 22:13:11.000000 django-reactor-5.0.2b0/reactor/templatetags/reactor.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      165 2022-07-30 12:06:00.000000 django-reactor-5.0.2b0/reactor/urls.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     2733 2023-06-10 22:13:11.000000 django-reactor-5.0.2b0/reactor/utils.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     1336 2023-07-07 13:09:24.416265 django-reactor-5.0.2b0/setup.cfg
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)       39 2023-06-01 09:29:36.000000 django-reactor-5.0.2b0/setup.py
```

### Comparing `django-reactor-5.0.1b0/PKG-INFO` & `django-reactor-5.0.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reactor
-Version: 5.0.1b0
+Version: 5.0.2b0
 Summary: Brings LiveView from Phoenix framework into Django
 Home-page: https://github.com/edelvalle/reactor
 Author: Eddy Ernesto del Valle Pino
 Author-email: eddy@edelvalle.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-reactor-5.0.1b0/README.md` & `django-reactor-5.0.2b0/README.md`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/django_reactor.egg-info/PKG-INFO` & `django-reactor-5.0.2b0/django_reactor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reactor
-Version: 5.0.1b0
+Version: 5.0.2b0
 Summary: Brings LiveView from Phoenix framework into Django
 Home-page: https://github.com/edelvalle/reactor
 Author: Eddy Ernesto del Valle Pino
 Author-email: eddy@edelvalle.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-reactor-5.0.1b0/django_reactor.egg-info/SOURCES.txt` & `django-reactor-5.0.2b0/django_reactor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/reactor/auto_broadcast.py` & `django-reactor-5.0.2b0/reactor/auto_broadcast.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/reactor/component.py` & `django-reactor-5.0.2b0/reactor/component.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/reactor/consumer.py` & `django-reactor-5.0.2b0/reactor/consumer.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/reactor/event_transpiler.py` & `django-reactor-5.0.2b0/reactor/event_transpiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,17 @@
     def inlinejs(code: str, stack: Stack):
         return code
 
     # Events
 
     @classmethod
     def debounce(cls, code: str, stack: Stack):
-        name = stack.pop()
-        delay = stack.pop()
+        delay = int(stack.pop())
         code = cls._add_curly(code)
-        return f"reactor.debounce('{name}', {delay})(() => {code})()"
+        return f"reactor.debounce({delay})(() => {code})()"
 
     @staticmethod
     def prevent(code: str, stack: Stack):
         return "event.preventDefault(); " + code
 
     @staticmethod
     def stop(code: str, stack: Stack):
```

### Comparing `django-reactor-5.0.1b0/reactor/repository.py` & `django-reactor-5.0.2b0/reactor/repository.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/reactor/schemas.py` & `django-reactor-5.0.2b0/reactor/schemas.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/reactor/serializer.py` & `django-reactor-5.0.2b0/reactor/serializer.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/reactor/settings.py` & `django-reactor-5.0.2b0/reactor/settings.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/reactor/static/reactor/reactor.js` & `django-reactor-5.0.2b0/reactor/static/reactor/reactor.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,7 @@
-import morphdom from "morphdom";
 import ReconnectingWebSocket from "reconnecting-websocket";
 import boost from "./reactor-boost";
 
 // Connection
 
 const parser = new DOMParser();
 
@@ -84,30 +83,36 @@
                 console.log("<<< REMOVE", id);
                 document.getElementById(id)?.remove();
                 break;
             case "focus_on":
                 var {
                     selector
                 } = payload;
-                console.log("<<< FOCUS-ON", `"${selector}"`, document.querySelector(selector));
+                console.log(
+                    "<<< FOCUS-ON",
+                    `"${selector}"`,
+                    document.querySelector(selector)
+                );
                 window.requestAnimationFrame(() =>
-                    document.querySelector(selector)?.focus())
+                    document.querySelector(selector)?.focus()
+                );
                 break;
             case "scroll_into_view":
                 var {
                     id, behavior, block, inline
                 } = payload;
                 window.requestAnimationFrame(() =>
                     document
                     .getElementById(id)
                     ?.scrollIntoView({
                         behavior,
                         block,
                         inline
-                    }))
+                    })
+                );
                 break;
             case "url_change":
                 var {
                     url
                 } = payload;
                 console.log("<< URL", payload.command, url);
                 switch (payload.command) {
@@ -224,33 +229,30 @@
             connection.addEventListener("close", this.wentOffline);
             this.join();
         }
 
         disconnectedCallback() {
             connection.removeEventListener("open", this.joinBind);
             connection.removeEventListener("close", this.wentOffline);
-            connection.sendLeave(this.id);
+            this.leave();
         }
 
         join() {
             this.classList.remove("reactor-disconnected");
             connection.sendJoin(this.dataset.name, this.parentId, this.dataset.state);
         }
 
+        leave() {
+            connection.sendLeave(this.id);
+        }
+
         applyDiff(diff) {
-            let html = this.getHtml(diff);
             window.requestAnimationFrame(() => {
-                morphdom(this, html, {
-                    onBeforeNodeAdded(node) {
-                        boost.boostElement(node);
-                    },
-                    onElUpdated(node) {
-                        boost.boostElement(node);
-                    },
-                });
+                let html = this.getHtml(diff);
+                boost.morph(this, html);
             });
         }
 
         getHtml(diff) {
             let fragments = [];
             let cursor = 0;
             for (let fragment of diff) {
@@ -342,15 +344,15 @@
 
     customElements.define(dataset.tagName, ReactorComponent, {
         extends: dataset.extends,
     });
 }
 
 connection.open();
-debounceTimeouts = {};
+var debounceTimeout = undefined;
 
 window.reactor = {
     /**
      * Forwards a user event to a component
      * @param {HTMLElement} element
      * @param {String} name
      * @param {Object} args
@@ -362,20 +364,19 @@
             let formScope = component.contains(form) ? form : component;
             component.dispatch(name, args, formScope);
         }
     },
 
     /**
      * Debounce a function call
-     * @param {String} delayName
      * @param {Number} delay
      * @returns
      */
-    debounce(delayName, delay) {
+    debounce(delay) {
         return (f) => {
             return (...args) => {
-                clearTimeout(debounceTimeouts[delayName]);
-                debounceTimeouts[delayName] = setTimeout(() => f(...args), delay);
+                clearTimeout(debounceTimeout);
+                debounceTimeout = setTimeout(() => f(...args), delay);
             };
         };
     },
 };
```

### Comparing `django-reactor-5.0.1b0/reactor/static/reactor/reactor.min.js` & `django-reactor-5.0.2b0/reactor/static/reactor/reactor.min.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,386 +1,484 @@
 (() => {
-    var ye = Object.defineProperty;
-    var we = (t, e, n) => e in t ? ye(t, e, {
-        enumerable: !0,
-        configurable: !0,
-        writable: !0,
-        value: n
-    }) : t[e] = n;
-    var H = (t, e, n) => (we(t, typeof e != "symbol" ? e + "" : e, n), n);
-    var oe = 11;
-
-    function Ee(t, e) {
-        var n = e.attributes,
-            i, r, o, a, u;
-        if (!(e.nodeType === oe || t.nodeType === oe)) {
-            for (var d = n.length - 1; d >= 0; d--) i = n[d], r = i.name, o = i.namespaceURI, a = i.value, o ? (r = i.localName || r, u = t.getAttributeNS(o, r), u !== a && (i.prefix === "xmlns" && (r = i.name), t.setAttributeNS(o, r, a))) : (u = t.getAttribute(r), u !== a && t.setAttribute(r, a));
-            for (var m = t.attributes, L = m.length - 1; L >= 0; L--) i = m[L], r = i.name, o = i.namespaceURI, o ? (r = i.localName || r, e.hasAttributeNS(o, r) || t.removeAttributeNS(o, r)) : e.hasAttribute(r) || t.removeAttribute(r)
-        }
-    }
-    var W, Te = "http://www.w3.org/1999/xhtml",
-        _ = typeof document == "undefined" ? void 0 : document,
-        Se = !!_ && "content" in _.createElement("template"),
-        Oe = !!_ && _.createRange && "createContextualFragment" in _.createRange();
-
-    function Ce(t) {
-        var e = _.createElement("template");
-        return e.innerHTML = t, e.content.childNodes[0]
-    }
+    var se = Object.create;
+    var U = Object.defineProperty;
+    var ae = Object.getOwnPropertyDescriptor;
+    var le = Object.getOwnPropertyNames;
+    var ce = Object.getPrototypeOf,
+        ue = Object.prototype.hasOwnProperty;
+    var de = t => U(t, "__esModule", {
+        value: !0
+    });
+    var fe = (t, e) => () => (e || t((e = {
+        exports: {}
+    }).exports, e), e.exports);
+    var he = (t, e, i) => {
+            if (e && typeof e == "object" || typeof e == "function")
+                for (let a of le(e)) !ue.call(t, a) && a !== "default" && U(t, a, {
+                    get: () => e[a],
+                    enumerable: !(i = ae(e, a)) || i.enumerable
+                });
+            return t
+        },
+        pe = t => he(de(U(t != null ? se(ce(t)) : {}, "default", t && t.__esModule && "default" in t ? {
+            get: () => t.default,
+            enumerable: !0
+        } : {
+            value: t,
+            enumerable: !0
+        })), t);
+    var Y = fe(z => {
+        (function(t, e) {
+            typeof define == "function" && define.amd ? define([], e) : t.Idiomorph = t.Idiomorph || e()
+        })(typeof self != "undefined" ? self : z, function() {
+            return function() {
+                "use strict";
+                let t = new Set;
+
+                function e(n, r, o = {}) {
+                    n instanceof Document && (n = n.documentElement), typeof r == "string" && (r = H(r));
+                    let l = E(r),
+                        c = D(n, l, o);
+                    return i(n, l, c)
+                }
+
+                function i(n, r, o) {
+                    if (o.head.block) {
+                        let l = n.querySelector("head"),
+                            c = r.querySelector("head");
+                        if (l && c) {
+                            let u = p(c, l, o);
+                            Promise.all(u).then(function() {
+                                i(n, r, Object.assign(o, {
+                                    head: {
+                                        block: !1,
+                                        ignore: !0
+                                    }
+                                }))
+                            });
+                            return
+                        }
+                    }
+                    if (o.morphStyle === "innerHTML") return s(r, n, o), n.children;
+                    if (o.morphStyle === "outerHTML" || o.morphStyle == null) {
+                        let l = T(r, n, o),
+                            c = l?.previousSibling,
+                            u = l?.nextSibling,
+                            m = a(n, l, o);
+                        return l ? C(c, m, u) : []
+                    } else throw "Do not understand how to morph style " + o.morphStyle
+                }
+
+                function a(n, r, o) {
+                    if (!(o.ignoreActive && n === document.activeElement)) return r == null ? (o.callbacks.beforeNodeRemoved(n), n.remove(), o.callbacks.afterNodeRemoved(n), null) : v(n, r) ? (o.callbacks.beforeNodeMorphed(n, r), n instanceof HTMLHeadElement && o.head.ignore || (n instanceof HTMLHeadElement && o.head.style !== "morph" ? p(r, n, o) : (d(r, n), s(r, n, o))), o.callbacks.afterNodeMorphed(n, r), n) : (o.callbacks.beforeNodeRemoved(n), o.callbacks.beforeNodeAdded(r), n.parentElement.replaceChild(r, n), o.callbacks.afterNodeAdded(r), o.callbacks.afterNodeRemoved(n), r)
+                }
+
+                function s(n, r, o) {
+                    let l = n.firstChild,
+                        c = r.firstChild;
+                    for (; l;) {
+                        let u = l;
+                        if (l = u.nextSibling, c == null) o.callbacks.beforeNodeAdded(u), r.appendChild(u), o.callbacks.afterNodeAdded(u);
+                        else if (R(u, c, o)) a(c, u, o), c = c.nextSibling;
+                        else {
+                            let m = I(n, r, u, c, o);
+                            if (m) c = O(c, m, o), a(m, u, o);
+                            else {
+                                let b = P(n, r, u, c, o);
+                                b ? (c = O(c, b, o), a(b, u, o)) : (o.callbacks.beforeNodeAdded(u), r.insertBefore(u, c), o.callbacks.afterNodeAdded(u))
+                            }
+                        }
+                        j(o, u)
+                    }
+                    for (; c !== null;) {
+                        let u = c;
+                        c = c.nextSibling, J(u, o)
+                    }
+                }
 
-    function Le(t) {
-        W || (W = _.createRange(), W.selectNode(_.body));
-        var e = W.createContextualFragment(t);
-        return e.childNodes[0]
-    }
+                function d(n, r) {
+                    let o = n.nodeType;
+                    if (o === 1) {
+                        let l = n.attributes,
+                            c = r.attributes;
+                        for (let u of l) r.getAttribute(u.name) !== u.value && r.setAttribute(u.name, u.value);
+                        for (let u of c) n.hasAttribute(u.name) || r.removeAttribute(u.name)
+                    }
+                    if ((o === 8 || o === 3) && r.nodeValue !== n.nodeValue && (r.nodeValue = n.nodeValue), n instanceof HTMLInputElement && r instanceof HTMLInputElement && n.type !== "file") {
+                        let l = n.value,
+                            c = r.value;
+                        f(n, r, "checked"), f(n, r, "disabled"), n.hasAttribute("value") ? l !== c && (r.setAttribute("value", l), r.value = l) : (r.value = "", r.removeAttribute("value"))
+                    } else if (n instanceof HTMLOptionElement) f(n, r, "selected");
+                    else if (n instanceof HTMLTextAreaElement && r instanceof HTMLTextAreaElement) {
+                        let l = n.value,
+                            c = r.value;
+                        l !== c && (r.value = l), r.firstChild && r.firstChild.nodeValue !== l && (r.firstChild.nodeValue = l)
+                    }
+                }
 
-    function Ae(t) {
-        var e = _.createElement("body");
-        return e.innerHTML = t, e.childNodes[0]
-    }
+                function f(n, r, o) {
+                    n[o] !== r[o] && (r[o] = n[o], n[o] ? r.setAttribute(o, "") : r.removeAttribute(o))
+                }
+
+                function p(n, r, o) {
+                    let l = [],
+                        c = [],
+                        u = [],
+                        m = [],
+                        b = o.head.style,
+                        S = new Map;
+                    for (let _ of n.children) S.set(_.outerHTML, _);
+                    for (let _ of r.children) {
+                        let g = S.has(_.outerHTML),
+                            A = o.head.shouldReAppend(_),
+                            B = o.head.shouldPreserve(_);
+                        g || B ? A ? c.push(_) : (S.delete(_.outerHTML), u.push(_)) : b === "append" ? A && (c.push(_), m.push(_)) : o.head.shouldRemove(_) !== !1 && c.push(_)
+                    }
+                    m.push(...S.values()), h("to append: ", m);
+                    let x = [];
+                    for (let _ of m) {
+                        h("adding: ", _);
+                        let g = document.createRange().createContextualFragment(_.outerHTML).firstChild;
+                        if (h(g), o.callbacks.beforeNodeAdded(g) !== !1) {
+                            if (g.href || g.src) {
+                                let A = null,
+                                    B = new Promise(function(ie) {
+                                        A = ie
+                                    });
+                                g.addEventListener("load", function() {
+                                    A()
+                                }), x.push(B)
+                            }
+                            r.appendChild(g), o.callbacks.afterNodeAdded(g), l.push(g)
+                        }
+                    }
+                    for (let _ of c) o.callbacks.beforeNodeRemoved(_) !== !1 && (r.removeChild(_), o.callbacks.afterNodeRemoved(_));
+                    return o.head.afterHeadMorphed(r, {
+                        added: l,
+                        kept: u,
+                        removed: c
+                    }), x
+                }
+
+                function h() {}
+
+                function y() {}
+
+                function D(n, r, o) {
+                    return {
+                        target: n,
+                        newContent: r,
+                        config: o,
+                        morphStyle: o.morphStyle,
+                        ignoreActive: o.ignoreActive,
+                        idMap: oe(n, r),
+                        deadIds: new Set,
+                        callbacks: Object.assign({
+                            beforeNodeAdded: y,
+                            afterNodeAdded: y,
+                            beforeNodeMorphed: y,
+                            afterNodeMorphed: y,
+                            beforeNodeRemoved: y,
+                            afterNodeRemoved: y
+                        }, o.callbacks),
+                        head: Object.assign({
+                            style: "merge",
+                            shouldPreserve: function(l) {
+                                return l.getAttribute("im-preserve") === "true"
+                            },
+                            shouldReAppend: function(l) {
+                                return l.getAttribute("im-re-append") === "true"
+                            },
+                            shouldRemove: y,
+                            afterHeadMorphed: y
+                        }, o.head)
+                    }
+                }
+
+                function R(n, r, o) {
+                    return n == null || r == null ? !1 : n.nodeType === r.nodeType && n.tagName === r.tagName ? n.id !== "" && n.id === r.id ? !0 : M(o, n, r) > 0 : !1
+                }
+
+                function v(n, r) {
+                    return n == null || r == null ? !1 : n.nodeType === r.nodeType && n.tagName === r.tagName
+                }
+
+                function O(n, r, o) {
+                    for (; n !== r;) {
+                        let l = n;
+                        n = n.nextSibling, J(l, o)
+                    }
+                    return j(o, r), r.nextSibling
+                }
+
+                function I(n, r, o, l, c) {
+                    let u = M(c, o, r),
+                        m = null;
+                    if (u > 0) {
+                        let b = l,
+                            S = 0;
+                        for (; b != null;) {
+                            if (R(o, b, c)) return b;
+                            if (S += M(c, b, n), S > u) return null;
+                            b = b.nextSibling
+                        }
+                    }
+                    return m
+                }
 
-    function Ne(t) {
-        return t = t.trim(), Se ? Ce(t) : Oe ? Le(t) : Ae(t)
-    }
+                function P(n, r, o, l, c) {
+                    let u = l,
+                        m = o.nextSibling,
+                        b = 0;
+                    for (; u != null;) {
+                        if (M(c, u, n) > 0) return null;
+                        if (v(o, u)) return u;
+                        if (v(m, u) && (b++, m = m.nextSibling, b >= 2)) return null;
+                        u = u.nextSibling
+                    }
+                    return u
+                }
+
+                function H(n) {
+                    let r = new DOMParser,
+                        o = n.replace(/<svg(\s[^>]*>|>)([\s\S]*?)<\/svg>/gim, "");
+                    if (o.match(/<\/html>/) || o.match(/<\/head>/) || o.match(/<\/body>/)) {
+                        let l = r.parseFromString(n, "text/html");
+                        if (o.match(/<\/html>/)) return l.generatedByIdiomorph = !0, l; {
+                            let c = l.firstChild;
+                            return c ? (c.generatedByIdiomorph = !0, c) : null
+                        }
+                    } else {
+                        let c = r.parseFromString("<body><template>" + n + "</template></body>", "text/html").body.querySelector("template").content;
+                        return c.generatedByIdiomorph = !0, c
+                    }
+                }
 
-    function V(t, e) {
-        var n = t.nodeName,
-            i = e.nodeName,
-            r, o;
-        return n === i ? !0 : (r = n.charCodeAt(0), o = i.charCodeAt(0), r <= 90 && o >= 97 ? n === i.toUpperCase() : o <= 90 && r >= 97 ? i === n.toUpperCase() : !1)
-    }
+                function E(n) {
+                    if (n == null) return document.createElement("div");
+                    if (n.generatedByIdiomorph) return n;
+                    if (n instanceof Node) {
+                        let r = document.createElement("div");
+                        return r.append(n), r
+                    } else {
+                        let r = document.createElement("div");
+                        for (let o of [...n]) r.append(o);
+                        return r
+                    }
+                }
 
-    function ke(t, e) {
-        return !e || e === Te ? _.createElement(t) : _.createElementNS(e, t)
-    }
+                function C(n, r, o) {
+                    let l = [],
+                        c = [];
+                    for (; n != null;) l.push(n), n = n.previousSibling;
+                    for (; l.length > 0;) {
+                        let u = l.pop();
+                        c.push(u), r.parentElement.insertBefore(u, r)
+                    }
+                    for (c.push(r); o != null;) l.push(o), c.push(o), o = o.nextSibling;
+                    for (; l.length > 0;) r.parentElement.insertBefore(l.pop(), r.nextSibling);
+                    return c
+                }
 
-    function Re(t, e) {
-        for (var n = t.firstChild; n;) {
-            var i = n.nextSibling;
-            e.appendChild(n), n = i
-        }
-        return e
-    }
+                function T(n, r, o) {
+                    let l;
+                    l = n.firstChild;
+                    let c = l,
+                        u = 0;
+                    for (; l;) {
+                        let m = N(l, r, o);
+                        m > u && (c = l, u = m), l = l.nextSibling
+                    }
+                    return c
+                }
 
-    function Y(t, e, n) {
-        t[n] !== e[n] && (t[n] = e[n], t[n] ? t.setAttribute(n, "") : t.removeAttribute(n))
-    }
-    var ae = {
-            OPTION: function(t, e) {
-                var n = t.parentNode;
-                if (n) {
-                    var i = n.nodeName.toUpperCase();
-                    i === "OPTGROUP" && (n = n.parentNode, i = n && n.nodeName.toUpperCase()), i === "SELECT" && !n.hasAttribute("multiple") && (t.hasAttribute("selected") && !e.selected && (t.setAttribute("selected", "selected"), t.removeAttribute("selected")), n.selectedIndex = -1)
-                }
-                Y(t, e, "selected")
-            },
-            INPUT: function(t, e) {
-                Y(t, e, "checked"), Y(t, e, "disabled"), t.value !== e.value && (t.value = e.value), e.hasAttribute("value") || t.removeAttribute("value")
-            },
-            TEXTAREA: function(t, e) {
-                var n = e.value;
-                t.value !== n && (t.value = n);
-                var i = t.firstChild;
-                if (i) {
-                    var r = i.nodeValue;
-                    if (r == n || !n && r == t.placeholder) return;
-                    i.nodeValue = n
-                }
-            },
-            SELECT: function(t, e) {
-                if (!e.hasAttribute("multiple")) {
-                    for (var n = -1, i = 0, r = t.firstChild, o, a; r;)
-                        if (a = r.nodeName && r.nodeName.toUpperCase(), a === "OPTGROUP") o = r, r = o.firstChild;
-                        else {
-                            if (a === "OPTION") {
-                                if (r.hasAttribute("selected")) {
-                                    n = i;
-                                    break
-                                }
-                                i++
-                            }
-                            r = r.nextSibling, !r && o && (r = o.nextSibling, o = null)
-                        } t.selectedIndex = n
+                function N(n, r, o) {
+                    return v(n, r) ? .5 + M(o, n, r) : 0
                 }
-            }
-        },
-        U = 1,
-        se = 11,
-        ce = 3,
-        le = 8;
 
-    function S() {}
+                function J(n, r) {
+                    j(r, n), r.callbacks.beforeNodeRemoved(n), n.remove(), r.callbacks.afterNodeRemoved(n)
+                }
 
-    function xe(t) {
-        if (t) return t.getAttribute && t.getAttribute("id") || t.id
-    }
+                function ne(n, r) {
+                    return !n.deadIds.has(r)
+                }
 
-    function Pe(t) {
-        return function(n, i, r) {
-            if (r || (r = {}), typeof i == "string")
-                if (n.nodeName === "#document" || n.nodeName === "HTML" || n.nodeName === "BODY") {
-                    var o = i;
-                    i = _.createElement("html"), i.innerHTML = o
-                } else i = Ne(i);
-            else i.nodeType === se && (i = i.firstElementChild);
-            var a = r.getNodeKey || xe,
-                u = r.onBeforeNodeAdded || S,
-                d = r.onNodeAdded || S,
-                m = r.onBeforeElUpdated || S,
-                L = r.onElUpdated || S,
-                $ = r.onBeforeNodeDiscarded || S,
-                g = r.onNodeDiscarded || S,
-                M = r.onBeforeElChildrenUpdated || S,
-                j = r.skipFromChildren || S,
-                P = r.addChild || function(c, s) {
-                    return c.appendChild(s)
-                },
-                k = r.childrenOnly === !0,
-                v = Object.create(null),
-                y = [];
-
-            function b(c) {
-                y.push(c)
-            }
-
-            function D(c, s) {
-                if (c.nodeType === U)
-                    for (var h = c.firstChild; h;) {
-                        var l = void 0;
-                        s && (l = a(h)) ? b(l) : (g(h), h.firstChild && D(h, s)), h = h.nextSibling
-                    }
-            }
-
-            function I(c, s, h) {
-                $(c) !== !1 && (s && s.removeChild(c), g(c), D(c, h))
-            }
-
-            function ne(c) {
-                if (c.nodeType === U || c.nodeType === se)
-                    for (var s = c.firstChild; s;) {
-                        var h = a(s);
-                        h && (v[h] = s), ne(s), s = s.nextSibling
-                    }
-            }
-            ne(n);
-
-            function Q(c) {
-                d(c);
-                for (var s = c.firstChild; s;) {
-                    var h = s.nextSibling,
-                        l = a(s);
-                    if (l) {
-                        var f = v[l];
-                        f && V(s, f) ? (s.parentNode.replaceChild(f, s), B(f, s)) : Q(s)
-                    } else Q(s);
-                    s = h
-                }
-            }
-
-            function me(c, s, h) {
-                for (; s;) {
-                    var l = s.nextSibling;
-                    (h = a(s)) ? b(h): I(s, c, !0), s = l
-                }
-            }
-
-            function B(c, s, h) {
-                var l = a(s);
-                l && delete v[l], !(!h && (m(c, s) === !1 || (t(c, s), L(c), M(c, s) === !1))) && (c.nodeName !== "TEXTAREA" ? ge(c, s) : ae.TEXTAREA(c, s))
-            }
-
-            function ge(c, s) {
-                var h = j(c),
-                    l = s.firstChild,
-                    f = c.firstChild,
-                    R, w, x, G, E;
-                e: for (; l;) {
-                    for (G = l.nextSibling, R = a(l); !h && f;) {
-                        if (x = f.nextSibling, l.isSameNode && l.isSameNode(f)) {
-                            l = G, f = x;
-                            continue e
-                        }
-                        w = a(f);
-                        var q = f.nodeType,
-                            T = void 0;
-                        if (q === l.nodeType && (q === U ? (R ? R !== w && ((E = v[R]) ? x === E ? T = !1 : (c.insertBefore(E, f), w ? b(w) : I(f, c, !0), f = E) : T = !1) : w && (T = !1), T = T !== !1 && V(f, l), T && B(f, l)) : (q === ce || q == le) && (T = !0, f.nodeValue !== l.nodeValue && (f.nodeValue = l.nodeValue))), T) {
-                            l = G, f = x;
-                            continue e
+                function re(n, r, o) {
+                    return (n.idMap.get(o) || t).has(r)
+                }
+
+                function j(n, r) {
+                    let o = n.idMap.get(r) || t;
+                    for (let l of o) n.deadIds.add(l)
+                }
+
+                function M(n, r, o) {
+                    let l = n.idMap.get(r) || t,
+                        c = 0;
+                    for (let u of l) ne(n, u) && re(n, u, o) && ++c;
+                    return c
+                }
+
+                function $(n, r) {
+                    let o = n.parentElement,
+                        l = n.querySelectorAll("[id]");
+                    for (let c of l) {
+                        let u = c;
+                        for (; u !== o && u != null;) {
+                            let m = r.get(u);
+                            m == null && (m = new Set, r.set(u, m)), m.add(c.id), u = u.parentElement
                         }
-                        w ? b(w) : I(f, c, !0), f = x
-                    }
-                    if (R && (E = v[R]) && V(E, l)) h || P(c, E), B(E, l);
-                    else {
-                        var X = u(l);
-                        X !== !1 && (X && (l = X), l.actualize && (l = l.actualize(c.ownerDocument || _)), P(c, l), Q(l))
-                    }
-                    l = G, f = x
-                }
-                me(c, f, w);
-                var ie = ae[c.nodeName];
-                ie && ie(c, s)
-            }
-            var p = n,
-                F = p.nodeType,
-                re = i.nodeType;
-            if (!k) {
-                if (F === U) re === U ? V(n, i) || (g(n), p = Re(n, ke(i.nodeName, i.namespaceURI))) : p = i;
-                else if (F === ce || F === le) {
-                    if (re === F) return p.nodeValue !== i.nodeValue && (p.nodeValue = i.nodeValue), p;
-                    p = i
-                }
-            }
-            if (p === i) g(n);
-            else {
-                if (i.isSameNode && i.isSameNode(p)) return;
-                if (B(p, i, k), y)
-                    for (var J = 0, be = y.length; J < be; J++) {
-                        var K = v[y[J]];
-                        K && I(K, K.parentNode, !1)
                     }
-            }
-            return !k && p !== n && n.parentNode && (p.actualize && (p = p.actualize(n.ownerDocument || _)), n.parentNode.replaceChild(p, n)), p
-        }
-    }
-    var De = Pe(Ee),
-        ue = De;
-    var Z = function(t, e) {
-        return Z = Object.setPrototypeOf || {
+                }
+
+                function oe(n, r) {
+                    let o = new Map;
+                    return $(n, o), $(r, o), o
+                }
+                return {
+                    morph: e
+                }
+            }()
+        })
+    });
+    var q = function(t, e) {
+        return q = Object.setPrototypeOf || {
             __proto__: []
         }
-        instanceof Array && function(n, i) {
-            n.__proto__ = i
-        } || function(n, i) {
-            for (var r in i) i.hasOwnProperty(r) && (n[r] = i[r])
-        }, Z(t, e)
+        instanceof Array && function(i, a) {
+            i.__proto__ = a
+        } || function(i, a) {
+            for (var s in a) a.hasOwnProperty(s) && (i[s] = a[s])
+        }, q(t, e)
     };
 
-    function de(t, e) {
-        Z(t, e);
+    function Q(t, e) {
+        q(t, e);
 
-        function n() {
+        function i() {
             this.constructor = t
         }
-        t.prototype = e === null ? Object.create(e) : (n.prototype = e.prototype, new n)
+        t.prototype = e === null ? Object.create(e) : (i.prototype = e.prototype, new i)
     }
 
-    function Ue(t) {
+    function me(t) {
         var e = typeof Symbol == "function" && t[Symbol.iterator],
-            n = 0;
+            i = 0;
         return e ? e.call(t) : {
             next: function() {
-                return t && n >= t.length && (t = void 0), {
-                    value: t && t[n++],
+                return t && i >= t.length && (t = void 0), {
+                    value: t && t[i++],
                     done: !t
                 }
             }
         }
     }
 
-    function Me(t, e) {
-        var n = typeof Symbol == "function" && t[Symbol.iterator];
-        if (!n) return t;
-        var i = n.call(t),
-            r, o = [],
-            a;
+    function _e(t, e) {
+        var i = typeof Symbol == "function" && t[Symbol.iterator];
+        if (!i) return t;
+        var a = i.call(t),
+            s, d = [],
+            f;
         try {
             for (;
-                (e === void 0 || e-- > 0) && !(r = i.next()).done;) o.push(r.value)
-        } catch (u) {
-            a = {
-                error: u
+                (e === void 0 || e-- > 0) && !(s = a.next()).done;) d.push(s.value)
+        } catch (p) {
+            f = {
+                error: p
             }
         } finally {
             try {
-                r && !r.done && (n = i.return) && n.call(i)
+                s && !s.done && (i = a.return) && i.call(a)
             } finally {
-                if (a) throw a.error
+                if (f) throw f.error
             }
         }
-        return o
+        return d
     }
 
-    function je() {
-        for (var t = [], e = 0; e < arguments.length; e++) t = t.concat(Me(arguments[e]));
+    function be() {
+        for (var t = [], e = 0; e < arguments.length; e++) t = t.concat(_e(arguments[e]));
         return t
     }
-    var fe = function() {
-            function t(e, n) {
-                this.target = n, this.type = e
+    var K = function() {
+            function t(e, i) {
+                this.target = i, this.type = e
             }
             return t
         }(),
-        Ie = function(t) {
-            de(e, t);
+        ye = function(t) {
+            Q(e, t);
 
-            function e(n, i) {
-                var r = t.call(this, "error", i) || this;
-                return r.message = n.message, r.error = n, r
+            function e(i, a) {
+                var s = t.call(this, "error", a) || this;
+                return s.message = i.message, s.error = i, s
             }
             return e
-        }(fe),
-        Be = function(t) {
-            de(e, t);
-
-            function e(n, i, r) {
-                n === void 0 && (n = 1e3), i === void 0 && (i = "");
-                var o = t.call(this, "close", r) || this;
-                return o.wasClean = !0, o.code = n, o.reason = i, o
+        }(K),
+        ge = function(t) {
+            Q(e, t);
+
+            function e(i, a, s) {
+                i === void 0 && (i = 1e3), a === void 0 && (a = "");
+                var d = t.call(this, "close", s) || this;
+                return d.wasClean = !0, d.code = i, d.reason = a, d
             }
             return e
-        }(fe);
-    var Fe = function() {
+        }(K);
+    var ve = function() {
             if (typeof WebSocket != "undefined") return WebSocket
         },
-        Ge = function(t) {
+        Ee = function(t) {
             return typeof t != "undefined" && !!t && t.CLOSING === 2
         },
-        A = {
+        k = {
             maxReconnectionDelay: 1e4,
             minReconnectionDelay: 1e3 + Math.random() * 4e3,
             minUptime: 5e3,
             reconnectionDelayGrowFactor: 1.3,
             connectionTimeout: 4e3,
             maxRetries: 1 / 0,
             maxEnqueuedMessages: 1 / 0,
             startClosed: !1,
             debug: !1
         },
-        qe = function() {
-            function t(e, n, i) {
-                var r = this;
-                i === void 0 && (i = {}), this._listeners = {
+        we = function() {
+            function t(e, i, a) {
+                var s = this;
+                a === void 0 && (a = {}), this._listeners = {
                     error: [],
                     message: [],
                     open: [],
                     close: []
-                }, this._retryCount = -1, this._shouldReconnect = !0, this._connectLock = !1, this._binaryType = "blob", this._closeCalled = !1, this._messageQueue = [], this.onclose = null, this.onerror = null, this.onmessage = null, this.onopen = null, this._handleOpen = function(o) {
-                    r._debug("open event");
-                    var a = r._options.minUptime,
-                        u = a === void 0 ? A.minUptime : a;
-                    clearTimeout(r._connectTimeout), r._uptimeTimeout = setTimeout(function() {
-                        return r._acceptOpen()
-                    }, u), r._ws.binaryType = r._binaryType, r._messageQueue.forEach(function(d) {
-                        return r._ws.send(d)
-                    }), r._messageQueue = [], r.onopen && r.onopen(o), r._listeners.open.forEach(function(d) {
-                        return r._callEventListener(o, d)
+                }, this._retryCount = -1, this._shouldReconnect = !0, this._connectLock = !1, this._binaryType = "blob", this._closeCalled = !1, this._messageQueue = [], this.onclose = null, this.onerror = null, this.onmessage = null, this.onopen = null, this._handleOpen = function(d) {
+                    s._debug("open event");
+                    var f = s._options.minUptime,
+                        p = f === void 0 ? k.minUptime : f;
+                    clearTimeout(s._connectTimeout), s._uptimeTimeout = setTimeout(function() {
+                        return s._acceptOpen()
+                    }, p), s._ws.binaryType = s._binaryType, s._messageQueue.forEach(function(h) {
+                        return s._ws.send(h)
+                    }), s._messageQueue = [], s.onopen && s.onopen(d), s._listeners.open.forEach(function(h) {
+                        return s._callEventListener(d, h)
                     })
-                }, this._handleMessage = function(o) {
-                    r._debug("message event"), r.onmessage && r.onmessage(o), r._listeners.message.forEach(function(a) {
-                        return r._callEventListener(o, a)
+                }, this._handleMessage = function(d) {
+                    s._debug("message event"), s.onmessage && s.onmessage(d), s._listeners.message.forEach(function(f) {
+                        return s._callEventListener(d, f)
                     })
-                }, this._handleError = function(o) {
-                    r._debug("error event", o.message), r._disconnect(void 0, o.message === "TIMEOUT" ? "timeout" : void 0), r.onerror && r.onerror(o), r._debug("exec error listeners"), r._listeners.error.forEach(function(a) {
-                        return r._callEventListener(o, a)
-                    }), r._connect()
-                }, this._handleClose = function(o) {
-                    r._debug("close event"), r._clearTimeouts(), r._shouldReconnect && r._connect(), r.onclose && r.onclose(o), r._listeners.close.forEach(function(a) {
-                        return r._callEventListener(o, a)
+                }, this._handleError = function(d) {
+                    s._debug("error event", d.message), s._disconnect(void 0, d.message === "TIMEOUT" ? "timeout" : void 0), s.onerror && s.onerror(d), s._debug("exec error listeners"), s._listeners.error.forEach(function(f) {
+                        return s._callEventListener(d, f)
+                    }), s._connect()
+                }, this._handleClose = function(d) {
+                    s._debug("close event"), s._clearTimeouts(), s._shouldReconnect && s._connect(), s.onclose && s.onclose(d), s._listeners.close.forEach(function(f) {
+                        return s._callEventListener(d, f)
                     })
-                }, this._url = e, this._protocols = n, this._options = i, this._options.startClosed && (this._shouldReconnect = !1), this._connect()
+                }, this._url = e, this._protocols = i, this._options = a, this._options.startClosed && (this._shouldReconnect = !1), this._connect()
             }
             return Object.defineProperty(t, "CONNECTING", {
                 get: function() {
                     return 0
                 },
                 enumerable: !0,
                 configurable: !0
@@ -439,16 +537,16 @@
                 get: function() {
                     return Math.max(this._retryCount, 0)
                 },
                 enumerable: !0,
                 configurable: !0
             }), Object.defineProperty(t.prototype, "bufferedAmount", {
                 get: function() {
-                    var e = this._messageQueue.reduce(function(n, i) {
-                        return typeof i == "string" ? n += i.length : i instanceof Blob ? n += i.size : n += i.byteLength, n
+                    var e = this._messageQueue.reduce(function(i, a) {
+                        return typeof a == "string" ? i += a.length : a instanceof Blob ? i += a.size : i += a.byteLength, i
                     }, 0);
                     return e + (this._ws ? this._ws.bufferedAmount : 0)
                 },
                 enumerable: !0,
                 configurable: !0
             }), Object.defineProperty(t.prototype, "extensions", {
                 get: function() {
@@ -470,465 +568,420 @@
                 configurable: !0
             }), Object.defineProperty(t.prototype, "url", {
                 get: function() {
                     return this._ws ? this._ws.url : ""
                 },
                 enumerable: !0,
                 configurable: !0
-            }), t.prototype.close = function(e, n) {
+            }), t.prototype.close = function(e, i) {
                 if (e === void 0 && (e = 1e3), this._closeCalled = !0, this._shouldReconnect = !1, this._clearTimeouts(), !this._ws) {
                     this._debug("close enqueued: no ws instance");
                     return
                 }
                 if (this._ws.readyState === this.CLOSED) {
                     this._debug("close: already closed");
                     return
                 }
-                this._ws.close(e, n)
-            }, t.prototype.reconnect = function(e, n) {
-                this._shouldReconnect = !0, this._closeCalled = !1, this._retryCount = -1, !this._ws || this._ws.readyState === this.CLOSED ? this._connect() : (this._disconnect(e, n), this._connect())
+                this._ws.close(e, i)
+            }, t.prototype.reconnect = function(e, i) {
+                this._shouldReconnect = !0, this._closeCalled = !1, this._retryCount = -1, !this._ws || this._ws.readyState === this.CLOSED ? this._connect() : (this._disconnect(e, i), this._connect())
             }, t.prototype.send = function(e) {
                 if (this._ws && this._ws.readyState === this.OPEN) this._debug("send", e), this._ws.send(e);
                 else {
-                    var n = this._options.maxEnqueuedMessages,
-                        i = n === void 0 ? A.maxEnqueuedMessages : n;
-                    this._messageQueue.length < i && (this._debug("enqueue", e), this._messageQueue.push(e))
+                    var i = this._options.maxEnqueuedMessages,
+                        a = i === void 0 ? k.maxEnqueuedMessages : i;
+                    this._messageQueue.length < a && (this._debug("enqueue", e), this._messageQueue.push(e))
                 }
-            }, t.prototype.addEventListener = function(e, n) {
-                this._listeners[e] && this._listeners[e].push(n)
+            }, t.prototype.addEventListener = function(e, i) {
+                this._listeners[e] && this._listeners[e].push(i)
             }, t.prototype.dispatchEvent = function(e) {
-                var n, i, r = this._listeners[e.type];
-                if (r) try {
-                    for (var o = Ue(r), a = o.next(); !a.done; a = o.next()) {
-                        var u = a.value;
-                        this._callEventListener(e, u)
-                    }
-                } catch (d) {
-                    n = {
-                        error: d
+                var i, a, s = this._listeners[e.type];
+                if (s) try {
+                    for (var d = me(s), f = d.next(); !f.done; f = d.next()) {
+                        var p = f.value;
+                        this._callEventListener(e, p)
+                    }
+                } catch (h) {
+                    i = {
+                        error: h
                     }
                 } finally {
                     try {
-                        a && !a.done && (i = o.return) && i.call(o)
+                        f && !f.done && (a = d.return) && a.call(d)
                     } finally {
-                        if (n) throw n.error
+                        if (i) throw i.error
                     }
                 }
                 return !0
-            }, t.prototype.removeEventListener = function(e, n) {
-                this._listeners[e] && (this._listeners[e] = this._listeners[e].filter(function(i) {
-                    return i !== n
+            }, t.prototype.removeEventListener = function(e, i) {
+                this._listeners[e] && (this._listeners[e] = this._listeners[e].filter(function(a) {
+                    return a !== i
                 }))
             }, t.prototype._debug = function() {
-                for (var e = [], n = 0; n < arguments.length; n++) e[n] = arguments[n];
-                this._options.debug && console.log.apply(console, je(["RWS>"], e))
+                for (var e = [], i = 0; i < arguments.length; i++) e[i] = arguments[i];
+                this._options.debug && console.log.apply(console, be(["RWS>"], e))
             }, t.prototype._getNextDelay = function() {
                 var e = this._options,
-                    n = e.reconnectionDelayGrowFactor,
-                    i = n === void 0 ? A.reconnectionDelayGrowFactor : n,
-                    r = e.minReconnectionDelay,
-                    o = r === void 0 ? A.minReconnectionDelay : r,
-                    a = e.maxReconnectionDelay,
-                    u = a === void 0 ? A.maxReconnectionDelay : a,
-                    d = 0;
-                return this._retryCount > 0 && (d = o * Math.pow(i, this._retryCount - 1), d > u && (d = u)), this._debug("next delay", d), d
+                    i = e.reconnectionDelayGrowFactor,
+                    a = i === void 0 ? k.reconnectionDelayGrowFactor : i,
+                    s = e.minReconnectionDelay,
+                    d = s === void 0 ? k.minReconnectionDelay : s,
+                    f = e.maxReconnectionDelay,
+                    p = f === void 0 ? k.maxReconnectionDelay : f,
+                    h = 0;
+                return this._retryCount > 0 && (h = d * Math.pow(a, this._retryCount - 1), h > p && (h = p)), this._debug("next delay", h), h
             }, t.prototype._wait = function() {
                 var e = this;
-                return new Promise(function(n) {
-                    setTimeout(n, e._getNextDelay())
+                return new Promise(function(i) {
+                    setTimeout(i, e._getNextDelay())
                 })
             }, t.prototype._getNextUrl = function(e) {
                 if (typeof e == "string") return Promise.resolve(e);
                 if (typeof e == "function") {
-                    var n = e();
-                    if (typeof n == "string") return Promise.resolve(n);
-                    if (n.then) return n
+                    var i = e();
+                    if (typeof i == "string") return Promise.resolve(i);
+                    if (i.then) return i
                 }
                 throw Error("Invalid URL")
             }, t.prototype._connect = function() {
                 var e = this;
                 if (!(this._connectLock || !this._shouldReconnect)) {
                     this._connectLock = !0;
-                    var n = this._options,
-                        i = n.maxRetries,
-                        r = i === void 0 ? A.maxRetries : i,
-                        o = n.connectionTimeout,
-                        a = o === void 0 ? A.connectionTimeout : o,
-                        u = n.WebSocket,
-                        d = u === void 0 ? Fe() : u;
-                    if (this._retryCount >= r) {
-                        this._debug("max retries reached", this._retryCount, ">=", r);
+                    var i = this._options,
+                        a = i.maxRetries,
+                        s = a === void 0 ? k.maxRetries : a,
+                        d = i.connectionTimeout,
+                        f = d === void 0 ? k.connectionTimeout : d,
+                        p = i.WebSocket,
+                        h = p === void 0 ? ve() : p;
+                    if (this._retryCount >= s) {
+                        this._debug("max retries reached", this._retryCount, ">=", s);
                         return
                     }
-                    if (this._retryCount++, this._debug("connect", this._retryCount), this._removeListeners(), !Ge(d)) throw Error("No valid WebSocket class provided");
+                    if (this._retryCount++, this._debug("connect", this._retryCount), this._removeListeners(), !Ee(h)) throw Error("No valid WebSocket class provided");
                     this._wait().then(function() {
                         return e._getNextUrl(e._url)
-                    }).then(function(m) {
+                    }).then(function(y) {
                         e._closeCalled || (e._debug("connect", {
-                            url: m,
+                            url: y,
                             protocols: e._protocols
-                        }), e._ws = e._protocols ? new d(m, e._protocols) : new d(m), e._ws.binaryType = e._binaryType, e._connectLock = !1, e._addListeners(), e._connectTimeout = setTimeout(function() {
+                        }), e._ws = e._protocols ? new h(y, e._protocols) : new h(y), e._ws.binaryType = e._binaryType, e._connectLock = !1, e._addListeners(), e._connectTimeout = setTimeout(function() {
                             return e._handleTimeout()
-                        }, a))
+                        }, f))
                     })
                 }
             }, t.prototype._handleTimeout = function() {
-                this._debug("timeout event"), this._handleError(new Ie(Error("TIMEOUT"), this))
-            }, t.prototype._disconnect = function(e, n) {
+                this._debug("timeout event"), this._handleError(new ye(Error("TIMEOUT"), this))
+            }, t.prototype._disconnect = function(e, i) {
                 if (e === void 0 && (e = 1e3), this._clearTimeouts(), !!this._ws) {
                     this._removeListeners();
                     try {
-                        this._ws.close(e, n), this._handleClose(new Be(e, n, this))
+                        this._ws.close(e, i), this._handleClose(new ge(e, i, this))
                     } catch {}
                 }
             }, t.prototype._acceptOpen = function() {
                 this._debug("accept open"), this._retryCount = 0
-            }, t.prototype._callEventListener = function(e, n) {
-                "handleEvent" in n ? n.handleEvent(e) : n(e)
+            }, t.prototype._callEventListener = function(e, i) {
+                "handleEvent" in i ? i.handleEvent(e) : i(e)
             }, t.prototype._removeListeners = function() {
                 !this._ws || (this._debug("removeListeners"), this._ws.removeEventListener("open", this._handleOpen), this._ws.removeEventListener("close", this._handleClose), this._ws.removeEventListener("message", this._handleMessage), this._ws.removeEventListener("error", this._handleError))
             }, t.prototype._addListeners = function() {
                 !this._ws || (this._debug("addListeners"), this._ws.addEventListener("open", this._handleOpen), this._ws.addEventListener("close", this._handleClose), this._ws.addEventListener("message", this._handleMessage), this._ws.addEventListener("error", this._handleError))
             }, t.prototype._clearTimeouts = function() {
                 clearTimeout(this._connectTimeout), clearTimeout(this._uptimeTimeout)
             }, t
         }(),
-        ee = qe;
-    var z = JSON.parse(document.querySelector("meta[name=reactor-boost]")?.dataset.enabled || "false");
-    console.log("BOOST_PAGES", z);
-
-    function he() {
-        if (z)
-            for (let t of document.querySelectorAll("a[href]")) pe(t)
-    }
-
-    function pe(t) {
-        z && t.tagName?.toLowerCase() === "a" && t.hasAttribute("href") && !(t.boosted || t.hasAttribute("onclick") || t.hasAttribute("target") || t.hasAttribute(":no-boost")) && (t.boosted = !0, t.addEventListener("click", He))
-    }
-
-    function He(t) {
-        t.preventDefault();
-        let e = t.target.tagName?.toLowerCase === "a" ? t.target.href : t.target.closest("a").href;
-        N.load(e)
+        W = we;
+    var X = pe(Y());
+    console.log(X.default);
+
+    function Z(t, e) {
+        newJoiners = new Set, Idiomorph.morph(t, e, {
+            ignoreActive: !0,
+            callbacks: {
+                beforeNodeMorphed: function(i, a) {
+                    i instanceof HTMLElement && a instanceof HTMLElement && i.hasAttribute("reactor-component") && a.hasAttribute("reactor-component") && i.id !== a.id && (i.leave(), newJoiners.add(a.id))
+                },
+                afterNodeMorphed: function(i, a) {
+                    newJoiners.has(i.id) && i.join()
+                }
+            }
+        })
     }
+    var F = JSON.parse(document.querySelector("meta[name=reactor-boost]")?.dataset.enabled || "false");
+    console.log("BOOST_PAGES", F);
+    F && document.addEventListener("click", t => {
+        let e = t.target;
+        e = e.tagName.toLowerCase() !== "a" ? e.closest("a") : e, e && e.href && (!e.target || e.target === "_self") && e.origin == document.location.origin && t.button === 0 && !t.metaKey && !t.ctrlKey && !t.altKey && !t.shiftKey && (t.preventDefault(), V.load(e.href))
+    });
 
-    function _e(t, e) {
-        console.log("replaceBodyContent", e);
-        let n = document.createElement("html");
-        n.innerHTML = t, window.requestAnimationFrame(() => {
-            e?.beforeReplace && e.beforeReplace(n), document.body = n.querySelector("body"), he(), e?.afterReplace && e.afterReplace(n), document.querySelector("[autofocus]")?.focus()
-        })
+    function G(t, e = void 0) {
+        let i = new DOMParser().parseFromString(t, "text/html");
+        document.title = i.querySelector("title")?.text ?? "", Z(document.body, i.body), e === void 0 ? document.querySelector("[autofocus]")?.focus() : window.scrollTo(0, e)
     }
 
-    function We(t) {
+    function Se(t) {
         return t.startsWith("http://") || t.startsWith("https://") ? new URL(t).origin === document.location.origin : !0
     }
-    var te = class {
-            static async load(e) {
-                z ? (this._saveCurrentPage(), console.log(e), We(e) ? (this.push(e), await this.restoreFromCurrentPath()) : location.assign(e)) : location.assign(e)
-            }
-            static async restoreFromCurrentPath() {
-                this._saveCurrentPage();
-                let e = window.location.pathname + window.location.search;
-                console.log("Restoring Page:", e);
-                let n = this._get(e);
-                n && (_e(n.content, {
-                    beforeReplace() {
-                        document.title = n.title
-                    },
-                    afterReplace() {
-                        window.scrollTo(0, n.scroll)
-                    }
-                }), console.log("currentPath", e), this.currentPath = e);
-                let i = await fetch(window.location.href),
-                    r = await i.text();
-                this.replace(i.url), _e(r, {
-                    beforeReplace(o) {
-                        document.title = o.querySelector("title")?.text ?? ""
-                    },
-                    afterReplace() {
-                        te._saveCurrentPage()
-                    }
-                })
-            }
-            static back() {
-                window.history.back()
-            }
-            static push(e) {
-                history.pushState({}, document.title, e), this.currentPath = e
-            }
-            static replace(e) {
-                history.replaceState({}, document.title, e), this.currentPath = e
-            }
-            static _saveCurrentPage() {
-                if (console.log("Saving page:", this.currentPath), this.cache = this.cache.filter(({
-                        url: e
-                    }) => e != this.currentPath), this.cache.push({
-                        url: this.currentPath,
-                        content: document.body.outerHTML,
-                        title: document.title,
-                        scroll: window.scrollY
-                    }), this.cache.length > this.maxSize) {
-                    let e = this.cache.shift();
-                    console.log("Evicted:", e.url)
-                }
-                console.log("Currently cached:", this.cache.map(({
-                    url: e
-                }) => e))
-            }
-            static _get(e) {
-                return this.cache.find(n => n.url == e)
-            }
-        },
-        N = te;
-    H(N, "maxSize", 10), H(N, "cache", []), H(N, "currentPath", window.location.pathname + window.location.search);
+    var V = class {
+        static async load(e) {
+            F && Se(e) ? this.push(e) : document.location.assign(e)
+        }
+        static back() {
+            window.history.back()
+        }
+        static async push(e) {
+            history.replaceState({
+                content: document.body.outerHTML,
+                scrollY: window.scrollY
+            }, document.title, document.location.href);
+            let a = await (await fetch(e)).text();
+            history.pushState({}, document.title, e), G(a)
+        }
+        static replace(e) {
+            history.replaceState({}, document.title, e)
+        }
+    };
     window.addEventListener("popstate", t => {
-        N.restoreFromCurrentPath()
-    });
-    window.addEventListener("load", () => {
-        he()
+        t.state?.content !== void 0 && G(t.state.content, t.state.scrollY), fetch(document.location.href).then(e => e.text()).then(e => G(e))
     });
-    var O = {
-        boostElement: pe,
-        HistoryCache: N
+    var L = {
+        HistoryCache: V,
+        morph: Z
     };
-    var Ve = new DOMParser,
-        ve = class extends EventTarget {
+    var ke = new DOMParser,
+        ee = class extends EventTarget {
             open(e = "__reactor__") {
-                let n = location.protocol.replace("http", "ws");
-                this.socket = new ee(`${n}//${location.host}/${e}`, [], {
+                let i = location.protocol.replace("http", "ws");
+                this.socket = new W(`${i}//${location.host}/${e}`, [], {
                     maxEnqueuedMessages: 0
                 }), this.socket.addEventListener("open", () => {
                     console.log("WS: OPEN"), this.dispatchEvent(new Event("open"))
-                }), this.socket.addEventListener("message", i => this._processMessage(i)), this.socket.addEventListener("close", () => {
+                }), this.socket.addEventListener("message", a => this._processMessage(a)), this.socket.addEventListener("close", () => {
                     console.log("WS: CLOSE"), this.dispatchEvent(new Event("close"))
                 })
             }
             get isOpen() {
-                return this.socket?.readyState == ee.OPEN
+                return this.socket?.readyState == W.OPEN
             }
             _processMessage(e) {
                 let {
-                    command: n,
-                    payload: i
+                    command: i,
+                    payload: a
                 } = JSON.parse(e.data);
-                switch (n) {
+                switch (i) {
                     case "render":
                         var {
-                            id: r, diff: o
-                        } = i;
-                        console.log("<<< RENDER", r), document.getElementById(r)?.applyDiff(o);
+                            id: s, diff: d
+                        } = a;
+                        console.log("<<< RENDER", s), document.getElementById(s)?.applyDiff(d);
                         break;
                     case "append":
                     case "prepend":
                     case "insert_after":
                     case "insert_before":
                     case "replace_with":
                         var {
-                            id: r, html: a
-                        } = i;
-                        console.log(`<<< ${n.toUpperCase()}`, r), a = Ve.parseFromString(a, "text/html").body.firstChild;
-                        var u = document.getElementById(r);
-                        switch (n) {
+                            id: s, html: f
+                        } = a;
+                        console.log(`<<< ${i.toUpperCase()}`, s), f = ke.parseFromString(f, "text/html").body.firstChild;
+                        var p = document.getElementById(s);
+                        switch (i) {
                             case "append":
-                                u?.append(a);
+                                p?.append(f);
                                 break;
                             case "prepend":
-                                u?.prepend(a);
+                                p?.prepend(f);
                                 break;
                             case "insert_after":
-                                u?.after(a);
+                                p?.after(f);
                                 break;
                             case "insert_before":
-                                u?.before(a);
+                                p?.before(f);
                                 break;
                             case "replace_with":
-                                u?.replaceWith(a);
+                                p?.replaceWith(f);
                                 break
                         }
                         break;
                     case "remove":
                         var {
-                            id: r
-                        } = i;
-                        console.log("<<< REMOVE", r), document.getElementById(r)?.remove();
+                            id: s
+                        } = a;
+                        console.log("<<< REMOVE", s), document.getElementById(s)?.remove();
                         break;
                     case "focus_on":
                         var {
-                            selector: d
-                        } = i;
-                        console.log("<<< FOCUS-ON", `"${d}"`, document.querySelector(d)), window.requestAnimationFrame(() => document.querySelector(d)?.focus());
+                            selector: h
+                        } = a;
+                        console.log("<<< FOCUS-ON", `"${h}"`, document.querySelector(h)), window.requestAnimationFrame(() => document.querySelector(h)?.focus());
                         break;
                     case "scroll_into_view":
                         var {
-                            id: r, behavior: m, block: L, inline: $
-                        } = i;
-                        window.requestAnimationFrame(() => document.getElementById(r)?.scrollIntoView({
-                            behavior: m,
-                            block: L,
-                            inline: $
+                            id: s, behavior: y, block: D, inline: R
+                        } = a;
+                        window.requestAnimationFrame(() => document.getElementById(s)?.scrollIntoView({
+                            behavior: y,
+                            block: D,
+                            inline: R
                         }));
                         break;
                     case "url_change":
                         var {
-                            url: g
-                        } = i;
-                        switch (console.log("<< URL", i.command, g), i.command) {
+                            url: v
+                        } = a;
+                        switch (console.log("<< URL", a.command, v), a.command) {
                             case "redirect":
-                                O.HistoryCache.load(g);
+                                L.HistoryCache.load(v);
                                 break;
                             case "replace":
-                                O.HistoryCache.replace(g);
+                                L.HistoryCache.replace(v);
                                 break;
                             case "push":
-                                O.HistoryCache.push(g);
+                                L.HistoryCache.push(v);
                                 break
                         }
                         break;
                     case "set_url_params":
-                        console.log("<< SET URL PARAMS", i);
-                        let M = document.location.search.slice(1),
-                            j = {};
-                        M.length && (j = M.split("&").map(v => v.split("=")).reduce((v, y) => {
-                            let [b, D] = y;
-                            return v[b] = D === void 0 ? void 0 : decodeURIComponent(D), v
+                        console.log("<< SET URL PARAMS", a);
+                        let O = document.location.search.slice(1),
+                            I = {};
+                        O.length && (I = O.split("&").map(E => E.split("=")).reduce((E, C) => {
+                            let [T, N] = C;
+                            return E[T] = N === void 0 ? void 0 : decodeURIComponent(N), E
                         }, {}));
-                        let P = Object.entries(Object.assign(j, i)).map(v => {
-                                let [y, b] = v;
-                                return y + (b === void 0 ? "" : `=${encodeURIComponent(b)}`)
+                        let P = Object.entries(Object.assign(I, a)).map(E => {
+                                let [C, T] = E;
+                                return C + (T === void 0 ? "" : `=${encodeURIComponent(T)}`)
                             }),
-                            k = document.location.pathname;
-                        P.length && (k += "?" + P.join("&")), O.HistoryCache.replace(k);
+                            H = document.location.pathname;
+                        P.length && (H += "?" + P.join("&")), L.HistoryCache.replace(H);
                         break;
                     case "back":
-                        O.HistoryCache.back();
+                        L.HistoryCache.back();
                         break;
                     default:
-                        console.error(`Unknown command "${n}"`, i)
+                        console.error(`Unknown command "${i}"`, a)
                 }
             }
-            sendJoin(e, n, i) {
+            sendJoin(e, i, a) {
                 this._send("join", {
                     name: e,
-                    parent_id: n,
-                    state: i
+                    parent_id: i,
+                    state: a
                 })
             }
             sendLeave(e) {
                 console.log(">>> LEAVE", e), this._send("leave", {
                     id: e
                 })
             }
-            sendUserEvent(e, n, i, r) {
-                console.log(">>> USER_EVENT", e, n, r), this._send("user_event", {
+            sendUserEvent(e, i, a, s) {
+                console.log(">>> USER_EVENT", e, i, s), this._send("user_event", {
                     id: e,
-                    command: n,
-                    implicit_args: i,
-                    explicit_args: r
+                    command: i,
+                    implicit_args: a,
+                    explicit_args: s
                 })
             }
-            _send(e, n) {
+            _send(e, i) {
                 this.isOpen && this.socket.send(JSON.stringify({
                     command: e,
-                    payload: n
+                    payload: i
                 }))
             }
         },
-        C = new ve;
+        w = new ee;
     for ({
             dataset
         }
         of document.querySelectorAll("meta[name=reactor-component]")) {
         let t = document.createElement(dataset.extends);
         class e extends t.constructor {
-            constructor(...i) {
-                super(...i);
+            constructor(...a) {
+                super(...a);
                 this._lastReceivedHtml = [], this.joinBind = () => this.join(), this.wentOffline = () => this.classList.add("reactor-disconnected")
             }
             connectedCallback() {
-                C.addEventListener("open", this.joinBind), C.addEventListener("close", this.wentOffline), this.join()
+                w.addEventListener("open", this.joinBind), w.addEventListener("close", this.wentOffline), this.join()
             }
             disconnectedCallback() {
-                C.removeEventListener("open", this.joinBind), C.removeEventListener("close", this.wentOffline), C.sendLeave(this.id)
+                w.removeEventListener("open", this.joinBind), w.removeEventListener("close", this.wentOffline), this.leave()
             }
             join() {
-                this.classList.remove("reactor-disconnected"), C.sendJoin(this.dataset.name, this.parentId, this.dataset.state)
+                this.classList.remove("reactor-disconnected"), w.sendJoin(this.dataset.name, this.parentId, this.dataset.state)
+            }
+            leave() {
+                w.sendLeave(this.id)
             }
-            applyDiff(i) {
-                let r = this.getHtml(i);
+            applyDiff(a) {
                 window.requestAnimationFrame(() => {
-                    ue(this, r, {
-                        onBeforeNodeAdded(o) {
-                            O.boostElement(o)
-                        },
-                        onElUpdated(o) {
-                            O.boostElement(o)
-                        }
-                    })
+                    let s = this.getHtml(a);
+                    L.morph(this, s)
                 })
             }
-            getHtml(i) {
-                let r = [],
-                    o = 0;
-                for (let a of i) typeof a == "string" ? r.push(a) : a < 0 ? o -= a : (r.push(...this._lastReceivedHtml.slice(o, o + a)), o += a);
-                return this._lastReceivedHtml = r, r.join(" ")
+            getHtml(a) {
+                let s = [],
+                    d = 0;
+                for (let f of a) typeof f == "string" ? s.push(f) : f < 0 ? d -= f : (s.push(...this._lastReceivedHtml.slice(d, d + f)), d += f);
+                return this._lastReceivedHtml = s, s.join(" ")
             }
             get parentId() {
                 return this.parentComponent?.id
             }
             get parentComponent() {
                 return this.parentElement?.closest("[reactor-component]")
             }
-            dispatch(i, r, o) {
-                C.sendUserEvent(this.id, i, this.serialize(o), r)
+            dispatch(a, s, d) {
+                w.sendUserEvent(this.id, a, this.serialize(d), s)
             }
-            serialize(i) {
-                let r = {};
-                for (let o of i.querySelectorAll("[name]")) {
-                    if (o.closest("[reactor-component]") !== this) continue;
-                    let a = null;
-                    switch (o.type.toLowerCase()) {
+            serialize(a) {
+                let s = {};
+                for (let d of a.querySelectorAll("[name]")) {
+                    if (d.closest("[reactor-component]") !== this) continue;
+                    let f = null;
+                    switch (d.type.toLowerCase()) {
                         case "checkbox":
                         case "radio":
-                            a = o.checked ? o.value || !0 : null;
+                            f = d.checked ? d.value || !0 : null;
                             break;
                         case "select-multiple":
-                            a = o.selectedOptions.map(u => u.value);
+                            f = d.selectedOptions.map(p => p.value);
                             break;
                         default:
-                            a = o.value;
+                            f = d.value;
                             break
                     }
-                    if (a !== null) {
-                        let u = o.getAttribute("name"),
-                            d = r[u] ?? [];
-                        d.push(a), r[u] = d
+                    if (f !== null) {
+                        let p = d.getAttribute("name"),
+                            h = s[p] ?? [];
+                        h.push(f), s[p] = h
                     }
                 }
-                return r
+                return s
             }
         }
         customElements.define(dataset.tagName, e, {
             extends: dataset.extends
         })
     }
-    C.open();
-    debounceTimeouts = {};
+    w.open();
+    var te = void 0;
     window.reactor = {
-        send(t, e, n) {
-            let i = t.closest("[reactor-component]");
-            if (i !== null) {
-                let r = t.closest("form"),
-                    o = i.contains(r) ? r : i;
-                i.dispatch(e, n, o)
+        send(t, e, i) {
+            let a = t.closest("[reactor-component]");
+            if (a !== null) {
+                let s = t.closest("form"),
+                    d = a.contains(s) ? s : a;
+                a.dispatch(e, i, d)
             }
         },
-        debounce(t, e) {
-            return n => (...i) => {
-                clearTimeout(debounceTimeouts[t]), debounceTimeouts[t] = setTimeout(() => n(...i), e)
+        debounce(t) {
+            return e => (...i) => {
+                clearTimeout(te), te = setTimeout(() => e(...i), t)
             }
         }
     };
 })();
 /*!
  * Reconnecting WebSocket
  * by Pedro Ladaria <pedro.ladaria@gmail.com>
```

### Comparing `django-reactor-5.0.1b0/reactor/static/reactor/reactor.min.js.map` & `django-reactor-5.0.2b0/reactor/static/reactor/reactor.min.js.map`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7742857142857142%*

 * *Differences: {"'mappings'": "'wmBAAA,aAKA,AAAC,UAAU,EAAM,EAAS,CAEtB,AAAI,MAAO,SAAW,YAAc,OAAO,IAGvC,OAAO,GAAI,GAGX,EAAK,UAAY,EAAK,WAAa,MAEzC,MAAO,OAAS,YAAc,KAAO,EACnC,UAAY,CACR,MAAQ,WAAY,CAChB,aAKA,GAAI,GAAY,GAAI,KAKpB,WAAe,EAAS,EAAY,EAAS,GAAI,CAE7C,AAAI,YAAmB,WACnB,GAAU,EAAQ,iBAGlB,MAAO,IAAe,UACtB,GAAa,EAAa,IAG9B,GAAI,GAAoB,EAAiB,GAErC,EAAM,EAAmB,EAAS,EAAmB,GAEzD,MAAO,GAAuB,EAAS,EAAmB,GAG9D,WAAgC,EAAS,EAAsB,EAAK,CAChE,GAAI,EAAI,KAAK,MAAO,CAChB,GAAI,GAAU,EAAQ,cAAc,QAChC,EAAU,EAAqB,cAAc,QACjD,GAAI,GAAW,EAAS,CACpB,GAAI,GAA […]*

```diff
@@ -1,17 +1,17 @@
 {
-    "mappings": "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",
+    "mappings": "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",
     "names": [],
     "sources": [
-        "../../../node_modules/morphdom/dist/morphdom-esm.js",
+        "../../../node_modules/idiomorph/dist/idiomorph.js",
         "../../../node_modules/reconnecting-websocket/dist/reconnecting-websocket-mjs.js",
         "reactor-boost.js",
         "reactor.js"
     ],
     "sourcesContent": [
-        "var DOCUMENT_FRAGMENT_NODE = 11;\n\nfunction morphAttrs(fromNode, toNode) {\n    var toNodeAttrs = toNode.attributes;\n    var attr;\n    var attrName;\n    var attrNamespaceURI;\n    var attrValue;\n    var fromValue;\n\n    // document-fragments dont have attributes so lets not do anything\n    if (toNode.nodeType === DOCUMENT_FRAGMENT_NODE || fromNode.nodeType === DOCUMENT_FRAGMENT_NODE) {\n      return;\n    }\n\n    // update attributes on original DOM element\n    for (var i = toNodeAttrs.length - 1; i >= 0; i--) {\n        attr = toNodeAttrs[i];\n        attrName = attr.name;\n        attrNamespaceURI = attr.namespaceURI;\n        attrValue = attr.value;\n\n        if (attrNamespaceURI) {\n            attrName = attr.localName || attrName;\n            fromValue = fromNode.getAttributeNS(attrNamespaceURI, attrName);\n\n            if (fromValue !== attrValue) {\n                if (attr.prefix === 'xmlns'){\n                    attrName = attr.name; // It's not allowed to set an attribute with the XMLNS namespace without specifying the `xmlns` prefix\n                }\n                fromNode.setAttributeNS(attrNamespaceURI, attrName, attrValue);\n            }\n        } else {\n            fromValue = fromNode.getAttribute(attrName);\n\n            if (fromValue !== attrValue) {\n                fromNode.setAttribute(attrName, attrValue);\n            }\n        }\n    }\n\n    // Remove any extra attributes found on the original DOM element that\n    // weren't found on the target element.\n    var fromNodeAttrs = fromNode.attributes;\n\n    for (var d = fromNodeAttrs.length - 1; d >= 0; d--) {\n        attr = fromNodeAttrs[d];\n        attrName = attr.name;\n        attrNamespaceURI = attr.namespaceURI;\n\n        if (attrNamespaceURI) {\n            attrName = attr.localName || attrName;\n\n            if (!toNode.hasAttributeNS(attrNamespaceURI, attrName)) {\n                fromNode.removeAttributeNS(attrNamespaceURI, attrName);\n            }\n        } else {\n            if (!toNode.hasAttribute(attrName)) {\n                fromNode.removeAttribute(attrName);\n            }\n        }\n    }\n}\n\nvar range; // Create a range object for efficently rendering strings to elements.\nvar NS_XHTML = 'http://www.w3.org/1999/xhtml';\n\nvar doc = typeof document === 'undefined' ? undefined : document;\nvar HAS_TEMPLATE_SUPPORT = !!doc && 'content' in doc.createElement('template');\nvar HAS_RANGE_SUPPORT = !!doc && doc.createRange && 'createContextualFragment' in doc.createRange();\n\nfunction createFragmentFromTemplate(str) {\n    var template = doc.createElement('template');\n    template.innerHTML = str;\n    return template.content.childNodes[0];\n}\n\nfunction createFragmentFromRange(str) {\n    if (!range) {\n        range = doc.createRange();\n        range.selectNode(doc.body);\n    }\n\n    var fragment = range.createContextualFragment(str);\n    return fragment.childNodes[0];\n}\n\nfunction createFragmentFromWrap(str) {\n    var fragment = doc.createElement('body');\n    fragment.innerHTML = str;\n    return fragment.childNodes[0];\n}\n\n/**\n * This is about the same\n * var html = new DOMParser().parseFromString(str, 'text/html');\n * return html.body.firstChild;\n *\n * @method toElement\n * @param {String} str\n */\nfunction toElement(str) {\n    str = str.trim();\n    if (HAS_TEMPLATE_SUPPORT) {\n      // avoid restrictions on content for things like `<tr><th>Hi</th></tr>` which\n      // createContextualFragment doesn't support\n      // <template> support not available in IE\n      return createFragmentFromTemplate(str);\n    } else if (HAS_RANGE_SUPPORT) {\n      return createFragmentFromRange(str);\n    }\n\n    return createFragmentFromWrap(str);\n}\n\n/**\n * Returns true if two node's names are the same.\n *\n * NOTE: We don't bother checking `namespaceURI` because you will never find two HTML elements with the same\n *       nodeName and different namespace URIs.\n *\n * @param {Element} a\n * @param {Element} b The target element\n * @return {boolean}\n */\nfunction compareNodeNames(fromEl, toEl) {\n    var fromNodeName = fromEl.nodeName;\n    var toNodeName = toEl.nodeName;\n    var fromCodeStart, toCodeStart;\n\n    if (fromNodeName === toNodeName) {\n        return true;\n    }\n\n    fromCodeStart = fromNodeName.charCodeAt(0);\n    toCodeStart = toNodeName.charCodeAt(0);\n\n    // If the target element is a virtual DOM node or SVG node then we may\n    // need to normalize the tag name before comparing. Normal HTML elements that are\n    // in the \"http://www.w3.org/1999/xhtml\"\n    // are converted to upper case\n    if (fromCodeStart <= 90 && toCodeStart >= 97) { // from is upper and to is lower\n        return fromNodeName === toNodeName.toUpperCase();\n    } else if (toCodeStart <= 90 && fromCodeStart >= 97) { // to is upper and from is lower\n        return toNodeName === fromNodeName.toUpperCase();\n    } else {\n        return false;\n    }\n}\n\n/**\n * Create an element, optionally with a known namespace URI.\n *\n * @param {string} name the element name, e.g. 'div' or 'svg'\n * @param {string} [namespaceURI] the element's namespace URI, i.e. the value of\n * its `xmlns` attribute or its inferred namespace.\n *\n * @return {Element}\n */\nfunction createElementNS(name, namespaceURI) {\n    return !namespaceURI || namespaceURI === NS_XHTML ?\n        doc.createElement(name) :\n        doc.createElementNS(namespaceURI, name);\n}\n\n/**\n * Copies the children of one DOM element to another DOM element\n */\nfunction moveChildren(fromEl, toEl) {\n    var curChild = fromEl.firstChild;\n    while (curChild) {\n        var nextChild = curChild.nextSibling;\n        toEl.appendChild(curChild);\n        curChild = nextChild;\n    }\n    return toEl;\n}\n\nfunction syncBooleanAttrProp(fromEl, toEl, name) {\n    if (fromEl[name] !== toEl[name]) {\n        fromEl[name] = toEl[name];\n        if (fromEl[name]) {\n            fromEl.setAttribute(name, '');\n        } else {\n            fromEl.removeAttribute(name);\n        }\n    }\n}\n\nvar specialElHandlers = {\n    OPTION: function(fromEl, toEl) {\n        var parentNode = fromEl.parentNode;\n        if (parentNode) {\n            var parentName = parentNode.nodeName.toUpperCase();\n            if (parentName === 'OPTGROUP') {\n                parentNode = parentNode.parentNode;\n                parentName = parentNode && parentNode.nodeName.toUpperCase();\n            }\n            if (parentName === 'SELECT' && !parentNode.hasAttribute('multiple')) {\n                if (fromEl.hasAttribute('selected') && !toEl.selected) {\n                    // Workaround for MS Edge bug where the 'selected' attribute can only be\n                    // removed if set to a non-empty value:\n                    // https://developer.microsoft.com/en-us/microsoft-edge/platform/issues/12087679/\n                    fromEl.setAttribute('selected', 'selected');\n                    fromEl.removeAttribute('selected');\n                }\n                // We have to reset select element's selectedIndex to -1, otherwise setting\n                // fromEl.selected using the syncBooleanAttrProp below has no effect.\n                // The correct selectedIndex will be set in the SELECT special handler below.\n                parentNode.selectedIndex = -1;\n            }\n        }\n        syncBooleanAttrProp(fromEl, toEl, 'selected');\n    },\n    /**\n     * The \"value\" attribute is special for the <input> element since it sets\n     * the initial value. Changing the \"value\" attribute without changing the\n     * \"value\" property will have no effect since it is only used to the set the\n     * initial value.  Similar for the \"checked\" attribute, and \"disabled\".\n     */\n    INPUT: function(fromEl, toEl) {\n        syncBooleanAttrProp(fromEl, toEl, 'checked');\n        syncBooleanAttrProp(fromEl, toEl, 'disabled');\n\n        if (fromEl.value !== toEl.value) {\n            fromEl.value = toEl.value;\n        }\n\n        if (!toEl.hasAttribute('value')) {\n            fromEl.removeAttribute('value');\n        }\n    },\n\n    TEXTAREA: function(fromEl, toEl) {\n        var newValue = toEl.value;\n        if (fromEl.value !== newValue) {\n            fromEl.value = newValue;\n        }\n\n        var firstChild = fromEl.firstChild;\n        if (firstChild) {\n            // Needed for IE. Apparently IE sets the placeholder as the\n            // node value and vise versa. This ignores an empty update.\n            var oldValue = firstChild.nodeValue;\n\n            if (oldValue == newValue || (!newValue && oldValue == fromEl.placeholder)) {\n                return;\n            }\n\n            firstChild.nodeValue = newValue;\n        }\n    },\n    SELECT: function(fromEl, toEl) {\n        if (!toEl.hasAttribute('multiple')) {\n            var selectedIndex = -1;\n            var i = 0;\n            // We have to loop through children of fromEl, not toEl since nodes can be moved\n            // from toEl to fromEl directly when morphing.\n            // At the time this special handler is invoked, all children have already been morphed\n            // and appended to / removed from fromEl, so using fromEl here is safe and correct.\n            var curChild = fromEl.firstChild;\n            var optgroup;\n            var nodeName;\n            while(curChild) {\n                nodeName = curChild.nodeName && curChild.nodeName.toUpperCase();\n                if (nodeName === 'OPTGROUP') {\n                    optgroup = curChild;\n                    curChild = optgroup.firstChild;\n                } else {\n                    if (nodeName === 'OPTION') {\n                        if (curChild.hasAttribute('selected')) {\n                            selectedIndex = i;\n                            break;\n                        }\n                        i++;\n                    }\n                    curChild = curChild.nextSibling;\n                    if (!curChild && optgroup) {\n                        curChild = optgroup.nextSibling;\n                        optgroup = null;\n                    }\n                }\n            }\n\n            fromEl.selectedIndex = selectedIndex;\n        }\n    }\n};\n\nvar ELEMENT_NODE = 1;\nvar DOCUMENT_FRAGMENT_NODE$1 = 11;\nvar TEXT_NODE = 3;\nvar COMMENT_NODE = 8;\n\nfunction noop() {}\n\nfunction defaultGetNodeKey(node) {\n  if (node) {\n    return (node.getAttribute && node.getAttribute('id')) || node.id;\n  }\n}\n\nfunction morphdomFactory(morphAttrs) {\n\n  return function morphdom(fromNode, toNode, options) {\n    if (!options) {\n      options = {};\n    }\n\n    if (typeof toNode === 'string') {\n      if (fromNode.nodeName === '#document' || fromNode.nodeName === 'HTML' || fromNode.nodeName === 'BODY') {\n        var toNodeHtml = toNode;\n        toNode = doc.createElement('html');\n        toNode.innerHTML = toNodeHtml;\n      } else {\n        toNode = toElement(toNode);\n      }\n    } else if (toNode.nodeType === DOCUMENT_FRAGMENT_NODE$1) {\n      toNode = toNode.firstElementChild;\n    }\n\n    var getNodeKey = options.getNodeKey || defaultGetNodeKey;\n    var onBeforeNodeAdded = options.onBeforeNodeAdded || noop;\n    var onNodeAdded = options.onNodeAdded || noop;\n    var onBeforeElUpdated = options.onBeforeElUpdated || noop;\n    var onElUpdated = options.onElUpdated || noop;\n    var onBeforeNodeDiscarded = options.onBeforeNodeDiscarded || noop;\n    var onNodeDiscarded = options.onNodeDiscarded || noop;\n    var onBeforeElChildrenUpdated = options.onBeforeElChildrenUpdated || noop;\n    var skipFromChildren = options.skipFromChildren || noop;\n    var addChild = options.addChild || function(parent, child){ return parent.appendChild(child); };\n    var childrenOnly = options.childrenOnly === true;\n\n    // This object is used as a lookup to quickly find all keyed elements in the original DOM tree.\n    var fromNodesLookup = Object.create(null);\n    var keyedRemovalList = [];\n\n    function addKeyedRemoval(key) {\n      keyedRemovalList.push(key);\n    }\n\n    function walkDiscardedChildNodes(node, skipKeyedNodes) {\n      if (node.nodeType === ELEMENT_NODE) {\n        var curChild = node.firstChild;\n        while (curChild) {\n\n          var key = undefined;\n\n          if (skipKeyedNodes && (key = getNodeKey(curChild))) {\n            // If we are skipping keyed nodes then we add the key\n            // to a list so that it can be handled at the very end.\n            addKeyedRemoval(key);\n          } else {\n            // Only report the node as discarded if it is not keyed. We do this because\n            // at the end we loop through all keyed elements that were unmatched\n            // and then discard them in one final pass.\n            onNodeDiscarded(curChild);\n            if (curChild.firstChild) {\n              walkDiscardedChildNodes(curChild, skipKeyedNodes);\n            }\n          }\n\n          curChild = curChild.nextSibling;\n        }\n      }\n    }\n\n    /**\n    * Removes a DOM node out of the original DOM\n    *\n    * @param  {Node} node The node to remove\n    * @param  {Node} parentNode The nodes parent\n    * @param  {Boolean} skipKeyedNodes If true then elements with keys will be skipped and not discarded.\n    * @return {undefined}\n    */\n    function removeNode(node, parentNode, skipKeyedNodes) {\n      if (onBeforeNodeDiscarded(node) === false) {\n        return;\n      }\n\n      if (parentNode) {\n        parentNode.removeChild(node);\n      }\n\n      onNodeDiscarded(node);\n      walkDiscardedChildNodes(node, skipKeyedNodes);\n    }\n\n    // // TreeWalker implementation is no faster, but keeping this around in case this changes in the future\n    // function indexTree(root) {\n    //     var treeWalker = document.createTreeWalker(\n    //         root,\n    //         NodeFilter.SHOW_ELEMENT);\n    //\n    //     var el;\n    //     while((el = treeWalker.nextNode())) {\n    //         var key = getNodeKey(el);\n    //         if (key) {\n    //             fromNodesLookup[key] = el;\n    //         }\n    //     }\n    // }\n\n    // // NodeIterator implementation is no faster, but keeping this around in case this changes in the future\n    //\n    // function indexTree(node) {\n    //     var nodeIterator = document.createNodeIterator(node, NodeFilter.SHOW_ELEMENT);\n    //     var el;\n    //     while((el = nodeIterator.nextNode())) {\n    //         var key = getNodeKey(el);\n    //         if (key) {\n    //             fromNodesLookup[key] = el;\n    //         }\n    //     }\n    // }\n\n    function indexTree(node) {\n      if (node.nodeType === ELEMENT_NODE || node.nodeType === DOCUMENT_FRAGMENT_NODE$1) {\n        var curChild = node.firstChild;\n        while (curChild) {\n          var key = getNodeKey(curChild);\n          if (key) {\n            fromNodesLookup[key] = curChild;\n          }\n\n          // Walk recursively\n          indexTree(curChild);\n\n          curChild = curChild.nextSibling;\n        }\n      }\n    }\n\n    indexTree(fromNode);\n\n    function handleNodeAdded(el) {\n      onNodeAdded(el);\n\n      var curChild = el.firstChild;\n      while (curChild) {\n        var nextSibling = curChild.nextSibling;\n\n        var key = getNodeKey(curChild);\n        if (key) {\n          var unmatchedFromEl = fromNodesLookup[key];\n          // if we find a duplicate #id node in cache, replace `el` with cache value\n          // and morph it to the child node.\n          if (unmatchedFromEl && compareNodeNames(curChild, unmatchedFromEl)) {\n            curChild.parentNode.replaceChild(unmatchedFromEl, curChild);\n            morphEl(unmatchedFromEl, curChild);\n          } else {\n            handleNodeAdded(curChild);\n          }\n        } else {\n          // recursively call for curChild and it's children to see if we find something in\n          // fromNodesLookup\n          handleNodeAdded(curChild);\n        }\n\n        curChild = nextSibling;\n      }\n    }\n\n    function cleanupFromEl(fromEl, curFromNodeChild, curFromNodeKey) {\n      // We have processed all of the \"to nodes\". If curFromNodeChild is\n      // non-null then we still have some from nodes left over that need\n      // to be removed\n      while (curFromNodeChild) {\n        var fromNextSibling = curFromNodeChild.nextSibling;\n        if ((curFromNodeKey = getNodeKey(curFromNodeChild))) {\n          // Since the node is keyed it might be matched up later so we defer\n          // the actual removal to later\n          addKeyedRemoval(curFromNodeKey);\n        } else {\n          // NOTE: we skip nested keyed nodes from being removed since there is\n          //       still a chance they will be matched up later\n          removeNode(curFromNodeChild, fromEl, true /* skip keyed nodes */);\n        }\n        curFromNodeChild = fromNextSibling;\n      }\n    }\n\n    function morphEl(fromEl, toEl, childrenOnly) {\n      var toElKey = getNodeKey(toEl);\n\n      if (toElKey) {\n        // If an element with an ID is being morphed then it will be in the final\n        // DOM so clear it out of the saved elements collection\n        delete fromNodesLookup[toElKey];\n      }\n\n      if (!childrenOnly) {\n        // optional\n        if (onBeforeElUpdated(fromEl, toEl) === false) {\n          return;\n        }\n\n        // update attributes on original DOM element first\n        morphAttrs(fromEl, toEl);\n        // optional\n        onElUpdated(fromEl);\n\n        if (onBeforeElChildrenUpdated(fromEl, toEl) === false) {\n          return;\n        }\n      }\n\n      if (fromEl.nodeName !== 'TEXTAREA') {\n        morphChildren(fromEl, toEl);\n      } else {\n        specialElHandlers.TEXTAREA(fromEl, toEl);\n      }\n    }\n\n    function morphChildren(fromEl, toEl) {\n      var skipFrom = skipFromChildren(fromEl);\n      var curToNodeChild = toEl.firstChild;\n      var curFromNodeChild = fromEl.firstChild;\n      var curToNodeKey;\n      var curFromNodeKey;\n\n      var fromNextSibling;\n      var toNextSibling;\n      var matchingFromEl;\n\n      // walk the children\n      outer: while (curToNodeChild) {\n        toNextSibling = curToNodeChild.nextSibling;\n        curToNodeKey = getNodeKey(curToNodeChild);\n\n        // walk the fromNode children all the way through\n        while (!skipFrom && curFromNodeChild) {\n          fromNextSibling = curFromNodeChild.nextSibling;\n\n          if (curToNodeChild.isSameNode && curToNodeChild.isSameNode(curFromNodeChild)) {\n            curToNodeChild = toNextSibling;\n            curFromNodeChild = fromNextSibling;\n            continue outer;\n          }\n\n          curFromNodeKey = getNodeKey(curFromNodeChild);\n\n          var curFromNodeType = curFromNodeChild.nodeType;\n\n          // this means if the curFromNodeChild doesnt have a match with the curToNodeChild\n          var isCompatible = undefined;\n\n          if (curFromNodeType === curToNodeChild.nodeType) {\n            if (curFromNodeType === ELEMENT_NODE) {\n              // Both nodes being compared are Element nodes\n\n              if (curToNodeKey) {\n                // The target node has a key so we want to match it up with the correct element\n                // in the original DOM tree\n                if (curToNodeKey !== curFromNodeKey) {\n                  // The current element in the original DOM tree does not have a matching key so\n                  // let's check our lookup to see if there is a matching element in the original\n                  // DOM tree\n                  if ((matchingFromEl = fromNodesLookup[curToNodeKey])) {\n                    if (fromNextSibling === matchingFromEl) {\n                      // Special case for single element removals. To avoid removing the original\n                      // DOM node out of the tree (since that can break CSS transitions, etc.),\n                      // we will instead discard the current node and wait until the next\n                      // iteration to properly match up the keyed target element with its matching\n                      // element in the original tree\n                      isCompatible = false;\n                    } else {\n                      // We found a matching keyed element somewhere in the original DOM tree.\n                      // Let's move the original DOM node into the current position and morph\n                      // it.\n\n                      // NOTE: We use insertBefore instead of replaceChild because we want to go through\n                      // the `removeNode()` function for the node that is being discarded so that\n                      // all lifecycle hooks are correctly invoked\n                      fromEl.insertBefore(matchingFromEl, curFromNodeChild);\n\n                      // fromNextSibling = curFromNodeChild.nextSibling;\n\n                      if (curFromNodeKey) {\n                        // Since the node is keyed it might be matched up later so we defer\n                        // the actual removal to later\n                        addKeyedRemoval(curFromNodeKey);\n                      } else {\n                        // NOTE: we skip nested keyed nodes from being removed since there is\n                        //       still a chance they will be matched up later\n                        removeNode(curFromNodeChild, fromEl, true /* skip keyed nodes */);\n                      }\n\n                      curFromNodeChild = matchingFromEl;\n                    }\n                  } else {\n                    // The nodes are not compatible since the \"to\" node has a key and there\n                    // is no matching keyed node in the source tree\n                    isCompatible = false;\n                  }\n                }\n              } else if (curFromNodeKey) {\n                // The original has a key\n                isCompatible = false;\n              }\n\n              isCompatible = isCompatible !== false && compareNodeNames(curFromNodeChild, curToNodeChild);\n              if (isCompatible) {\n                // We found compatible DOM elements so transform\n                // the current \"from\" node to match the current\n                // target DOM node.\n                // MORPH\n                morphEl(curFromNodeChild, curToNodeChild);\n              }\n\n            } else if (curFromNodeType === TEXT_NODE || curFromNodeType == COMMENT_NODE) {\n              // Both nodes being compared are Text or Comment nodes\n              isCompatible = true;\n              // Simply update nodeValue on the original node to\n              // change the text value\n              if (curFromNodeChild.nodeValue !== curToNodeChild.nodeValue) {\n                curFromNodeChild.nodeValue = curToNodeChild.nodeValue;\n              }\n\n            }\n          }\n\n          if (isCompatible) {\n            // Advance both the \"to\" child and the \"from\" child since we found a match\n            // Nothing else to do as we already recursively called morphChildren above\n            curToNodeChild = toNextSibling;\n            curFromNodeChild = fromNextSibling;\n            continue outer;\n          }\n\n          // No compatible match so remove the old node from the DOM and continue trying to find a\n          // match in the original DOM. However, we only do this if the from node is not keyed\n          // since it is possible that a keyed node might match up with a node somewhere else in the\n          // target tree and we don't want to discard it just yet since it still might find a\n          // home in the final DOM tree. After everything is done we will remove any keyed nodes\n          // that didn't find a home\n          if (curFromNodeKey) {\n            // Since the node is keyed it might be matched up later so we defer\n            // the actual removal to later\n            addKeyedRemoval(curFromNodeKey);\n          } else {\n            // NOTE: we skip nested keyed nodes from being removed since there is\n            //       still a chance they will be matched up later\n            removeNode(curFromNodeChild, fromEl, true /* skip keyed nodes */);\n          }\n\n          curFromNodeChild = fromNextSibling;\n        } // END: while(curFromNodeChild) {}\n\n        // If we got this far then we did not find a candidate match for\n        // our \"to node\" and we exhausted all of the children \"from\"\n        // nodes. Therefore, we will just append the current \"to\" node\n        // to the end\n        if (curToNodeKey && (matchingFromEl = fromNodesLookup[curToNodeKey]) && compareNodeNames(matchingFromEl, curToNodeChild)) {\n          // MORPH\n          if(!skipFrom){ addChild(fromEl, matchingFromEl); }\n          morphEl(matchingFromEl, curToNodeChild);\n        } else {\n          var onBeforeNodeAddedResult = onBeforeNodeAdded(curToNodeChild);\n          if (onBeforeNodeAddedResult !== false) {\n            if (onBeforeNodeAddedResult) {\n              curToNodeChild = onBeforeNodeAddedResult;\n            }\n\n            if (curToNodeChild.actualize) {\n              curToNodeChild = curToNodeChild.actualize(fromEl.ownerDocument || doc);\n            }\n            addChild(fromEl, curToNodeChild);\n            handleNodeAdded(curToNodeChild);\n          }\n        }\n\n        curToNodeChild = toNextSibling;\n        curFromNodeChild = fromNextSibling;\n      }\n\n      cleanupFromEl(fromEl, curFromNodeChild, curFromNodeKey);\n\n      var specialElHandler = specialElHandlers[fromEl.nodeName];\n      if (specialElHandler) {\n        specialElHandler(fromEl, toEl);\n      }\n    } // END: morphChildren(...)\n\n    var morphedNode = fromNode;\n    var morphedNodeType = morphedNode.nodeType;\n    var toNodeType = toNode.nodeType;\n\n    if (!childrenOnly) {\n      // Handle the case where we are given two DOM nodes that are not\n      // compatible (e.g. <div> --> <span> or <div> --> TEXT)\n      if (morphedNodeType === ELEMENT_NODE) {\n        if (toNodeType === ELEMENT_NODE) {\n          if (!compareNodeNames(fromNode, toNode)) {\n            onNodeDiscarded(fromNode);\n            morphedNode = moveChildren(fromNode, createElementNS(toNode.nodeName, toNode.namespaceURI));\n          }\n        } else {\n          // Going from an element node to a text node\n          morphedNode = toNode;\n        }\n      } else if (morphedNodeType === TEXT_NODE || morphedNodeType === COMMENT_NODE) { // Text or comment node\n        if (toNodeType === morphedNodeType) {\n          if (morphedNode.nodeValue !== toNode.nodeValue) {\n            morphedNode.nodeValue = toNode.nodeValue;\n          }\n\n          return morphedNode;\n        } else {\n          // Text node to something else\n          morphedNode = toNode;\n        }\n      }\n    }\n\n    if (morphedNode === toNode) {\n      // The \"to node\" was not compatible with the \"from node\" so we had to\n      // toss out the \"from node\" and use the \"to node\"\n      onNodeDiscarded(fromNode);\n    } else {\n      if (toNode.isSameNode && toNode.isSameNode(morphedNode)) {\n        return;\n      }\n\n      morphEl(morphedNode, toNode, childrenOnly);\n\n      // We now need to loop over any keyed nodes that might need to be\n      // removed. We only do the removal if we know that the keyed node\n      // never found a match. When a keyed node is matched up we remove\n      // it out of fromNodesLookup and we use fromNodesLookup to determine\n      // if a keyed node has been matched up or not\n      if (keyedRemovalList) {\n        for (var i=0, len=keyedRemovalList.length; i<len; i++) {\n          var elToRemove = fromNodesLookup[keyedRemovalList[i]];\n          if (elToRemove) {\n            removeNode(elToRemove, elToRemove.parentNode, false);\n          }\n        }\n      }\n    }\n\n    if (!childrenOnly && morphedNode !== fromNode && fromNode.parentNode) {\n      if (morphedNode.actualize) {\n        morphedNode = morphedNode.actualize(fromNode.ownerDocument || doc);\n      }\n      // If we had to swap out the from node with a new node because the old\n      // node was not compatible with the target node then we need to\n      // replace the old DOM node in the original DOM tree. This is only\n      // possible if the original DOM node was part of a DOM tree which\n      // we know is the case if it has a parent node.\n      fromNode.parentNode.replaceChild(morphedNode, fromNode);\n    }\n\n    return morphedNode;\n  };\n}\n\nvar morphdom = morphdomFactory(morphAttrs);\n\nexport default morphdom;\n",
+        "//=============================================================================\n// AMD insanity... i hate javascript so much\n//\n// IGNORE EVERYTHING FROM HERE UNTIL THE COMMENT SAYING 'AND NOW IT BEGINS...\"\n//=============================================================================\n(function (root, factory) {\n    //@ts-ignore\n    if (typeof define === 'function' && define.amd) {\n        // AMD. Register as an anonymous module.\n        //@ts-ignore\n        define([], factory);\n    } else {\n        // Browser globals\n        root.Idiomorph = root.Idiomorph || factory();\n    }\n}(typeof self !== 'undefined' ? self : this,\n    function () {\n        return (function () {\n            'use strict';\n\n            //=============================================================================\n            // AND NOW IT BEGINS...\n            //=============================================================================\n            let EMPTY_SET = new Set();\n\n            //=============================================================================\n            // Core Morphing Algorithm - morph, morphNormalizedContent, morphOldNodeTo, morphChildren\n            //=============================================================================\n            function morph(oldNode, newContent, config = {}) {\n\n                if (oldNode instanceof Document) {\n                    oldNode = oldNode.documentElement;\n                }\n\n                if (typeof newContent === 'string') {\n                    newContent = parseContent(newContent);\n                }\n\n                let normalizedContent = normalizeContent(newContent);\n\n                let ctx = createMorphContext(oldNode, normalizedContent, config);\n\n                return morphNormalizedContent(oldNode, normalizedContent, ctx);\n            }\n\n            function morphNormalizedContent(oldNode, normalizedNewContent, ctx) {\n                if (ctx.head.block) {\n                    let oldHead = oldNode.querySelector('head');\n                    let newHead = normalizedNewContent.querySelector('head');\n                    if (oldHead && newHead) {\n                        let promises = handleHeadElement(newHead, oldHead, ctx);\n                        // when head promises resolve, call morph again, ignoring the head tag\n                        Promise.all(promises).then(function () {\n                            morphNormalizedContent(oldNode, normalizedNewContent, Object.assign(ctx, {\n                                head: {\n                                    block: false,\n                                    ignore: true\n                                }\n                            }));\n                        });\n                        return;\n                    }\n                }\n\n                if (ctx.morphStyle === \"innerHTML\") {\n\n                    // innerHTML, so we are only updating the children\n                    morphChildren(normalizedNewContent, oldNode, ctx);\n                    return oldNode.children;\n\n                } else if (ctx.morphStyle === \"outerHTML\" || ctx.morphStyle == null) {\n                    // otherwise find the best element match in the new content, morph that, and merge its siblings\n                    // into either side of the best match\n                    let bestMatch = findBestNodeMatch(normalizedNewContent, oldNode, ctx);\n\n                    // stash the siblings that will need to be inserted on either side of the best match\n                    let previousSibling = bestMatch?.previousSibling;\n                    let nextSibling = bestMatch?.nextSibling;\n\n                    // morph it\n                    let morphedNode = morphOldNodeTo(oldNode, bestMatch, ctx);\n\n                    if (bestMatch) {\n                        // if there was a best match, merge the siblings in too and return the\n                        // whole bunch\n                        return insertSiblings(previousSibling, morphedNode, nextSibling);\n                    } else {\n                        // otherwise nothing was added to the DOM\n                        return []\n                    }\n                } else {\n                    throw \"Do not understand how to morph style \" + ctx.morphStyle;\n                }\n            }\n\n\n\n            /**\n             * @param oldNode root node to merge content into\n             * @param newContent new content to merge\n             * @param ctx the merge context\n             * @returns {Element} the element that ended up in the DOM\n             */\n            function morphOldNodeTo(oldNode, newContent, ctx) {\n                if (ctx.ignoreActive && oldNode === document.activeElement) {\n                    // don't morph focused element\n                } else if (newContent == null) {\n                    ctx.callbacks.beforeNodeRemoved(oldNode);\n                    oldNode.remove();\n                    ctx.callbacks.afterNodeRemoved(oldNode);\n                    return null;\n                } else if (!isSoftMatch(oldNode, newContent)) {\n                    ctx.callbacks.beforeNodeRemoved(oldNode);\n                    ctx.callbacks.beforeNodeAdded(newContent);\n                    oldNode.parentElement.replaceChild(newContent, oldNode);\n                    ctx.callbacks.afterNodeAdded(newContent);\n                    ctx.callbacks.afterNodeRemoved(oldNode);\n                    return newContent;\n                } else {\n                    ctx.callbacks.beforeNodeMorphed(oldNode, newContent);\n                    if (oldNode instanceof HTMLHeadElement && ctx.head.ignore) {\n                        // ignore the head element\n                    } else if (oldNode instanceof HTMLHeadElement && ctx.head.style !== \"morph\") {\n                        handleHeadElement(newContent, oldNode, ctx);\n                    } else {\n                        syncNodeFrom(newContent, oldNode);\n                        morphChildren(newContent, oldNode, ctx);\n                    }\n                    ctx.callbacks.afterNodeMorphed(oldNode, newContent);\n                    return oldNode;\n                }\n            }\n\n            /**\n             * This is the core algorithm for matching up children.  The idea is to use id sets to try to match up\n             * nodes as faithfully as possible.  We greedily match, which allows us to keep the algorithm fast, but\n             * by using id sets, we are able to better match up with content deeper in the DOM.\n             *\n             * Basic algorithm is, for each node in the new content:\n             *\n             * - if we have reached the end of the old parent, append the new content\n             * - if the new content has an id set match with the current insertion point, morph\n             * - search for an id set match\n             * - if id set match found, morph\n             * - otherwise search for a \"soft\" match\n             * - if a soft match is found, morph\n             * - otherwise, prepend the new node before the current insertion point\n             *\n             * The two search algorithms terminate if competing node matches appear to outweigh what can be achieved\n             * with the current node.  See findIdSetMatch() and findSoftMatch() for details.\n             *\n             * @param {Element} newParent the parent element of the new content\n             * @param {Element } oldParent the old content that we are merging the new content into\n             * @param ctx the merge context\n             */\n            function morphChildren(newParent, oldParent, ctx) {\n\n                let nextNewChild = newParent.firstChild;\n                let insertionPoint = oldParent.firstChild;\n\n                // run through all the new content\n                while (nextNewChild) {\n\n                    let newChild = nextNewChild;\n                    nextNewChild = newChild.nextSibling;\n\n                    // if we are at the end of the exiting parent's children, just append\n                    if (insertionPoint == null) {\n\n                        ctx.callbacks.beforeNodeAdded(newChild);\n                        oldParent.appendChild(newChild);\n                        ctx.callbacks.afterNodeAdded(newChild);\n\n                        // if the current node has an id set match then morph\n                    } else if (isIdSetMatch(newChild, insertionPoint, ctx)) {\n\n                        morphOldNodeTo(insertionPoint, newChild, ctx);\n                        insertionPoint = insertionPoint.nextSibling;\n\n                    } else {\n\n                        // otherwise search forward in the existing old children for an id set match\n                        let idSetMatch = findIdSetMatch(newParent, oldParent, newChild, insertionPoint, ctx);\n\n                        // if we found a potential match, remove the nodes until that point and morph\n                        if (idSetMatch) {\n\n                            insertionPoint = removeNodesBetween(insertionPoint, idSetMatch, ctx);\n                            morphOldNodeTo(idSetMatch, newChild, ctx);\n\n                        } else {\n\n                            // no id set match found, so scan forward for a soft match for the current node\n                            let softMatch = findSoftMatch(newParent, oldParent, newChild, insertionPoint, ctx);\n\n                            // if we found a soft match for the current node, morph\n                            if (softMatch) {\n\n                                insertionPoint = removeNodesBetween(insertionPoint, softMatch, ctx);\n                                morphOldNodeTo(softMatch, newChild, ctx);\n\n                            } else {\n\n                                // abandon all hope of morphing, just insert the new child before the insertion point\n                                // and move on\n                                ctx.callbacks.beforeNodeAdded(newChild);\n                                oldParent.insertBefore(newChild, insertionPoint);\n                                ctx.callbacks.afterNodeAdded(newChild);\n\n                            }\n                        }\n                    }\n\n                    // remove the processed new contents ids from consideration in future merge decisions\n                    removeIdsFromConsideration(ctx, newChild);\n                }\n\n                // remove any remaining old nodes that didn't match up with new content\n                while (insertionPoint !== null) {\n\n                    let tempNode = insertionPoint;\n                    insertionPoint = insertionPoint.nextSibling;\n                    removeNode(tempNode, ctx);\n                }\n            }\n\n            //=============================================================================\n            // Attribute Syncing Code\n            //=============================================================================\n\n            /**\n             * syncs a given node with another node, copying over all attributes and\n             * inner element state from the 'from' node to the 'to' node\n             *\n             * @param {Element} from the element to copy attributes & state from\n             * @param {Element} to the element to copy attributes & state to\n             */\n            function syncNodeFrom(from, to) {\n                let type = from.nodeType\n\n                // if is an element type, sync the attributes from the\n                // new node into the new node\n                if (type === 1 /* element type */) {\n                    const fromAttributes = from.attributes;\n                    const toAttributes = to.attributes;\n                    for (const fromAttribute of fromAttributes) {\n                        if (to.getAttribute(fromAttribute.name) !== fromAttribute.value) {\n                            to.setAttribute(fromAttribute.name, fromAttribute.value);\n                        }\n                    }\n                    for (const toAttribute of toAttributes) {\n                        if (!from.hasAttribute(toAttribute.name)) {\n                            to.removeAttribute(toAttribute.name);\n                        }\n                    }\n                }\n\n                // sync text nodes\n                if (type === 8 /* comment */ || type === 3 /* text */) {\n                    if (to.nodeValue !== from.nodeValue) {\n                        to.nodeValue = from.nodeValue;\n                    }\n                }\n\n                // NB: many bothans died to bring us information:\n                //\n                // https://github.com/patrick-steele-idem/morphdom/blob/master/src/specialElHandlers.js\n                // https://github.com/choojs/nanomorph/blob/master/lib/morph.jsL113\n\n                // sync input value\n                if (from instanceof HTMLInputElement &&\n                    to instanceof HTMLInputElement &&\n                    from.type !== 'file') {\n\n                    let fromValue = from.value;\n                    let toValue = to.value;\n\n                    // sync boolean attributes\n                    syncBooleanAttribute(from, to, 'checked');\n                    syncBooleanAttribute(from, to, 'disabled');\n\n                    if (!from.hasAttribute('value')) {\n                        to.value = '';\n                        to.removeAttribute('value');\n                    } else if (fromValue !== toValue) {\n                        to.setAttribute('value', fromValue);\n                        to.value = fromValue;\n                    }\n                } else if (from instanceof HTMLOptionElement) {\n                    syncBooleanAttribute(from, to, 'selected')\n                } else if (from instanceof HTMLTextAreaElement && to instanceof HTMLTextAreaElement) {\n                    let fromValue = from.value;\n                    let toValue = to.value;\n                    if (fromValue !== toValue) {\n                        to.value = fromValue;\n                    }\n                    if (to.firstChild && to.firstChild.nodeValue !== fromValue) {\n                        to.firstChild.nodeValue = fromValue\n                    }\n                }\n            }\n\n            function syncBooleanAttribute(from, to, attributeName) {\n                if (from[attributeName] !== to[attributeName]) {\n                    to[attributeName] = from[attributeName];\n                    if (from[attributeName]) {\n                        to.setAttribute(attributeName, '');\n                    } else {\n                        to.removeAttribute(attributeName);\n                    }\n                }\n            }\n\n            //=============================================================================\n            // the HEAD tag can be handled specially, either w/ a 'merge' or 'append' style\n            //=============================================================================\n            function handleHeadElement(newHeadTag, currentHead, ctx) {\n\n                let added = []\n                let removed = []\n                let preserved = []\n                let nodesToAppend = []\n\n                let headMergeStyle = ctx.head.style;\n\n                // put all new head elements into a Map, by their outerHTML\n                let srcToNewHeadNodes = new Map();\n                for (const newHeadChild of newHeadTag.children) {\n                    srcToNewHeadNodes.set(newHeadChild.outerHTML, newHeadChild);\n                }\n\n                // for each elt in the current head\n                for (const currentHeadElt of currentHead.children) {\n\n                    // If the current head element is in the map\n                    let inNewContent = srcToNewHeadNodes.has(currentHeadElt.outerHTML);\n                    let isReAppended = ctx.head.shouldReAppend(currentHeadElt);\n                    let isPreserved = ctx.head.shouldPreserve(currentHeadElt);\n                    if (inNewContent || isPreserved) {\n                        if (isReAppended) {\n                            // remove the current version and let the new version replace it and re-execute\n                            removed.push(currentHeadElt);\n                        } else {\n                            // this element already exists and should not be re-appended, so remove it from\n                            // the new content map, preserving it in the DOM\n                            srcToNewHeadNodes.delete(currentHeadElt.outerHTML);\n                            preserved.push(currentHeadElt);\n                        }\n                    } else {\n                        if (headMergeStyle === \"append\") {\n                            // we are appending and this existing element is not new content\n                            // so if and only if it is marked for re-append do we do anything\n                            if (isReAppended) {\n                                removed.push(currentHeadElt);\n                                nodesToAppend.push(currentHeadElt);\n                            }\n                        } else {\n                            // if this is a merge, we remove this content since it is not in the new head\n                            if (ctx.head.shouldRemove(currentHeadElt) !== false) {\n                                removed.push(currentHeadElt);\n                            }\n                        }\n                    }\n                }\n\n                // Push the remaining new head elements in the Map into the\n                // nodes to append to the head tag\n                nodesToAppend.push(...srcToNewHeadNodes.values());\n                log(\"to append: \", nodesToAppend);\n\n                let promises = [];\n                for (const newNode of nodesToAppend) {\n                    log(\"adding: \", newNode);\n                    let newElt = document.createRange().createContextualFragment(newNode.outerHTML).firstChild;\n                    log(newElt);\n                    if (ctx.callbacks.beforeNodeAdded(newElt) !== false) {\n                        if (newElt.href || newElt.src) {\n                            let resolve = null;\n                            let promise = new Promise(function (_resolve) {\n                                resolve = _resolve;\n                            });\n                            newElt.addEventListener('load',function() {\n                                resolve();\n                            });\n                            promises.push(promise);\n                        }\n                        currentHead.appendChild(newElt);\n                        ctx.callbacks.afterNodeAdded(newElt);\n                        added.push(newElt);\n                    }\n                }\n\n                // remove all removed elements, after we have appended the new elements to avoid\n                // additional network requests for things like style sheets\n                for (const removedElement of removed) {\n                    if (ctx.callbacks.beforeNodeRemoved(removedElement) !== false) {\n                        currentHead.removeChild(removedElement);\n                        ctx.callbacks.afterNodeRemoved(removedElement);\n                    }\n                }\n\n                ctx.head.afterHeadMorphed(currentHead, {added: added, kept: preserved, removed: removed});\n                return promises;\n            }\n\n            //=============================================================================\n            // Misc\n            //=============================================================================\n\n            function log() {\n                //console.log(arguments);\n            }\n\n            function noOp() {}\n\n            function createMorphContext(oldNode, newContent, config) {\n                return {\n                    target:oldNode,\n                    newContent: newContent,\n                    config: config,\n                    morphStyle : config.morphStyle,\n                    ignoreActive : config.ignoreActive,\n                    idMap: createIdMap(oldNode, newContent),\n                    deadIds: new Set(),\n                    callbacks: Object.assign({\n                        beforeNodeAdded: noOp,\n                        afterNodeAdded : noOp,\n                        beforeNodeMorphed: noOp,\n                        afterNodeMorphed : noOp,\n                        beforeNodeRemoved: noOp,\n                        afterNodeRemoved : noOp,\n\n                    }, config.callbacks),\n                    head: Object.assign({\n                        style: 'merge',\n                        shouldPreserve : function(elt) {\n                            return elt.getAttribute(\"im-preserve\") === \"true\";\n                        },\n                        shouldReAppend : function(elt) {\n                            return elt.getAttribute(\"im-re-append\") === \"true\";\n                        },\n                        shouldRemove : noOp,\n                        afterHeadMorphed : noOp,\n                    }, config.head),\n                }\n            }\n\n            function isIdSetMatch(node1, node2, ctx) {\n                if (node1 == null || node2 == null) {\n                    return false;\n                }\n                if (node1.nodeType === node2.nodeType && node1.tagName === node2.tagName) {\n                    if (node1.id !== \"\" && node1.id === node2.id) {\n                        return true;\n                    } else {\n                        return getIdIntersectionCount(ctx, node1, node2) > 0;\n                    }\n                }\n                return false;\n            }\n\n            function isSoftMatch(node1, node2) {\n                if (node1 == null || node2 == null) {\n                    return false;\n                }\n                return node1.nodeType === node2.nodeType && node1.tagName === node2.tagName\n            }\n\n            function removeNodesBetween(startInclusive, endExclusive, ctx) {\n                while (startInclusive !== endExclusive) {\n                    let tempNode = startInclusive;\n                    startInclusive = startInclusive.nextSibling;\n                    removeNode(tempNode, ctx);\n                }\n                removeIdsFromConsideration(ctx, endExclusive);\n                return endExclusive.nextSibling;\n            }\n\n            //=============================================================================\n            // Scans forward from the insertionPoint in the old parent looking for a potential id match\n            // for the newChild.  We stop if we find a potential id match for the new child OR\n            // if the number of potential id matches we are discarding is greater than the\n            // potential id matches for the new child\n            //=============================================================================\n            function findIdSetMatch(newContent, oldParent, newChild, insertionPoint, ctx) {\n\n                // max id matches we are willing to discard in our search\n                let newChildPotentialIdCount = getIdIntersectionCount(ctx, newChild, oldParent);\n\n                let potentialMatch = null;\n\n                // only search forward if there is a possibility of an id match\n                if (newChildPotentialIdCount > 0) {\n                    let potentialMatch = insertionPoint;\n                    // if there is a possibility of an id match, scan forward\n                    // keep track of the potential id match count we are discarding (the\n                    // newChildPotentialIdCount must be greater than this to make it likely\n                    // worth it)\n                    let otherMatchCount = 0;\n                    while (potentialMatch != null) {\n\n                        // If we have an id match, return the current potential match\n                        if (isIdSetMatch(newChild, potentialMatch, ctx)) {\n                            return potentialMatch;\n                        }\n\n                        // computer the other potential matches of this new content\n                        otherMatchCount += getIdIntersectionCount(ctx, potentialMatch, newContent);\n                        if (otherMatchCount > newChildPotentialIdCount) {\n                            // if we have more potential id matches in _other_ content, we\n                            // do not have a good candidate for an id match, so return null\n                            return null;\n                        }\n\n                        // advanced to the next old content child\n                        potentialMatch = potentialMatch.nextSibling;\n                    }\n                }\n                return potentialMatch;\n            }\n\n            //=============================================================================\n            // Scans forward from the insertionPoint in the old parent looking for a potential soft match\n            // for the newChild.  We stop if we find a potential soft match for the new child OR\n            // if we find a potential id match in the old parents children OR if we find two\n            // potential soft matches for the next two pieces of new content\n            //=============================================================================\n            function findSoftMatch(newContent, oldParent, newChild, insertionPoint, ctx) {\n\n                let potentialSoftMatch = insertionPoint;\n                let nextSibling = newChild.nextSibling;\n                let siblingSoftMatchCount = 0;\n\n                while (potentialSoftMatch != null) {\n\n                    if (getIdIntersectionCount(ctx, potentialSoftMatch, newContent) > 0) {\n                        // the current potential soft match has a potential id set match with the remaining new\n                        // content so bail out of looking\n                        return null;\n                    }\n\n                    // if we have a soft match with the current node, return it\n                    if (isSoftMatch(newChild, potentialSoftMatch)) {\n                        return potentialSoftMatch;\n                    }\n\n                    if (isSoftMatch(nextSibling, potentialSoftMatch)) {\n                        // the next new node has a soft match with this node, so\n                        // increment the count of future soft matches\n                        siblingSoftMatchCount++;\n                        nextSibling = nextSibling.nextSibling;\n\n                        // If there are two future soft matches, bail to allow the siblings to soft match\n                        // so that we don't consume future soft matches for the sake of the current node\n                        if (siblingSoftMatchCount >= 2) {\n                            return null;\n                        }\n                    }\n\n                    // advanced to the next old content child\n                    potentialSoftMatch = potentialSoftMatch.nextSibling;\n                }\n\n                return potentialSoftMatch;\n            }\n\n            function parseContent(newContent) {\n                let parser = new DOMParser();\n\n                // remove svgs to avoid false-positive matches on head, etc.\n                let contentWithSvgsRemoved = newContent.replace(/<svg(\\s[^>]*>|>)([\\s\\S]*?)<\\/svg>/gim, '');\n\n                // if the newContent contains a html, head or body tag, we can simply parse it w/o wrapping\n                if (contentWithSvgsRemoved.match(/<\\/html>/) || contentWithSvgsRemoved.match(/<\\/head>/) || contentWithSvgsRemoved.match(/<\\/body>/)) {\n                    let content = parser.parseFromString(newContent, \"text/html\");\n                    // if it is a full HTML document, return the document itself as the parent container\n                    if (contentWithSvgsRemoved.match(/<\\/html>/)) {\n                        content.generatedByIdiomorph = true;\n                        return content;\n                    } else {\n                        // otherwise return the html element as the parent container\n                        let htmlElement = content.firstChild;\n                        if (htmlElement) {\n                            htmlElement.generatedByIdiomorph = true;\n                            return htmlElement;\n                        } else {\n                            return null;\n                        }\n                    }\n                } else {\n                    // if it is partial HTML, wrap it in a template tag to provide a parent element and also to help\n                    // deal with touchy tags like tr, tbody, etc.\n                    let responseDoc = parser.parseFromString(\"<body><template>\" + newContent + \"</template></body>\", \"text/html\");\n                    let content = responseDoc.body.querySelector('template').content;\n                    content.generatedByIdiomorph = true;\n                    return content\n                }\n            }\n\n            function normalizeContent(newContent) {\n                if (newContent == null) {\n                    // noinspection UnnecessaryLocalVariableJS\n                    const dummyParent = document.createElement('div');\n                    return dummyParent;\n                } else if (newContent.generatedByIdiomorph) {\n                    // the template tag created by idiomorph parsing can serve as a dummy parent\n                    return newContent;\n                } else if (newContent instanceof Node) {\n                    // a single node is added as a child to a dummy parent\n                    const dummyParent = document.createElement('div');\n                    dummyParent.append(newContent);\n                    return dummyParent;\n                } else {\n                    // all nodes in the array or HTMLElement collection are consolidated under\n                    // a single dummy parent element\n                    const dummyParent = document.createElement('div');\n                    for (const elt of [...newContent]) {\n                        dummyParent.append(elt);\n                    }\n                    return dummyParent;\n                }\n            }\n\n            function insertSiblings(previousSibling, morphedNode, nextSibling) {\n                let stack = []\n                let added = []\n                while (previousSibling != null) {\n                    stack.push(previousSibling);\n                    previousSibling = previousSibling.previousSibling;\n                }\n                while (stack.length > 0) {\n                    let node = stack.pop();\n                    added.push(node); // push added preceding siblings on in order and insert\n                    morphedNode.parentElement.insertBefore(node, morphedNode);\n                }\n                added.push(morphedNode);\n                while (nextSibling != null) {\n                    stack.push(nextSibling);\n                    added.push(nextSibling); // here we are going in order, so push on as we scan, rather than add\n                    nextSibling = nextSibling.nextSibling;\n                }\n                while (stack.length > 0) {\n                    morphedNode.parentElement.insertBefore(stack.pop(), morphedNode.nextSibling);\n                }\n                return added;\n            }\n\n            function findBestNodeMatch(newContent, oldNode, ctx) {\n                let currentElement;\n                currentElement = newContent.firstChild;\n                let bestElement = currentElement;\n                let score = 0;\n                while (currentElement) {\n                    let newScore = scoreElement(currentElement, oldNode, ctx);\n                    if (newScore > score) {\n                        bestElement = currentElement;\n                        score = newScore;\n                    }\n                    currentElement = currentElement.nextSibling;\n                }\n                return bestElement;\n            }\n\n            function scoreElement(node1, node2, ctx) {\n                if (isSoftMatch(node1, node2)) {\n                    return .5 + getIdIntersectionCount(ctx, node1, node2);\n                }\n                return 0;\n            }\n\n            function removeNode(tempNode, ctx) {\n                removeIdsFromConsideration(ctx, tempNode)\n                ctx.callbacks.beforeNodeRemoved(tempNode);\n                tempNode.remove();\n                ctx.callbacks.afterNodeRemoved(tempNode);\n            }\n\n            //=============================================================================\n            // ID Set Functions\n            //=============================================================================\n\n            function isIdInConsideration(ctx, id) {\n                return !ctx.deadIds.has(id);\n            }\n\n            function idIsWithinNode(ctx, id, targetNode) {\n                let idSet = ctx.idMap.get(targetNode) || EMPTY_SET;\n                return idSet.has(id);\n            }\n\n            function removeIdsFromConsideration(ctx, node) {\n                let idSet = ctx.idMap.get(node) || EMPTY_SET;\n                for (const id of idSet) {\n                    ctx.deadIds.add(id);\n                }\n            }\n\n            function getIdIntersectionCount(ctx, node1, node2) {\n                let sourceSet = ctx.idMap.get(node1) || EMPTY_SET;\n                let matchCount = 0;\n                for (const id of sourceSet) {\n                    // a potential match is an id in the source and potentialIdsSet, but\n                    // that has not already been merged into the DOM\n                    if (isIdInConsideration(ctx, id) && idIsWithinNode(ctx, id, node2)) {\n                        ++matchCount;\n                    }\n                }\n                return matchCount;\n            }\n\n            /**\n             * A bottom up algorithm that finds all elements with ids inside of the node\n             * argument and populates id sets for those nodes and all their parents, generating\n             * a set of ids contained within all nodes for the entire hierarchy in the DOM\n             *\n             * @param node {Element}\n             * @param {Map<Node, Set<String>>} idMap\n             */\n            function populateIdMapForNode(node, idMap) {\n                let nodeParent = node.parentElement;\n                // find all elements with an id property\n                let idElements = node.querySelectorAll('[id]');\n                for (const elt of idElements) {\n                    let current = elt;\n                    // walk up the parent hierarchy of that element, adding the id\n                    // of element to the parent's id set\n                    while (current !== nodeParent && current != null) {\n                        let idSet = idMap.get(current);\n                        // if the id set doesn't exist, create it and insert it in the  map\n                        if (idSet == null) {\n                            idSet = new Set();\n                            idMap.set(current, idSet);\n                        }\n                        idSet.add(elt.id);\n                        current = current.parentElement;\n                    }\n                }\n            }\n\n            /**\n             * This function computes a map of nodes to all ids contained within that node (inclusive of the\n             * node).  This map can be used to ask if two nodes have intersecting sets of ids, which allows\n             * for a looser definition of \"matching\" than tradition id matching, and allows child nodes\n             * to contribute to a parent nodes matching.\n             *\n             * @param {Element} oldContent  the old content that will be morphed\n             * @param {Element} newContent  the new content to morph to\n             * @returns {Map<Node, Set<String>>} a map of nodes to id sets for the\n             */\n            function createIdMap(oldContent, newContent) {\n                let idMap = new Map();\n                populateIdMapForNode(oldContent, idMap);\n                populateIdMapForNode(newContent, idMap);\n                return idMap;\n            }\n\n            //=============================================================================\n            // This is what ends up becoming the Idiomorph global object\n            //=============================================================================\n            return {\n                morph\n            }\n        })()\n    }));\n\n",
         "/*! *****************************************************************************\r\nCopyright (c) Microsoft Corporation. All rights reserved.\r\nLicensed under the Apache License, Version 2.0 (the \"License\"); you may not use\r\nthis file except in compliance with the License. You may obtain a copy of the\r\nLicense at http://www.apache.org/licenses/LICENSE-2.0\r\n\r\nTHIS CODE IS PROVIDED ON AN *AS IS* BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\r\nKIND, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION ANY IMPLIED\r\nWARRANTIES OR CONDITIONS OF TITLE, FITNESS FOR A PARTICULAR PURPOSE,\r\nMERCHANTABLITY OR NON-INFRINGEMENT.\r\n\r\nSee the Apache Version 2.0 License for specific language governing permissions\r\nand limitations under the License.\r\n***************************************************************************** */\r\n/* global Reflect, Promise */\r\n\r\nvar extendStatics = function(d, b) {\r\n    extendStatics = Object.setPrototypeOf ||\r\n        ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\r\n        function (d, b) { for (var p in b) if (b.hasOwnProperty(p)) d[p] = b[p]; };\r\n    return extendStatics(d, b);\r\n};\r\n\r\nfunction __extends(d, b) {\r\n    extendStatics(d, b);\r\n    function __() { this.constructor = d; }\r\n    d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\r\n}\r\n\r\nfunction __values(o) {\r\n    var m = typeof Symbol === \"function\" && o[Symbol.iterator], i = 0;\r\n    if (m) return m.call(o);\r\n    return {\r\n        next: function () {\r\n            if (o && i >= o.length) o = void 0;\r\n            return { value: o && o[i++], done: !o };\r\n        }\r\n    };\r\n}\r\n\r\nfunction __read(o, n) {\r\n    var m = typeof Symbol === \"function\" && o[Symbol.iterator];\r\n    if (!m) return o;\r\n    var i = m.call(o), r, ar = [], e;\r\n    try {\r\n        while ((n === void 0 || n-- > 0) && !(r = i.next()).done) ar.push(r.value);\r\n    }\r\n    catch (error) { e = { error: error }; }\r\n    finally {\r\n        try {\r\n            if (r && !r.done && (m = i[\"return\"])) m.call(i);\r\n        }\r\n        finally { if (e) throw e.error; }\r\n    }\r\n    return ar;\r\n}\r\n\r\nfunction __spread() {\r\n    for (var ar = [], i = 0; i < arguments.length; i++)\r\n        ar = ar.concat(__read(arguments[i]));\r\n    return ar;\r\n}\n\nvar Event = /** @class */ (function () {\r\n    function Event(type, target) {\r\n        this.target = target;\r\n        this.type = type;\r\n    }\r\n    return Event;\r\n}());\r\nvar ErrorEvent = /** @class */ (function (_super) {\r\n    __extends(ErrorEvent, _super);\r\n    function ErrorEvent(error, target) {\r\n        var _this = _super.call(this, 'error', target) || this;\r\n        _this.message = error.message;\r\n        _this.error = error;\r\n        return _this;\r\n    }\r\n    return ErrorEvent;\r\n}(Event));\r\nvar CloseEvent = /** @class */ (function (_super) {\r\n    __extends(CloseEvent, _super);\r\n    function CloseEvent(code, reason, target) {\r\n        if (code === void 0) { code = 1000; }\r\n        if (reason === void 0) { reason = ''; }\r\n        var _this = _super.call(this, 'close', target) || this;\r\n        _this.wasClean = true;\r\n        _this.code = code;\r\n        _this.reason = reason;\r\n        return _this;\r\n    }\r\n    return CloseEvent;\r\n}(Event));\n\n/*!\r\n * Reconnecting WebSocket\r\n * by Pedro Ladaria <pedro.ladaria@gmail.com>\r\n * https://github.com/pladaria/reconnecting-websocket\r\n * License MIT\r\n */\r\nvar getGlobalWebSocket = function () {\r\n    if (typeof WebSocket !== 'undefined') {\r\n        // @ts-ignore\r\n        return WebSocket;\r\n    }\r\n};\r\n/**\r\n * Returns true if given argument looks like a WebSocket class\r\n */\r\nvar isWebSocket = function (w) { return typeof w !== 'undefined' && !!w && w.CLOSING === 2; };\r\nvar DEFAULT = {\r\n    maxReconnectionDelay: 10000,\r\n    minReconnectionDelay: 1000 + Math.random() * 4000,\r\n    minUptime: 5000,\r\n    reconnectionDelayGrowFactor: 1.3,\r\n    connectionTimeout: 4000,\r\n    maxRetries: Infinity,\r\n    maxEnqueuedMessages: Infinity,\r\n    startClosed: false,\r\n    debug: false,\r\n};\r\nvar ReconnectingWebSocket = /** @class */ (function () {\r\n    function ReconnectingWebSocket(url, protocols, options) {\r\n        var _this = this;\r\n        if (options === void 0) { options = {}; }\r\n        this._listeners = {\r\n            error: [],\r\n            message: [],\r\n            open: [],\r\n            close: [],\r\n        };\r\n        this._retryCount = -1;\r\n        this._shouldReconnect = true;\r\n        this._connectLock = false;\r\n        this._binaryType = 'blob';\r\n        this._closeCalled = false;\r\n        this._messageQueue = [];\r\n        /**\r\n         * An event listener to be called when the WebSocket connection's readyState changes to CLOSED\r\n         */\r\n        this.onclose = null;\r\n        /**\r\n         * An event listener to be called when an error occurs\r\n         */\r\n        this.onerror = null;\r\n        /**\r\n         * An event listener to be called when a message is received from the server\r\n         */\r\n        this.onmessage = null;\r\n        /**\r\n         * An event listener to be called when the WebSocket connection's readyState changes to OPEN;\r\n         * this indicates that the connection is ready to send and receive data\r\n         */\r\n        this.onopen = null;\r\n        this._handleOpen = function (event) {\r\n            _this._debug('open event');\r\n            var _a = _this._options.minUptime, minUptime = _a === void 0 ? DEFAULT.minUptime : _a;\r\n            clearTimeout(_this._connectTimeout);\r\n            _this._uptimeTimeout = setTimeout(function () { return _this._acceptOpen(); }, minUptime);\r\n            _this._ws.binaryType = _this._binaryType;\r\n            // send enqueued messages (messages sent before websocket open event)\r\n            _this._messageQueue.forEach(function (message) { return _this._ws.send(message); });\r\n            _this._messageQueue = [];\r\n            if (_this.onopen) {\r\n                _this.onopen(event);\r\n            }\r\n            _this._listeners.open.forEach(function (listener) { return _this._callEventListener(event, listener); });\r\n        };\r\n        this._handleMessage = function (event) {\r\n            _this._debug('message event');\r\n            if (_this.onmessage) {\r\n                _this.onmessage(event);\r\n            }\r\n            _this._listeners.message.forEach(function (listener) { return _this._callEventListener(event, listener); });\r\n        };\r\n        this._handleError = function (event) {\r\n            _this._debug('error event', event.message);\r\n            _this._disconnect(undefined, event.message === 'TIMEOUT' ? 'timeout' : undefined);\r\n            if (_this.onerror) {\r\n                _this.onerror(event);\r\n            }\r\n            _this._debug('exec error listeners');\r\n            _this._listeners.error.forEach(function (listener) { return _this._callEventListener(event, listener); });\r\n            _this._connect();\r\n        };\r\n        this._handleClose = function (event) {\r\n            _this._debug('close event');\r\n            _this._clearTimeouts();\r\n            if (_this._shouldReconnect) {\r\n                _this._connect();\r\n            }\r\n            if (_this.onclose) {\r\n                _this.onclose(event);\r\n            }\r\n            _this._listeners.close.forEach(function (listener) { return _this._callEventListener(event, listener); });\r\n        };\r\n        this._url = url;\r\n        this._protocols = protocols;\r\n        this._options = options;\r\n        if (this._options.startClosed) {\r\n            this._shouldReconnect = false;\r\n        }\r\n        this._connect();\r\n    }\r\n    Object.defineProperty(ReconnectingWebSocket, \"CONNECTING\", {\r\n        get: function () {\r\n            return 0;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket, \"OPEN\", {\r\n        get: function () {\r\n            return 1;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket, \"CLOSING\", {\r\n        get: function () {\r\n            return 2;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket, \"CLOSED\", {\r\n        get: function () {\r\n            return 3;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"CONNECTING\", {\r\n        get: function () {\r\n            return ReconnectingWebSocket.CONNECTING;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"OPEN\", {\r\n        get: function () {\r\n            return ReconnectingWebSocket.OPEN;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"CLOSING\", {\r\n        get: function () {\r\n            return ReconnectingWebSocket.CLOSING;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"CLOSED\", {\r\n        get: function () {\r\n            return ReconnectingWebSocket.CLOSED;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"binaryType\", {\r\n        get: function () {\r\n            return this._ws ? this._ws.binaryType : this._binaryType;\r\n        },\r\n        set: function (value) {\r\n            this._binaryType = value;\r\n            if (this._ws) {\r\n                this._ws.binaryType = value;\r\n            }\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"retryCount\", {\r\n        /**\r\n         * Returns the number or connection retries\r\n         */\r\n        get: function () {\r\n            return Math.max(this._retryCount, 0);\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"bufferedAmount\", {\r\n        /**\r\n         * The number of bytes of data that have been queued using calls to send() but not yet\r\n         * transmitted to the network. This value resets to zero once all queued data has been sent.\r\n         * This value does not reset to zero when the connection is closed; if you keep calling send(),\r\n         * this will continue to climb. Read only\r\n         */\r\n        get: function () {\r\n            var bytes = this._messageQueue.reduce(function (acc, message) {\r\n                if (typeof message === 'string') {\r\n                    acc += message.length; // not byte size\r\n                }\r\n                else if (message instanceof Blob) {\r\n                    acc += message.size;\r\n                }\r\n                else {\r\n                    acc += message.byteLength;\r\n                }\r\n                return acc;\r\n            }, 0);\r\n            return bytes + (this._ws ? this._ws.bufferedAmount : 0);\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"extensions\", {\r\n        /**\r\n         * The extensions selected by the server. This is currently only the empty string or a list of\r\n         * extensions as negotiated by the connection\r\n         */\r\n        get: function () {\r\n            return this._ws ? this._ws.extensions : '';\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"protocol\", {\r\n        /**\r\n         * A string indicating the name of the sub-protocol the server selected;\r\n         * this will be one of the strings specified in the protocols parameter when creating the\r\n         * WebSocket object\r\n         */\r\n        get: function () {\r\n            return this._ws ? this._ws.protocol : '';\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"readyState\", {\r\n        /**\r\n         * The current state of the connection; this is one of the Ready state constants\r\n         */\r\n        get: function () {\r\n            if (this._ws) {\r\n                return this._ws.readyState;\r\n            }\r\n            return this._options.startClosed\r\n                ? ReconnectingWebSocket.CLOSED\r\n                : ReconnectingWebSocket.CONNECTING;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"url\", {\r\n        /**\r\n         * The URL as resolved by the constructor\r\n         */\r\n        get: function () {\r\n            return this._ws ? this._ws.url : '';\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    /**\r\n     * Closes the WebSocket connection or connection attempt, if any. If the connection is already\r\n     * CLOSED, this method does nothing\r\n     */\r\n    ReconnectingWebSocket.prototype.close = function (code, reason) {\r\n        if (code === void 0) { code = 1000; }\r\n        this._closeCalled = true;\r\n        this._shouldReconnect = false;\r\n        this._clearTimeouts();\r\n        if (!this._ws) {\r\n            this._debug('close enqueued: no ws instance');\r\n            return;\r\n        }\r\n        if (this._ws.readyState === this.CLOSED) {\r\n            this._debug('close: already closed');\r\n            return;\r\n        }\r\n        this._ws.close(code, reason);\r\n    };\r\n    /**\r\n     * Closes the WebSocket connection or connection attempt and connects again.\r\n     * Resets retry counter;\r\n     */\r\n    ReconnectingWebSocket.prototype.reconnect = function (code, reason) {\r\n        this._shouldReconnect = true;\r\n        this._closeCalled = false;\r\n        this._retryCount = -1;\r\n        if (!this._ws || this._ws.readyState === this.CLOSED) {\r\n            this._connect();\r\n        }\r\n        else {\r\n            this._disconnect(code, reason);\r\n            this._connect();\r\n        }\r\n    };\r\n    /**\r\n     * Enqueue specified data to be transmitted to the server over the WebSocket connection\r\n     */\r\n    ReconnectingWebSocket.prototype.send = function (data) {\r\n        if (this._ws && this._ws.readyState === this.OPEN) {\r\n            this._debug('send', data);\r\n            this._ws.send(data);\r\n        }\r\n        else {\r\n            var _a = this._options.maxEnqueuedMessages, maxEnqueuedMessages = _a === void 0 ? DEFAULT.maxEnqueuedMessages : _a;\r\n            if (this._messageQueue.length < maxEnqueuedMessages) {\r\n                this._debug('enqueue', data);\r\n                this._messageQueue.push(data);\r\n            }\r\n        }\r\n    };\r\n    /**\r\n     * Register an event handler of a specific event type\r\n     */\r\n    ReconnectingWebSocket.prototype.addEventListener = function (type, listener) {\r\n        if (this._listeners[type]) {\r\n            // @ts-ignore\r\n            this._listeners[type].push(listener);\r\n        }\r\n    };\r\n    ReconnectingWebSocket.prototype.dispatchEvent = function (event) {\r\n        var e_1, _a;\r\n        var listeners = this._listeners[event.type];\r\n        if (listeners) {\r\n            try {\r\n                for (var listeners_1 = __values(listeners), listeners_1_1 = listeners_1.next(); !listeners_1_1.done; listeners_1_1 = listeners_1.next()) {\r\n                    var listener = listeners_1_1.value;\r\n                    this._callEventListener(event, listener);\r\n                }\r\n            }\r\n            catch (e_1_1) { e_1 = { error: e_1_1 }; }\r\n            finally {\r\n                try {\r\n                    if (listeners_1_1 && !listeners_1_1.done && (_a = listeners_1.return)) _a.call(listeners_1);\r\n                }\r\n                finally { if (e_1) throw e_1.error; }\r\n            }\r\n        }\r\n        return true;\r\n    };\r\n    /**\r\n     * Removes an event listener\r\n     */\r\n    ReconnectingWebSocket.prototype.removeEventListener = function (type, listener) {\r\n        if (this._listeners[type]) {\r\n            // @ts-ignore\r\n            this._listeners[type] = this._listeners[type].filter(function (l) { return l !== listener; });\r\n        }\r\n    };\r\n    ReconnectingWebSocket.prototype._debug = function () {\r\n        var args = [];\r\n        for (var _i = 0; _i < arguments.length; _i++) {\r\n            args[_i] = arguments[_i];\r\n        }\r\n        if (this._options.debug) {\r\n            // not using spread because compiled version uses Symbols\r\n            // tslint:disable-next-line\r\n            console.log.apply(console, __spread(['RWS>'], args));\r\n        }\r\n    };\r\n    ReconnectingWebSocket.prototype._getNextDelay = function () {\r\n        var _a = this._options, _b = _a.reconnectionDelayGrowFactor, reconnectionDelayGrowFactor = _b === void 0 ? DEFAULT.reconnectionDelayGrowFactor : _b, _c = _a.minReconnectionDelay, minReconnectionDelay = _c === void 0 ? DEFAULT.minReconnectionDelay : _c, _d = _a.maxReconnectionDelay, maxReconnectionDelay = _d === void 0 ? DEFAULT.maxReconnectionDelay : _d;\r\n        var delay = 0;\r\n        if (this._retryCount > 0) {\r\n            delay =\r\n                minReconnectionDelay * Math.pow(reconnectionDelayGrowFactor, this._retryCount - 1);\r\n            if (delay > maxReconnectionDelay) {\r\n                delay = maxReconnectionDelay;\r\n            }\r\n        }\r\n        this._debug('next delay', delay);\r\n        return delay;\r\n    };\r\n    ReconnectingWebSocket.prototype._wait = function () {\r\n        var _this = this;\r\n        return new Promise(function (resolve) {\r\n            setTimeout(resolve, _this._getNextDelay());\r\n        });\r\n    };\r\n    ReconnectingWebSocket.prototype._getNextUrl = function (urlProvider) {\r\n        if (typeof urlProvider === 'string') {\r\n            return Promise.resolve(urlProvider);\r\n        }\r\n        if (typeof urlProvider === 'function') {\r\n            var url = urlProvider();\r\n            if (typeof url === 'string') {\r\n                return Promise.resolve(url);\r\n            }\r\n            if (!!url.then) {\r\n                return url;\r\n            }\r\n        }\r\n        throw Error('Invalid URL');\r\n    };\r\n    ReconnectingWebSocket.prototype._connect = function () {\r\n        var _this = this;\r\n        if (this._connectLock || !this._shouldReconnect) {\r\n            return;\r\n        }\r\n        this._connectLock = true;\r\n        var _a = this._options, _b = _a.maxRetries, maxRetries = _b === void 0 ? DEFAULT.maxRetries : _b, _c = _a.connectionTimeout, connectionTimeout = _c === void 0 ? DEFAULT.connectionTimeout : _c, _d = _a.WebSocket, WebSocket = _d === void 0 ? getGlobalWebSocket() : _d;\r\n        if (this._retryCount >= maxRetries) {\r\n            this._debug('max retries reached', this._retryCount, '>=', maxRetries);\r\n            return;\r\n        }\r\n        this._retryCount++;\r\n        this._debug('connect', this._retryCount);\r\n        this._removeListeners();\r\n        if (!isWebSocket(WebSocket)) {\r\n            throw Error('No valid WebSocket class provided');\r\n        }\r\n        this._wait()\r\n            .then(function () { return _this._getNextUrl(_this._url); })\r\n            .then(function (url) {\r\n            // close could be called before creating the ws\r\n            if (_this._closeCalled) {\r\n                return;\r\n            }\r\n            _this._debug('connect', { url: url, protocols: _this._protocols });\r\n            _this._ws = _this._protocols\r\n                ? new WebSocket(url, _this._protocols)\r\n                : new WebSocket(url);\r\n            _this._ws.binaryType = _this._binaryType;\r\n            _this._connectLock = false;\r\n            _this._addListeners();\r\n            _this._connectTimeout = setTimeout(function () { return _this._handleTimeout(); }, connectionTimeout);\r\n        });\r\n    };\r\n    ReconnectingWebSocket.prototype._handleTimeout = function () {\r\n        this._debug('timeout event');\r\n        this._handleError(new ErrorEvent(Error('TIMEOUT'), this));\r\n    };\r\n    ReconnectingWebSocket.prototype._disconnect = function (code, reason) {\r\n        if (code === void 0) { code = 1000; }\r\n        this._clearTimeouts();\r\n        if (!this._ws) {\r\n            return;\r\n        }\r\n        this._removeListeners();\r\n        try {\r\n            this._ws.close(code, reason);\r\n            this._handleClose(new CloseEvent(code, reason, this));\r\n        }\r\n        catch (error) {\r\n            // ignore\r\n        }\r\n    };\r\n    ReconnectingWebSocket.prototype._acceptOpen = function () {\r\n        this._debug('accept open');\r\n        this._retryCount = 0;\r\n    };\r\n    ReconnectingWebSocket.prototype._callEventListener = function (event, listener) {\r\n        if ('handleEvent' in listener) {\r\n            // @ts-ignore\r\n            listener.handleEvent(event);\r\n        }\r\n        else {\r\n            // @ts-ignore\r\n            listener(event);\r\n        }\r\n    };\r\n    ReconnectingWebSocket.prototype._removeListeners = function () {\r\n        if (!this._ws) {\r\n            return;\r\n        }\r\n        this._debug('removeListeners');\r\n        this._ws.removeEventListener('open', this._handleOpen);\r\n        this._ws.removeEventListener('close', this._handleClose);\r\n        this._ws.removeEventListener('message', this._handleMessage);\r\n        // @ts-ignore\r\n        this._ws.removeEventListener('error', this._handleError);\r\n    };\r\n    ReconnectingWebSocket.prototype._addListeners = function () {\r\n        if (!this._ws) {\r\n            return;\r\n        }\r\n        this._debug('addListeners');\r\n        this._ws.addEventListener('open', this._handleOpen);\r\n        this._ws.addEventListener('close', this._handleClose);\r\n        this._ws.addEventListener('message', this._handleMessage);\r\n        // @ts-ignore\r\n        this._ws.addEventListener('error', this._handleError);\r\n    };\r\n    ReconnectingWebSocket.prototype._clearTimeouts = function () {\r\n        clearTimeout(this._connectTimeout);\r\n        clearTimeout(this._uptimeTimeout);\r\n    };\r\n    return ReconnectingWebSocket;\r\n}());\n\nexport default ReconnectingWebSocket;\n",
-        "const BOOST_PAGES = JSON.parse(\n  document.querySelector(\"meta[name=reactor-boost]\")?.dataset.enabled || \"false\"\n);\nconsole.log(\"BOOST_PAGES\", BOOST_PAGES);\n\nfunction boostAllLinks() {\n  if (BOOST_PAGES) {\n    for (let link of document.querySelectorAll(\"a[href]\")) {\n      boostElement(link);\n    }\n  }\n}\n\n/**\n * Intercepts a clicks on links and loads them from cache and then network\n * @param {HTMLElement} element\n */\nfunction boostElement(element) {\n  if (BOOST_PAGES) {\n    if (\n      element.tagName?.toLowerCase() === \"a\" &&\n      element.hasAttribute(\"href\") &&\n      !(\n        element.boosted ||\n        element.hasAttribute(\"onclick\") ||\n        element.hasAttribute(\"target\") ||\n        element.hasAttribute(\":no-boost\")\n      )\n    ) {\n      element.boosted = true;\n      element.addEventListener(\"click\", _load);\n    }\n  }\n}\n\n/**\n * Event handler for links\n * @param {MouseEvent} event\n */\nfunction _load(event) {\n  event.preventDefault();\n  let url =\n    event.target.tagName?.toLowerCase === \"a\"\n      ? event.target.href\n      : event.target.closest(\"a\").href;\n  HistoryCache.load(url);\n}\n\nfunction replaceBodyContent(withHtmlContent, options) {\n  console.log(\"replaceBodyContent\", options);\n  let html = document.createElement(\"html\");\n  html.innerHTML = withHtmlContent;\n  window.requestAnimationFrame(() => {\n    if (options?.beforeReplace) options.beforeReplace(html);\n    document.body = html.querySelector(\"body\");\n    boostAllLinks();\n    if (options?.afterReplace) options.afterReplace(html);\n    document.querySelector(\"[autofocus]\")?.focus();\n  });\n}\n\nfunction hasSameOriginAsDocument(url) {\n  if (url.startsWith(\"http://\") || url.startsWith(\"https://\")) {\n    return new URL(url).origin === document.location.origin;\n  } else {\n    return true;\n  }\n}\n\nclass HistoryCache {\n  /**  @type {Array<{url: String, content: String, title: String, scroll: Number}>} */\n  static maxSize = 10;\n  static cache = [];\n  static currentPath = window.location.pathname + window.location.search;\n\n  static async load(url) {\n    if (BOOST_PAGES) {\n      this._saveCurrentPage();\n      console.log(url);\n      if (hasSameOriginAsDocument(url)) {\n        this.push(url);\n        await this.restoreFromCurrentPath();\n      } else {\n        location.assign(url);\n      }\n    } else {\n      location.assign(url);\n    }\n  }\n\n  static async restoreFromCurrentPath() {\n    this._saveCurrentPage();\n    let path = window.location.pathname + window.location.search;\n    console.log(\"Restoring Page:\", path);\n    let page = this._get(path);\n    if (page) {\n      replaceBodyContent(page.content, {\n        beforeReplace() {\n          document.title = page.title;\n        },\n        afterReplace() {\n          window.scrollTo(0, page.scroll);\n        },\n      });\n      console.log(\"currentPath\", path);\n      this.currentPath = path;\n    }\n\n    // I don't care if the page is restored or came from the network\n    // This will pull the page from the server just in case of any change\n\n    let response = await fetch(window.location.href);\n    let content = await response.text();\n    this.replace(response.url);\n    replaceBodyContent(content, {\n      beforeReplace(html) {\n        document.title = html.querySelector(\"title\")?.text ?? \"\";\n      },\n      afterReplace() {\n        HistoryCache._saveCurrentPage();\n      },\n    });\n  }\n\n  static back() {\n    window.history.back();\n  }\n\n  static push(path) {\n    history.pushState({}, document.title, path);\n    this.currentPath = path;\n  }\n\n  static replace(path) {\n    history.replaceState({}, document.title, path);\n    this.currentPath = path;\n  }\n\n  static _saveCurrentPage() {\n    console.log(\"Saving page:\", this.currentPath);\n\n    // Remove path from the history cache if is already existed\n    this.cache = this.cache.filter(({ url }) => url != this.currentPath);\n\n    // Put the new entry in the cache\n    this.cache.push({\n      url: this.currentPath,\n      content: document.body.outerHTML,\n      title: document.title,\n      scroll: window.scrollY,\n    });\n\n    // Keep the history at a reasonable size\n    if (this.cache.length > this.maxSize) {\n      let page = this.cache.shift();\n      console.log(\"Evicted:\", page.url);\n    }\n\n    console.log(\n      \"Currently cached:\",\n      this.cache.map(({ url }) => url)\n    );\n  }\n\n  static _get(path) {\n    return this.cache.find((page) => page.url == path);\n  }\n}\n\nwindow.addEventListener(\"popstate\", (event) => {\n  HistoryCache.restoreFromCurrentPath();\n});\n\nwindow.addEventListener(\"load\", () => {\n  boostAllLinks();\n});\n\nexport default {\n  boostElement,\n  HistoryCache: HistoryCache,\n};\n",
-        "import morphdom from \"morphdom\";\nimport ReconnectingWebSocket from \"reconnecting-websocket\";\nimport boost from \"./reactor-boost\";\n\n// Connection\n\nconst parser = new DOMParser();\n\nclass ServerConnection extends EventTarget {\n  open(path = \"__reactor__\") {\n    let protocol = location.protocol.replace(\"http\", \"ws\");\n    this.socket = new ReconnectingWebSocket(\n      `${protocol}//${location.host}/${path}`,\n      [],\n      {\n        maxEnqueuedMessages: 0,\n      }\n    );\n\n    this.socket.addEventListener(\"open\", () => {\n      console.log(\"WS: OPEN\");\n      this.dispatchEvent(new Event(\"open\"));\n    });\n\n    this.socket.addEventListener(\"message\", (event) =>\n      this._processMessage(event)\n    );\n\n    this.socket.addEventListener(\"close\", () => {\n      console.log(\"WS: CLOSE\");\n      this.dispatchEvent(new Event(\"close\"));\n    });\n  }\n\n  get isOpen() {\n    return this.socket?.readyState == ReconnectingWebSocket.OPEN;\n  }\n\n  _processMessage(event) {\n    let { command, payload } = JSON.parse(event.data);\n    switch (command) {\n      case \"render\":\n        var { id, diff } = payload;\n        console.log(\"<<< RENDER\", id);\n        document.getElementById(id)?.applyDiff(diff);\n        break;\n      case \"append\":\n      case \"prepend\":\n      case \"insert_after\":\n      case \"insert_before\":\n      case \"replace_with\":\n        var { id, html } = payload;\n        console.log(`<<< ${command.toUpperCase()}`, id);\n        html = parser.parseFromString(html, \"text/html\").body.firstChild;\n        var element = document.getElementById(id);\n        switch (command) {\n          case \"append\":\n            element?.append(html);\n            break;\n          case \"prepend\":\n            element?.prepend(html);\n            break;\n          case \"insert_after\":\n            element?.after(html);\n            break;\n          case \"insert_before\":\n            element?.before(html);\n            break;\n          case \"replace_with\":\n            element?.replaceWith(html);\n            break;\n        }\n        break;\n      case \"remove\":\n        var { id } = payload;\n        console.log(\"<<< REMOVE\", id);\n        document.getElementById(id)?.remove();\n        break;\n      case \"focus_on\":\n        var { selector } = payload;\n        console.log(\"<<< FOCUS-ON\", `\"${selector}\"`, document.querySelector(selector));\n        window.requestAnimationFrame(() =>\n          document.querySelector(selector)?.focus())\n        break;\n      case \"scroll_into_view\":\n        var { id, behavior, block, inline } = payload;\n        window.requestAnimationFrame(() =>\n          document\n            .getElementById(id)\n            ?.scrollIntoView({ behavior, block, inline }))\n        break;\n      case \"url_change\":\n        var { url } = payload;\n        console.log(\"<< URL\", payload.command, url);\n        switch (payload.command) {\n          case \"redirect\":\n            boost.HistoryCache.load(url);\n            break;\n          case \"replace\":\n            boost.HistoryCache.replace(url);\n            break;\n          case \"push\":\n            boost.HistoryCache.push(url);\n            break;\n        }\n        break;\n      case \"set_url_params\":\n        console.log(\"<< SET URL PARAMS\", payload);\n\n        // \"?a=x&...\" -> \"a=x&...\"\n        let searchParams = document.location.search.slice(1);\n\n        let currentParams = {};\n        if (searchParams.length) {\n          currentParams = searchParams\n            .split(\"&\") // [\"a=x\", ...]\n            .map((x) => x.split(\"=\")) // [[\"a\", \"x\"], ...]\n            .reduce(\n              // {a: \"x\", ...}\n              (acc, data) => {\n                let [key, value] = data;\n                acc[key] =\n                  value === undefined ? undefined : decodeURIComponent(value);\n                return acc;\n              },\n              {}\n            );\n        }\n\n        let newParams = Object.entries(\n          Object.assign(currentParams, payload)\n        ).map((key_value) => {\n          let [key, value] = key_value;\n          return (\n            key + (value === undefined ? \"\" : `=${encodeURIComponent(value)}`)\n          );\n        });\n\n        let newpath = document.location.pathname;\n        if (newParams.length) {\n          newpath += \"?\" + newParams.join(\"&\");\n        }\n        boost.HistoryCache.replace(newpath);\n        break;\n\n      case \"back\":\n        boost.HistoryCache.back();\n        break;\n      default:\n        console.error(`Unknown command \"${command}\"`, payload);\n    }\n  }\n\n  sendJoin(name, parent_id, state) {\n    this._send(\"join\", { name, parent_id, state });\n  }\n\n  sendLeave(id) {\n    console.log(\">>> LEAVE\", id);\n    this._send(\"leave\", { id });\n  }\n\n  sendUserEvent(id, command, implicit_args, explicit_args) {\n    console.log(\">>> USER_EVENT\", id, command, explicit_args);\n    this._send(\"user_event\", { id, command, implicit_args, explicit_args });\n  }\n\n  _send(command, payload) {\n    if (this.isOpen) {\n      this.socket.send(JSON.stringify({ command, payload }));\n    }\n  }\n}\n\nlet connection = new ServerConnection();\n\nfor ({ dataset } of document.querySelectorAll(\"meta[name=reactor-component]\")) {\n  let baseElement = document.createElement(dataset.extends);\n\n  class ReactorComponent extends baseElement.constructor {\n    constructor(...args) {\n      super(...args);\n      this._lastReceivedHtml = [];\n      this.joinBind = () => this.join();\n      this.wentOffline = () => this.classList.add(\"reactor-disconnected\");\n    }\n\n    connectedCallback() {\n      connection.addEventListener(\"open\", this.joinBind);\n      connection.addEventListener(\"close\", this.wentOffline);\n      this.join();\n    }\n\n    disconnectedCallback() {\n      connection.removeEventListener(\"open\", this.joinBind);\n      connection.removeEventListener(\"close\", this.wentOffline);\n      connection.sendLeave(this.id);\n    }\n\n    join() {\n      this.classList.remove(\"reactor-disconnected\");\n      connection.sendJoin(this.dataset.name, this.parentId, this.dataset.state);\n    }\n\n    applyDiff(diff) {\n      let html = this.getHtml(diff);\n      window.requestAnimationFrame(() => {\n        morphdom(this, html, {\n          onBeforeNodeAdded(node) {\n            boost.boostElement(node);\n          },\n          onElUpdated(node) {\n            boost.boostElement(node);\n          },\n        });\n      });\n    }\n\n    getHtml(diff) {\n      let fragments = [];\n      let cursor = 0;\n      for (let fragment of diff) {\n        if (typeof fragment === \"string\") {\n          fragments.push(fragment);\n        } else if (fragment < 0) {\n          cursor -= fragment;\n        } else {\n          fragments.push(\n            ...this._lastReceivedHtml.slice(cursor, cursor + fragment)\n          );\n          cursor += fragment;\n        }\n      }\n      this._lastReceivedHtml = fragments;\n      return fragments.join(\" \");\n    }\n\n    /**\n     * Returns the id of the parent component\n     *\n     * @returns {?String}\n     */\n    get parentId() {\n      return this.parentComponent?.id;\n    }\n\n    /**\n     * Returns the high parent reactor component if any is found component\n     *\n     * @returns {?ReactorComponent}\n     */\n    get parentComponent() {\n      return this.parentElement?.closest(\"[reactor-component]\");\n    }\n\n    /**\n     * Dispatches a command to this component and sends it to the backend\n     * @param {String} command\n     * @param {Object} args\n     * @param {?HTMLFormElement} form\n     */\n    dispatch(command, args, formScope) {\n      connection.sendUserEvent(\n        this.id,\n        command,\n        this.serialize(formScope),\n        args\n      );\n    }\n\n    /**\n     * Serialize all elements inside `element` with a [name] attribute into\n     * a an array of `[element[name], element[value]]`\n     * @param {HTMLElement} element\n     */\n    serialize(element) {\n      let result = {};\n      for (let el of element.querySelectorAll(\"[name]\")) {\n        // Avoid serializing data of a nested component\n        if (el.closest(\"[reactor-component]\") !== this) {\n          continue;\n        }\n\n        let value = null;\n        switch (el.type.toLowerCase()) {\n          case \"checkbox\":\n          case \"radio\":\n            value = el.checked ? el.value || true : null;\n            break;\n          case \"select-multiple\":\n            value = el.selectedOptions.map((option) => option.value);\n            break;\n          default:\n            value = el.value;\n            break;\n        }\n\n        if (value !== null) {\n          let key = el.getAttribute(\"name\");\n          let values = result[key] ?? [];\n          values.push(value);\n          result[key] = values;\n        }\n      }\n      return result;\n    }\n  }\n\n  customElements.define(dataset.tagName, ReactorComponent, {\n    extends: dataset.extends,\n  });\n}\n\nconnection.open();\ndebounceTimeouts = {};\n\nwindow.reactor = {\n  /**\n   * Forwards a user event to a component\n   * @param {HTMLElement} element\n   * @param {String} name\n   * @param {Object} args\n   */\n  send(element, name, args) {\n    let component = element.closest(\"[reactor-component]\");\n    if (component !== null) {\n      let form = element.closest(\"form\");\n      let formScope = component.contains(form) ? form : component;\n      component.dispatch(name, args, formScope);\n    }\n  },\n\n  /**\n   * Debounce a function call\n   * @param {String} delayName\n   * @param {Number} delay\n   * @returns\n   */\n  debounce(delayName, delay) {\n    return (f) => {\n      return (...args) => {\n        clearTimeout(debounceTimeouts[delayName]);\n        debounceTimeouts[delayName] = setTimeout(() => f(...args), delay);\n      };\n    };\n  },\n};\n"
+        "import idiomorph from \"idiomorph\";\n\nconsole.log(idiomorph);\n\nfunction morph(oldNode, newNode) {\n  newJoiners = new Set();\n  Idiomorph.morph(oldNode, newNode, {\n    ignoreActive: true,\n    callbacks: {\n      beforeNodeMorphed: function (oldNode, newNode) {\n        if (\n          oldNode instanceof HTMLElement &&\n          newNode instanceof HTMLElement &&\n          oldNode.hasAttribute(\"reactor-component\") &&\n          newNode.hasAttribute(\"reactor-component\") &&\n          oldNode.id !== newNode.id\n        ) {\n          oldNode.leave();\n          newJoiners.add(newNode.id);\n        }\n      },\n      afterNodeMorphed: function (oldNode, newNode) {\n        if (newJoiners.has(oldNode.id)) {\n          oldNode.join();\n        }\n      },\n    },\n  });\n}\n\nconst BOOST_PAGES = JSON.parse(\n  document.querySelector(\"meta[name=reactor-boost]\")?.dataset.enabled || \"false\"\n);\n\nconsole.log(\"BOOST_PAGES\", BOOST_PAGES);\n\nif (BOOST_PAGES) {\n  document.addEventListener(\"click\", (e) => {\n    let link = e.target;\n    link = link.tagName.toLowerCase() !== \"a\" ? link.closest(\"a\") : link;\n    if (\n      link &&\n      link.href &&\n      (!link.target || link.target === \"_self\") &&\n      link.origin == document.location.origin &&\n      e.button === 0 && // left click only\n      !e.metaKey && // open in new tab (mac)\n      !e.ctrlKey && // open in new tab (win & linux)\n      !e.altKey && // download\n      !e.shiftKey\n    ) {\n      e.preventDefault();\n      HistoryCache.load(link.href);\n    }\n  });\n}\n\nfunction replaceBodyContent(withHtmlContent, scrollY = undefined) {\n  let html = new DOMParser().parseFromString(withHtmlContent, \"text/html\");\n  document.title = html.querySelector(\"title\")?.text ?? \"\";\n  morph(document.body, html.body);\n  if (scrollY === undefined) {\n    document.querySelector(\"[autofocus]\")?.focus();\n  } else {\n    window.scrollTo(0, scrollY);\n  }\n}\n\nfunction hasSameOriginAsDocument(url) {\n  if (url.startsWith(\"http://\") || url.startsWith(\"https://\")) {\n    return new URL(url).origin === document.location.origin;\n  } else {\n    return true;\n  }\n}\n\nclass HistoryCache {\n  static async load(url) {\n    if (BOOST_PAGES) {\n      // this._saveCurrentPage();\n      if (hasSameOriginAsDocument(url)) {\n        this.push(url);\n      } else {\n        document.location.assign(url);\n      }\n    } else {\n      document.location.assign(url);\n    }\n  }\n\n  static back() {\n    window.history.back();\n  }\n\n  static async push(path) {\n    history.replaceState(\n      {\n        content: document.body.outerHTML,\n        scrollY: window.scrollY,\n      },\n      document.title,\n      document.location.href\n    );\n    let response = await fetch(path);\n    let content = await response.text();\n    history.pushState({}, document.title, path);\n    replaceBodyContent(content);\n  }\n\n  static replace(path) {\n    history.replaceState({}, document.title, path);\n  }\n}\n\nwindow.addEventListener(\"popstate\", (event) => {\n  if (event.state?.content !== undefined) {\n    replaceBodyContent(event.state.content, event.state.scrollY);\n  }\n  fetch(document.location.href)\n    .then((response) => response.text())\n    .then((content) => replaceBodyContent(content));\n});\n\nexport default {\n  HistoryCache: HistoryCache,\n  morph: morph,\n};\n",
+        "import ReconnectingWebSocket from \"reconnecting-websocket\";\nimport boost from \"./reactor-boost\";\n\n// Connection\n\nconst parser = new DOMParser();\n\nclass ServerConnection extends EventTarget {\n  open(path = \"__reactor__\") {\n    let protocol = location.protocol.replace(\"http\", \"ws\");\n    this.socket = new ReconnectingWebSocket(\n      `${protocol}//${location.host}/${path}`,\n      [],\n      {\n        maxEnqueuedMessages: 0,\n      }\n    );\n\n    this.socket.addEventListener(\"open\", () => {\n      console.log(\"WS: OPEN\");\n      this.dispatchEvent(new Event(\"open\"));\n    });\n\n    this.socket.addEventListener(\"message\", (event) =>\n      this._processMessage(event)\n    );\n\n    this.socket.addEventListener(\"close\", () => {\n      console.log(\"WS: CLOSE\");\n      this.dispatchEvent(new Event(\"close\"));\n    });\n  }\n\n  get isOpen() {\n    return this.socket?.readyState == ReconnectingWebSocket.OPEN;\n  }\n\n  _processMessage(event) {\n    let { command, payload } = JSON.parse(event.data);\n    switch (command) {\n      case \"render\":\n        var { id, diff } = payload;\n        console.log(\"<<< RENDER\", id);\n        document.getElementById(id)?.applyDiff(diff);\n        break;\n      case \"append\":\n      case \"prepend\":\n      case \"insert_after\":\n      case \"insert_before\":\n      case \"replace_with\":\n        var { id, html } = payload;\n        console.log(`<<< ${command.toUpperCase()}`, id);\n        html = parser.parseFromString(html, \"text/html\").body.firstChild;\n        var element = document.getElementById(id);\n        switch (command) {\n          case \"append\":\n            element?.append(html);\n            break;\n          case \"prepend\":\n            element?.prepend(html);\n            break;\n          case \"insert_after\":\n            element?.after(html);\n            break;\n          case \"insert_before\":\n            element?.before(html);\n            break;\n          case \"replace_with\":\n            element?.replaceWith(html);\n            break;\n        }\n        break;\n      case \"remove\":\n        var { id } = payload;\n        console.log(\"<<< REMOVE\", id);\n        document.getElementById(id)?.remove();\n        break;\n      case \"focus_on\":\n        var { selector } = payload;\n        console.log(\n          \"<<< FOCUS-ON\",\n          `\"${selector}\"`,\n          document.querySelector(selector)\n        );\n        window.requestAnimationFrame(() =>\n          document.querySelector(selector)?.focus()\n        );\n        break;\n      case \"scroll_into_view\":\n        var { id, behavior, block, inline } = payload;\n        window.requestAnimationFrame(() =>\n          document\n            .getElementById(id)\n            ?.scrollIntoView({ behavior, block, inline })\n        );\n        break;\n      case \"url_change\":\n        var { url } = payload;\n        console.log(\"<< URL\", payload.command, url);\n        switch (payload.command) {\n          case \"redirect\":\n            boost.HistoryCache.load(url);\n            break;\n          case \"replace\":\n            boost.HistoryCache.replace(url);\n            break;\n          case \"push\":\n            boost.HistoryCache.push(url);\n            break;\n        }\n        break;\n      case \"set_url_params\":\n        console.log(\"<< SET URL PARAMS\", payload);\n\n        // \"?a=x&...\" -> \"a=x&...\"\n        let searchParams = document.location.search.slice(1);\n\n        let currentParams = {};\n        if (searchParams.length) {\n          currentParams = searchParams\n            .split(\"&\") // [\"a=x\", ...]\n            .map((x) => x.split(\"=\")) // [[\"a\", \"x\"], ...]\n            .reduce(\n              // {a: \"x\", ...}\n              (acc, data) => {\n                let [key, value] = data;\n                acc[key] =\n                  value === undefined ? undefined : decodeURIComponent(value);\n                return acc;\n              },\n              {}\n            );\n        }\n\n        let newParams = Object.entries(\n          Object.assign(currentParams, payload)\n        ).map((key_value) => {\n          let [key, value] = key_value;\n          return (\n            key + (value === undefined ? \"\" : `=${encodeURIComponent(value)}`)\n          );\n        });\n\n        let newpath = document.location.pathname;\n        if (newParams.length) {\n          newpath += \"?\" + newParams.join(\"&\");\n        }\n        boost.HistoryCache.replace(newpath);\n        break;\n\n      case \"back\":\n        boost.HistoryCache.back();\n        break;\n      default:\n        console.error(`Unknown command \"${command}\"`, payload);\n    }\n  }\n\n  sendJoin(name, parent_id, state) {\n    this._send(\"join\", { name, parent_id, state });\n  }\n\n  sendLeave(id) {\n    console.log(\">>> LEAVE\", id);\n    this._send(\"leave\", { id });\n  }\n\n  sendUserEvent(id, command, implicit_args, explicit_args) {\n    console.log(\">>> USER_EVENT\", id, command, explicit_args);\n    this._send(\"user_event\", { id, command, implicit_args, explicit_args });\n  }\n\n  _send(command, payload) {\n    if (this.isOpen) {\n      this.socket.send(JSON.stringify({ command, payload }));\n    }\n  }\n}\n\nlet connection = new ServerConnection();\n\nfor ({ dataset } of document.querySelectorAll(\"meta[name=reactor-component]\")) {\n  let baseElement = document.createElement(dataset.extends);\n\n  class ReactorComponent extends baseElement.constructor {\n    constructor(...args) {\n      super(...args);\n      this._lastReceivedHtml = [];\n      this.joinBind = () => this.join();\n      this.wentOffline = () => this.classList.add(\"reactor-disconnected\");\n    }\n\n    connectedCallback() {\n      connection.addEventListener(\"open\", this.joinBind);\n      connection.addEventListener(\"close\", this.wentOffline);\n      this.join();\n    }\n\n    disconnectedCallback() {\n      connection.removeEventListener(\"open\", this.joinBind);\n      connection.removeEventListener(\"close\", this.wentOffline);\n      this.leave();\n    }\n\n    join() {\n      this.classList.remove(\"reactor-disconnected\");\n      connection.sendJoin(this.dataset.name, this.parentId, this.dataset.state);\n    }\n\n    leave() {\n      connection.sendLeave(this.id);\n    }\n\n    applyDiff(diff) {\n      window.requestAnimationFrame(() => {\n        let html = this.getHtml(diff);\n        boost.morph(this, html);\n      });\n    }\n\n    getHtml(diff) {\n      let fragments = [];\n      let cursor = 0;\n      for (let fragment of diff) {\n        if (typeof fragment === \"string\") {\n          fragments.push(fragment);\n        } else if (fragment < 0) {\n          cursor -= fragment;\n        } else {\n          fragments.push(\n            ...this._lastReceivedHtml.slice(cursor, cursor + fragment)\n          );\n          cursor += fragment;\n        }\n      }\n      this._lastReceivedHtml = fragments;\n      return fragments.join(\" \");\n    }\n\n    /**\n     * Returns the id of the parent component\n     *\n     * @returns {?String}\n     */\n    get parentId() {\n      return this.parentComponent?.id;\n    }\n\n    /**\n     * Returns the high parent reactor component if any is found component\n     *\n     * @returns {?ReactorComponent}\n     */\n    get parentComponent() {\n      return this.parentElement?.closest(\"[reactor-component]\");\n    }\n\n    /**\n     * Dispatches a command to this component and sends it to the backend\n     * @param {String} command\n     * @param {Object} args\n     * @param {?HTMLFormElement} form\n     */\n    dispatch(command, args, formScope) {\n      connection.sendUserEvent(\n        this.id,\n        command,\n        this.serialize(formScope),\n        args\n      );\n    }\n\n    /**\n     * Serialize all elements inside `element` with a [name] attribute into\n     * a an array of `[element[name], element[value]]`\n     * @param {HTMLElement} element\n     */\n    serialize(element) {\n      let result = {};\n      for (let el of element.querySelectorAll(\"[name]\")) {\n        // Avoid serializing data of a nested component\n        if (el.closest(\"[reactor-component]\") !== this) {\n          continue;\n        }\n\n        let value = null;\n        switch (el.type.toLowerCase()) {\n          case \"checkbox\":\n          case \"radio\":\n            value = el.checked ? el.value || true : null;\n            break;\n          case \"select-multiple\":\n            value = el.selectedOptions.map((option) => option.value);\n            break;\n          default:\n            value = el.value;\n            break;\n        }\n\n        if (value !== null) {\n          let key = el.getAttribute(\"name\");\n          let values = result[key] ?? [];\n          values.push(value);\n          result[key] = values;\n        }\n      }\n      return result;\n    }\n  }\n\n  customElements.define(dataset.tagName, ReactorComponent, {\n    extends: dataset.extends,\n  });\n}\n\nconnection.open();\nvar debounceTimeout = undefined;\n\nwindow.reactor = {\n  /**\n   * Forwards a user event to a component\n   * @param {HTMLElement} element\n   * @param {String} name\n   * @param {Object} args\n   */\n  send(element, name, args) {\n    let component = element.closest(\"[reactor-component]\");\n    if (component !== null) {\n      let form = element.closest(\"form\");\n      let formScope = component.contains(form) ? form : component;\n      component.dispatch(name, args, formScope);\n    }\n  },\n\n  /**\n   * Debounce a function call\n   * @param {Number} delay\n   * @returns\n   */\n  debounce(delay) {\n    return (f) => {\n      return (...args) => {\n        clearTimeout(debounceTimeout);\n        debounceTimeout = setTimeout(() => f(...args), delay);\n      };\n    };\n  },\n};\n"
     ],
     "version": 3
 }
```

### Comparing `django-reactor-5.0.1b0/reactor/templatetags/reactor.py` & `django-reactor-5.0.2b0/reactor/templatetags/reactor.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/reactor/utils.py` & `django-reactor-5.0.2b0/reactor/utils.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.1b0/setup.cfg` & `django-reactor-5.0.2b0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-reactor
-version = 5.0.1b0
+version = 5.0.2b0
 description = Brings LiveView from Phoenix framework into Django
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
 	Framework :: Django
```

