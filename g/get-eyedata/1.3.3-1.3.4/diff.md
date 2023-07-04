# Comparing `tmp/get_eyedata-1.3.3-py3-none-any.whl.zip` & `tmp/get_eyedata-1.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 8120 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-05 08:24 get_eyedata/__init__.py
--rw-rw-rw-  2.0 fat     2340 b- defN 23-Jun-30 06:07 get_eyedata/frame_utils.py
--rw-rw-rw-  2.0 fat     3977 b- defN 23-Jul-03 00:46 get_eyedata/ow2.py
--rw-rw-rw-  2.0 fat     5284 b- defN 23-Jun-30 06:28 get_eyedata/valo.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-03 00:48 get_eyedata-1.3.3.dist-info/LICENCE
--rw-rw-rw-  2.0 fat     1869 b- defN 23-Jul-03 00:48 get_eyedata-1.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 00:48 get_eyedata-1.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-03 00:48 get_eyedata-1.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      717 b- defN 23-Jul-03 00:48 get_eyedata-1.3.3.dist-info/RECORD
-9 files, 15388 bytes uncompressed, 6884 bytes compressed:  55.3%
+Zip file size: 9050 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        3 b- defN 23-Jul-04 05:39 get_eyedata/__init__.py
+-rw-r--r--  2.0 unx     2272 b- defN 23-Jul-04 05:39 get_eyedata/frame_utils.py
+-rw-r--r--  2.0 unx     3861 b- defN 23-Jul-04 05:39 get_eyedata/ow2.py
+-rw-r--r--  2.0 unx     5142 b- defN 23-Jul-04 05:39 get_eyedata/valo.py
+-rw-r--r--  2.0 unx     2153 b- defN 23-Jul-04 07:56 get_eyedata/video_edit.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Jul-04 08:01 get_eyedata-1.3.4.dist-info/LICENCE
+-rw-r--r--  2.0 unx     1801 b- defN 23-Jul-04 08:01 get_eyedata-1.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 08:01 get_eyedata-1.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-04 08:01 get_eyedata-1.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      799 b- defN 23-Jul-04 08:01 get_eyedata-1.3.4.dist-info/RECORD
+10 files, 17205 bytes uncompressed, 7688 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -6,23 +6,26 @@
 
 Filename: get_eyedata/ow2.py
 Comment: 
 
 Filename: get_eyedata/valo.py
 Comment: 
 
-Filename: get_eyedata-1.3.3.dist-info/LICENCE
+Filename: get_eyedata/video_edit.py
 Comment: 
 
-Filename: get_eyedata-1.3.3.dist-info/METADATA
+Filename: get_eyedata-1.3.4.dist-info/LICENCE
 Comment: 
 
-Filename: get_eyedata-1.3.3.dist-info/WHEEL
+Filename: get_eyedata-1.3.4.dist-info/METADATA
 Comment: 
 
-Filename: get_eyedata-1.3.3.dist-info/top_level.txt
+Filename: get_eyedata-1.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: get_eyedata-1.3.3.dist-info/RECORD
+Filename: get_eyedata-1.3.4.dist-info/top_level.txt
+Comment: 
+
+Filename: get_eyedata-1.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## get_eyedata/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
-
-
-
+
+
+
```

## get_eyedata/frame_utils.py

 * *Ordering differences only*

```diff
@@ -1,68 +1,68 @@
-import cv2
-import numpy as np
-from moviepy.editor import VideoFileClip
-import os
-
-#1と0で表現されたバイナリイメージに書き換える関数
-def binarize_image(image):
-    gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
-    _, binary = cv2.threshold(gray, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
-    binary_array = np.where(binary == 0, 0, 1)
-    return binary_array
-
-def cog(binary_img):
-    '''
-    Center of Gravity
-    重心を座標として出力する（左下を0,0とする座標系）
-    '''
-    # ラベリング処理
-    nlabels, labels, stats, center = cv2.connectedComponentsWithStats(binary_img)
-    
-    # 背景のオブジェクト情報の削除
-    nlabels = nlabels - 1
-    stats = np.delete(stats, 0, 0)
-    center = np.delete(center, 0, 0)
-    
-    # 面積が最大のオブジェクトのラベル番号を取得
-    try:
-        max_index = np.argmax(stats[:, 4])
-        center_x = int(center[max_index][0])
-        center_y = binary_img.shape[0] - int(center[max_index][1])  # y座標を変更
-    except ValueError:
-        center_x = np.nan
-        center_y = np.nan
-    
-    return center_x, center_y
-
-
-def sep_y(image,corrd:int = None):
-    '''
-    frameを回しているfor文の中での利用を前提とする
-    '''
-    if corrd:
-        # 動画を上下で半分に分割
-        top_half = image[:corrd, :]
-        bottom_half = image[corrd:, :]
-    else:
-        # 動画を上下で半分に分割
-        top_half = image[:2160 // 2, :]
-        bottom_half = image[2160 // 2:, :]
-    
-    return top_half,bottom_half
-
-def make_displayonly_video(video_path:str, output_dir:str='displayonly_video'):
-    clip = VideoFileClip(video_path)
-    cropped_clip = clip.crop(y1=0, y2=clip.h // 2)  # cropping the upper half of the video
-    
-    os.makedirs(output_dir, exist_ok=True)  # create the directory if it doesn't exist
-    
-    output_path = os.path.join(output_dir, os.path.basename(video_path))
-    base_name, ext = os.path.splitext(output_path)
-    i = 1
-    while os.path.exists(output_path):
-        print(f"{output_path} already exists, saving as {base_name}{i}.mp4 instead.")
-        output_path = f"{base_name}{i}.mp4"
-        i += 1
-
-    cropped_clip.write_videofile(output_path, codec='libx264')
-
+import cv2
+import numpy as np
+from moviepy.editor import VideoFileClip
+import os
+
+#1と0で表現されたバイナリイメージに書き換える関数
+def binarize_image(image):
+    gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+    _, binary = cv2.threshold(gray, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
+    binary_array = np.where(binary == 0, 0, 1)
+    return binary_array
+
+def cog(binary_img):
+    '''
+    Center of Gravity
+    重心を座標として出力する（左下を0,0とする座標系）
+    '''
+    # ラベリング処理
+    nlabels, labels, stats, center = cv2.connectedComponentsWithStats(binary_img)
+    
+    # 背景のオブジェクト情報の削除
+    nlabels = nlabels - 1
+    stats = np.delete(stats, 0, 0)
+    center = np.delete(center, 0, 0)
+    
+    # 面積が最大のオブジェクトのラベル番号を取得
+    try:
+        max_index = np.argmax(stats[:, 4])
+        center_x = int(center[max_index][0])
+        center_y = binary_img.shape[0] - int(center[max_index][1])  # y座標を変更
+    except ValueError:
+        center_x = np.nan
+        center_y = np.nan
+    
+    return center_x, center_y
+
+
+def sep_y(image,corrd:int = None):
+    '''
+    frameを回しているfor文の中での利用を前提とする
+    '''
+    if corrd:
+        # 動画を上下で半分に分割
+        top_half = image[:corrd, :]
+        bottom_half = image[corrd:, :]
+    else:
+        # 動画を上下で半分に分割
+        top_half = image[:2160 // 2, :]
+        bottom_half = image[2160 // 2:, :]
+    
+    return top_half,bottom_half
+
+def make_displayonly_video(video_path:str, output_dir:str='displayonly_video'):
+    clip = VideoFileClip(video_path)
+    cropped_clip = clip.crop(y1=0, y2=clip.h // 2)  # cropping the upper half of the video
+    
+    os.makedirs(output_dir, exist_ok=True)  # create the directory if it doesn't exist
+    
+    output_path = os.path.join(output_dir, os.path.basename(video_path))
+    base_name, ext = os.path.splitext(output_path)
+    i = 1
+    while os.path.exists(output_path):
+        print(f"{output_path} already exists, saving as {base_name}{i}.mp4 instead.")
+        output_path = f"{base_name}{i}.mp4"
+        i += 1
+
+    cropped_clip.write_videofile(output_path, codec='libx264')
+
```

## get_eyedata/ow2.py

 * *Ordering differences only*

```diff
@@ -1,117 +1,117 @@
-from .frame_utils import cog, sep_y, binarize_image, make_displayonly_video
-import cv2
-import numpy as np
-import pandas as pd
-from dataclasses import dataclass
-from queue import Queue
-from threading import Thread
-from concurrent.futures import ProcessPoolExecutor, as_completed
-from tqdm import tqdm
-import os
-
-@dataclass
-class Area:
-    name: str
-    top_x: int
-    top_y: int
-    bottom_x: int
-    bottom_y: int
-    
-areas = [
-    Area('hp', 50, 50, 500, 250),
-    Area('chat', 50, 330, 500, 500),
-    Area('ult', 880, 50, 1040, 220),
-    Area('my_status', 1450, 50, 1900, 280),
-    Area('match_status', 650, 880, 1300, 1080),
-    Area('kill_log', 1450, 880, 1920, 1080)
-]
-
-def get_roi(x, y):
-    if ((x - 960)**2 + (y - 540)**2) <= 125**2:
-        return 'center'
-    else:
-        for area in areas:
-            if area.top_x <= x <= area.bottom_x and area.top_y <= y <= area.bottom_y:
-                return area.name
-    return 'other'
-
-def check(file_path:str):
-    if os.path.exists(file_path):
-        return True
-    else:
-        print('FileNotFoundError')
-        return False
-
-#フレームの読み込みと画像処理の並列化
-def frame_reader(cap, queue):
-    while True:
-        ret, frame = cap.read()
-        if not ret:
-            print('ret is False')
-            break
-        queue.put(frame)
-    queue.put(None)  # signal that all frames have been read
-
-def make_dataset(video_path:str, save:bool = True, get_display:bool = True):
-    #動画の読み込み
-    mov_file = os.path.normpath(video_path)
-    check(mov_file)
-    cap = cv2.VideoCapture(mov_file)
-    total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-    print(f'total_frames:{total_frames}')
-    #中心座標を格納するリスト
-    frame_ids = []
-    eye_x = []
-    eye_y = []
-    rois = []
-    images = []
-    #メインループスタート
-    cap.set(cv2.CAP_PROP_POS_FRAMES, 0)
-    for frame_id in tqdm(range(0,total_frames)):
-        #フレームを取得
-        ret, frame = cap.read()
-        if ret:
-            #get binarized iamge 
-            if frame.shape[0] != 1080:
-                game,eye = sep_y(frame)
-            else:
-                eye = frame
-            bin_image = binarize_image(eye)
-            #get center of biggest object
-            x,y = cog(bin_image.astype(np.uint8))
-            roi = get_roi(x,y)
-            eye_x.append(x)
-            eye_y.append(y)
-            rois.append(roi)
-            frame_ids.append(frame_id)
-        else:
-            print(f'error occurd at frame{frame_id}')
-            break   
-    cap.release()
-    df = pd.DataFrame({'frame_ids':frame_ids,'x':eye_x,'y':eye_y,'roi':rois})
-    if save:
-        # Get the base name of the video file and use it to create csv filename
-        base_name = os.path.basename(video_path)
-        file_name, _ = os.path.splitext(base_name)
-        df.to_csv(f'{file_name}.csv',index=False)
-    if get_display:
-        make_displayonly_video(video_path)
-    return df
-
-def make_dataset_from_folder(folder_path:str, max_workers:int = 4, save:bool = True, get_display:bool = True):
-    # Get a list of all video files in the folder
-    video_files = [f for f in os.listdir(folder_path) if f.endswith('.mp4') or f.endswith('.mkv')]
-
-    video_files = [os.path.join(folder_path, f) for f in video_files]
-
-    with ProcessPoolExecutor(max_workers=max_workers) as executor:
-        # Create a list to hold the Future objects
-        futures = [executor.submit(make_dataset, video_file, save, get_display) for video_file in video_files]
-
-        # Use tqdm for progress bar
-        for future in tqdm(as_completed(futures), total=len(futures)):
-            # Results are ready only when processing is complete, so we don't need to do anything here
-            pass
-if __name__ == "__main__":
-    df = make_dataset('F:\git-repo\get_eyedata\data\test.mkv')
+from .frame_utils import cog, sep_y, binarize_image, make_displayonly_video
+import cv2
+import numpy as np
+import pandas as pd
+from dataclasses import dataclass
+from queue import Queue
+from threading import Thread
+from concurrent.futures import ProcessPoolExecutor, as_completed
+from tqdm import tqdm
+import os
+
+@dataclass
+class Area:
+    name: str
+    top_x: int
+    top_y: int
+    bottom_x: int
+    bottom_y: int
+    
+areas = [
+    Area('hp', 50, 50, 500, 250),
+    Area('chat', 50, 330, 500, 500),
+    Area('ult', 880, 50, 1040, 220),
+    Area('my_status', 1450, 50, 1900, 280),
+    Area('match_status', 650, 880, 1300, 1080),
+    Area('kill_log', 1450, 880, 1920, 1080)
+]
+
+def get_roi(x, y):
+    if ((x - 960)**2 + (y - 540)**2) <= 125**2:
+        return 'center'
+    else:
+        for area in areas:
+            if area.top_x <= x <= area.bottom_x and area.top_y <= y <= area.bottom_y:
+                return area.name
+    return 'other'
+
+def check(file_path:str):
+    if os.path.exists(file_path):
+        return True
+    else:
+        print('FileNotFoundError')
+        return False
+
+#フレームの読み込みと画像処理の並列化
+def frame_reader(cap, queue):
+    while True:
+        ret, frame = cap.read()
+        if not ret:
+            print('ret is False')
+            break
+        queue.put(frame)
+    queue.put(None)  # signal that all frames have been read
+
+def make_dataset(video_path:str, save:bool = True, get_display:bool = True):
+    #動画の読み込み
+    mov_file = os.path.normpath(video_path)
+    check(mov_file)
+    cap = cv2.VideoCapture(mov_file)
+    total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+    print(f'total_frames:{total_frames}')
+    #中心座標を格納するリスト
+    frame_ids = []
+    eye_x = []
+    eye_y = []
+    rois = []
+    images = []
+    #メインループスタート
+    cap.set(cv2.CAP_PROP_POS_FRAMES, 0)
+    for frame_id in tqdm(range(0,total_frames)):
+        #フレームを取得
+        ret, frame = cap.read()
+        if ret:
+            #get binarized iamge 
+            if frame.shape[0] != 1080:
+                game,eye = sep_y(frame)
+            else:
+                eye = frame
+            bin_image = binarize_image(eye)
+            #get center of biggest object
+            x,y = cog(bin_image.astype(np.uint8))
+            roi = get_roi(x,y)
+            eye_x.append(x)
+            eye_y.append(y)
+            rois.append(roi)
+            frame_ids.append(frame_id)
+        else:
+            print(f'error occurd at frame{frame_id}')
+            break   
+    cap.release()
+    df = pd.DataFrame({'frame_ids':frame_ids,'x':eye_x,'y':eye_y,'roi':rois})
+    if save:
+        # Get the base name of the video file and use it to create csv filename
+        base_name = os.path.basename(video_path)
+        file_name, _ = os.path.splitext(base_name)
+        df.to_csv(f'{file_name}.csv',index=False)
+    if get_display:
+        make_displayonly_video(video_path)
+    return df
+
+def make_dataset_from_folder(folder_path:str, max_workers:int = 4, save:bool = True, get_display:bool = True):
+    # Get a list of all video files in the folder
+    video_files = [f for f in os.listdir(folder_path) if f.endswith('.mp4') or f.endswith('.mkv')]
+
+    video_files = [os.path.join(folder_path, f) for f in video_files]
+
+    with ProcessPoolExecutor(max_workers=max_workers) as executor:
+        # Create a list to hold the Future objects
+        futures = [executor.submit(make_dataset, video_file, save, get_display) for video_file in video_files]
+
+        # Use tqdm for progress bar
+        for future in tqdm(as_completed(futures), total=len(futures)):
+            # Results are ready only when processing is complete, so we don't need to do anything here
+            pass
+if __name__ == "__main__":
+    df = make_dataset('F:\git-repo\get_eyedata\data\test.mkv')
     print(df)
```

## get_eyedata/valo.py

 * *Ordering differences only*

```diff
@@ -1,143 +1,143 @@
-from .frame_utils import cog, sep_y, binarize_image, make_displayonly_video
-import cv2
-import numpy as np
-import pandas as pd
-from dataclasses import dataclass
-from queue import Queue
-from threading import Thread
-from concurrent.futures import ProcessPoolExecutor, as_completed
-from tqdm import tqdm
-import os
-
-
-@dataclass
-class Area:
-    name: str
-    top_x: int
-    top_y: int
-    bottom_x: int
-    bottom_y: int
-
-
-# minimap = Area('minimap',15,620,435,1040)
-# left_team = Area('left_team',440,0,870,100)
-# right_team = Area('right_team',1050,0,1480,100)
-# timer = Area('timer',870,0,1050,100)
-# kill_log = Area('kill_log',1490,60,1920,300)
-# hp = Area('hp',520,980,685,1080)
-# skill = Area('skill',745,980,1175,1080)
-# amo = Area('amo',1235,980,1400,1080)
-# center = ('center',960,540,125)
-
-minimap = Area('minimap',15,620,435,1040)
-left_team = Area('left_team',440,980,870,1080)
-right_team = Area('right_team',1050,980,1480,1080)
-timer = Area('timer',870,980,1050,1080)
-kill_log = Area('kill_log',1490,780,1920,1020)
-hp = Area('hp',520,0,685,100)
-skill = Area('skill',745,0,1175,100)
-amo = Area('amo',1235,0,1400,100)
-center = ('center',960,540,125)
-
-def get_roi(x, y):
-    if ((x - center[1])**2 + (y - center[2])**2) <= center[3]**2:
-        return center[0]
-    elif left_team.top_x <= x <= left_team.bottom_x and left_team.top_y <= y <= left_team.bottom_y:
-        return left_team.name
-    elif right_team.top_x <= x <= right_team.bottom_x and right_team.top_y <= y <= right_team.bottom_y:
-        return right_team.name
-    elif timer.top_x <= x <= timer.bottom_x and timer.top_y <= y <= timer.bottom_y:
-        return timer.name
-    elif kill_log.top_x <= x <= kill_log.bottom_x and kill_log.top_y <= y <= kill_log.bottom_y:
-        return kill_log.name
-    elif hp.top_x <= x <= hp.bottom_x and hp.top_y <= y <= hp.bottom_y:
-        return hp.name
-    elif skill.top_x <= x <= skill.bottom_x and skill.top_y <= y <= skill.bottom_y:
-        return skill.name
-    elif amo.top_x <= x <= amo.bottom_x and amo.top_y <= y <= amo.bottom_y:
-        return amo.name
-    elif minimap.top_x <= x <= minimap.bottom_x and minimap.top_y <= y <= minimap.bottom_y:
-        return minimap.name
-    else:
-        return 'other'
-
-def check(file_path:str):
-    if os.path.exists(file_path):
-        return True
-    else:
-        print('FileNotFoundError')
-        return False
-
-#フレームの読み込みと画像処理の並列化
-def frame_reader(cap, queue):
-    while True:
-        ret, frame = cap.read()
-        if not ret:
-            print('ret is False')
-            break
-        queue.put(frame)
-    queue.put(None)  # signal that all frames have been read
-
-def make_dataset(video_path:str, save:bool = True, get_display:bool = True):
-    #動画の読み込み
-    mov_file = os.path.normpath(video_path)
-    check(mov_file)
-    cap = cv2.VideoCapture(mov_file)
-    total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-    print(f'total_frames:{total_frames}')
-    #中心座標を格納するリスト
-    frame_ids = []
-    eye_x = []
-    eye_y = []
-    rois = []
-    images = []
-    #メインループスタート
-    cap.set(cv2.CAP_PROP_POS_FRAMES, 0)
-    for frame_id in tqdm(range(0,total_frames)):
-        #フレームを取得
-        ret, frame = cap.read()
-        if ret:
-            #get binarized iamge 
-            if frame.shape[0] != 1080:
-                game,eye = sep_y(frame)
-            else:
-                eye = frame
-            bin_image = binarize_image(eye)
-            #get center of biggest object
-            x,y = cog(bin_image.astype(np.uint8))
-            roi = get_roi(x,y)
-            eye_x.append(x)
-            eye_y.append(y)
-            rois.append(roi)
-            frame_ids.append(frame_id)
-        else:
-            print(f'error occurd at frame{frame_id}')
-            break   
-    cap.release()
-    df = pd.DataFrame({'frame_ids':frame_ids,'x':eye_x,'y':eye_y,'roi':rois})
-    if save:
-        # Get the base name of the video file and use it to create csv filename
-        base_name = os.path.basename(video_path)
-        file_name, _ = os.path.splitext(base_name)
-        df.to_csv(f'{file_name}.csv',index=False)
-    if get_display:
-        make_displayonly_video(video_path)
-    return df
-
-def make_dataset_from_folder(folder_path:str, max_workers:int = 4, save:bool = True, get_display:bool = True):
-    # Get a list of all video files in the folder
-    video_files = [f for f in os.listdir(folder_path) if f.endswith('.mp4') or f.endswith('.mkv')]
-
-    video_files = [os.path.join(folder_path, f) for f in video_files]
-
-    with ProcessPoolExecutor(max_workers=max_workers) as executor:
-        # Create a list to hold the Future objects
-        futures = [executor.submit(make_dataset, video_file, save, get_display) for video_file in video_files]
-
-        # Use tqdm for progress bar
-        for future in tqdm(as_completed(futures), total=len(futures)):
-            # Results are ready only when processing is complete, so we don't need to do anything here
-            pass
-if __name__ == "__main__":
-    df = make_dataset('F:\git-repo\get_eyedata\data\test.mkv')
+from .frame_utils import cog, sep_y, binarize_image, make_displayonly_video
+import cv2
+import numpy as np
+import pandas as pd
+from dataclasses import dataclass
+from queue import Queue
+from threading import Thread
+from concurrent.futures import ProcessPoolExecutor, as_completed
+from tqdm import tqdm
+import os
+
+
+@dataclass
+class Area:
+    name: str
+    top_x: int
+    top_y: int
+    bottom_x: int
+    bottom_y: int
+
+
+# minimap = Area('minimap',15,620,435,1040)
+# left_team = Area('left_team',440,0,870,100)
+# right_team = Area('right_team',1050,0,1480,100)
+# timer = Area('timer',870,0,1050,100)
+# kill_log = Area('kill_log',1490,60,1920,300)
+# hp = Area('hp',520,980,685,1080)
+# skill = Area('skill',745,980,1175,1080)
+# amo = Area('amo',1235,980,1400,1080)
+# center = ('center',960,540,125)
+
+minimap = Area('minimap',15,620,435,1040)
+left_team = Area('left_team',440,980,870,1080)
+right_team = Area('right_team',1050,980,1480,1080)
+timer = Area('timer',870,980,1050,1080)
+kill_log = Area('kill_log',1490,780,1920,1020)
+hp = Area('hp',520,0,685,100)
+skill = Area('skill',745,0,1175,100)
+amo = Area('amo',1235,0,1400,100)
+center = ('center',960,540,125)
+
+def get_roi(x, y):
+    if ((x - center[1])**2 + (y - center[2])**2) <= center[3]**2:
+        return center[0]
+    elif left_team.top_x <= x <= left_team.bottom_x and left_team.top_y <= y <= left_team.bottom_y:
+        return left_team.name
+    elif right_team.top_x <= x <= right_team.bottom_x and right_team.top_y <= y <= right_team.bottom_y:
+        return right_team.name
+    elif timer.top_x <= x <= timer.bottom_x and timer.top_y <= y <= timer.bottom_y:
+        return timer.name
+    elif kill_log.top_x <= x <= kill_log.bottom_x and kill_log.top_y <= y <= kill_log.bottom_y:
+        return kill_log.name
+    elif hp.top_x <= x <= hp.bottom_x and hp.top_y <= y <= hp.bottom_y:
+        return hp.name
+    elif skill.top_x <= x <= skill.bottom_x and skill.top_y <= y <= skill.bottom_y:
+        return skill.name
+    elif amo.top_x <= x <= amo.bottom_x and amo.top_y <= y <= amo.bottom_y:
+        return amo.name
+    elif minimap.top_x <= x <= minimap.bottom_x and minimap.top_y <= y <= minimap.bottom_y:
+        return minimap.name
+    else:
+        return 'other'
+
+def check(file_path:str):
+    if os.path.exists(file_path):
+        return True
+    else:
+        print('FileNotFoundError')
+        return False
+
+#フレームの読み込みと画像処理の並列化
+def frame_reader(cap, queue):
+    while True:
+        ret, frame = cap.read()
+        if not ret:
+            print('ret is False')
+            break
+        queue.put(frame)
+    queue.put(None)  # signal that all frames have been read
+
+def make_dataset(video_path:str, save:bool = True, get_display:bool = True):
+    #動画の読み込み
+    mov_file = os.path.normpath(video_path)
+    check(mov_file)
+    cap = cv2.VideoCapture(mov_file)
+    total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+    print(f'total_frames:{total_frames}')
+    #中心座標を格納するリスト
+    frame_ids = []
+    eye_x = []
+    eye_y = []
+    rois = []
+    images = []
+    #メインループスタート
+    cap.set(cv2.CAP_PROP_POS_FRAMES, 0)
+    for frame_id in tqdm(range(0,total_frames)):
+        #フレームを取得
+        ret, frame = cap.read()
+        if ret:
+            #get binarized iamge 
+            if frame.shape[0] != 1080:
+                game,eye = sep_y(frame)
+            else:
+                eye = frame
+            bin_image = binarize_image(eye)
+            #get center of biggest object
+            x,y = cog(bin_image.astype(np.uint8))
+            roi = get_roi(x,y)
+            eye_x.append(x)
+            eye_y.append(y)
+            rois.append(roi)
+            frame_ids.append(frame_id)
+        else:
+            print(f'error occurd at frame{frame_id}')
+            break   
+    cap.release()
+    df = pd.DataFrame({'frame_ids':frame_ids,'x':eye_x,'y':eye_y,'roi':rois})
+    if save:
+        # Get the base name of the video file and use it to create csv filename
+        base_name = os.path.basename(video_path)
+        file_name, _ = os.path.splitext(base_name)
+        df.to_csv(f'{file_name}.csv',index=False)
+    if get_display:
+        make_displayonly_video(video_path)
+    return df
+
+def make_dataset_from_folder(folder_path:str, max_workers:int = 4, save:bool = True, get_display:bool = True):
+    # Get a list of all video files in the folder
+    video_files = [f for f in os.listdir(folder_path) if f.endswith('.mp4') or f.endswith('.mkv')]
+
+    video_files = [os.path.join(folder_path, f) for f in video_files]
+
+    with ProcessPoolExecutor(max_workers=max_workers) as executor:
+        # Create a list to hold the Future objects
+        futures = [executor.submit(make_dataset, video_file, save, get_display) for video_file in video_files]
+
+        # Use tqdm for progress bar
+        for future in tqdm(as_completed(futures), total=len(futures)):
+            # Results are ready only when processing is complete, so we don't need to do anything here
+            pass
+if __name__ == "__main__":
+    df = make_dataset('F:\git-repo\get_eyedata\data\test.mkv')
     print(df)
```

## Comparing `get_eyedata-1.3.3.dist-info/LICENCE` & `get_eyedata-1.3.4.dist-info/LICENCE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Takuma Nobuto
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Takuma Nobuto
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `get_eyedata-1.3.3.dist-info/RECORD` & `get_eyedata-1.3.4.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-get_eyedata/__init__.py,sha256=rqUtJyMLicobcyhmr74TepjmUQAEmlazKT3vjV_n3aA,6
-get_eyedata/frame_utils.py,sha256=YEFiSBzqLeJ12s0KBDzxYVdloB45AgOQrJxU-xGM1Y8,2340
-get_eyedata/ow2.py,sha256=0JS1rvnijzZ7gnaBNZd7v0oCsFmQeZDFr1Qoz7x93tk,3977
-get_eyedata/valo.py,sha256=9NAJFBDHIoHGKbvwIL_5QWDtxheWg_3LPjMBxU5sdEA,5284
-get_eyedata-1.3.3.dist-info/LICENCE,sha256=44r0hK-BnpFZTBiPxTYe52HFlT034sEPBfHrJyaNI0g,1091
-get_eyedata-1.3.3.dist-info/METADATA,sha256=6N1zX0nqzgfvJVAoXakDyCTRkqWzzBRmfYPwfsMhgms,1869
-get_eyedata-1.3.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-get_eyedata-1.3.3.dist-info/top_level.txt,sha256=zlueM7ZefajCSIgOyib56hk_6HWx15EsED6S68g0mWE,12
-get_eyedata-1.3.3.dist-info/RECORD,,
+get_eyedata/__init__.py,sha256=ajz1GSNU9xYVrFEDSz6Xwg7amWQ_yvW75tQa1ZvRIWc,3
+get_eyedata/frame_utils.py,sha256=cy1LDgOX2T3u2geaZtCn931guqBmRi0H3H9ff6Cbfy4,2272
+get_eyedata/ow2.py,sha256=dFbjQEqmxozDQ-7GeVzH7tPED2waP9Uau5Xxx9mNrlU,3861
+get_eyedata/valo.py,sha256=lEjlNiSRLai_RflE6U6sPExGW5nVC6TeUv5-5sJJ3ZU,5142
+get_eyedata/video_edit.py,sha256=UourqZT1TsuvMDsFVhb5skgk8_RUNBQxkHd4yyzST_8,2153
+get_eyedata-1.3.4.dist-info/LICENCE,sha256=nGFMKIMSd6r9IzCIIoNrV5UgwCHzG8i0bYcWhWNy6SE,1070
+get_eyedata-1.3.4.dist-info/METADATA,sha256=nBD8PbCzduVpwKM7XXXRDEzMYItV4S-Ebhfh-ypljHQ,1801
+get_eyedata-1.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+get_eyedata-1.3.4.dist-info/top_level.txt,sha256=zlueM7ZefajCSIgOyib56hk_6HWx15EsED6S68g0mWE,12
+get_eyedata-1.3.4.dist-info/RECORD,,
```

