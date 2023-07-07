# Comparing `tmp/BaseDeploy-0.0.3.tar.gz` & `tmp/BaseDeploy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseDeploy-0.0.3.tar", last modified: Mon Jun 19 06:01:24 2023, max compression
+gzip compressed data, was "dist/BaseDeploy-0.0.4.tar", last modified: Mon Jun 26 05:47:56 2023, max compression
```

## Comparing `BaseDeploy-0.0.3.tar` & `BaseDeploy-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy/
--rw-rw-r--   0 user      (1001) user      (1001)    23218 2023-06-19 05:59:49.000000 BaseDeploy-0.0.3/BaseDeploy/BaseDeploy.py
--rw-rw-r--   0 user      (1001) user      (1001)      206 2023-06-13 08:04:12.000000 BaseDeploy-0.0.3/BaseDeploy/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     1298 2023-06-19 06:01:09.000000 BaseDeploy-0.0.3/BaseDeploy/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       57 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       60 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       11 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-07 11:34:56.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDeploy-0.0.3/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       59 2023-06-08 08:27:27.000000 BaseDeploy-0.0.3/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4238 2023-06-19 06:01:03.000000 BaseDeploy-0.0.3/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/BaseDeploy/
+-rw-rw-r--   0 user      (1001) user      (1001)    24013 2023-06-26 05:45:40.000000 BaseDeploy-0.0.4/BaseDeploy/BaseDeploy.py
+-rw-rw-r--   0 user      (1001) user      (1001)      206 2023-06-13 08:04:12.000000 BaseDeploy-0.0.4/BaseDeploy/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1298 2023-06-26 05:47:37.000000 BaseDeploy-0.0.4/BaseDeploy/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/BaseDeploy.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/BaseDeploy.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/BaseDeploy.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/BaseDeploy.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       57 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/BaseDeploy.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       60 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/BaseDeploy.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       11 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/BaseDeploy.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-07 11:34:56.000000 BaseDeploy-0.0.4/BaseDeploy.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDeploy-0.0.4/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       59 2023-06-08 08:27:27.000000 BaseDeploy-0.0.4/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-26 05:47:56.000000 BaseDeploy-0.0.4/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4238 2023-06-26 05:47:29.000000 BaseDeploy-0.0.4/setup.py
```

### Comparing `BaseDeploy-0.0.3/BaseDeploy/BaseDeploy.py` & `BaseDeploy-0.0.4/BaseDeploy/BaseDeploy.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self.model = None
         self.info = None
         self.class_names = None
         self.backbone = None
         self.codebase = None
         self.ip_addr = None
         self.siot = None
+        self.score = None
         # 用以判断siot一次至显示或回传一张图片
         self.is_show = False
 
         if backend == 'ort':
             self.model_path = model_path
             self.model = self._use_ort_backend()
             self.device = device
@@ -55,247 +56,226 @@
             self.ip_addr = model_path
 
     def _use_ort_backend(self):
         import onnxruntime as ort
         sess = ort.InferenceSession(self.model_path, None)
         return sess
 
-
     def inference(self, 
                 input_data: Union[str, List[str], ImageData, List[ImageData]], 
                 show: bool = False, 
                 get_img: str = None,
-                score: float = 0.65,
+                score: float = None,
                 show_path: bool = False):
         if self.backend == 'siot':
             try:
                 import base64
             except ImportError:
                 print("The library 'base64' does not exist. Please use 'pip3 install base64' to install library.")
             self.is_show = True
             IOT_Topic  = 'XEdu/model_infer'
             IOT_Result_Topic = 'XEdu/model_result'
             print('Inference using a remote siot server.')
-            #self.stop_siot()
-            #self.run_siot(self.ip_addr, 'upload')
             def rec_cb(client, userdata, msg):
                 if not self.is_show:
                     return
                 payload = msg.payload.decode()
                 decoded_data = base64.b64decode(payload)
                 decoded_image = cv2.imdecode(np.frombuffer(decoded_data, np.uint8), cv2.IMREAD_COLOR)
                 image_rgb = cv2.cvtColor(decoded_image, cv2.COLOR_BGR2RGB)
                 plt.imshow(image_rgb)
                 plt.axis('off')
                 plt.show()
                 self.is_show = False
             if isinstance(input_data, str):
-
                 img = cv2.imread(input_data)
                 _, encoded_image = cv2.imencode('.jpg', img)
                 encoded_string = base64.b64encode(encoded_image).decode('utf-8')
                 self.siot.publish(IOT_Topic, encoded_string)
-
                 self.siot.subscribe(IOT_Result_Topic, rec_cb)
         if self.backend == 'ort':
             if self.backbone == '':
                 input_shape = self.model.get_inputs()[0].shape
                 if input_shape[0] == 'unk__606':
                     img_size = tuple(input_shape[1:3])
                 else:
                     img_size = tuple(input_shape[-2:])
                 if isinstance(input_data, str):
                     if os.path.isfile(input_data):
                         input_data = ImageData(input_data, size = img_size)
                     elif os.path.isdir(input_data):
-                        input_data = [ImageData(os.path.join(input_data, f), size = img_size) for f in os.listdir(input_data) if os.path.isfile(os.path.join(input_data, f))]
+                        input_data = [ImageData(os.path.join(input_data, f), size = img_size) for f in os.listdir(input_data) if os.path.isfile(os.path.join(input_data, f)) and f.lower().endswith((".jpg", ".jpeg", ".png"))]
                 if isinstance(input_data, np.ndarray):
                     input_data = ImageData(input_data, size = img_size)
             else:
                 if isinstance(input_data, str):
                     if os.path.isfile(input_data):
                         input_data = ImageData(input_data, backbone = self.backbone)
                     elif os.path.isdir(input_data):
-                        input_data = [ImageData(os.path.join(input_data, f), backbone = self.backbone) for f in os.listdir(input_data) if os.path.isfile(os.path.join(input_data, f))]
+                        input_data = [ImageData(os.path.join(input_data, f), backbone = self.backbone) for f in os.listdir(input_data) if os.path.isfile(os.path.join(input_data, f)) and f.lower().endswith((".jpg", ".jpeg", ".png"))]
                 if isinstance(input_data, np.ndarray):
                     input_data = ImageData(input_data, backbone = self.backbone)
             if isinstance(input_data, ImageData):
                 input_data = [input_data]
             assert isinstance(input_data, list)
             input_name = self.model.get_inputs()[0].name
             output_names = [o.name for o in self.model.get_outputs()]
             results = []
             for dt in input_data:
                 assert isinstance(dt, ImageData)
                 if self.codebase == 'MMCls':
-                    score = 0
+                    if score is None:
+                        score = 0
+                    self.score = score
                     pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
-                    if pred_onx[0].ndim == 1:
-                        pred_onx[0] = pred_onx[0][np.newaxis,:]
-                    idx = np.argmax(pred_onx[0], axis=1)[0]
-                    result = {'标签':idx, '置信度':pred_onx[0][0][idx], 
-                                   '预测结果':self.class_names[idx]}
+                    results.append(pred_onx)
+                    result = self.print_result(pred_onx, score)
                     if show_path:
                         result['路径'] = dt.data_source
-                    results.append(result)
+                    #results.append(result)
                     if show:
                         if result['置信度'] >= score:
                             from BaseDT.plot import show_cls
                             show_cls([dt], [result])
                             print(result)
                         else:
                             print("The accuracy is lower than the preset value, "
                                   "if you want to draw a picture, "
                                   "please set score={:.2f}, or lower.".format(result['置信度']))
                 elif self.codebase == 'MMDet':
+                    if score is None:
+                        score = 0.65
+                    self.score = score
                     pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
-                    boxes = dt.map_orig_coords(pred_onx[0][0])
-                    labels = pred_onx[1][0]
-                    result = []
-
-                    for box, label in zip(boxes, labels):
-                        if box[4] >= score:
-                            box_int = box.astype(np.int32)
-                            tmp_dict = {'标签':label, '置信度':box[4], '预测结果':self.class_names[label],
-                                           '坐标': {'x1':box_int[0], 
-                                                 'y1':box_int[1],
-                                                 'x2':box_int[2],
-                                                 'y2':box_int[3]}}
-                            if show_path:
-                                tmp_dict['路径'] = dt.data_source
-                            result.append(tmp_dict)
-                    results.append(result)
+                    pred_onx[0][0] = dt.map_orig_coords(pred_onx[0][0])
+                    results.append(pred_onx)
+                    result = self.print_result(pred_onx, score)
+                    if show_path:
+                        for item in result:
+                            item['路径'] = dt.data_source
                     if show:
                         from BaseDT.plot import show_det
                         show_det([dt], [result])        
                         print(result)
                 elif self.codebase == 'TFJS':
-                    score = 0
+                    if score is None:
+                        score = 0
+                    self.score = score
                     import copy
                     copy_dt = copy.deepcopy(dt)
                     input_tensor = copy_dt.to_tensor()
                     input_data_tfjs = np.transpose(input_tensor, (0, 2, 3, 1))
-                    output_data = self.model.run(output_names, {input_name: input_data_tfjs})[0]
-                    idx = np.argmax(output_data)
-                    acc = output_data[0][idx]
-                    result = {'标签':idx, '置信度':acc, 
-                                   '预测结果':self.class_names[idx]}
+                    output_data = self.model.run(output_names, {input_name: input_data_tfjs})
+                    results.append(output_data)
+                    result = self.print_result(output_data)
                     if show_path:
                         result['路径'] = dt.data_source
-                    results.append(result)
                     if show:
                         if result['置信度'] >= score:
                             from BaseDT.plot import show_cls
                             show_cls([dt], [result])
                             print(result)
                         else:
                             print("The accuracy is lower than the preset value, "
                                   "if you want to draw a picture, "
                                   "please set score={:.2f}, or lower.".format(result['置信度']))
-                    #pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
                 elif self.codebase == 'MMPose':
                     h, w = self.model.get_inputs()[0].shape[2:]
                     model_input_size = (w, h)
                     img_shape = dt.raw_value.shape[:2]
                     img = dt.raw_value
                     bbox = np.array([0, 0, img_shape[1], img_shape[0]])
                     resized_img, center, scale = mmpose_preprocess(img, model_input_size)
                     input_tensor = [resized_img.transpose(2, 0, 1)]
                     outputs = self.model.run(output_names, {input_name: input_tensor})
                     keypoints, scores = mmpose_postprocess(outputs, model_input_size, center, scale)
+                    results.append([keypoints, scores])
                     result = {'关键点':keypoints, '得分':scores}
                     if show_path:
                         result['路径'] = dt.data_source
-                    results.append(result)
                     if show:
                         from BaseDT.plot import show_pose
                         show_pose([dt], [result])
                         print(result)
                 else:
                     input_shape = self.model.get_inputs()[0].shape
                     print('The onnx model is not exported by the XEdu tool.'\
 						' BaseDeploy calls BaseDT to adapt the input to {}.'\
 						' \'mean\': [123.675, 116.28, 103.53], \'std\': [58.395, 57.12, 57.375], \'normalize\': True'.format(input_shape))
                     if input_shape[0] == 'unk__606':
-                        score = 0
+                        self.codebase = 'TFJS'
+                        if score is None:
+                            score = 0
+                        self.score = score
                         import copy
                         copy_dt = copy.deepcopy(dt)
                         input_tensor = copy_dt.to_tensor()
                         input_data_tfjs = np.transpose(input_tensor, (0, 2, 3, 1))
-                        output_data = self.model.run(output_names, {input_name: input_data_tfjs})[0]
-                        idx = np.argmax(output_data)
-                        acc = output_data[0][idx]
-                        result = {'标签':idx, '置信度':acc}
+                        output_data = self.model.run(output_names, {input_name: input_data_tfjs})
+                        results.append(output_data)
+                        result = self.print_result(output_data)
                         if show_path:
                             result['路径'] = dt.data_source
-                        results.append(result)
                         if show:
                             if result['置信度'] >= score:
                                 from BaseDT.plot import show_cls
                                 show_cls([dt], [result])
                                 print(result)
                             else:
                                 print("The accuracy is lower than the preset value, "
                                     "if you want to draw a picture, "
                                     "please set score={:.2f}, or lower.".format(result['置信度']))
                     else:
                         pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
                         if len(pred_onx) == 1:
                             # consider as cls
-                            score = 0
-                            if pred_onx[0].ndim == 1:
-                                pred_onx[0] = pred_onx[0][np.newaxis,:]
-                            idx = np.argmax(pred_onx[0], axis=1)[0]
-                            result = {'标签':idx, '置信度':pred_onx[0][0][idx]}
+                            self.codebase = 'MMCls'
+                            if score is None:
+                                score = 0
+                            self.score = score
+                            results.append(pred_onx)
+                            result = self.print_result(pred_onx)
                             if show_path:
                                 result['路径'] = dt.data_source
-                            results.append(result)
                             if show:
                                 if result['置信度'] >= score:
                                     from BaseDT.plot import show_cls
                                     show_cls([dt], [result])
                                     print(result)
                                 else:
                                     print("The accuracy is lower than the preset value, "
                                         "if you want to draw a picture, "
                                         "please set score={:.2f}, or lower.".format(result['置信度']))
                         elif len(pred_onx) == 2:
                             # consider as det
-                            pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
-                            boxes = dt.map_orig_coords(pred_onx[0][0])
-                            labels = pred_onx[1][0]
-                            result = []
-
-                            for box, label in zip(boxes, labels):
-                                if box[4] >= score:
-                                    box_int = box.astype(np.int32)
-                                    tmp_dict = {'标签':label, '置信度':box[4], 
-                                                '坐标': {'x1':box_int[0], 
-                                                        'y1':box_int[1],
-                                                        'x2':box_int[2],
-                                                        'y2':box_int[3]}}
-                                    if show_path:
-                                        tmp_dict['路径'] = dt.data_source
-                                    result.append(tmp_dict)
-                            results.append(result)
+                            self.codebase = 'MMDet'
+                            if score is None:
+                                score = 0.65
+                            self.score = score
+                            #pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
+                            pred_onx[0][0] = dt.map_orig_coords(pred_onx[0][0])
+                            results.append(pred_onx)
+                            result = self.print_result(pred_onx, score)
                             print(result)
+                            if show_path:
+                                for item in result:
+                                    item['路径'] = dt.data_source
                             if show:
                                 from BaseDT.plot import show_det
-                                show_det([dt], [result])        
+                                show_det([dt], [result])
                                 print(result)
                         else:
                             return pred_onx
-                    #print(f'CodeBase {self.codebase} will be supported latter')
             if get_img == 'pil':
-                results, imgs = self._get_img(input_data, results, score, show)
+                imgs = self._get_img(input_data, self.print_result(results), score, show)
                 results = results[0] if len(results) == 1 else results
                 imgs = imgs[0] if len(imgs) == 1 else imgs
                 return results, imgs
             elif get_img == 'cv2':
-                results, imgs = self._get_img(input_data, results, score, show)
+                imgs = self._get_img(input_data, self.print_result(results), score, show)
                 for i in range(len(imgs)):
                     imgs[i] = cv2.cvtColor(np.array(imgs[i]), cv2.COLOR_RGB2BGR)
                 results = results[0] if len(results) == 1 else results
                 imgs = imgs[0] if len(imgs) == 1 else imgs
                 return results, imgs
             results = results[0] if len(results) == 1 else results
             return results
@@ -383,38 +363,26 @@
             decoded_image = cv2.imdecode(np.frombuffer(decoded_data, np.uint8), cv2.IMREAD_COLOR)
             result, img = self.inference(decoded_image, get_img='cv2')
             print(result)
             IOT_Result_Topic = 'XEdu/model_result'
             _, encoded_image = cv2.imencode('.jpg', img)
             encoded_string = base64.b64encode(encoded_image).decode('utf-8')
             self.siot.publish(IOT_Result_Topic, encoded_string)
-            #cv2.namedWindow("Decoded Image", cv2.WINDOW_NORMAL)
-            #cv2.imshow("Decoded Image", img)
-            #cv2.waitKey(0)
-            #cv2.destroyAllWindows()
         if mode == 'infer':
             SERVER = ip
             CLIENT_ID = "XEdu"
             IOT_Topic  = 'XEdu/model_infer'
             IOT_UserName ='siot'
             IOT_PassWord ='dfrobot'
             siot.init(CLIENT_ID, SERVER, user=IOT_UserName, password=IOT_PassWord)
             siot.connect()
             self.siot = siot
             print(msg)
             siot.subscribe(IOT_Topic, sub_cb)
             siot.loop()
-            '''
-            try:
-              while True:
-                pass
-            except:
-              siot.stop()
-              print("disconnect seccused")
-            '''
         else:
             SERVER = ip
             CLIENT_ID = "XEdu"
             IOT_Topic  = 'XEdu/model_infer'
             IOT_UserName ='siot'
             IOT_PassWord ='dfrobot'
             siot.init(CLIENT_ID, SERVER, user=IOT_UserName, password=IOT_PassWord)
@@ -425,15 +393,14 @@
             self.siot = siot
 
 
     def stop_siot(self):
         if self.use_siot:
             self.siot.stop()
             self.siot = None
-            #self.use_siot = False
             print('The siot\'s run has been terminated')
         else:
             print('The siot\'s run has already been terminated')
 
 
     def run_flask(self):
         pass
@@ -447,42 +414,101 @@
                         print("The accuracy is lower than the preset value, "
                           "if you want to draw a picture, "
                           "please set score={:.2f}, or lower.".format(results[i]['置信度']))
                         dt.init_plt()
                     else:
                         from BaseDT.plot import draw_single_cls
                         draw_single_cls(dt, results[i])
-                #imgs.append(dt.get_image())
             elif self.codebase == 'MMDet':
                 if show == False:
                     from BaseDT.plot import draw_single_det
-                    draw_single_det(dt, results[i])      
-                
-                #imgs.append(dt.get_image())
+                    draw_single_det(dt, results[i])
             elif self.codebase == 'TFJS':
                 if show == False:
                     if results[i]['置信度'] < score:
                         print("The accuracy is lower than the preset value, "
                           "if you want to draw a picture, "
                           "please set score={:.2f}, or lower.".format(results[i]['置信度']))
                         dt.init_plt()
                     else:
                         from BaseDT.plot import draw_single_cls
                         draw_single_cls(dt, results[i])
-                #imgs.append(dt.get_image())
             elif self.codebase == 'MMPose':
                 if show == False:
                     from BaseDT.plot import draw_single_pose
                     draw_single_pose(dt, results[i])
             imgs.append(dt.get_image())
-        return results, imgs
+        return imgs
     
     def diy_inference(self, input_data):
         assert isinstance(input_data, np.ndarray)
         input_name = self.model.get_inputs()[0].name
         output_names = [o.name for o in self.model.get_outputs()]
         pred_onx = self.model.run(output_names, {input_name: input_data})
         return pred_onx
-    
-    def print_result(self, result):
-        print('推理结果如下：')
-        print(result)
+
+    def print_single_cls(self, pred_onx: list):
+        if pred_onx[0].ndim == 1:
+            pred_onx[0] = pred_onx[0][np.newaxis, :]
+        idx = np.argmax(pred_onx[0], axis=1)[0]
+        result = {'标签': idx, '置信度': pred_onx[0][0][idx]}
+        if isinstance(self.class_names, list):
+            result['预测结果'] = self.class_names[idx]
+        return result
+
+    def print_single_det(self, pred_onx: list, score):
+        boxes = pred_onx[0][0]
+        labels = pred_onx[1][0]
+        result = []
+        for box, label in zip(boxes, labels):
+            if box[4] >= score:
+                box_int = box.astype(np.int32)
+                tmp_dict = {'标签': label, '置信度': box[4],
+                            '坐标': {'x1': box_int[0],
+                                     'y1': box_int[1],
+                                     'x2': box_int[2],
+                                     'y2': box_int[3]}}
+                if isinstance(self.class_names, list):
+                    tmp_dict['预测结果'] = self.class_names[label]
+                result.append(tmp_dict)
+        return result
+
+    def print_single_pose(self, pred_onx: list):
+        keypoints, scores = pred_onx
+        result = {'关键点': keypoints, '得分': scores}
+        return result
+
+    def print_result(self, pred_onx: list, score: float = None):
+        if self.codebase == 'MMCls':
+            if isinstance(pred_onx[0], list):
+                result = []
+                for item in pred_onx:
+                    result.append(self.print_single_cls(item))
+            else:
+                result = self.print_single_cls(pred_onx)
+        elif self.codebase == 'MMDet':
+            score = self.score
+            if score is None:
+               score = 0.65
+            if isinstance(pred_onx[0], list):
+                result = []
+                for item in pred_onx:
+                    result.append(self.print_single_det(item, score))
+            else:
+                result = self.print_single_det(pred_onx, score)
+        elif self.codebase == 'TFJS':
+            if isinstance(pred_onx[0], list):
+                result = []
+                for item in pred_onx:
+                    result.append(self.print_single_cls(item))
+            else:
+                result = self.print_single_cls(pred_onx)
+        elif self.codebase == 'MMPose':
+            if isinstance(pred_onx[0], list):
+                result = []
+                for item in pred_onx:
+                    result.append(self.print_single_pose(item))
+            else:
+                result = self.print_single_pose(pred_onx)
+        else:
+            result = pred_onx
+        return result
```

### Comparing `BaseDeploy-0.0.3/BaseDeploy/version.py` & `BaseDeploy-0.0.4/BaseDeploy/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.0.3'
+__version__='0.0.4'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseDeploy-0.0.3/setup.py` & `BaseDeploy-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDeploy',
-    version='0.0.3',
+    version='0.0.4',
     # version='0.0.1rc1',
     description='BaseDeploy is a simple deployment tool made by XEdu.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
```

