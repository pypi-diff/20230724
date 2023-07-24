# Comparing `tmp/pdt_extract-0.1.5-py3-none-any.whl.zip` & `tmp/pdt_extract-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 10693 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat    11413 b- defN 23-Apr-25 23:53 pdt_canny.py
--rw-rw-rw-  2.0 fat      136 b- defN 23-May-02 13:45 pdt_extract/__init__.py
--rw-rw-rw-  2.0 fat     5716 b- defN 23-Apr-28 23:10 pdt_extract/feature_extract.py
--rw-rw-rw-  2.0 fat    11583 b- defN 23-May-02 13:36 pdt_extract/pdt_extract.py
--rw-rw-rw-  2.0 fat      662 b- defN 23-May-02 13:46 pdt_extract-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 13:46 pdt_extract-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-02 13:46 pdt_extract-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      633 b- defN 23-May-02 13:46 pdt_extract-0.1.5.dist-info/RECORD
-8 files, 30247 bytes uncompressed, 9593 bytes compressed:  68.3%
+Zip file size: 14549 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx    11133 b- defN 23-Jul-24 17:07 pdt_canny.py
+-rw-rw-r--  2.0 unx      134 b- defN 23-Jul-24 17:07 pdt_extract/__init__.py
+-rw-rw-r--  2.0 unx     9558 b- defN 23-Jul-24 19:29 pdt_extract/feature_extract.py
+-rw-rw-r--  2.0 unx     5747 b- defN 23-Jul-24 17:14 pdt_extract/original_extraction_functions.py
+-rw-rw-r--  2.0 unx    13550 b- defN 23-Jul-24 19:24 pdt_extract/pdt_extract.py
+-rw-rw-r--  2.0 unx      662 b- defN 23-Jul-24 19:34 pdt_extract-0.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-24 19:34 pdt_extract-0.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jul-24 19:34 pdt_extract-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      734 b- defN 23-Jul-24 19:34 pdt_extract-0.1.6.dist-info/RECORD
+9 files, 41622 bytes uncompressed, 13285 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: pdt_extract/__init__.py
 Comment: 
 
 Filename: pdt_extract/feature_extract.py
 Comment: 
 
+Filename: pdt_extract/original_extraction_functions.py
+Comment: 
+
 Filename: pdt_extract/pdt_extract.py
 Comment: 
 
-Filename: pdt_extract-0.1.5.dist-info/METADATA
+Filename: pdt_extract-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: pdt_extract-0.1.5.dist-info/WHEEL
+Filename: pdt_extract-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: pdt_extract-0.1.5.dist-info/top_level.txt
+Filename: pdt_extract-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pdt_extract-0.1.5.dist-info/RECORD
+Filename: pdt_extract-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pdt_canny.py

 * *Ordering differences only*

```diff
@@ -1,280 +1,280 @@
-"""
-Author: Dmitri Lyalikov-Dlyalikov01@manhattan.edu
-
-Canny Edge Detection Processor
-This module will process all image files from the folder: pendant_drops
-and output the extracted canny generated drop profile to the subdirectory: drop_profiles
-
-TODO: Implement Feature extraction from apex radius and:
-    - generate CSV of features from all profiles with extract_from_dir
-    - return dictionary of features {Drop Height, Capillary Radius, Rs, Re} with extract_from_file, extract_from_img
-"""
-
-import imageio
-import os
-from scipy import ndimage
-
-import numpy as np
-from numpy import fft
-import matplotlib.pyplot as plt
-from circle_fit import taubinSVD
-
-
-class DropProfile:
-    def __init__(self, path="Pendant Drops", dest="Drop Profiles"):
-        self.path = path
-        self.destination = dest
-        self.max_height = 0
-        self.max_width = 0
-
-    # Perform bulk profile and feature extraction on all files in self.path
-    # generate drop profile .jpg and save to self.destination
-    def extract_from_dir(self):
-        os.chdir(self.path)
-        for filename in os.listdir():
-            if not os.path.isdir(filename):
-                print(f"Extracting profile from: {filename}...")
-                profile = extract_profile_from_image(os.path.join(filename))
-                os.chdir(self.destination)
-                get_profile(profile, filename)
-                os.chdir("..")
-            else:
-                print(f"not file: {filename}")
-
-        print(f"Done Extracting Profiles")
-
-    # perform extraction of profile and feature set given a path to an image with respect to self.path
-    def extract_from_file(self, fname: str) -> (ndimage, list):
-        os.chdir(self.path)
-        profile = extract_profile_from_image(os.path.join(fname))
-        return get_profile(profile)
-
-    # perform extraction of profile and feature set given a ndimage
-    def extract_from_img(self, img: ndimage) -> (ndimage, list):
-        profile = extract_profile_from_image(img, load=False, path_to_file=None)
-
-
-# label connected components as edge profiles
-def get_profile(final_image, filename=None, save=True):
-    labeled_image, num_features = ndimage.label(final_image)
-    # Remove feature 2 which is the internal noise from light
-    final_image[labeled_image == 2] = 0
-    final_image[labeled_image == 1] = 255
-    final_image = split_profile(final_image)
-    R0 = find_apex_radius(final_image, 0.15, 0.005)
-    print(f"Apex_Radius (cm): {R0}")  # 0.05 /44
-    show_image(final_image)
-
-    fft_profile(final_image)
-    if save:
-        imageio.imwrite(filename, np.uint8(final_image))
-    else:
-        return final_image, {"Apex Radius": R0}
-
-
-# Use Circle fit to approximate apex radius of edge profile
-# ratio_drop_length: 1 >= float value > 0 representing number points along profile to approximate with
-# change_ro: float value representing minimum value of change in circle radius before stopping approximation
-def find_apex_radius(profile: ndimage, ratio_drop_length: float, change_ro: float) -> float:
-    indices = np.where(profile == 255)
-    x = np.flip(indices[1])
-    y = np.flip(indices[0])
-
-    num_point_ro_circlefit = round(len(x) * ratio_drop_length) + 1
-
-    percent_drop_ro = 0.1
-    i = 0
-    diff = 0
-    r0 = 0
-    r_0 = []
-    while diff >= change_ro*r0 or num_point_ro_circlefit <= percent_drop_ro * len(x):
-        points_ro_circlefit = np.stack((x[:num_point_ro_circlefit], y[:num_point_ro_circlefit]), axis=1)
-        xc, yc, r0, sigma = taubinSVD(points_ro_circlefit)
-        r_0.append(r0)
-        if i > 1:
-            diff = abs(r_0[i] - r_0[i-1])
-        i += 1
-        num_point_ro_circlefit += 1
-
-    return r_0[-1]
-
-
-#    Execute the Canny Sequence on the image
-#    gaussian_blur_sigma value = 1.2
-#    high_threshold_ratio = 0.2
-#    low_threshold_ratio = 0.15
-def extract_profile_from_image(path_to_file: str, img: ndimage = None, load=True):
-    if load:
-        img = load_convert_image(path_to_file)
-    dx = ndimage.sobel(img, axis=1)  # horizontal derivative
-    dy = ndimage.sobel(img, axis=0)  # vertical derivative
-    mag = normalize(np.hypot(dx, dy))
-    gradient = np.degrees(np.arctan2(dy, dx))
-    nms = normalize(nms_with_interpol(mag, gradient, dx, dy))
-    profile = hysteresis_threshold(nms)
-    return profile
-
-
-# We have a grayscale ndarray.
-# We want to find the vertically-lowest pixel that has the value 255.
-# When we find that column, before cutting the image and keeping the right side,
-# we need to make sure it is either the only vertical minimum,
-# or find the midpoint between the furthest away vertical minimum column and split the image at that midpoint instead
-def split_profile(img: ndimage):
-    # Find the indices of all pixels with value 255 along the vertical axis
-    indices = np.where(img == 255)[0]
-
-    # Find the lowest index, which corresponds to the lowest pixel in the image with value 255
-    lowest_index = np.min(indices)
-
-    # Find the columns that have this lowest pixel value
-    cols = np.where(img[lowest_index, :] == 255)[0]
-
-    # If there is only one such column, use it as the cutting point
-    if len(cols) == 1:
-        cutting_point = cols[0]
-
-    # Otherwise, find the midpoint between the furthest away vertical minimum columns
-    else:
-        left_col = cols[0]
-        right_col = cols[-1]
-        midpoint = (left_col + right_col) // 2
-        cutting_point = midpoint
-
-    # Cut the image and keep the right side
-    return img[:, cutting_point:]
-
-
-def show_image(img):
-    plt.imshow(img, cmap=plt.get_cmap('gray'))
-    plt.show()
-
-
-# Load the next image in subdir
-# img: passed in as full directory
-def load_convert_image(img: str, sigma_val=1.2):
-    lion = imageio.v2.imread(img, None)
-    lion_gray = np.dot(lion[..., :3], [0.299, 0.587, 0.114])
-    # Optionally change or take parameter for sigma
-    img = ndimage.gaussian_filter(lion_gray, sigma=sigma_val)
-    return img
-
-
-# Normalize the pixel array, so that values are <= 1
-def normalize(img):
-    img = img / np.max(img)
-    return img
-
-
-# Do Non-Maximum Suppression with interpolation to get a better
-# Estimate of the magnitude values of the pixels in the gradient
-# Direction. This is done to get thin edges
-def nms_with_interpol(g_mag, grad, gx, gy):
-    nms = np.zeros(g_mag.shape)
-
-    for i in range(1, int(g_mag.shape[0]) - 1):
-        for j in range(1, int(g_mag.shape[1]) - 1):
-            if grad[i, j] >= 0 and grad[i, j] <= 45 or grad[i, j] < -135 and grad[i, j] >= -180:
-                y_bot = np.array([g_mag[i, j + 1], g_mag[i + 1, j + 1]])
-                y_top = np.array([g_mag[i, j - 1], g_mag[i - 1, j - 1]])
-                x_est = np.absolute(gy[i, j] / g_mag[i, j])
-                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
-                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
-                    nms[i, j] = g_mag[i, j]
-                else:
-                    nms[i, j] = 0
-            if grad[i, j] > 45 and grad[i, j] <= 90 or grad[i, j] < -90 and grad[i, j] >= -135:
-                y_bot = np.array([g_mag[i + 1, j], g_mag[i + 1, j + 1]])
-                y_top = np.array([g_mag[i - 1, j], g_mag[i - 1, j - 1]])
-                x_est = np.absolute(gx[i, j] / g_mag[i, j])
-                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
-                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
-                    nms[i, j] = g_mag[i, j]
-                else:
-                    nms[i, j] = 0
-            if grad[i, j] > 90 and grad[i, j] <= 135 or grad[i, j] < -45 and grad[i, j] >= -90:
-                y_bot = np.array([g_mag[i + 1, j], g_mag[i + 1, j - 1]])
-                y_top = np.array([g_mag[i - 1, j], g_mag[i - 1, j + 1]])
-                x_est = np.absolute(gx[i, j] / g_mag[i, j])
-                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
-                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
-                    nms[i, j] = g_mag[i, j]
-                else:
-                    nms[i, j] = 0
-            if grad[i, j] > 135 and grad[i, j] <= 180 or grad[i, j] < 0 and grad[i, j] >= -45:
-                y_bot = np.array([g_mag[i, j - 1], g_mag[i + 1, j - 1]])
-                y_top = np.array([g_mag[i, j + 1], g_mag[i - 1, j + 1]])
-                x_est = np.absolute(gy[i, j] / g_mag[i, j])
-                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
-                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
-                    nms[i, j] = g_mag[i, j]
-                else:
-                    nms[i, j] = 0
-
-    return nms
-
-
-# Double threshold Hysteresis
-def hysteresis_threshold(img, high_threshold_ratio=0.2, low_threshold_ratio=0.15):
-    high_threshold_ratio = 0.2
-    low_threshold_ratio = 0.15
-    g_sup = np.copy(img)
-    h = int(g_sup.shape[0])
-    w = int(g_sup.shape[1])
-    high_threshold = np.max(g_sup) * high_threshold_ratio
-    low_threshold = high_threshold * low_threshold_ratio
-    x = 0.1
-    old_x = 0
-
-    # The while loop is used so that the loop will keep executing till the number of strong edges
-    # do not change, i.e. all weak edges connected to strong edges have been found
-    while old_x != x:
-        old_x = x
-        for i in range(1, h - 1):
-            for j in range(1, w - 1):
-                if g_sup[i, j] > high_threshold:
-                    g_sup[i, j] = 1
-                elif g_sup[i, j] < low_threshold:
-                    g_sup[i, j] = 0
-                else:
-                    if ((g_sup[i - 1, j - 1] > high_threshold) or
-                            (g_sup[i - 1, j] > high_threshold) or
-                            (g_sup[i - 1, j + 1] > high_threshold) or
-                            (g_sup[i, j - 1] > high_threshold) or
-                            (g_sup[i, j + 1] > high_threshold) or
-                            (g_sup[i + 1, j - 1] > high_threshold) or
-                            (g_sup[i + 1, j] > high_threshold) or
-                            (g_sup[i + 1, j + 1] > high_threshold)):
-                        g_sup[i, j] = 1
-        x = np.sum(g_sup == 1)
-
-    # This is done to remove/clean all the weak edges which are not connected to strong edges
-    g_sup = (g_sup == 1) * g_sup
-
-    return g_sup
-
-
-# Remove connected edges that are noise
-# Assuming edge profile is the longest edge
-def extract_profile(img):
-    labeled_image, num_features = ndimage.label(img)
-    # Remove all features that are not labeled 1 or 0, (profile or background)
-    img[labeled_image == 2] = 0
-    img[labeled_image == 1] = 255
-    return img
-
-
-# Fast Fourier Transform of edge profile
-# Can expect high frequency components in magnitude spectrum of edges
-# Computed in Decibels
-def fft_profile(profile):
-    fft_image = fft.fft2(profile)
-    fft_image = fft.fftshift(fft_image)
-    # Shift the zero-frequency component to the center of the spectrum
-    magnitude_spectrum = 20 * np.log(np.abs(fft_image))
-    phase_spectrum = np.angle(fft_image)
-
-
-if __name__ == '__main__':
-    profiles = DropProfile()
-    profiles.extract_from_dir()
+"""
+Author: Dmitri Lyalikov-Dlyalikov01@manhattan.edu
+
+Canny Edge Detection Processor
+This module will process all image files from the folder: pendant_drops
+and output the extracted canny generated drop profile to the subdirectory: drop_profiles
+
+TODO: Implement Feature extraction from apex radius and:
+    - generate CSV of features from all profiles with extract_from_dir
+    - return dictionary of features {Drop Height, Capillary Radius, Rs, Re} with extract_from_file, extract_from_img
+"""
+
+import imageio
+import os
+from scipy import ndimage
+
+import numpy as np
+from numpy import fft
+import matplotlib.pyplot as plt
+from circle_fit import taubinSVD
+
+
+class DropProfile:
+    def __init__(self, path="Pendant Drops", dest="Drop Profiles"):
+        self.path = path
+        self.destination = dest
+        self.max_height = 0
+        self.max_width = 0
+
+    # Perform bulk profile and feature extraction on all files in self.path
+    # generate drop profile .jpg and save to self.destination
+    def extract_from_dir(self):
+        os.chdir(self.path)
+        for filename in os.listdir():
+            if not os.path.isdir(filename):
+                print(f"Extracting profile from: {filename}...")
+                profile = extract_profile_from_image(os.path.join(filename))
+                os.chdir(self.destination)
+                get_profile(profile, filename)
+                os.chdir("..")
+            else:
+                print(f"not file: {filename}")
+
+        print(f"Done Extracting Profiles")
+
+    # perform extraction of profile and feature set given a path to an image with respect to self.path
+    def extract_from_file(self, fname: str) -> (ndimage, list):
+        os.chdir(self.path)
+        profile = extract_profile_from_image(os.path.join(fname))
+        return get_profile(profile)
+
+    # perform extraction of profile and feature set given a ndimage
+    def extract_from_img(self, img: ndimage) -> (ndimage, list):
+        profile = extract_profile_from_image(img, load=False, path_to_file=None)
+
+
+# label connected components as edge profiles
+def get_profile(final_image, filename=None, save=True):
+    labeled_image, num_features = ndimage.label(final_image)
+    # Remove feature 2 which is the internal noise from light
+    final_image[labeled_image == 2] = 0
+    final_image[labeled_image == 1] = 255
+    final_image = split_profile(final_image)
+    R0 = find_apex_radius(final_image, 0.15, 0.005)
+    print(f"Apex_Radius (cm): {R0}")  # 0.05 /44
+    show_image(final_image)
+
+    fft_profile(final_image)
+    if save:
+        imageio.imwrite(filename, np.uint8(final_image))
+    else:
+        return final_image, {"Apex Radius": R0}
+
+
+# Use Circle fit to approximate apex radius of edge profile
+# ratio_drop_length: 1 >= float value > 0 representing number points along profile to approximate with
+# change_ro: float value representing minimum value of change in circle radius before stopping approximation
+def find_apex_radius(profile: ndimage, ratio_drop_length: float, change_ro: float) -> float:
+    indices = np.where(profile == 255)
+    x = np.flip(indices[1])
+    y = np.flip(indices[0])
+
+    num_point_ro_circlefit = round(len(x) * ratio_drop_length) + 1
+
+    percent_drop_ro = 0.1
+    i = 0
+    diff = 0
+    r0 = 0
+    r_0 = []
+    while diff >= change_ro*r0 or num_point_ro_circlefit <= percent_drop_ro * len(x):
+        points_ro_circlefit = np.stack((x[:num_point_ro_circlefit], y[:num_point_ro_circlefit]), axis=1)
+        xc, yc, r0, sigma = taubinSVD(points_ro_circlefit)
+        r_0.append(r0)
+        if i > 1:
+            diff = abs(r_0[i] - r_0[i-1])
+        i += 1
+        num_point_ro_circlefit += 1
+
+    return r_0[-1]
+
+
+#    Execute the Canny Sequence on the image
+#    gaussian_blur_sigma value = 1.2
+#    high_threshold_ratio = 0.2
+#    low_threshold_ratio = 0.15
+def extract_profile_from_image(path_to_file: str, img: ndimage = None, load=True):
+    if load:
+        img = load_convert_image(path_to_file)
+    dx = ndimage.sobel(img, axis=1)  # horizontal derivative
+    dy = ndimage.sobel(img, axis=0)  # vertical derivative
+    mag = normalize(np.hypot(dx, dy))
+    gradient = np.degrees(np.arctan2(dy, dx))
+    nms = normalize(nms_with_interpol(mag, gradient, dx, dy))
+    profile = hysteresis_threshold(nms)
+    return profile
+
+
+# We have a grayscale ndarray.
+# We want to find the vertically-lowest pixel that has the value 255.
+# When we find that column, before cutting the image and keeping the right side,
+# we need to make sure it is either the only vertical minimum,
+# or find the midpoint between the furthest away vertical minimum column and split the image at that midpoint instead
+def split_profile(img: ndimage):
+    # Find the indices of all pixels with value 255 along the vertical axis
+    indices = np.where(img == 255)[0]
+
+    # Find the lowest index, which corresponds to the lowest pixel in the image with value 255
+    lowest_index = np.min(indices)
+
+    # Find the columns that have this lowest pixel value
+    cols = np.where(img[lowest_index, :] == 255)[0]
+
+    # If there is only one such column, use it as the cutting point
+    if len(cols) == 1:
+        cutting_point = cols[0]
+
+    # Otherwise, find the midpoint between the furthest away vertical minimum columns
+    else:
+        left_col = cols[0]
+        right_col = cols[-1]
+        midpoint = (left_col + right_col) // 2
+        cutting_point = midpoint
+
+    # Cut the image and keep the right side
+    return img[:, cutting_point:]
+
+
+def show_image(img):
+    plt.imshow(img, cmap=plt.get_cmap('gray'))
+    plt.show()
+
+
+# Load the next image in subdir
+# img: passed in as full directory
+def load_convert_image(img: str, sigma_val=1.2):
+    lion = imageio.v2.imread(img, None)
+    lion_gray = np.dot(lion[..., :3], [0.299, 0.587, 0.114])
+    # Optionally change or take parameter for sigma
+    img = ndimage.gaussian_filter(lion_gray, sigma=sigma_val)
+    return img
+
+
+# Normalize the pixel array, so that values are <= 1
+def normalize(img):
+    img = img / np.max(img)
+    return img
+
+
+# Do Non-Maximum Suppression with interpolation to get a better
+# Estimate of the magnitude values of the pixels in the gradient
+# Direction. This is done to get thin edges
+def nms_with_interpol(g_mag, grad, gx, gy):
+    nms = np.zeros(g_mag.shape)
+
+    for i in range(1, int(g_mag.shape[0]) - 1):
+        for j in range(1, int(g_mag.shape[1]) - 1):
+            if grad[i, j] >= 0 and grad[i, j] <= 45 or grad[i, j] < -135 and grad[i, j] >= -180:
+                y_bot = np.array([g_mag[i, j + 1], g_mag[i + 1, j + 1]])
+                y_top = np.array([g_mag[i, j - 1], g_mag[i - 1, j - 1]])
+                x_est = np.absolute(gy[i, j] / g_mag[i, j])
+                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
+                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
+                    nms[i, j] = g_mag[i, j]
+                else:
+                    nms[i, j] = 0
+            if grad[i, j] > 45 and grad[i, j] <= 90 or grad[i, j] < -90 and grad[i, j] >= -135:
+                y_bot = np.array([g_mag[i + 1, j], g_mag[i + 1, j + 1]])
+                y_top = np.array([g_mag[i - 1, j], g_mag[i - 1, j - 1]])
+                x_est = np.absolute(gx[i, j] / g_mag[i, j])
+                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
+                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
+                    nms[i, j] = g_mag[i, j]
+                else:
+                    nms[i, j] = 0
+            if grad[i, j] > 90 and grad[i, j] <= 135 or grad[i, j] < -45 and grad[i, j] >= -90:
+                y_bot = np.array([g_mag[i + 1, j], g_mag[i + 1, j - 1]])
+                y_top = np.array([g_mag[i - 1, j], g_mag[i - 1, j + 1]])
+                x_est = np.absolute(gx[i, j] / g_mag[i, j])
+                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
+                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
+                    nms[i, j] = g_mag[i, j]
+                else:
+                    nms[i, j] = 0
+            if grad[i, j] > 135 and grad[i, j] <= 180 or grad[i, j] < 0 and grad[i, j] >= -45:
+                y_bot = np.array([g_mag[i, j - 1], g_mag[i + 1, j - 1]])
+                y_top = np.array([g_mag[i, j + 1], g_mag[i - 1, j + 1]])
+                x_est = np.absolute(gy[i, j] / g_mag[i, j])
+                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
+                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
+                    nms[i, j] = g_mag[i, j]
+                else:
+                    nms[i, j] = 0
+
+    return nms
+
+
+# Double threshold Hysteresis
+def hysteresis_threshold(img, high_threshold_ratio=0.2, low_threshold_ratio=0.15):
+    high_threshold_ratio = 0.2
+    low_threshold_ratio = 0.15
+    g_sup = np.copy(img)
+    h = int(g_sup.shape[0])
+    w = int(g_sup.shape[1])
+    high_threshold = np.max(g_sup) * high_threshold_ratio
+    low_threshold = high_threshold * low_threshold_ratio
+    x = 0.1
+    old_x = 0
+
+    # The while loop is used so that the loop will keep executing till the number of strong edges
+    # do not change, i.e. all weak edges connected to strong edges have been found
+    while old_x != x:
+        old_x = x
+        for i in range(1, h - 1):
+            for j in range(1, w - 1):
+                if g_sup[i, j] > high_threshold:
+                    g_sup[i, j] = 1
+                elif g_sup[i, j] < low_threshold:
+                    g_sup[i, j] = 0
+                else:
+                    if ((g_sup[i - 1, j - 1] > high_threshold) or
+                            (g_sup[i - 1, j] > high_threshold) or
+                            (g_sup[i - 1, j + 1] > high_threshold) or
+                            (g_sup[i, j - 1] > high_threshold) or
+                            (g_sup[i, j + 1] > high_threshold) or
+                            (g_sup[i + 1, j - 1] > high_threshold) or
+                            (g_sup[i + 1, j] > high_threshold) or
+                            (g_sup[i + 1, j + 1] > high_threshold)):
+                        g_sup[i, j] = 1
+        x = np.sum(g_sup == 1)
+
+    # This is done to remove/clean all the weak edges which are not connected to strong edges
+    g_sup = (g_sup == 1) * g_sup
+
+    return g_sup
+
+
+# Remove connected edges that are noise
+# Assuming edge profile is the longest edge
+def extract_profile(img):
+    labeled_image, num_features = ndimage.label(img)
+    # Remove all features that are not labeled 1 or 0, (profile or background)
+    img[labeled_image == 2] = 0
+    img[labeled_image == 1] = 255
+    return img
+
+
+# Fast Fourier Transform of edge profile
+# Can expect high frequency components in magnitude spectrum of edges
+# Computed in Decibels
+def fft_profile(profile):
+    fft_image = fft.fft2(profile)
+    fft_image = fft.fftshift(fft_image)
+    # Shift the zero-frequency component to the center of the spectrum
+    magnitude_spectrum = 20 * np.log(np.abs(fft_image))
+    phase_spectrum = np.angle(fft_image)
+
+
+if __name__ == '__main__':
+    profiles = DropProfile()
+    profiles.extract_from_dir()
```

## pdt_extract/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
-from pdt_extract.pdt_extract import DropProfile
-from feature_extract import FeatureExtract
+from pdt_extract.pdt_extract import DropProfile
+from feature_extract import FeatureExtract
 __all__ = ['DropProfile', 'FeatureExtract']
```

## pdt_extract/feature_extract.py

```diff
@@ -1,141 +1,262 @@
-"""
-Author: Dmitri Lyalikov
-Email:  Dlyalikov01@manhattan.edu
-Date of last revision: 04/28/2023
-
-Status:
-    in development / validating
-
-feature_extract.py
-    This module performs characteristic feature extraction on the x and y coordinates of an
-    edge profile.
-    These methods derive numerical profile characteristics of the pendant drop
-        - Apex Radius: Found with circle fit approximation
-        - Equator Radius
-        - Radius_S: Radius at y = 2 * (Equator Radius
-        - Drop_Height
-        - Capillary Radius
-    By instantiating a FeatureExtract object with the x, y profile coordinates, all of these features
-    are automatically saved to a dictionary: self.feature_set as a key, value pair
-"""
-
-import numpy as np
-from circle_fit import taubinSVD
-
-
-class FeatureExtract:
-    def __init__(self, x: list[int], y: list[int]):
-        """
-        :param x: globally used ordered set of x coordinates of the pendant drop profile
-        :param y: globally used ordered set of x coordinates of the pendant drop profile
-        """
-
-        self.x = x
-        self.y = y
-
-        self.capillary_radius = self.x[-1]
-        self.drop_height = self.y[0]
-        self.equator_radius = self.find_equator_radius()
-        self.s_radius = self.find_s_radius()
-        self.apex_radius = self.find_apex_radius()
-        # Normalize to dimensionless ratio to apex radius
-        self.feature_set = {
-            "Drop height": self.drop_height / self.apex_radius,
-            "Capillary radius": self.capillary_radius / self.apex_radius,
-            "R-s": self.s_radius / self.apex_radius,
-            "R-e": self.equator_radius / self.apex_radius,
-        }
-        print(f"Apex radius (Pixels): {self.apex_radius }")
-        print(f"Equator radius: {self.equator_radius }\n"
-              f"S radius: {self.s_radius }\n"
-              f"Capillary radius: {self.capillary_radius}\n"
-              f"Drop Height: {self.drop_height }")
-
-    def average_x(self, i: int, n: int) -> int:
-        s = 0
-        for j in range(i-n, i+n+1):
-            s = s + self.x[j]
-        return s / (2 * n + 1)
-
-    def recursive_equator_radius(self, i, n):
-        # use recursive approach: start from apex, continue until x decreases
-        # at i-th point we average x of x-n to x+n to suppress noise
-        # compare x-i_th vs x_i+t_th until it decreases to find equator
-        if self.average_x(i, n) < self.average_x(i+1, n) and i <= len(self.x) - n-3:
-            i += 1
-            output = self.recursive_equator_radius(i, n)
-            if output:
-                self.equator_radius = output
-        else:
-            if i <= len(self.x) * 0.7:
-                # assumed 70% of drop is enough for the equator radius
-                return self.x[i]
-            else:
-                return
-
-    def find_re_rs(self, n=5) -> (int, int):
-        # Finding Equator Radius (Re) and Rs @ y=2Re
-        """
-        ;param self:
-        :param n:
-        :return: tuple (equator_radius: int, s_radius: int)
-        """
-
-        i = n
-        self.equator_radius = 0
-        # A recursive function that returns equator radius
-        self.recursive_equator_radius(i, n)
-        if self.equator_radius == 0:
-
-            # equator radius is 0: drop is not well-deformed: Beta>0.7
-            # find equator radius from circle fitting
-            # select 40% of the total number of points for circle fitting
-            num_points_to_circlefit = round(0.4 * len(self.x))
-            points_rh_circlefit = np.stack(
-                (self.x[:num_points_to_circlefit],
-                 self.y[:num_points_to_circlefit]), axis=1)
-            xc, yc, self.equator_radius, sigma = taubinSVD(points_rh_circlefit)
-
-        # Find s_radius at y = 2 * equator_radius
-        if self.equator_radius < 0.5 * self.drop_height:
-            # res = index of y if y > 2 * equator_radius
-            res = next(xx for xx, val in enumerate(self.y) if val > 2 * self.equator_radius)
-            self.s_radius = self.x[res]
-        else:
-            # Drop is too small
-            self.s_radius = self.capillary_radius
-        return self.equator_radius, self.s_radius
-
-    # Use Circle fit to approximate apex radius of edge profile
-    # ratio_drop_length: 1 >= float value > 0 representing number points along profile to approximate with
-    # change_ro: float value representing minimum value of change in circle radius before stopping approximation
-    def find_apex_radius(self, ratio_drop_length: float = 0.15, change_ro: float = .005) -> float:
-
-        num_point_ro_circlefit = round(len(self.x) * ratio_drop_length) + 1
-
-        percent_drop_ro = 0.1
-        i = 0
-        diff = 0
-        r0 = 0
-        r_0 = []
-        while diff >= change_ro*r0 or num_point_ro_circlefit <= percent_drop_ro * len(self.x):
-            points_ro_circlefit = np.stack((self.x[:num_point_ro_circlefit], self.y[:num_point_ro_circlefit]), axis=1)
-            xc, yc, r0, sigma = taubinSVD(points_ro_circlefit)
-            r_0.append(r0)
-            if i > 1:
-                diff = abs(r_0[i] - r_0[i-1])
-            i += 1
-            num_point_ro_circlefit += 1
-
-        return r_0[-1]
-
-    # Find maximum (bulge) x value from 70% of profile
-    def find_equator_radius(self):
-        split = int(len(self.x) * 0.7)
-
-        # Slice the first 70% of the list from bottom and find the maximum value
-        return max(self.x[:split])
-
-    # Find radius at point X = [2 * equator_radius] between capillary and equator
-    def find_s_radius(self):
-        return self.x[-2 * int(self.equator_radius)]
+"""
+feature_extract.py
+
+- Author: Dmitri Lyalikov
+- Email:  Dlyalikov01@manhattan.edu
+- Date of last revision: 05/02/2023
+- Status: in development / validating
+
+This module performs characteristic feature extraction on the x and y coordinates of an
+edge profile.
+These methods derive numerical profile characteristics of the pendant drop:
+    - Apex Radius: Found with circle fit approximation
+    - Equator Radius
+    - Radius_S: Radius at y = 2 * (Equator Radius
+    - Drop_Height
+    - Capillary Radius
+By instantiating a FeatureExtract object with the x, y profile coordinates, all of these features
+are automatically saved to a dictionary: self.feature_set as a key, value pair
+"""
+
+import numpy as np
+from circle_fit import taubinSVD
+import matplotlib.pyplot as plt
+
+class FeatureExtract:
+    def __init__(self, x: list[int], y: list[int]):
+        """
+        :param x: globally used ordered set of x coordinates of the pendant drop profile
+        :param y: globally used ordered set of x coordinates of the pendant drop profile
+        """
+
+        # dbg_log = file.open("FeatureExtract-Dbg-log.txt", 'a')
+
+
+        self.x = x
+        self.y = y
+
+        self.capillary_radius = self.x[-1]
+        self.drop_height = self.y[0]
+        self.equator_radius, self.s_radius = self.find_re_rs()
+        #self.equator_radius, self.s_radius = Find_Re_Rs(x[::-1], y[::-1], 5, self.drop_height, self.capillary_radius)
+        self.equator_radius, self.s_radius, self.re_pos, self.rs_pos = Find_Re_Rs(x[::-1], y[::-1], 5, self.drop_height, self.capillary_radius)
+        # self.s_radius = self.find_s_radius(equator_index)
+        self.apex_radius = self.find_apex_radius()
+        #self.print_debug_log("After init")
+        # Normalize to dimensionless ratio to apex radius
+        self.feature_set = {
+            "Drop height": self.drop_height / self.apex_radius,
+            "Capillary radius": self.capillary_radius / self.apex_radius,
+            "R-s": self.s_radius / self.apex_radius,
+            "R-e": self.equator_radius / self.apex_radius,
+            "Apex Radius": self.apex_radius
+        }
+        print(f"Apex radius (Pixels): {self.apex_radius }")
+        print(f"Equator radius: {self.equator_radius }\n"
+              f"S radius: {self.s_radius }\n"
+              f"Capillary radius: {self.capillary_radius}\n"
+              f"Drop Height: {self.drop_height }")
+        self.reconstruct()
+
+    def show_features(self):
+        str_features = ""
+        for key, value in self.feature_set.items():
+            str_features += key + " " + str(value) + " "
+        return str_features
+
+    def average_x(self, i: int, n: int) -> int:
+        s = 0
+        for j in range(i-n, i+n+1):
+            s = s + self.x[j]
+        return s / (2 * n + 1)
+
+    def recursive_equator_radius(self, i, n):
+        # use recursive approach: start from apex, continue until x decreases
+        # at i-th point we average x of x-n to x+n to suppress noise
+        # compare x-i_th vs x_i+t_th until it decreases to find equator
+        if self.average_x(i, n) < self.average_x(i+1, n) and i <= len(self.x) - n-3:
+            i += 1
+            output = self.recursive_equator_radius(i, n)
+            if output is not None:
+                self.equator_radius = output
+        else:
+            if i <= len(self.x) * 0.7:
+                # assumed 70% of drop is enough for the equator radius
+                return self.x[i]
+            else:
+                return
+
+    def find_re_rs(self, n=5) -> (int, int):
+        # Finding Equator Radius (Re) and Rs @ y=2Re
+        """
+        ;param self:
+        :param n:
+        :return: tuple (equator_radius: int, s_radius: int)
+        """
+
+        i = n
+        self.equator_radius = 0
+        # A recursive function that returns equator radius
+        self.recursive_equator_radius(i, n)
+        if self.equator_radius == 0:
+
+            # equator radius is 0: drop is not well-deformed: Beta>0.7
+            # find equator radius from circle fitting
+            # select 40% of the total number of points for circle fitting
+            num_points_to_circlefit = round(0.4 * len(self.x))
+            points_rh_circlefit = np.stack(
+                (self.x[:num_points_to_circlefit],
+                 self.y[:num_points_to_circlefit]), axis=1)
+            xc, yc, self.equator_radius, sigma = taubinSVD(points_rh_circlefit)
+
+        # Find s_radius at y = 2 * equator_radius
+        if self.equator_radius < 0.5 * self.drop_height:
+            # res = index of y if y > 2 * equator_radiuso
+            res = next(xx for xx, val in enumerate(self.y) if val > 2 * self.equator_radius)
+            self.s_radius = self.x[res]
+        else:
+            # Drop is too small
+            self.s_radius = self.capillary_radius
+        return self.equator_radius, self.s_radius
+
+    # Use Circle fit to approximate apex radius of edge profile
+    # ratio_drop_length: 1 >= float value > 0 representing number points along profile to approximate with
+    # change_ro: float value representing minimum value of change in circle radius before stopping approximation
+    def find_apex_radius(self, ratio_drop_length: float = 0.15, change_ro: float = .005) -> float:
+
+        num_point_ro_circlefit = round(len(self.x) * ratio_drop_length) + 1
+
+        percent_drop_ro = 0.1
+        i = 0
+        diff = 0
+        r0 = 0
+        r_0 = []
+        while diff >= change_ro*r0 or num_point_ro_circlefit <= percent_drop_ro * len(self.x):
+            points_ro_circlefit = np.stack((self.x[:num_point_ro_circlefit], self.y[:num_point_ro_circlefit]), axis=1)
+            xc, yc, r0, sigma = taubinSVD(points_ro_circlefit)
+            r_0.append(r0)
+            if i > 1:
+                diff = abs(r_0[i] - r_0[i-1])
+            i += 1
+            num_point_ro_circlefit += 1
+        self.apex_pos = len(r_0)
+        return r_0[-1]
+
+    # Find maximum (bulge) x value from 70% of profile
+    def find_equator_radius(self):
+        split = int(len(self.x) * 0.7)
+
+        # Slice the first 70% of the list from bottom and find the maximum value
+        return max(self.x[:split]), np.argmax(self.x[:split])
+
+    # Find radius at point X = [2 * equator_radius] between capillary and equator
+    def find_s_radius(self, equator_index):
+        print(equator_index)
+        rs_index = ((len(self.x) - equator_index) / 2) + equator_index
+        print(rs_index)
+        return self.x[int(rs_index)]
+
+    def Find_Re_Rs(self, x, y, n):
+        global R_e
+        R_e = 0
+        i = n
+
+    def reconstruct(self):
+        image_array = np.zeros((500, 500), dtype=np.uint8)
+        #for x, y in zip(self.x, self.y):
+        #    image_array[y, x] = 255
+        xdh, ydh = self.show_drop_height()
+        for x, y in zip(xdh, ydh):
+            image_array[y, x] = 255
+        xcap, ycap= self.show_cap()
+        for x, y in zip(xcap, ycap):
+            image_array[y, x] = 255
+        xa, ya= self.show_apex()
+        for x, y in zip(xa, ya):
+            image_array[y, x] = 255
+        xre, yre, xrs, yrs = self.show_rs_re()
+        for x, y in zip(xre, yre):
+            image_array[y, x] = 255
+        for x, y in zip(xrs, yrs):
+            image_array[y, x] = 255
+        self.show_image(image_array)
+
+    def show_image(self, img):
+        plt.imshow(img, cmap=plt.get_cmap('gray'))
+        plt.show()
+
+    def show_drop_height(self):
+        x, y = [], []
+        for i in range(self.drop_height):
+            x.append(5)
+            y.append(i)
+        return x, y
+
+    def show_cap(self):
+        x, y = [], []
+        for i in range(self.capillary_radius):
+            x.append(i)
+            y.append(5)
+        return x, y
+
+    def show_rs_re(self):
+        xre, yre, xrs, yrs = [], [],  [], []
+        for i in range(int(self.equator_radius)):
+            xre.append(i)
+            yre.append(self.y[int(self.re_pos)])
+        print(self.rs_pos)
+        if self.rs_pos == None:
+            xrs, yrs = self.show_cap()
+        else:
+            for i in range(int(self.s_radius)):
+                xre.append(i)
+                yre.append(self.y[int(self.rs_pos)])
+        return xre, yre, xrs, yrs
+    def show_apex(self):
+        xa, ya = [], []
+        for i in range(int(self.apex_radius)):
+            xa.append(i)
+            ya.append(self.y[self.apex_pos])
+        return xa, ya
+def Find_Re_Rs(x,y,n,Drop_Height, R_Cap):
+  rs_pos, re_pos = 0, 0
+  #Averaging function used in
+  def Average_x(x,i,n):
+  # i-n>=0. So I set i=n
+    s=0
+    for j in range(i-n,i+n+1):
+        s=s+x[j]
+    return s/(2*n+1)
+
+  #Finding Re using updated recursive.
+  def Recur_Equator_Radius(x,i,n):
+  #base condition
+      if Average_x(x,i,n)>Average_x(x,i+1,n):
+        re_pos = i
+        return x[i]
+      elif i>=len(x)-n-3 or i>len(x)*0.7:
+        # I searcg 70% for finding R_e
+        return None
+      return Recur_Equator_Radius(x,i+1,n)
+  i=n
+  R_e=Recur_Equator_Radius(x,i+1,n)
+  if R_e is None:
+  # R_e=None: drop is not well-deformed e.g. Beta>0.7. Find R_e from cirle fitting
+  # I selected 30% of the total number of points for circle fitting
+    num_point_RH_Circlefit=round(0.3*len(x))
+    Points_RH_Circlefit=np.stack((x[:num_point_RH_Circlefit],y[:num_point_RH_Circlefit]),axis=1)
+    xc, yc, R_e, sigma = taubinSVD(Points_RH_Circlefit)
+    re_pos = xc
+  # Find R_s at y=2*R_e
+  if R_e<0.5*Drop_Height:
+    #res=index of y if y>2*R_e
+    res = next(xx for xx, val in enumerate(y) if val > 2*R_e)
+    R_s=x[res]
+    rs_pos = res
+
+  else:
+    # Drop is too small
+    R_s=R_Cap
+    rs_pos = 0
+  return R_e,R_s, re_pos, rs_pos
+
```

## pdt_extract/pdt_extract.py

```diff
@@ -1,277 +1,332 @@
-"""
-Author: Dmitri Lyalikov
-Email:  Dlyalikov01@manhattan.edu
-Date of last revision: 04/28/2023
-
-Status:
-    in development / validating
-
-pdt-extract.py
-    This module is the entry point and controller of the profile and feature extraction sequence
-    implemented by the pdt-extract project.
-    It can be used as a standalone script or imported with DropProfile class to:
-        - process one or more image files from the folder: path, or from a single .png file or image (ndarray)
-        - output the extracted canny generated drop profile to the subdirectory: dest
-        - extract and generate a .csv file of characteristic features to file: dest/feature_set.csv
-
-"""
-
-import imageio
-import os
-from scipy import ndimage
-from feature_extract import FeatureExtract
-
-import numpy as np
-from numpy import fft
-import matplotlib.pyplot as plt
-import pandas as pd
-
-
-class DropProfile:
-    def __init__(self, path: str = "../Pendant Drops", dest: str = "Drop Profiles", feature_set: str = "features.csv"):
-        """
-        :param path: poth to directory to access input images.
-        :param dest: path to subdir to save output images. It is assumed destination dir is a subdirectory in path: (path/dest)
-        :param feature_set: file name to save feature set as csv to (should include .csv)
-        """
-        self.path = path
-        self.destination = dest
-        self.feature_set = feature_set
-        self.max_height = 0
-        self.max_width = 0
-        self.feature_list = []
-
-    # Perform bulk profile and feature extraction on all files in self.path
-    # generate drop profile .jpg and save to self.destination
-    def extract_from_dir(self):
-        os.chdir("../pdt_extract")
-        os.chdir(self.path)
-        for filename in os.listdir():
-            if not os.path.isdir(filename):
-                print(f"Extracting profile from: {filename}...")
-                profile = extract_profile_from_image(os.path.join(filename))
-                os.chdir(self.destination)
-                self.get_profile(profile, filename)
-                os.chdir("..")
-            else:
-                print(f"not file: {filename}")
-        df = pd.DataFrame(self.feature_list)
-        df.to_csv(self.destination + '/' + self.feature_set, index=False)
-        os.chdir("../pdt_extract")
-
-        print(f"Done Extracting Profiles")
-
-    # perform extraction of profile and feature set given a path to an image with respect to self.path
-    def extract_from_file(self, fname: str) -> (ndimage, list):
-        os.chdir(self.path)
-        profile = extract_profile_from_image(os.path.join(fname))
-        return self.get_profile(profile)
-
-    # perform extraction of profile and feature set given a ndimage
-    def extract_from_img(self, img: ndimage) -> (ndimage, list):
-        profile = extract_profile_from_image(img, load=False, path_to_file=None)
-
-    # label connected components as edge profiles
-    def get_profile(self, final_image, filename=None, save=True):
-        labeled_image, num_features = ndimage.label(final_image)
-        # Remove feature 2 which is the internal noise from light
-        final_image[labeled_image == 2] = 0
-        final_image[labeled_image == 1] = 255
-        final_image = split_profile(final_image)
-
-        # Create ordered set of X and Y coordinates along edge profile
-        indices = np.where(final_image == 255)
-        x = np.flip(indices[1])
-        y = np.flip(indices[0])
-        # Extract and save profile features to feature list
-        features = FeatureExtract(x, y)
-        #features.feature_set["image"] = filename
-        self.feature_list.append(features.feature_set)
-        show_image(final_image)
-
-        fft_profile(final_image)
-        if save:
-            imageio.imwrite(filename, np.uint8(final_image))
-        else:
-            return final_image, features.feature_set
-
-
-#    Execute the Canny Sequence on the image
-#    gaussian_blur_sigma value = 1.2
-#    high_threshold_ratio = 0.2
-#    low_threshold_ratio = 0.15
-def extract_profile_from_image(path_to_file: str, img: ndimage = None, load=True):
-    if load:
-        img = load_convert_image(path_to_file)
-    dx = ndimage.sobel(img, axis=1)  # horizontal derivative
-    dy = ndimage.sobel(img, axis=0)  # vertical derivative
-    mag = normalize(np.hypot(dx, dy))
-    gradient = np.degrees(np.arctan2(dy, dx))
-    nms = normalize(nms_with_interpol(mag, gradient, dx, dy))
-    profile = hysteresis_threshold(nms)
-    return profile
-
-
-# We have a grayscale ndarray.
-# We want to find the vertically-lowest pixel that has the value 255.
-# When we find that column, before cutting the image and keeping the right side,
-# we need to make sure it is either the only vertical minimum,
-# or find the midpoint between the furthest away vertical minimum column and split the image at that midpoint instead
-def split_profile(img: ndimage):
-    # Find the indices of all pixels with value 255 along the vertical axis
-    indices = np.where(img == 255)[0]
-
-    # Find the lowest index, which corresponds to the lowest pixel in the image with value 255
-    lowest_index = np.min(indices)
-
-    # Find the columns that have this lowest pixel value
-    cols = np.where(img[lowest_index, :] == 255)[0]
-
-    # If there is only one such column, use it as the cutting point
-    if len(cols) == 1:
-        cutting_point = cols[0]
-
-    # Otherwise, find the midpoint between the furthest away vertical minimum columns
-    else:
-        left_col = cols[0]
-        right_col = cols[-1]
-        midpoint = (left_col + right_col) // 2
-        cutting_point = midpoint
-
-    # Cut the image and keep the right side
-    return img[:, cutting_point:]
-
-
-def show_image(img):
-    plt.imshow(img, cmap=plt.get_cmap('gray'))
-    plt.show()
-
-
-# Load the next image in subdir
-# img: passed in as full directory
-def load_convert_image(img: str, sigma_val=1.2):
-    lion = imageio.v2.imread(img, None)
-    lion_gray = np.dot(lion[..., :3], [0.299, 0.587, 0.114])
-    # Optionally change or take parameter for sigma
-    img = ndimage.gaussian_filter(lion_gray, sigma=sigma_val)
-    return img
-
-
-# Normalize the pixel array, so that values are <= 1
-def normalize(img):
-    img = img / np.max(img)
-    return img
-
-
-# Do Non-Maximum Suppression with interpolation to get a better
-# Estimate of the magnitude values of the pixels in the gradient
-# Direction. This is done to get thin edges
-def nms_with_interpol(g_mag, grad, gx, gy):
-    nms = np.zeros(g_mag.shape)
-
-    for i in range(1, int(g_mag.shape[0]) - 1):
-        for j in range(1, int(g_mag.shape[1]) - 1):
-            if grad[i, j] >= 0 and grad[i, j] <= 45 or grad[i, j] < -135 and grad[i, j] >= -180:
-                y_bot = np.array([g_mag[i, j + 1], g_mag[i + 1, j + 1]])
-                y_top = np.array([g_mag[i, j - 1], g_mag[i - 1, j - 1]])
-                x_est = np.absolute(gy[i, j] / g_mag[i, j])
-                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
-                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
-                    nms[i, j] = g_mag[i, j]
-                else:
-                    nms[i, j] = 0
-            if grad[i, j] > 45 and grad[i, j] <= 90 or grad[i, j] < -90 and grad[i, j] >= -135:
-                y_bot = np.array([g_mag[i + 1, j], g_mag[i + 1, j + 1]])
-                y_top = np.array([g_mag[i - 1, j], g_mag[i - 1, j - 1]])
-                x_est = np.absolute(gx[i, j] / g_mag[i, j])
-                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
-                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
-                    nms[i, j] = g_mag[i, j]
-                else:
-                    nms[i, j] = 0
-            if grad[i, j] > 90 and grad[i, j] <= 135 or grad[i, j] < -45 and grad[i, j] >= -90:
-                y_bot = np.array([g_mag[i + 1, j], g_mag[i + 1, j - 1]])
-                y_top = np.array([g_mag[i - 1, j], g_mag[i - 1, j + 1]])
-                x_est = np.absolute(gx[i, j] / g_mag[i, j])
-                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
-                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
-                    nms[i, j] = g_mag[i, j]
-                else:
-                    nms[i, j] = 0
-            if grad[i, j] > 135 and grad[i, j] <= 180 or grad[i, j] < 0 and grad[i, j] >= -45:
-                y_bot = np.array([g_mag[i, j - 1], g_mag[i + 1, j - 1]])
-                y_top = np.array([g_mag[i, j + 1], g_mag[i - 1, j + 1]])
-                x_est = np.absolute(gy[i, j] / g_mag[i, j])
-                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
-                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
-                    nms[i, j] = g_mag[i, j]
-                else:
-                    nms[i, j] = 0
-
-    return nms
-
-
-# Double threshold Hysteresis
-def hysteresis_threshold(img, high_threshold_ratio=0.2, low_threshold_ratio=0.15):
-    high_threshold_ratio = 0.2
-    low_threshold_ratio = 0.15
-    g_sup = np.copy(img)
-    h = int(g_sup.shape[0])
-    w = int(g_sup.shape[1])
-    high_threshold = np.max(g_sup) * high_threshold_ratio
-    low_threshold = high_threshold * low_threshold_ratio
-    x = 0.1
-    old_x = 0
-
-    # The while loop is used so that the loop will keep executing till the number of strong edges
-    # do not change, i.e. all weak edges connected to strong edges have been found
-    while old_x != x:
-        old_x = x
-        for i in range(1, h - 1):
-            for j in range(1, w - 1):
-                if g_sup[i, j] > high_threshold:
-                    g_sup[i, j] = 1
-                elif g_sup[i, j] < low_threshold:
-                    g_sup[i, j] = 0
-                else:
-                    if ((g_sup[i - 1, j - 1] > high_threshold) or
-                            (g_sup[i - 1, j] > high_threshold) or
-                            (g_sup[i - 1, j + 1] > high_threshold) or
-                            (g_sup[i, j - 1] > high_threshold) or
-                            (g_sup[i, j + 1] > high_threshold) or
-                            (g_sup[i + 1, j - 1] > high_threshold) or
-                            (g_sup[i + 1, j] > high_threshold) or
-                            (g_sup[i + 1, j + 1] > high_threshold)):
-                        g_sup[i, j] = 1
-        x = np.sum(g_sup == 1)
-
-    # This is done to remove/clean all the weak edges which are not connected to strong edges
-    g_sup = (g_sup == 1) * g_sup
-
-    return g_sup
-
-
-# Remove connected edges that are noise
-# Assuming edge profile is the longest edge
-def extract_profile(img):
-    labeled_image, num_features = ndimage.label(img)
-    # Remove all features that are not labeled 1 or 0, (profile or background)
-    img[labeled_image == 2] = 0
-    img[labeled_image == 1] = 255
-    return img
-
-
-# Fast Fourier Transform of edge profile
-# Can expect high frequency components in magnitude spectrum of edges
-# Computed in Decibels
-def fft_profile(profile):
-    fft_image = fft.fft2(profile)
-    fft_image = fft.fftshift(fft_image)
-    # Shift the zero-frequency component to the center of the spectrum
-    magnitude_spectrum = 20 * np.log(np.abs(fft_image))
-    phase_spectrum = np.angle(fft_image)
-
-
-if __name__ == '__main__':
-    profiles = DropProfile()
-    profiles.extract_from_dir()
+"""
+pdt-extract.py
+
+- Author: Dmitri Lyalikov
+- Email:  Dlyalikov01@manhattan.edu
+- Date of last revision: 05/02/2023
+- Status: in development / validating
+
+This module is the entry point and controller of the profile and feature extraction sequence
+implemented by the pdt-extract project.
+It can be used as a standalone script or imported with DropProfile class to:
+    - process one or more image files from the folder: path, or from a single .png file or image (ndarray)
+    - output the extracted canny generated drop profile to the subdirectory: dest
+    - extract and generate a .csv file of characteristic features to file: Feature Sets/feature_set.csv
+
+"""
+
+import imageio
+import os
+from scipy import ndimage
+from feature_extract import FeatureExtract
+
+import numpy as np
+from numpy import fft
+import matplotlib.pyplot as plt
+import pandas as pd
+
+
+class DropProfile:
+    def __init__(self, path: str = "../Pendant Drops", dest: str = "Drop Profiles", feature_set: str = "features.csv"):
+        """
+        :param path: poth to directory to access input images.
+        :param dest: path to subdir to save output images. It is assumed destination dir is a subdirectory in path: (path/dest)
+        :param feature_set: file name to save feature set as csv to (should include .csv)
+        """
+        self.path = path
+        self.destination = dest
+        self.feature_set = feature_set
+        self.max_height = 0
+        self.max_width = 0
+        self.feature_list = []
+
+    # Perform bulk profile and feature extraction on all files in self.path
+    # generate drop profile .jpg and save to self.destination
+    def extract_from_dir(self, canny_done=False, extract=True):
+        os.chdir("../pdt_extract")
+        os.chdir(self.path)
+        coord_list = {}
+        if canny_done:
+            for filename in os.listdir():
+                if not os.path.isdir(filename):
+                    print(f"Extracting profile from: {filename}...")
+                    profile = load_edge(filename)
+                    os.chdir(self.destination)
+                    image, features, x, y = self.get_profile(profile, filename, extract=extract)
+                    coord_list[f"{filename}"] = [x, y]
+                    os.chdir("..")
+                else:
+                    print(f"not file: {filename}")
+            if not os.path.exists("Feature Sets"):
+                os.mkdir("Feature Sets")
+            df = pd.DataFrame(self.feature_list)
+            df.to_csv("Feature Sets" + '/' + self.feature_set, index=False)
+            os.chdir("../pdt_extract")
+        else:
+            for filename in os.listdir():
+                if not os.path.isdir(filename):
+                    print(f"Extracting profile from: {filename}...")
+                    profile = extract_profile_from_image(os.path.join(filename))
+                    os.chdir(self.destination)
+                    image, features, x, y = self.get_profile(profile, filename, extract=extract)
+                    coord_list[f"{filename}"] = [x, y]
+                    os.chdir("..")
+                else:
+                    print(f"not file: {filename}")
+            if not os.path.exists("Feature Sets"):
+                os.mkdir("Feature Sets")
+            df = pd.DataFrame(self.feature_list)
+            df.to_csv("Feature Sets" + '/' + self.feature_set, index=False)
+            os.chdir("../pdt_extract")
+
+        print(f"Done Extracting Profiles")
+        return coord_list
+
+    # perform extraction of profile and feature set given a path to an image with respect to self.path
+    def extract_from_file(self, fname: str, canny_done: bool, extract=True) -> (ndimage, list):
+        if canny_done:
+            profile = load_edge(fname)
+            self.get_profile(profile, fname)
+        else:
+            os.chdir(self.path)
+            profile = extract_profile_from_image(os.path.join(fname))
+            return self.get_profile(profile, extract=extract)
+
+    # perform extraction of profile and feature set given a ndimage
+    def extract_from_img(self, img: ndimage, extract=True) -> (ndimage, list):
+        profile = extract_profile_from_image(img, load=False, path_to_file=None)
+
+    # label connected components as edge profiles
+    def get_profile(self, final_image, filename=None, save=True, extract=True):
+        labeled_image, num_features = ndimage.label(final_image)
+        # show_image(labeled_image)
+        # Remove feature 2 which is the internal noise from light
+
+        final_image[labeled_image == 1] = 255
+
+        final_image = split_profile(final_image)
+
+        # Create ordered set of X and Y coordinates along edge profile
+        indices = np.where(final_image > 0)
+        x = np.flip(indices[1])
+        y = np.flip(indices[0])
+        reconstruct(x, y)
+        if save:
+            imageio.imwrite(filename, np.uint8(final_image))
+        # Extract and save profile features to feature list
+        if extract:
+            features = FeatureExtract(x, y)
+            features.feature_set["image"] = filename
+            self.feature_list.append(features.feature_set)
+            show_image(final_image)
+            print(f"{filename}: {features.show_features()}")
+            return final_image, features.feature_set, x, y
+        fft_profile(final_image)
+
+        return final_image, None, x, y
+
+
+def reconstruct(x_coords, y_coords):
+    image_array = np.zeros((500, 500), dtype=np.uint8)
+    for x, y in zip(x_coords, y_coords):
+        image_array[y, x] = 255
+    show_image(image_array)
+
+#    Execute the Canny Sequence on the image
+#    gaussian_blur_sigma value = 1.2
+#    high_threshold_ratio = 0.2
+#    low_threshold_ratio = 0.15
+def extract_profile_from_image(path_to_file: str, img: ndimage = None, load=True, extract=True):
+    if load:
+        img = load_convert_image(path_to_file)
+    dx = ndimage.sobel(img, axis=1)  # horizontal derivative
+    dy = ndimage.sobel(img, axis=0)  # vertical derivative
+    mag = normalize(np.hypot(dx, dy))
+    gradient = np.degrees(np.arctan2(dy, dx))
+    nms = normalize(nms_with_interpol(mag, gradient, dx, dy))
+    profile = hysteresis_threshold(nms)
+    show_image(profile)
+    return profile
+
+
+# We have a grayscale ndarray.
+# We want to find the vertically-lowest pixel that has the value 255.
+# When we find that column, before cutting the image and keeping the right side,
+# we need to make sure it is either the only vertical minimum,
+# or find the midpoint between the furthest away vertical minimum column and split the image at that midpoint instead
+def split_profile(img: ndimage):
+    show_image(img)
+
+    nonzero_coords = np.argwhere(img != 0)
+    lowest_position = np.min(nonzero_coords, axis=0)
+    # Find the indices of all pixels with value 255 along the vertical axis
+    indices = np.where(img > 0)[1]
+
+    # Find the lowest index, which corresponds to the lowest pixel in the image with value 255
+    lowest_index = np.min(indices)
+
+    # Find the columns that have this lowest pixel value
+    cols = np.where(img[lowest_index, :] > 0)[0]
+
+    # If there is only one such column, use it as the cutting point
+    if len(cols) == 1:
+        cutting_point = cols[0]
+
+    # Otherwise, find the midpoint between the furthest away vertical minimum columns
+    else:
+        left_col = cols[0]
+        right_col = cols[-1]
+        midpoint = (left_col + right_col) // 2
+        cutting_point = midpoint
+
+    # Cut the image and keep the right side
+    return img[:, cutting_point:]
+
+
+def show_image(img):
+    plt.imshow(img, cmap=plt.get_cmap('gray'))
+    plt.show()
+
+
+# load a preprocessed edge profile
+# img: passed in as full directory
+def load_edge(img: str) -> ndimage:
+    lion = imageio.v2.imread(img, None)
+    show_image(lion)
+    # Convert to grayscale
+    img = np.dot(lion[..., :3], [0.299, 0.587, 0.114])
+    show_image(img)
+    return img
+
+
+# Load the next image in subdir
+# img: passed in as full directory
+def load_convert_image(img: str, sigma_val=1):
+    lion = imageio.v2.imread(img, None)
+    lion_gray = np.dot(lion[..., :3], [0.299, 0.587, 0.114])
+    # Find the middle row index
+    # Optionally change or take parameter for sigma
+    img = ndimage.gaussian_filter(lion_gray, sigma=sigma_val)
+    return img
+
+
+# Normalize the pixel array, so that values are <= 1
+def normalize(img):
+    img = img / np.max(img)
+    return img
+
+
+# Do Non-Maximum Suppression with interpolation to get a better
+# Estimate of the magnitude values of the pixels in the gradient
+# Direction. This is done to get thin edges
+def nms_with_interpol(g_mag, grad, gx, gy):
+    nms = np.zeros(g_mag.shape)
+
+    for i in range(1, int(g_mag.shape[0]) - 1):
+        for j in range(1, int(g_mag.shape[1]) - 1):
+            if grad[i, j] >= 0 and grad[i, j] <= 45 or grad[i, j] < -135 and grad[i, j] >= -180:
+                y_bot = np.array([g_mag[i, j + 1], g_mag[i + 1, j + 1]])
+                y_top = np.array([g_mag[i, j - 1], g_mag[i - 1, j - 1]])
+                x_est = np.absolute(gy[i, j] / g_mag[i, j])
+                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
+                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
+                    nms[i, j] = g_mag[i, j]
+                else:
+                    nms[i, j] = 0
+            if grad[i, j] > 45 and grad[i, j] <= 90 or grad[i, j] < -90 and grad[i, j] >= -135:
+                y_bot = np.array([g_mag[i + 1, j], g_mag[i + 1, j + 1]])
+                y_top = np.array([g_mag[i - 1, j], g_mag[i - 1, j - 1]])
+                x_est = np.absolute(gx[i, j] / g_mag[i, j])
+                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
+                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
+                    nms[i, j] = g_mag[i, j]
+                else:
+                    nms[i, j] = 0
+            if grad[i, j] > 90 and grad[i, j] <= 135 or grad[i, j] < -45 and grad[i, j] >= -90:
+                y_bot = np.array([g_mag[i + 1, j], g_mag[i + 1, j - 1]])
+                y_top = np.array([g_mag[i - 1, j], g_mag[i - 1, j + 1]])
+                x_est = np.absolute(gx[i, j] / g_mag[i, j])
+                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
+                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
+                    nms[i, j] = g_mag[i, j]
+                else:
+                    nms[i, j] = 0
+            if grad[i, j] > 135 and grad[i, j] <= 180 or grad[i, j] < 0 and grad[i, j] >= -45:
+                y_bot = np.array([g_mag[i, j - 1], g_mag[i + 1, j - 1]])
+                y_top = np.array([g_mag[i, j + 1], g_mag[i - 1, j + 1]])
+                x_est = np.absolute(gy[i, j] / g_mag[i, j])
+                if (g_mag[i, j] >= ((y_bot[1] - y_bot[0]) * x_est + y_bot[0]) and g_mag[i, j] >= (
+                        (y_top[1] - y_top[0]) * x_est + y_top[0])):
+                    nms[i, j] = g_mag[i, j]
+                else:
+                    nms[i, j] = 0
+
+    return nms
+
+
+# Double threshold Hysteresis
+def hysteresis_threshold(img, high_threshold_ratio=0.2, low_threshold_ratio=0.15):
+    high_threshold_ratio = 0.4
+    low_threshold_ratio = 0.15
+    g_sup = np.copy(img)
+    h = int(g_sup.shape[0])
+    w = int(g_sup.shape[1])
+    high_threshold = np.max(g_sup) * high_threshold_ratio
+    low_threshold = high_threshold * low_threshold_ratio
+    x = 0.1
+    old_x = 0
+
+    # The while loop is used so that the loop will keep executing till the number of strong edges
+    # do not change, i.e. all weak edges connected to strong edges have been found
+    while old_x != x:
+        old_x = x
+        for i in range(1, h - 1):
+            for j in range(1, w - 1):
+                if g_sup[i, j] > high_threshold:
+                    g_sup[i, j] = 1
+                elif g_sup[i, j] < low_threshold:
+                    g_sup[i, j] = 0
+                else:
+                    if ((g_sup[i - 1, j - 1] > high_threshold) or
+                            (g_sup[i - 1, j] > high_threshold) or
+                            (g_sup[i - 1, j + 1] > high_threshold) or
+                            (g_sup[i, j - 1] > high_threshold) or
+                            (g_sup[i, j + 1] > high_threshold) or
+                            (g_sup[i + 1, j - 1] > high_threshold) or
+                            (g_sup[i + 1, j] > high_threshold) or
+                            (g_sup[i + 1, j + 1] > high_threshold)):
+                        g_sup[i, j] = 1
+        x = np.sum(g_sup == 1)
+
+    # This is done to remove/clean all the weak edges which are not connected to strong edges
+    g_sup = (g_sup == 1) * g_sup
+
+    return g_sup
+
+
+# Remove connected edges that are noise
+# Assuming edge profile is the longest edge
+def extract_profile(img):
+    labeled_image, num_features = ndimage.label(img)
+    # Remove all features that are not labeled 1 or 0, (profile or background)
+    img[labeled_image == 2] = 0
+    img[labeled_image == 1] = 255
+    return img
+
+
+
+# Fast Fourier Transform of edge profile
+# Can expect high frequency components in magnitude spectrum of edges
+# Computed in Decibels
+def fft_profile(profile):
+    fft_image = fft.fft2(profile)
+    fft_image = fft.fftshift(fft_image)
+    # Shift the zero-frequency component to the center of the spectrum
+    magnitude_spectrum = 20 * np.log(np.abs(fft_image))
+    phase_spectrum = np.angle(fft_image)
+
+
+if __name__ == '__main__':
+    profiles = DropProfile()
+    profiles.extract_from_dir(canny_done=False, extract=False)
+    # profiles.extract_from_file(fname="../matlab_canny/d-1-55.png", canny_done=True)
```

## Comparing `pdt_extract-0.1.5.dist-info/METADATA` & `pdt_extract-0.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdt-extract
-Version: 0.1.5
+Version: 0.1.6
 Summary: Perform edge profile and characteristic feature extraction from images of pendant drops
 Home-page: https://github.com/DmitriLyalikov/pdt-canny-edge-detector
 Author: Dmitri Lyalikov
 Author-email: Dlyalikov01@manhattan.edu
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 Requires-Dist: imageio
```

