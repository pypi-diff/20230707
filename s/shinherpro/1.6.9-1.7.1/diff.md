# Comparing `tmp/shinherpro-1.6.9.tar.gz` & `tmp/shinherpro-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.6.9.tar", last modified: Thu Jun 22 15:59:09 2023, max compression
+gzip compressed data, was "shinherpro-1.7.1.tar", last modified: Wed Jul  5 13:38:01 2023, max compression
```

## Comparing `shinherpro-1.6.9.tar` & `shinherpro-1.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 15:59:09.367439 shinherpro-1.6.9/
--rw-rw-rw-   0        0        0      178 2023-06-22 15:59:09.366943 shinherpro-1.6.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-22 15:59:09.367934 shinherpro-1.6.9/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-06-19 15:20:34.000000 shinherpro-1.6.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:59:09.352557 shinherpro-1.6.9/shinherpro/
--rw-rw-rw-   0        0        0    20214 2023-06-22 15:52:20.000000 shinherpro-1.6.9/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.6.9/shinherpro/__init__.py
--rw-rw-rw-   0        0        0     1421 2023-06-19 15:22:28.000000 shinherpro-1.6.9/shinherpro/chormeDriver.py
--rw-rw-rw-   0        0        0      547 2023-06-22 15:54:06.000000 shinherpro-1.6.9/shinherpro/logSave.py
--rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.9/shinherpro/vfcModel.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:59:09.365951 shinherpro-1.6.9/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-22 15:59:09.000000 shinherpro-1.6.9/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-06-22 15:59:09.000000 shinherpro-1.6.9/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 15:59:09.000000 shinherpro-1.6.9/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-06-22 15:59:09.000000 shinherpro-1.6.9/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 15:59:09.000000 shinherpro-1.6.9/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 13:38:01.758457 shinherpro-1.7.1/
+-rw-rw-rw-   0        0        0      178 2023-07-05 13:38:01.758457 shinherpro-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-05 13:38:01.759454 shinherpro-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-07-05 06:01:29.000000 shinherpro-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:38:01.747299 shinherpro-1.7.1/shinherpro/
+-rw-rw-rw-   0        0        0    29020 2023-07-05 13:37:59.000000 shinherpro-1.7.1/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.7.1/shinherpro/__init__.py
+-rw-rw-rw-   0        0        0     1421 2023-06-19 15:22:28.000000 shinherpro-1.7.1/shinherpro/chormeDriver.py
+-rw-rw-rw-   0        0        0      547 2023-06-22 15:54:06.000000 shinherpro-1.7.1/shinherpro/logSave.py
+-rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.7.1/shinherpro/vfcModel.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:38:01.757460 shinherpro-1.7.1/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-07-05 13:38:01.000000 shinherpro-1.7.1/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-05 13:38:01.000000 shinherpro-1.7.1/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 13:38:01.000000 shinherpro-1.7.1/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-05 13:38:01.000000 shinherpro-1.7.1/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-05 13:38:01.000000 shinherpro-1.7.1/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.6.9/setup.py` & `shinherpro-1.7.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     def run(self):
         print("\033[98m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.6.9',
-    description='shinher-pro 1.6.9',
+    version='1.7.1',
+    description='shinher-pro 1.7.1',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.6.9/shinherpro/TYAI.py` & `shinherpro-1.7.1/shinherpro/TYAI.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,31 +25,26 @@
 from shinherpro import vfcModel
 from shinherpro import chormeDriver
 from shinherpro import logSave
 import sys
 
 
 ###################################################
-# V 1.6.4 By Yihuan Studio --> 2023/5/21/05:09:19
-
-#############################################
-#  vfcCode AI model 5.1  x4307 picture
-##  image enhancement algorithm V1 By Sam
+# V 1.7.0 By Yihuan --> 2023/6/25
 
 RESET = "\033[0m"
 RED = "\033[31m"
 GREEN = "\033[32m"
 YELLOW = "\033[33m"
 
 global UserNameSave
 
 def urlGet():
     return "https://sai.tyai.tyc.edu.tw/online/"
 
-# get var to set driver and model
 def setup(driverIn,modelIn):
     global driver,model
     driver = driverIn
     model = modelIn
 
 def score_tolist(new_page_source):
     
@@ -61,14 +56,16 @@
     for row in rows:
         subject = row.select_one('td.top').text.strip()
         score_elements = row.select('td.top.right span')
         if len(score_elements) >= 2:
             user_score = score_elements[0].text.strip()
             class_average = score_elements[1].text.strip()
             subject_scores.append({'考試科目': subject, '個人成績': user_score, '全班平均': class_average})
+        else:
+            subject_scores.append({'考試科目': subject, '個人成績': '未公布', '全班平均': '未公布'})
 
     total_score = soup.select_one('table.scoreTable-inline td.score').text.strip()
 
     average_score_elements = soup.select('table.scoreTable-inline td.score')
     average_score = average_score_elements[1].text.strip() if len(average_score_elements) >= 3 else "N/A"
 
     ranking_elements = soup.select('table.scoreTable-inline td.score')
@@ -238,59 +235,59 @@
     class_name = student_info[0].split('：')[1]
     seat_number = student_info[2].split('：')[1]
     student_id = student_info[4].split('：')[1]
     student_name = student_info[6].split('：')[1]
 
     subjects = []
     table_rows = soup.find('table', id='restudyList').find_all('tr')
-    #print(table_rows)
     for row in table_rows[1:]:
         cells = row.find_all('td')
-        subject_code = cells[0].text.strip()
-        subject_name = cells[1].text.strip()
-        retake_semester = cells[2].text.strip()
-        historical_records = cells[3].text.strip()
-        credits = cells[4].text.strip()
+        subject_code = cells[0].text.strip() if cells[0].text else None
+        subject_name = cells[1].text.strip() if cells[1].text else None
+        retake_semester = cells[2].text.strip() if cells[2].text else None
+        historical_records = cells[3].text.strip() if cells[3].text else None
+        credits = cells[4].text.strip() if cells[4].text else None
         subjects.append({
             '科目代碼': subject_code,
             '科目名稱': subject_name,
             '重補修學期': retake_semester,
             '歷年成績記錄': historical_records,
             '學分': credits
         })
 
     electronic_rows = soup.find_all('tr', class_='電子二甲')
     electronic_contents = []
     for row in electronic_rows:
         cells = row.find_all('td')
-        content = [cell.text.strip() for cell in cells]
+        content = [cell.text.strip() if cell.text else None for cell in cells]
         electronic_contents.append(content)
 
     bt_rows = soup.find_all('tr', class_='bt')
     bt_contents = []
     for row in bt_rows:
         cells = row.find_all('td')
-        content = [cell.text.strip() for cell in cells]
+        content = [cell.text.strip() if cell.text else None for cell in cells]
         bt_contents.append(content)
 
     merged_contents = electronic_contents + bt_contents
 
     data = {
         '班級': class_name,
         '座號': seat_number,
         '學號': student_id,
         '姓名': student_name,
         '不及格科目': subjects,
         '學分': merged_contents,
     }
 
     json_data = json.dumps(data, ensure_ascii=False)
-    return json_data
+    return json_data,data
+
 
-def getGrades(examname,stepPrint=False):
+def getGrades(examname,stepPrint=False,justReturnHTML=False):
     driver.refresh()
     stepSave = 0
     try:
         stepSave = 1
 
         # 進入成績查詢頁面
         # 切換到左測選單
@@ -347,15 +344,19 @@
         stepSave = 4
 
         JsonResult = JsonGrade
 
         if stepPrint==False : sys.stdout = sys.__stdout__
         
         logSave.addLog("GetGrade",UserNameSave,JsonResult)
-        return JsonResult
+
+        if justReturnHTML :
+            return new_page_source
+        else:
+            return JsonResult
 
 
     except Exception as e:
         error_message = str(e) 
         if stepPrint == False:
             sys.stdout = sys.__stdout__
 
@@ -513,11 +514,233 @@
 
         return json_output
 
 
     except Exception as e:
         error_message = str(e) 
         return {'code': 33, 'reason': f'something Wrong, step {stepSave}try的錯誤原應: {error_message}'}
+
+
+def getAllData():
+
+    # get user base data
+    driver.refresh()
+    stepSave = 1
+    try:
+        chormeDriver.switch_frame(False, ["left"], driver)
+    except:
+        return {'code':1}
+    student_data_link = driver.find_element(By.ID, 'lnkStudentData')  # 按鈕名稱 "學生 xxx 的資料"
+    student_data_link.click()
+    # 尋找按鈕名稱 "查詢學生資料"
+    button_name = '查詢學生資料'
+    button_elements = driver.find_elements(By.CSS_SELECTOR, 'td.SubMenuItem') 
+    for button in button_elements:
+        button_text = button.text
+        if button_text == button_name:
+            button.click()
+            break
+                
+    stepSave = 2
+
+    # 切換到框架"right"的框架"right_below"
+    chormeDriver.switch_frame(True, ["right", "right_below"], driver)
+    # 找到查詢資料按鈕
+    button = driver.find_element(By.CSS_SELECTOR, "button[onclick*='window.open']")
+    button.click()
+    # 切換到框架"right"的框架"right_below"
+    chormeDriver.switch_frame(True, ["right", "right_top"], driver)
+    # 找到查詢基本資料按鈕
+    button = driver.find_element(By.XPATH, "//img[@title='查詢基本資料']")
+    button.click()
+    chormeDriver.switch_frame(True, ["right","right_below"], driver)
+    new_page_source = driver.page_source
+    #print(new_page_source)
+    soup = BeautifulSoup(new_page_source, 'html.parser')
+
+    list_items = soup.find_all('tr')
+    bastDataList = []
+    for count,item in enumerate(list_items):
+        bastDataList.append([])
+        for item2 in item.find_all('td'):
+            bastDataList[count].append(item2.text)
+    #print(bastDataList)
+    studentID = bastDataList[0][2]
+    studentName = bastDataList[0][4]
+    studentGender = bastDataList[2][3]
+    studentIdentity = bastDataList[2][1]
+    studentEnglishName = bastDataList[6][1]
+    studentClass = bastDataList[3][1]
+    studentBirthday = bastDataList[1][1]
+    studentJuniorHighSchool = bastDataList[11][1]
+    studentInschool = bastDataList[13][1]
+
+    UserBastData = {
+        'schoolID':studentID,
+        'name':studentName,
+        'englishName':studentEnglishName,
+        'gender':studentGender,
+        'class':studentClass,
+        'birthday':studentBirthday,
+        'juniorHighSchool':studentJuniorHighSchool,
+        'inschool':studentInschool,
+        'identity':studentIdentity
+    }
+
+    #get life performance
+
+    stepSave = 3
+
+    
+    # 切換到框架"right"的框架"right_below"
+    chormeDriver.switch_frame(True, ["right", "right_top"], driver)
+    # 找到查詢基本資料按鈕
+    button = driver.find_element(By.XPATH, "//img[@title='查詢德育獎懲資料']")
+    button.click()
+    chormeDriver.switch_frame(True, ["right","right_below"], driver)
+    new_page_source = driver.page_source
+    #print(new_page_source)
+    soup = BeautifulSoup(new_page_source, 'html.parser')
+
+    list_items = soup.find_all('tr')
+    lifeDataList = []
+    for count,item in enumerate(list_items):
+        lifeDataList.append([])
+        for item2 in item.find_all('td'):
+            lifeDataList[count].append(item2.text)
+
+    award = {'嘉獎':lifeDataList[1][2],'小功':lifeDataList[1][4],'大功':lifeDataList[1][6]}
+    punish = {'警告':lifeDataList[2][2],'小過':lifeDataList[2][4],'大過':lifeDataList[2][6]}
+    record = []
+    for item in lifeDataList[5:]:
+        record.append(item)
+    
+    UserLifeData = {
+        'award':award,
+        'punish':punish,
+        'record':record
+    }
+
+    YearExamList = ['一年級歷年成績','二年級歷年成績','三年級歷年成績','四年級歷年成績']
+    YearDataList = []
+    
+    for YearExam in YearExamList:
+        # 切換到框架"right"的框架"right_below"
+        chormeDriver.switch_frame(True, ["right", "right_top"], driver)
+        # 找到查詢基本資料按鈕
+        button = driver.find_element(By.XPATH, "//img[@title='查詢歷年成績資料']")
+        button.click()
+        # 選擇彈出的選單
+        window_handles = driver.window_handles
+        driver.switch_to.window(window_handles[-1])  # 切换到最新打开的窗口
+        # 等待下拉框載入完成
+        ddl_exam_list = WebDriverWait(driver, 10).until(EC.presence_of_element_located((By.NAME, 'ddlItems1')))
+        # 創建 Select 對象
+        select = Select(ddl_exam_list)
+        # 選擇下拉選單中的選項
+        select.select_by_visible_text(YearExam)
+        # 切换回原始窗口
+        driver.switch_to.window(window_handles[0])
+        # 成績讀取
+        # 切换到右侧框架
+        chormeDriver.switch_frame(True, ["right", "right_below"], driver)
+        # 獲取新窗口的頁面內容(成績表格)
+        new_page_source = driver.page_source
+        #print(new_page_source)
+
+        soup = BeautifulSoup(new_page_source, 'html.parser')
+        list_items = soup.find_all('tr')
+        oneYearDataList = []
+        for count,item in enumerate(list_items):
+            oneYearDataList.append([])
+            for item2 in item.find_all('td'):
+                oneYearDataList[count].append(item2.text)
+        
+        #print(oneYearDataList)
+
+        sujectData = []
+        for item in oneYearDataList[3:]:
+            if len(item) != 8:
+                break
+            else:
+                sujectData.append({
+                    item[0]:{
+                        '上學期':{
+                            '屬性':item[1],
+                            '學分':item[2],
+                            '成績':item[3],
+                        },
+                        '下學期':{
+                            '屬性':item[4],
+                            '學分':item[5],
+                            '成績':item[6],
+                        },
+                        '學年':item[7]
+                    }
+                })
+
+        oneDataItem = {
+            'year':oneYearDataList[0][0],
+            'tag':oneYearDataList[2],
+            'sujectData':sujectData
+        }
+        YearDataList.append({YearExam:oneDataItem})
+
+    #get All exam data
+
+    # 切換到框架"right"的框架"right_below"
+    chormeDriver.switch_frame(True, ["right", "right_top"], driver)
+    # 找到查詢基本資料按鈕
+    button = driver.find_element(By.XPATH, "//img[@title='各式成績查詢']")
+    button.click()
+    # 選擇彈出選擇考試的選單
+    window_handles = driver.window_handles
+    driver.switch_to.window(window_handles[-1])  # 切换到最新打开的窗口
+    # 等待下拉框載入完成
+    ddl_exam_list = WebDriverWait(driver, 10).until(EC.presence_of_element_located((By.ID, 'ddlExamList')))
+    # 創建 Select 對象
+    select = Select(ddl_exam_list)
+    options = select.options
+    allExamName = []
+    for exam in options[2:]:
+        allExamName.append(exam.text)
+
+    Allexam = {}
+
+    for exam in allExamName:
+
+        # 選擇下拉選單中的選項
+        select.select_by_visible_text(exam)
+        # 切换回原始窗口
+        driver.switch_to.window(window_handles[0])
+        # 成績讀取
+        # 切换到右侧框架
+        chormeDriver.switch_frame(True, ["right", "right_below"], driver)
+        # 獲取新窗口的頁面內容(成績表格)
+        new_page_source = driver.page_source
+        Allexam.update({exam:score_tolist(new_page_source)})
+
+        # 切換到框架"right"的框架"right_below"
+        chormeDriver.switch_frame(True, ["right", "right_top"], driver)
+        # 找到查詢基本資料按鈕
+        button = driver.find_element(By.XPATH, "//img[@title='各式成績查詢']")
+        button.click()
+        # 選擇彈出選擇考試的選單
+        window_handles = driver.window_handles
+        driver.switch_to.window(window_handles[-1])  # 切换到最新打开的窗口
+        # 等待下拉框載入完成
+        ddl_exam_list = WebDriverWait(driver, 10).until(EC.presence_of_element_located((By.ID, 'ddlExamList')))
+        # 創建 Select 對象
+        select = Select(ddl_exam_list)
+        options = select.options
+
+    # 選擇下拉選單中的選項
+    select.select_by_visible_text(allExamName[0])
+    # 切换回原始窗口
+    driver.switch_to.window(window_handles[0])  
     
 
+    UserCredit = getCredit()[1]
 
+    #print(Allexam)
 
+    return {'code':0,'UserBastData':UserBastData,'UserLifeData':UserLifeData,'YearDataList':YearDataList,'ALLExamData':Allexam,'UserCredit':UserCredit}
```

### Comparing `shinherpro-1.6.9/shinherpro/chormeDriver.py` & `shinherpro-1.7.1/shinherpro/chormeDriver.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.9/shinherpro/logSave.py` & `shinherpro-1.7.1/shinherpro/logSave.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.9/shinherpro/vfcModel.py` & `shinherpro-1.7.1/shinherpro/vfcModel.py`

 * *Files identical despite different names*

