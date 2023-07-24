# Comparing `tmp/PyQt6-6.5.1.tar.gz` & `tmp/PyQt6-6.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6-6.5.1.tar", last modified: Fri Jun  2 10:41:06 2023, max compression
+gzip compressed data, was "PyQt6-6.5.2.tar", last modified: Sat Jul 22 15:08:32 2023, max compression
```

## Comparing `PyQt6-6.5.1.tar` & `PyQt6-6.5.2.tar`

### file list

```diff
@@ -1,1157 +1,1157 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.071292 PyQt6-6.5.1/
--rw-r--r--   0 phil       (501) staff       (20)   119816 2023-06-02 10:40:57.300344 PyQt6-6.5.1/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2023-06-02 10:40:56.748132 PyQt6-6.5.1/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)     3662 2023-06-02 10:40:57.301942 PyQt6-6.5.1/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     2075 2023-06-02 10:41:06.071410 PyQt6-6.5.1/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1735 2023-06-02 10:40:57.549569 PyQt6-6.5.1/README
--rw-r--r--   0 phil       (501) staff       (20)      960 2023-06-02 10:40:57.312961 PyQt6-6.5.1/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.717705 PyQt6-6.5.1/config-tests/
--rw-r--r--   0 phil       (501) staff       (20)      823 2023-06-02 10:40:57.311180 PyQt6-6.5.1/config-tests/cfgtest_QtCore.cpp
--rw-r--r--   0 phil       (501) staff       (20)      813 2023-06-02 10:40:57.309548 PyQt6-6.5.1/config-tests/cfgtest_QtGui.cpp
--rw-r--r--   0 phil       (501) staff       (20)      569 2023-06-02 10:40:57.311844 PyQt6-6.5.1/config-tests/cfgtest_QtNetwork.cpp
--rw-r--r--   0 phil       (501) staff       (20)      752 2023-06-02 10:40:57.310446 PyQt6-6.5.1/config-tests/cfgtest_QtPrintSupport.cpp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.716203 PyQt6-6.5.1/dbus/
--rw-r--r--   0 phil       (501) staff       (20)    11344 2023-06-02 10:40:57.542735 PyQt6-6.5.1/dbus/dbus.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2067 2023-06-02 10:40:57.540804 PyQt6-6.5.1/dbus/helper.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.826588 PyQt6-6.5.1/designer/
--rw-r--r--   0 phil       (501) staff       (20)      435 2023-06-02 10:40:57.543625 PyQt6-6.5.1/designer/designer.pro-in
--rw-r--r--   0 phil       (501) staff       (20)     9229 2023-06-02 10:40:57.545514 PyQt6-6.5.1/designer/pluginloader.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1982 2023-06-02 10:40:57.545902 PyQt6-6.5.1/designer/pluginloader.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.824945 PyQt6-6.5.1/examples/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.817548 PyQt6-6.5.1/examples/designer/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.818345 PyQt6-6.5.1/examples/designer/calculatorform/
--rw-r--r--   0 phil       (501) staff       (20)     2805 2023-06-02 10:06:50.150263 PyQt6-6.5.1/examples/designer/calculatorform/calculatorform.py
--rw-r--r--   0 phil       (501) staff       (20)     7150 2023-06-02 10:06:50.149750 PyQt6-6.5.1/examples/designer/calculatorform/calculatorform.ui
--rw-r--r--   0 phil       (501) staff       (20)     5538 2023-06-02 10:06:50.150827 PyQt6-6.5.1/examples/designer/calculatorform/ui_calculatorform.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.814076 PyQt6-6.5.1/examples/designer/plugins/
--rw-r--r--   0 phil       (501) staff       (20)     3578 2023-06-02 10:06:50.146079 PyQt6-6.5.1/examples/designer/plugins/plugins.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.813770 PyQt6-6.5.1/examples/designer/plugins/python/
--rw-r--r--   0 phil       (501) staff       (20)     5548 2023-06-02 10:06:50.146275 PyQt6-6.5.1/examples/designer/plugins/python/analogclockplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     5106 2023-06-02 10:06:50.148731 PyQt6-6.5.1/examples/designer/plugins/python/bubbleswidgetplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     3447 2023-06-02 10:06:50.288421 PyQt6-6.5.1/examples/designer/plugins/python/counterlabelplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     4401 2023-06-02 10:06:50.148819 PyQt6-6.5.1/examples/designer/plugins/python/datetimeeditplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     3566 2023-06-02 10:06:50.147584 PyQt6-6.5.1/examples/designer/plugins/python/helloglwidgetplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     5126 2023-06-02 10:06:50.150168 PyQt6-6.5.1/examples/designer/plugins/python/multipagewidgetplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     4714 2023-06-02 10:06:50.148947 PyQt6-6.5.1/examples/designer/plugins/python/polygonwidgetplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     4184 2023-06-02 10:06:50.151045 PyQt6-6.5.1/examples/designer/plugins/python/pydemoplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     4612 2023-06-02 10:06:50.152554 PyQt6-6.5.1/examples/designer/plugins/python/pythonconsoleplugin.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.817162 PyQt6-6.5.1/examples/designer/plugins/widgets/
--rw-r--r--   0 phil       (501) staff       (20)     6253 2023-06-02 10:06:50.151661 PyQt6-6.5.1/examples/designer/plugins/widgets/analogclock.py
--rw-r--r--   0 phil       (501) staff       (20)    10365 2023-06-02 10:06:50.152082 PyQt6-6.5.1/examples/designer/plugins/widgets/bubbleswidget.py
--rw-r--r--   0 phil       (501) staff       (20)     5187 2023-06-02 10:06:50.147190 PyQt6-6.5.1/examples/designer/plugins/widgets/counterlabel.py
--rw-r--r--   0 phil       (501) staff       (20)    16152 2023-06-02 10:06:50.147695 PyQt6-6.5.1/examples/designer/plugins/widgets/datetimeedit.py
--rw-r--r--   0 phil       (501) staff       (20)     8302 2023-06-02 10:06:50.150024 PyQt6-6.5.1/examples/designer/plugins/widgets/helloglwidget.py
--rw-r--r--   0 phil       (501) staff       (20)     3985 2023-06-02 10:06:50.289081 PyQt6-6.5.1/examples/designer/plugins/widgets/multipagewidget.py
--rw-r--r--   0 phil       (501) staff       (20)     5827 2023-06-02 10:06:50.150179 PyQt6-6.5.1/examples/designer/plugins/widgets/polygonwidget.py
--rw-r--r--   0 phil       (501) staff       (20)     5619 2023-06-02 10:06:50.148603 PyQt6-6.5.1/examples/designer/plugins/widgets/pydemo.py
--rw-r--r--   0 phil       (501) staff       (20)     3016 2023-06-02 10:06:50.151539 PyQt6-6.5.1/examples/designer/plugins/widgets/pythonconsolewidget.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.806585 PyQt6-6.5.1/examples/desktop/
--rw-r--r--   0 phil       (501) staff       (20)     6605 2023-06-02 10:06:50.150108 PyQt6-6.5.1/examples/desktop/screenshot.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.806979 PyQt6-6.5.1/examples/desktop/systray/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.808028 PyQt6-6.5.1/examples/desktop/systray/images/
--rw-r--r--   0 phil       (501) staff       (20)     2496 2023-06-02 10:06:50.152875 PyQt6-6.5.1/examples/desktop/systray/images/bad.png
--rw-r--r--   0 phil       (501) staff       (20)    25780 2023-06-02 10:06:50.154520 PyQt6-6.5.1/examples/desktop/systray/images/heart.png
--rw-r--r--   0 phil       (501) staff       (20)    12128 2023-06-02 10:06:50.153636 PyQt6-6.5.1/examples/desktop/systray/images/trash.png
--rw-r--r--   0 phil       (501) staff       (20)     9595 2023-06-02 10:06:50.153712 PyQt6-6.5.1/examples/desktop/systray/systray.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.823334 PyQt6-6.5.1/examples/dialogs/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.820921 PyQt6-6.5.1/examples/dialogs/classwizard/
--rw-r--r--   0 phil       (501) staff       (20)    15515 2023-06-02 10:06:50.148495 PyQt6-6.5.1/examples/dialogs/classwizard/classwizard.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.823030 PyQt6-6.5.1/examples/dialogs/classwizard/images/
--rw-r--r--   0 phil       (501) staff       (20)    22578 2023-06-02 10:06:50.149188 PyQt6-6.5.1/examples/dialogs/classwizard/images/background.png
--rw-r--r--   0 phil       (501) staff       (20)     3947 2023-06-02 10:06:50.151628 PyQt6-6.5.1/examples/dialogs/classwizard/images/banner.png
--rw-r--r--   0 phil       (501) staff       (20)     1619 2023-06-02 10:06:50.289616 PyQt6-6.5.1/examples/dialogs/classwizard/images/logo1.png
--rw-r--r--   0 phil       (501) staff       (20)     1619 2023-06-02 10:06:50.152259 PyQt6-6.5.1/examples/dialogs/classwizard/images/logo2.png
--rw-r--r--   0 phil       (501) staff       (20)     1619 2023-06-02 10:06:50.150881 PyQt6-6.5.1/examples/dialogs/classwizard/images/logo3.png
--rw-r--r--   0 phil       (501) staff       (20)    14516 2023-06-02 10:06:50.153601 PyQt6-6.5.1/examples/dialogs/classwizard/images/watermark1.png
--rw-r--r--   0 phil       (501) staff       (20)    14912 2023-06-02 10:06:50.153160 PyQt6-6.5.1/examples/dialogs/classwizard/images/watermark2.png
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.823782 PyQt6-6.5.1/examples/dialogs/configdialog/
--rw-r--r--   0 phil       (501) staff       (20)     8989 2023-06-02 10:06:50.154320 PyQt6-6.5.1/examples/dialogs/configdialog/configdialog.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.824584 PyQt6-6.5.1/examples/dialogs/configdialog/images/
--rw-r--r--   0 phil       (501) staff       (20)     7059 2023-06-02 10:06:50.156113 PyQt6-6.5.1/examples/dialogs/configdialog/images/config.png
--rw-r--r--   0 phil       (501) staff       (20)     2269 2023-06-02 10:06:50.155037 PyQt6-6.5.1/examples/dialogs/configdialog/images/query.png
--rw-r--r--   0 phil       (501) staff       (20)     8296 2023-06-02 10:06:50.156080 PyQt6-6.5.1/examples/dialogs/configdialog/images/update.png
--rw-r--r--   0 phil       (501) staff       (20)     4434 2023-06-02 10:06:50.149599 PyQt6-6.5.1/examples/dialogs/extension.py
--rw-r--r--   0 phil       (501) staff       (20)     8264 2023-06-02 10:06:50.150439 PyQt6-6.5.1/examples/dialogs/findfiles.py
--rw-r--r--   0 phil       (501) staff       (20)    13995 2023-06-02 10:06:50.153598 PyQt6-6.5.1/examples/dialogs/standarddialogs.py
--rw-r--r--   0 phil       (501) staff       (20)     7401 2023-06-02 10:06:50.290139 PyQt6-6.5.1/examples/dialogs/tabdialog.py
--rw-r--r--   0 phil       (501) staff       (20)     3603 2023-06-02 10:06:50.153416 PyQt6-6.5.1/examples/dialogs/trivialwizard.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.766419 PyQt6-6.5.1/examples/draganddrop/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.765637 PyQt6-6.5.1/examples/draganddrop/delayedencoding/
--rw-r--r--   0 phil       (501) staff       (20)     4979 2023-06-02 10:06:50.152902 PyQt6-6.5.1/examples/draganddrop/delayedencoding/delayedencoding.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.766036 PyQt6-6.5.1/examples/draganddrop/delayedencoding/images/
--rw-r--r--   0 phil       (501) staff       (20)      977 2023-06-02 10:06:50.154951 PyQt6-6.5.1/examples/draganddrop/delayedencoding/images/drag.png
--rw-r--r--   0 phil       (501) staff       (20)     2689 2023-06-02 10:06:50.155193 PyQt6-6.5.1/examples/draganddrop/delayedencoding/images/example.svg
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.763056 PyQt6-6.5.1/examples/draganddrop/draggableicons/
--rw-r--r--   0 phil       (501) staff       (20)     5975 2023-06-02 10:06:50.156519 PyQt6-6.5.1/examples/draganddrop/draggableicons/draggableicons.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.763985 PyQt6-6.5.1/examples/draganddrop/draggableicons/images/
--rw-r--r--   0 phil       (501) staff       (20)     2772 2023-06-02 10:06:50.157469 PyQt6-6.5.1/examples/draganddrop/draggableicons/images/boat.png
--rw-r--r--   0 phil       (501) staff       (20)     2963 2023-06-02 10:06:50.156462 PyQt6-6.5.1/examples/draganddrop/draggableicons/images/car.png
--rw-r--r--   0 phil       (501) staff       (20)     3292 2023-06-02 10:06:50.158238 PyQt6-6.5.1/examples/draganddrop/draggableicons/images/house.png
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.764855 PyQt6-6.5.1/examples/draganddrop/draggabletext/
--rw-r--r--   0 phil       (501) staff       (20)     5414 2023-06-02 10:06:50.152279 PyQt6-6.5.1/examples/draganddrop/draggabletext/draggabletext.py
--rw-r--r--   0 phil       (501) staff       (20)      247 2023-06-02 10:06:50.151674 PyQt6-6.5.1/examples/draganddrop/draggabletext/words.txt
--rw-r--r--   0 phil       (501) staff       (20)     6826 2023-06-02 10:06:50.155271 PyQt6-6.5.1/examples/draganddrop/dropsite.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.766839 PyQt6-6.5.1/examples/draganddrop/fridgemagnets/
--rw-r--r--   0 phil       (501) staff       (20)     6903 2023-06-02 10:06:50.290815 PyQt6-6.5.1/examples/draganddrop/fridgemagnets/fridgemagnets.py
--rw-r--r--   0 phil       (501) staff       (20)      278 2023-06-02 10:06:50.154618 PyQt6-6.5.1/examples/draganddrop/fridgemagnets/words.txt
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.762155 PyQt6-6.5.1/examples/draganddrop/puzzle/
--rw-r--r--   0 phil       (501) staff       (20)    42654 2023-06-02 10:06:50.154818 PyQt6-6.5.1/examples/draganddrop/puzzle/example.jpg
--rw-r--r--   0 phil       (501) staff       (20)    12900 2023-06-02 10:06:50.156635 PyQt6-6.5.1/examples/draganddrop/puzzle/puzzle.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.808795 PyQt6-6.5.1/examples/multimedia/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.809645 PyQt6-6.5.1/examples/multimedia/audiodevices/
--rw-r--r--   0 phil       (501) staff       (20)     7889 2023-06-02 10:06:50.157298 PyQt6-6.5.1/examples/multimedia/audiodevices/audiodevices.py
--rw-r--r--   0 phil       (501) staff       (20)    11927 2023-06-02 10:06:50.158563 PyQt6-6.5.1/examples/multimedia/audiodevices/audiodevicesbase.ui
--rw-r--r--   0 phil       (501) staff       (20)    12232 2023-06-02 10:06:50.159025 PyQt6-6.5.1/examples/multimedia/audiodevices/ui_audiodevicesbase.py
--rw-r--r--   0 phil       (501) staff       (20)     9047 2023-06-02 10:06:50.158157 PyQt6-6.5.1/examples/multimedia/audiooutput.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.771848 PyQt6-6.5.1/examples/multimediawidgets/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.774376 PyQt6-6.5.1/examples/multimediawidgets/camera/
--rw-r--r--   0 phil       (501) staff       (20)    21481 2023-06-02 10:06:50.160164 PyQt6-6.5.1/examples/multimediawidgets/camera/camera.py
--rw-r--r--   0 phil       (501) staff       (20)    13064 2023-06-02 10:06:50.153996 PyQt6-6.5.1/examples/multimediawidgets/camera/camera.ui
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.774481 PyQt6-6.5.1/examples/multimediawidgets/camera/images/
--rw-r--r--   0 phil       (501) staff       (20)     1491 2023-06-02 10:06:50.154087 PyQt6-6.5.1/examples/multimediawidgets/camera/images/shutter.svg
--rw-r--r--   0 phil       (501) staff       (20)     3290 2023-06-02 10:06:50.156641 PyQt6-6.5.1/examples/multimediawidgets/camera/imagesettings.ui
--rw-r--r--   0 phil       (501) staff       (20)    10689 2023-06-02 10:06:50.291441 PyQt6-6.5.1/examples/multimediawidgets/camera/ui_camera.py
--rw-r--r--   0 phil       (501) staff       (20)     3453 2023-06-02 10:06:50.155746 PyQt6-6.5.1/examples/multimediawidgets/camera/ui_imagesettings.py
--rw-r--r--   0 phil       (501) staff       (20)     6492 2023-06-02 10:06:50.156306 PyQt6-6.5.1/examples/multimediawidgets/camera/ui_videosettings.py
--rw-r--r--   0 phil       (501) staff       (20)     5727 2023-06-02 10:06:50.158283 PyQt6-6.5.1/examples/multimediawidgets/camera/videosettings.ui
--rw-r--r--   0 phil       (501) staff       (20)     6277 2023-06-02 10:06:50.158660 PyQt6-6.5.1/examples/multimediawidgets/videographicsitem.py
--rw-r--r--   0 phil       (501) staff       (20)     5857 2023-06-02 10:06:50.159869 PyQt6-6.5.1/examples/multimediawidgets/videowidget.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.767294 PyQt6-6.5.1/examples/qml/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.770655 PyQt6-6.5.1/examples/qml/referenceexamples/
--rwxr-xr-x   0 phil       (501) staff       (20)     3228 2023-06-02 10:06:50.160277 PyQt6-6.5.1/examples/qml/referenceexamples/adding.py
--rwxr-xr-x   0 phil       (501) staff       (20)     6032 2023-06-02 10:06:50.159488 PyQt6-6.5.1/examples/qml/referenceexamples/attached.py
--rwxr-xr-x   0 phil       (501) staff       (20)     8823 2023-06-02 10:06:50.161516 PyQt6-6.5.1/examples/qml/referenceexamples/binding.py
--rwxr-xr-x   0 phil       (501) staff       (20)     4133 2023-06-02 10:06:50.156214 PyQt6-6.5.1/examples/qml/referenceexamples/coercion.py
--rwxr-xr-x   0 phil       (501) staff       (20)     4168 2023-06-02 10:06:50.155467 PyQt6-6.5.1/examples/qml/referenceexamples/default.py
--rwxr-xr-x   0 phil       (501) staff       (20)     5630 2023-06-02 10:06:50.157729 PyQt6-6.5.1/examples/qml/referenceexamples/grouped.py
--rwxr-xr-x   0 phil       (501) staff       (20)     4157 2023-06-02 10:06:50.292131 PyQt6-6.5.1/examples/qml/referenceexamples/methods.py
--rwxr-xr-x   0 phil       (501) staff       (20)     3945 2023-06-02 10:06:50.156887 PyQt6-6.5.1/examples/qml/referenceexamples/properties.py
--rwxr-xr-x   0 phil       (501) staff       (20)     6504 2023-06-02 10:06:50.158420 PyQt6-6.5.1/examples/qml/referenceexamples/signal.py
--rwxr-xr-x   0 phil       (501) staff       (20)     8821 2023-06-02 10:06:50.159733 PyQt6-6.5.1/examples/qml/referenceexamples/valuesource.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.805114 PyQt6-6.5.1/examples/quick/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.781302 PyQt6-6.5.1/examples/quick/animation/
--rw-r--r--   0 phil       (501) staff       (20)     2415 2023-06-02 10:06:50.160122 PyQt6-6.5.1/examples/quick/animation/animation.py
--rw-r--r--   0 phil       (501) staff       (20)     3371 2023-06-02 10:06:50.160942 PyQt6-6.5.1/examples/quick/animation/animation.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.776513 PyQt6-6.5.1/examples/quick/animation/basics/
--rw-r--r--   0 phil       (501) staff       (20)     4957 2023-06-02 10:06:50.161857 PyQt6-6.5.1/examples/quick/animation/basics/color-animation.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.778100 PyQt6-6.5.1/examples/quick/animation/basics/images/
--rw-r--r--   0 phil       (501) staff       (20)    15408 2023-06-02 10:06:50.161140 PyQt6-6.5.1/examples/quick/animation/basics/images/face-smile.png
--rw-r--r--   0 phil       (501) staff       (20)     2433 2023-06-02 10:06:50.163145 PyQt6-6.5.1/examples/quick/animation/basics/images/moon.png
--rw-r--r--   0 phil       (501) staff       (20)      425 2023-06-02 10:06:50.158137 PyQt6-6.5.1/examples/quick/animation/basics/images/shadow.png
--rw-r--r--   0 phil       (501) staff       (20)      349 2023-06-02 10:06:50.157264 PyQt6-6.5.1/examples/quick/animation/basics/images/star.png
--rw-r--r--   0 phil       (501) staff       (20)     8153 2023-06-02 10:06:50.159210 PyQt6-6.5.1/examples/quick/animation/basics/images/sun.png
--rw-r--r--   0 phil       (501) staff       (20)     4187 2023-06-02 10:06:50.292831 PyQt6-6.5.1/examples/quick/animation/basics/property-animation.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.781001 PyQt6-6.5.1/examples/quick/animation/behaviors/
--rw-r--r--   0 phil       (501) staff       (20)     2401 2023-06-02 10:06:50.158085 PyQt6-6.5.1/examples/quick/animation/behaviors/SideRect.qml
--rw-r--r--   0 phil       (501) staff       (20)     4444 2023-06-02 10:06:50.160543 PyQt6-6.5.1/examples/quick/animation/behaviors/behavior-example.qml
--rw-r--r--   0 phil       (501) staff       (20)     4376 2023-06-02 10:06:50.161141 PyQt6-6.5.1/examples/quick/animation/behaviors/tvtennis.qml
--rw-r--r--   0 phil       (501) staff       (20)     4090 2023-06-02 10:06:50.161431 PyQt6-6.5.1/examples/quick/animation/behaviors/wigglytext.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.778565 PyQt6-6.5.1/examples/quick/animation/easing/
--rw-r--r--   0 phil       (501) staff       (20)     8398 2023-06-02 10:06:50.162689 PyQt6-6.5.1/examples/quick/animation/easing/easing.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.779500 PyQt6-6.5.1/examples/quick/animation/pathanimation/
--rw-r--r--   0 phil       (501) staff       (20)     3407 2023-06-02 10:06:50.163316 PyQt6-6.5.1/examples/quick/animation/pathanimation/pathanimation.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.778958 PyQt6-6.5.1/examples/quick/animation/pathinterpolator/
--rw-r--r--   0 phil       (501) staff       (20)     3596 2023-06-02 10:06:50.162626 PyQt6-6.5.1/examples/quick/animation/pathinterpolator/pathinterpolator.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.782128 PyQt6-6.5.1/examples/quick/animation/states/
--rw-r--r--   0 phil       (501) staff       (20)     5149 2023-06-02 10:06:50.164680 PyQt6-6.5.1/examples/quick/animation/states/qt-logo.png
--rw-r--r--   0 phil       (501) staff       (20)     3876 2023-06-02 10:06:50.159730 PyQt6-6.5.1/examples/quick/animation/states/states.qml
--rw-r--r--   0 phil       (501) staff       (20)     4932 2023-06-02 10:06:50.158882 PyQt6-6.5.1/examples/quick/animation/states/transitions.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.798092 PyQt6-6.5.1/examples/quick/canvas/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.797732 PyQt6-6.5.1/examples/quick/canvas/bezierCurve/
--rw-r--r--   0 phil       (501) staff       (20)     4728 2023-06-02 10:06:50.160828 PyQt6-6.5.1/examples/quick/canvas/bezierCurve/bezierCurve.qml
--rw-r--r--   0 phil       (501) staff       (20)     2412 2023-06-02 10:06:50.293396 PyQt6-6.5.1/examples/quick/canvas/canvas.py
--rw-r--r--   0 phil       (501) staff       (20)     3069 2023-06-02 10:06:50.159424 PyQt6-6.5.1/examples/quick/canvas/canvas.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.795183 PyQt6-6.5.1/examples/quick/canvas/clip/
--rw-r--r--   0 phil       (501) staff       (20)     5037 2023-06-02 10:06:50.161963 PyQt6-6.5.1/examples/quick/canvas/clip/clip.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.790282 PyQt6-6.5.1/examples/quick/canvas/contents/
--rw-r--r--   0 phil       (501) staff       (20)     3026 2023-06-02 10:06:50.162562 PyQt6-6.5.1/examples/quick/canvas/contents/Button.qml
--rw-r--r--   0 phil       (501) staff       (20)     3391 2023-06-02 10:06:50.163028 PyQt6-6.5.1/examples/quick/canvas/contents/ScrollBar.qml
--rw-r--r--   0 phil       (501) staff       (20)     3915 2023-06-02 10:06:50.164066 PyQt6-6.5.1/examples/quick/canvas/contents/Slider.qml
--rw-r--r--   0 phil       (501) staff       (20)     2826 2023-06-02 10:06:50.164400 PyQt6-6.5.1/examples/quick/canvas/contents/TitleBar.qml
--rw-r--r--   0 phil       (501) staff       (20)     2564 2023-06-02 10:06:50.163890 PyQt6-6.5.1/examples/quick/canvas/contents/ToolBar.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.794758 PyQt6-6.5.1/examples/quick/canvas/contents/images/
--rw-r--r--   0 phil       (501) staff       (20)      571 2023-06-02 10:06:50.166314 PyQt6-6.5.1/examples/quick/canvas/contents/images/button-pressed.png
--rw-r--r--   0 phil       (501) staff       (20)      564 2023-06-02 10:06:50.161335 PyQt6-6.5.1/examples/quick/canvas/contents/images/button.png
--rw-r--r--   0 phil       (501) staff       (20)     7458 2023-06-02 10:06:50.161147 PyQt6-6.5.1/examples/quick/canvas/contents/images/default.svg
--rw-r--r--   0 phil       (501) staff       (20)     1236 2023-06-02 10:06:50.162316 PyQt6-6.5.1/examples/quick/canvas/contents/images/gloss.png
--rw-r--r--   0 phil       (501) staff       (20)     1415 2023-06-02 10:06:50.293982 PyQt6-6.5.1/examples/quick/canvas/contents/images/lineedit.png
--rw-r--r--   0 phil       (501) staff       (20)       87 2023-06-02 10:06:50.161058 PyQt6-6.5.1/examples/quick/canvas/contents/images/lineedit.sci
--rw-r--r--   0 phil       (501) staff       (20)     2369 2023-06-02 10:06:50.163311 PyQt6-6.5.1/examples/quick/canvas/contents/images/quit.png
--rw-r--r--   0 phil       (501) staff       (20)      257 2023-06-02 10:06:50.163978 PyQt6-6.5.1/examples/quick/canvas/contents/images/stripes.png
--rw-r--r--   0 phil       (501) staff       (20)     1436 2023-06-02 10:06:50.164370 PyQt6-6.5.1/examples/quick/canvas/contents/images/titlebar.png
--rw-r--r--   0 phil       (501) staff       (20)       87 2023-06-02 10:06:50.165417 PyQt6-6.5.1/examples/quick/canvas/contents/images/titlebar.sci
--rw-r--r--   0 phil       (501) staff       (20)     2550 2023-06-02 10:06:50.166104 PyQt6-6.5.1/examples/quick/canvas/contents/images/toolbutton.png
--rw-r--r--   0 phil       (501) staff       (20)       87 2023-06-02 10:06:50.165238 PyQt6-6.5.1/examples/quick/canvas/contents/images/toolbutton.sci
--rw-r--r--   0 phil       (501) staff       (20)    23519 2023-06-02 10:06:50.168261 PyQt6-6.5.1/examples/quick/canvas/contents/qt-logo.png
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.796400 PyQt6-6.5.1/examples/quick/canvas/quadraticCurveTo/
--rw-r--r--   0 phil       (501) staff       (20)     4992 2023-06-02 10:06:50.162780 PyQt6-6.5.1/examples/quick/canvas/quadraticCurveTo/quadraticCurveTo.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.787737 PyQt6-6.5.1/examples/quick/canvas/roundedrect/
--rw-r--r--   0 phil       (501) staff       (20)     5070 2023-06-02 10:06:50.162926 PyQt6-6.5.1/examples/quick/canvas/roundedrect/roundedrect.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.798197 PyQt6-6.5.1/examples/quick/canvas/smile/
--rw-r--r--   0 phil       (501) staff       (20)     5063 2023-06-02 10:06:50.163872 PyQt6-6.5.1/examples/quick/canvas/smile/smile.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.797213 PyQt6-6.5.1/examples/quick/canvas/squircle/
--rw-r--r--   0 phil       (501) staff       (20)      771 2023-06-02 10:06:50.294476 PyQt6-6.5.1/examples/quick/canvas/squircle/squircle.png
--rw-r--r--   0 phil       (501) staff       (20)     5379 2023-06-02 10:06:50.162428 PyQt6-6.5.1/examples/quick/canvas/squircle/squircle.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.795968 PyQt6-6.5.1/examples/quick/canvas/tiger/
--rw-r--r--   0 phil       (501) staff       (20)    93676 2023-06-02 10:06:50.166688 PyQt6-6.5.1/examples/quick/canvas/tiger/tiger.js
--rw-r--r--   0 phil       (501) staff       (20)     4864 2023-06-02 10:06:50.165329 PyQt6-6.5.1/examples/quick/canvas/tiger/tiger.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.786019 PyQt6-6.5.1/examples/quick/models/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.785692 PyQt6-6.5.1/examples/quick/models/abstractitemmodel/
--rw-r--r--   0 phil       (501) staff       (20)     4051 2023-06-02 10:06:50.165947 PyQt6-6.5.1/examples/quick/models/abstractitemmodel/abstractitemmodel.py
--rw-r--r--   0 phil       (501) staff       (20)     2151 2023-06-02 10:06:50.166685 PyQt6-6.5.1/examples/quick/models/abstractitemmodel/view.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.784887 PyQt6-6.5.1/examples/quick/models/objectlistmodel/
--rw-r--r--   0 phil       (501) staff       (20)     3630 2023-06-02 10:06:50.167480 PyQt6-6.5.1/examples/quick/models/objectlistmodel/objectlistmodel.py
--rw-r--r--   0 phil       (501) staff       (20)     2784 2023-06-02 10:06:50.166552 PyQt6-6.5.1/examples/quick/models/objectlistmodel/view.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.786480 PyQt6-6.5.1/examples/quick/models/stringlistmodel/
--rw-r--r--   0 phil       (501) staff       (20)     2607 2023-06-02 10:06:50.169553 PyQt6-6.5.1/examples/quick/models/stringlistmodel/stringlistmodel.py
--rw-r--r--   0 phil       (501) staff       (20)     2772 2023-06-02 10:06:50.164296 PyQt6-6.5.1/examples/quick/models/stringlistmodel/view.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.805162 PyQt6-6.5.1/examples/quick/scenegraph/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.805712 PyQt6-6.5.1/examples/quick/scenegraph/customgeometry/
--rw-r--r--   0 phil       (501) staff       (20)     5922 2023-06-02 10:06:50.164540 PyQt6-6.5.1/examples/quick/scenegraph/customgeometry/customgeometry.py
--rw-r--r--   0 phil       (501) staff       (20)     2732 2023-06-02 10:06:50.165585 PyQt6-6.5.1/examples/quick/scenegraph/customgeometry/main.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.783642 PyQt6-6.5.1/examples/quick/shared/
--rw-r--r--   0 phil       (501) staff       (20)     3291 2023-06-02 10:06:50.294983 PyQt6-6.5.1/examples/quick/shared/Button.qml
--rw-r--r--   0 phil       (501) staff       (20)     5174 2023-06-02 10:06:50.163696 PyQt6-6.5.1/examples/quick/shared/LauncherList.qml
--rw-r--r--   0 phil       (501) staff       (20)     3287 2023-06-02 10:06:50.167892 PyQt6-6.5.1/examples/quick/shared/SimpleLauncherDelegate.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.784046 PyQt6-6.5.1/examples/quick/shared/images/
--rw-r--r--   0 phil       (501) staff       (20)     1590 2023-06-02 10:06:50.166945 PyQt6-6.5.1/examples/quick/shared/images/back.png
--rw-r--r--   0 phil       (501) staff       (20)     1371 2023-06-02 10:06:50.167257 PyQt6-6.5.1/examples/quick/shared/images/next.png
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.798770 PyQt6-6.5.1/examples/quick/tutorials/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.804228 PyQt6-6.5.1/examples/quick/tutorials/extending/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.804746 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter1-basics/
--rw-r--r--   0 phil       (501) staff       (20)     2385 2023-06-02 10:06:50.168529 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter1-basics/app.qml
--rw-r--r--   0 phil       (501) staff       (20)     3492 2023-06-02 10:06:50.168954 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter1-basics/chapter1-basics.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.799234 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter2-methods/
--rw-r--r--   0 phil       (501) staff       (20)     2532 2023-06-02 10:06:50.168159 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter2-methods/app.qml
--rw-r--r--   0 phil       (501) staff       (20)     3538 2023-06-02 10:06:50.170865 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter2-methods/chapter2-methods.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.800152 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter3-bindings/
--rw-r--r--   0 phil       (501) staff       (20)     2650 2023-06-02 10:06:50.166073 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter3-bindings/app.qml
--rw-r--r--   0 phil       (501) staff       (20)     3625 2023-06-02 10:06:50.166230 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter3-bindings/chapter3-bindings.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.801960 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter4-customPropertyTypes/
--rw-r--r--   0 phil       (501) staff       (20)     2361 2023-06-02 10:06:50.167615 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter4-customPropertyTypes/app.qml
--rw-r--r--   0 phil       (501) staff       (20)     3724 2023-06-02 10:06:50.295562 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter4-customPropertyTypes/chapter4-customPropertyTypes.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.801030 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter5-listproperties/
--rw-r--r--   0 phil       (501) staff       (20)     2643 2023-06-02 10:06:50.166621 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter5-listproperties/app.qml
--rw-r--r--   0 phil       (501) staff       (20)     4116 2023-06-02 10:06:50.169606 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter5-listproperties/chapter5-listproperties.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.802761 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.803937 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/Charts/
--rw-r--r--   0 phil       (501) staff       (20)     2292 2023-06-02 10:06:50.168903 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/Charts/chartsplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     2587 2023-06-02 10:06:50.169043 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/Charts/piechart.py
--rw-r--r--   0 phil       (501) staff       (20)     3132 2023-06-02 10:06:50.169898 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/Charts/pieslice.py
--rw-r--r--   0 phil       (501) staff       (20)       36 2023-06-02 10:06:50.170225 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/Charts/qmldir
--rw-r--r--   0 phil       (501) staff       (20)     2643 2023-06-02 10:06:50.169574 PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/app.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.824997 PyQt6-6.5.1/examples/richtext/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.825556 PyQt6-6.5.1/examples/richtext/textobject/
--rw-r--r--   0 phil       (501) staff       (20)     3873 2023-06-02 10:06:50.172084 PyQt6-6.5.1/examples/richtext/textobject/heart.svg
--rw-r--r--   0 phil       (501) staff       (20)     4491 2023-06-02 10:06:50.167915 PyQt6-6.5.1/examples/richtext/textobject/textobject.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.705146 PyQt6-6.5.1/lupdate/
--rw-r--r--   0 phil       (501) staff       (20)      875 2023-06-02 10:40:57.508557 PyQt6-6.5.1/lupdate/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2479 2023-06-02 10:40:57.509497 PyQt6-6.5.1/lupdate/designer_source.py
--rw-r--r--   0 phil       (501) staff       (20)     3416 2023-06-02 10:40:57.512109 PyQt6-6.5.1/lupdate/lupdate.py
--rw-r--r--   0 phil       (501) staff       (20)     3062 2023-06-02 10:40:57.505460 PyQt6-6.5.1/lupdate/pylupdate.py
--rw-r--r--   0 phil       (501) staff       (20)    11176 2023-06-02 10:40:57.511485 PyQt6-6.5.1/lupdate/python_source.py
--rw-r--r--   0 phil       (501) staff       (20)     1114 2023-06-02 10:40:57.509004 PyQt6-6.5.1/lupdate/source_file.py
--rw-r--r--   0 phil       (501) staff       (20)    14976 2023-06-02 10:40:57.507699 PyQt6-6.5.1/lupdate/translation_file.py
--rw-r--r--   0 phil       (501) staff       (20)     1633 2023-06-02 10:40:57.508240 PyQt6-6.5.1/lupdate/translations.py
--rw-r--r--   0 phil       (501) staff       (20)     1504 2023-06-02 10:40:57.504645 PyQt6-6.5.1/lupdate/user.py
--rw-r--r--   0 phil       (501) staff       (20)    29937 2023-06-02 10:40:57.553051 PyQt6-6.5.1/project.py
--rw-r--r--   0 phil       (501) staff       (20)      546 2023-06-02 10:40:57.553341 PyQt6-6.5.1/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.071054 PyQt6-6.5.1/qmlscene/
--rw-r--r--   0 phil       (501) staff       (20)     9302 2023-06-02 10:40:57.548539 PyQt6-6.5.1/qmlscene/pluginloader.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1670 2023-06-02 10:40:57.549040 PyQt6-6.5.1/qmlscene/pluginloader.h
--rw-r--r--   0 phil       (501) staff       (20)      451 2023-06-02 10:40:57.546508 PyQt6-6.5.1/qmlscene/qmlscene.pro-in
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.740945 PyQt6-6.5.1/qpy/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.760700 PyQt6-6.5.1/qpy/QtCore/
--rw-r--r--   0 phil       (501) staff       (20)     3878 2023-06-02 10:40:57.409247 PyQt6-6.5.1/qpy/QtCore/qpycore_api.h
--rw-r--r--   0 phil       (501) staff       (20)    49695 2023-06-02 10:40:57.358866 PyQt6-6.5.1/qpy/QtCore/qpycore_chimera.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9586 2023-06-02 10:40:57.373818 PyQt6-6.5.1/qpy/QtCore/qpycore_chimera.h
--rw-r--r--   0 phil       (501) staff       (20)     2557 2023-06-02 10:40:57.395499 PyQt6-6.5.1/qpy/QtCore/qpycore_chimera_signature.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3515 2023-06-02 10:40:57.393263 PyQt6-6.5.1/qpy/QtCore/qpycore_chimera_storage.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3077 2023-06-02 10:40:57.396861 PyQt6-6.5.1/qpy/QtCore/qpycore_classinfo.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1089 2023-06-02 10:40:57.319587 PyQt6-6.5.1/qpy/QtCore/qpycore_classinfo.h
--rw-r--r--   0 phil       (501) staff       (20)     4385 2023-06-02 10:40:57.350064 PyQt6-6.5.1/qpy/QtCore/qpycore_decorators.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5930 2023-06-02 10:40:57.344617 PyQt6-6.5.1/qpy/QtCore/qpycore_enums_flags.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1261 2023-06-02 10:40:57.394939 PyQt6-6.5.1/qpy/QtCore/qpycore_enums_flags.h
--rw-r--r--   0 phil       (501) staff       (20)     4006 2023-06-02 10:40:57.325301 PyQt6-6.5.1/qpy/QtCore/qpycore_event_handlers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1376 2023-06-02 10:40:57.398054 PyQt6-6.5.1/qpy/QtCore/qpycore_event_handlers.h
--rw-r--r--   0 phil       (501) staff       (20)     3908 2023-06-02 10:40:57.346018 PyQt6-6.5.1/qpy/QtCore/qpycore_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1815 2023-06-02 10:40:57.375496 PyQt6-6.5.1/qpy/QtCore/qpycore_misc.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1136 2023-06-02 10:40:57.332980 PyQt6-6.5.1/qpy/QtCore/qpycore_misc.h
--rw-r--r--   0 phil       (501) staff       (20)     1136 2023-06-02 10:40:57.348027 PyQt6-6.5.1/qpy/QtCore/qpycore_namespace.h
--rw-r--r--   0 phil       (501) staff       (20)     1183 2023-06-02 10:40:57.379539 PyQt6-6.5.1/qpy/QtCore/qpycore_objectified_strings.h
--rw-r--r--   0 phil       (501) staff       (20)     4375 2023-06-02 10:40:57.326830 PyQt6-6.5.1/qpy/QtCore/qpycore_post_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12835 2023-06-02 10:40:57.401265 PyQt6-6.5.1/qpy/QtCore/qpycore_public_api.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4908 2023-06-02 10:40:57.398656 PyQt6-6.5.1/qpy/QtCore/qpycore_public_api.h
--rw-r--r--   0 phil       (501) staff       (20)    29685 2023-06-02 10:40:57.387069 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtboundsignal.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2023 2023-06-02 10:40:57.402645 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtboundsignal.h
--rw-r--r--   0 phil       (501) staff       (20)     6090 2023-06-02 10:40:57.388451 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtconfigure.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7424 2023-06-02 10:40:57.382854 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtmethodproxy.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1769 2023-06-02 10:40:57.349323 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtmethodproxy.h
--rw-r--r--   0 phil       (501) staff       (20)     2072 2023-06-02 10:40:57.394484 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtmutexlocker.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1438 2023-06-02 10:40:57.369582 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtmutexlocker.h
--rw-r--r--   0 phil       (501) staff       (20)    15571 2023-06-02 10:40:57.342475 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtproperty.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2076 2023-06-02 10:40:57.343317 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtproperty.h
--rw-r--r--   0 phil       (501) staff       (20)     4765 2023-06-02 10:40:57.377359 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtpyobject.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1742 2023-06-02 10:40:57.348738 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtpyobject.h
--rw-r--r--   0 phil       (501) staff       (20)    20440 2023-06-02 10:40:57.324450 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtsignal.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2537 2023-06-02 10:40:57.376164 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtsignal.h
--rw-r--r--   0 phil       (501) staff       (20)     9102 2023-06-02 10:40:57.361443 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtslot.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2284 2023-06-02 10:40:57.399114 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtslot.h
--rw-r--r--   0 phil       (501) staff       (20)    10864 2023-06-02 10:40:57.390718 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtslotproxy.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3552 2023-06-02 10:40:57.380381 PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtslotproxy.h
--rw-r--r--   0 phil       (501) staff       (20)     4375 2023-06-02 10:40:57.402138 PyQt6-6.5.1/qpy/QtCore/qpycore_qjsonvalue.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3016 2023-06-02 10:40:57.397508 PyQt6-6.5.1/qpy/QtCore/qpycore_qmessagelogger.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4296 2023-06-02 10:40:57.370669 PyQt6-6.5.1/qpy/QtCore/qpycore_qmetaobject.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4569 2023-06-02 10:40:57.392464 PyQt6-6.5.1/qpy/QtCore/qpycore_qmetaobject_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3505 2023-06-02 10:40:57.372162 PyQt6-6.5.1/qpy/QtCore/qpycore_qmetaobjectbuilder.h
--rw-r--r--   0 phil       (501) staff       (20)     4273 2023-06-02 10:40:57.381301 PyQt6-6.5.1/qpy/QtCore/qpycore_qobject_getattr.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8681 2023-06-02 10:40:57.379057 PyQt6-6.5.1/qpy/QtCore/qpycore_qobject_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1408 2023-06-02 10:40:57.403050 PyQt6-6.5.1/qpy/QtCore/qpycore_qobject_helpers.h
--rw-r--r--   0 phil       (501) staff       (20)     4181 2023-06-02 10:40:57.362330 PyQt6-6.5.1/qpy/QtCore/qpycore_qstring.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3178 2023-06-02 10:40:57.335111 PyQt6-6.5.1/qpy/QtCore/qpycore_qt_conf.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2535 2023-06-02 10:40:57.393864 PyQt6-6.5.1/qpy/QtCore/qpycore_qvariant.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6459 2023-06-02 10:40:57.347427 PyQt6-6.5.1/qpy/QtCore/qpycore_qvariant_value.cpp
--rw-r--r--   0 phil       (501) staff       (20)    17334 2023-06-02 10:40:57.338615 PyQt6-6.5.1/qpy/QtCore/qpycore_types.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1576 2023-06-02 10:40:57.339637 PyQt6-6.5.1/qpy/QtCore/qpycore_types.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.738575 PyQt6-6.5.1/qpy/QtDBus/
--rw-r--r--   0 phil       (501) staff       (20)      999 2023-06-02 10:40:57.413211 PyQt6-6.5.1/qpy/QtDBus/qpydbus_api.h
--rw-r--r--   0 phil       (501) staff       (20)     5739 2023-06-02 10:40:57.416793 PyQt6-6.5.1/qpy/QtDBus/qpydbus_chimera_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1236 2023-06-02 10:40:57.415484 PyQt6-6.5.1/qpy/QtDBus/qpydbus_chimera_helpers.h
--rw-r--r--   0 phil       (501) staff       (20)     1471 2023-06-02 10:40:57.412340 PyQt6-6.5.1/qpy/QtDBus/qpydbus_post_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1865 2023-06-02 10:40:57.412753 PyQt6-6.5.1/qpy/QtDBus/qpydbuspendingreply.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1340 2023-06-02 10:40:57.415110 PyQt6-6.5.1/qpy/QtDBus/qpydbuspendingreply.h
--rw-r--r--   0 phil       (501) staff       (20)     3583 2023-06-02 10:40:57.414704 PyQt6-6.5.1/qpy/QtDBus/qpydbusreply.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1788 2023-06-02 10:40:57.411952 PyQt6-6.5.1/qpy/QtDBus/qpydbusreply.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.730536 PyQt6-6.5.1/qpy/QtDesigner/
--rw-r--r--   0 phil       (501) staff       (20)     1410 2023-06-02 10:40:57.418564 PyQt6-6.5.1/qpy/QtDesigner/qpydesignercontainerextension.h
--rw-r--r--   0 phil       (501) staff       (20)     1492 2023-06-02 10:40:57.420426 PyQt6-6.5.1/qpy/QtDesigner/qpydesignercustomwidgetcollectionplugin.h
--rw-r--r--   0 phil       (501) staff       (20)     1402 2023-06-02 10:40:57.419668 PyQt6-6.5.1/qpy/QtDesigner/qpydesignercustomwidgetplugin.h
--rw-r--r--   0 phil       (501) staff       (20)     1430 2023-06-02 10:40:57.417785 PyQt6-6.5.1/qpy/QtDesigner/qpydesignermembersheetextension.h
--rw-r--r--   0 phil       (501) staff       (20)     1450 2023-06-02 10:40:57.418959 PyQt6-6.5.1/qpy/QtDesigner/qpydesignerpropertysheetextension.h
--rw-r--r--   0 phil       (501) staff       (20)     1400 2023-06-02 10:40:57.421136 PyQt6-6.5.1/qpy/QtDesigner/qpydesignertaskmenuextension.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.722279 PyQt6-6.5.1/qpy/QtOpenGL/
--rw-r--r--   0 phil       (501) staff       (20)   209932 2023-06-02 10:40:57.457748 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_add_constants.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2585 2023-06-02 10:40:57.463820 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_api.h
--rw-r--r--   0 phil       (501) staff       (20)     4002 2023-06-02 10:40:57.462182 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_array_convertors.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7165 2023-06-02 10:40:57.460011 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_attribute_array.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5002 2023-06-02 10:40:57.463284 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_data_cache.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2413 2023-06-02 10:40:57.432520 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_data_cache.h
--rw-r--r--   0 phil       (501) staff       (20)     4686 2023-06-02 10:40:57.458698 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_get.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1228 2023-06-02 10:40:57.464564 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1261 2023-06-02 10:40:57.433081 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_misc.h
--rw-r--r--   0 phil       (501) staff       (20)    12637 2023-06-02 10:40:57.435114 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_uniform_value_array.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9947 2023-06-02 10:40:57.437266 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_value_array.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3103 2023-06-02 10:40:57.460645 PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_version_functions.cpp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.728339 PyQt6-6.5.1/qpy/QtQml/
--rw-r--r--   0 phil       (501) staff       (20)     2279 2023-06-02 10:40:57.476389 PyQt6-6.5.1/qpy/QtQml/qpyqml_api.h
--rw-r--r--   0 phil       (501) staff       (20)     1799 2023-06-02 10:40:57.480886 PyQt6-6.5.1/qpy/QtQml/qpyqml_listdata.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1431 2023-06-02 10:40:57.486221 PyQt6-6.5.1/qpy/QtQml/qpyqml_listdata.h
--rw-r--r--   0 phil       (501) staff       (20)     2595 2023-06-02 10:40:57.482061 PyQt6-6.5.1/qpy/QtQml/qpyqml_post_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3089 2023-06-02 10:40:57.480361 PyQt6-6.5.1/qpy/QtQml/qpyqml_qjsvalue.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5283 2023-06-02 10:40:57.472844 PyQt6-6.5.1/qpy/QtQml/qpyqml_register_singleton_type.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12648 2023-06-02 10:40:57.483978 PyQt6-6.5.1/qpy/QtQml/qpyqml_register_type.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9495 2023-06-02 10:40:57.485751 PyQt6-6.5.1/qpy/QtQml/qpyqmllistproperty.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1118 2023-06-02 10:40:57.479639 PyQt6-6.5.1/qpy/QtQml/qpyqmllistproperty.h
--rw-r--r--   0 phil       (501) staff       (20)     6171 2023-06-02 10:40:57.477970 PyQt6-6.5.1/qpy/QtQml/qpyqmllistpropertywrapper.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1884 2023-06-02 10:40:57.476894 PyQt6-6.5.1/qpy/QtQml/qpyqmllistpropertywrapper.h
--rw-r--r--   0 phil       (501) staff       (20)    17618 2023-06-02 10:40:57.475849 PyQt6-6.5.1/qpy/QtQml/qpyqmlobject.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7477 2023-06-02 10:40:57.468120 PyQt6-6.5.1/qpy/QtQml/qpyqmlobject.h
--rw-r--r--   0 phil       (501) staff       (20)     3201 2023-06-02 10:40:57.478722 PyQt6-6.5.1/qpy/QtQml/qpyqmlsingletonobject.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3097 2023-06-02 10:40:57.469207 PyQt6-6.5.1/qpy/QtQml/qpyqmlsingletonobject.h
--rw-r--r--   0 phil       (501) staff       (20)    10140 2023-06-02 10:40:57.471922 PyQt6-6.5.1/qpy/QtQml/qpyqmlvalidator.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3440 2023-06-02 10:40:57.470063 PyQt6-6.5.1/qpy/QtQml/qpyqmlvalidator.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.736082 PyQt6-6.5.1/qpy/QtQuick/
--rw-r--r--   0 phil       (501) staff       (20)     1136 2023-06-02 10:40:57.490235 PyQt6-6.5.1/qpy/QtQuick/qpyquick_api.h
--rw-r--r--   0 phil       (501) staff       (20)     4162 2023-06-02 10:40:57.491437 PyQt6-6.5.1/qpy/QtQuick/qpyquick_chimera_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1601 2023-06-02 10:40:57.488629 PyQt6-6.5.1/qpy/QtQuick/qpyquick_chimera_helpers.h
--rw-r--r--   0 phil       (501) staff       (20)     2528 2023-06-02 10:40:57.487018 PyQt6-6.5.1/qpy/QtQuick/qpyquick_post_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2490 2023-06-02 10:40:57.488182 PyQt6-6.5.1/qpy/QtQuick/qpyquick_register_type.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1297 2023-06-02 10:40:57.495072 PyQt6-6.5.1/qpy/QtQuick/qpyquick_register_type.h
--rw-r--r--   0 phil       (501) staff       (20)     6763 2023-06-02 10:40:57.492390 PyQt6-6.5.1/qpy/QtQuick/qpyquickframebufferobject.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3136 2023-06-02 10:40:57.487673 PyQt6-6.5.1/qpy/QtQuick/qpyquickframebufferobject.h
--rw-r--r--   0 phil       (501) staff       (20)     7803 2023-06-02 10:40:57.496252 PyQt6-6.5.1/qpy/QtQuick/qpyquickitem.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3255 2023-06-02 10:40:57.497098 PyQt6-6.5.1/qpy/QtQuick/qpyquickitem.h
--rw-r--r--   0 phil       (501) staff       (20)     6215 2023-06-02 10:40:57.489755 PyQt6-6.5.1/qpy/QtQuick/qpyquickpainteditem.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2873 2023-06-02 10:40:57.493193 PyQt6-6.5.1/qpy/QtQuick/qpyquickpainteditem.h
--rw-r--r--   0 phil       (501) staff       (20)     5020 2023-06-02 10:40:57.494090 PyQt6-6.5.1/qpy/QtQuick/qpyquickview.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2326 2023-06-02 10:40:57.498765 PyQt6-6.5.1/qpy/QtQuick/qpyquickview.h
--rw-r--r--   0 phil       (501) staff       (20)     5160 2023-06-02 10:40:57.498029 PyQt6-6.5.1/qpy/QtQuick/qpyquickwindow.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2396 2023-06-02 10:40:57.494647 PyQt6-6.5.1/qpy/QtQuick/qpyquickwindow.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.740600 PyQt6-6.5.1/qpy/QtWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     1008 2023-06-02 10:40:57.499564 PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_api.h
--rw-r--r--   0 phil       (501) staff       (20)     1805 2023-06-02 10:40:57.500409 PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_chimera_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1247 2023-06-02 10:40:57.501703 PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_chimera_helpers.h
--rw-r--r--   0 phil       (501) staff       (20)     1703 2023-06-02 10:40:57.502776 PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_post_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1195 2023-06-02 10:40:57.499889 PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_qaction_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1147 2023-06-02 10:40:57.502177 PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_qaction_helpers.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.069540 PyQt6-6.5.1/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.888438 PyQt6-6.5.1/sip/QAxContainer/
--rw-r--r--   0 phil       (501) staff       (20)     1998 2023-06-02 10:41:04.424536 PyQt6-6.5.1/sip/QAxContainer/QAxContainermod.sip
--rw-r--r--   0 phil       (501) staff       (20)     4938 2023-06-02 10:41:04.425399 PyQt6-6.5.1/sip/QAxContainer/qaxbase.sip
--rw-r--r--   0 phil       (501) staff       (20)     2540 2023-06-02 10:41:04.426932 PyQt6-6.5.1/sip/QAxContainer/qaxobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     1251 2023-06-02 10:41:04.425810 PyQt6-6.5.1/sip/QAxContainer/qaxobjectinterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     2350 2023-06-02 10:41:04.426344 PyQt6-6.5.1/sip/QAxContainer/qaxwidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.857484 PyQt6-6.5.1/sip/QtBluetooth/
--rw-r--r--   0 phil       (501) staff       (20)     2777 2023-06-02 10:41:04.321223 PyQt6-6.5.1/sip/QtBluetooth/QtBluetoothmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1559 2023-06-02 10:41:04.320245 PyQt6-6.5.1/sip/QtBluetooth/qbluetooth.sip
--rw-r--r--   0 phil       (501) staff       (20)     1673 2023-06-02 10:41:04.311484 PyQt6-6.5.1/sip/QtBluetooth/qbluetoothaddress.sip
--rw-r--r--   0 phil       (501) staff       (20)     2670 2023-06-02 10:41:04.315983 PyQt6-6.5.1/sip/QtBluetooth/qbluetoothdevicediscoveryagent.sip
--rw-r--r--   0 phil       (501) staff       (20)     6598 2023-06-02 10:41:04.309594 PyQt6-6.5.1/sip/QtBluetooth/qbluetoothdeviceinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1541 2023-06-02 10:41:04.322807 PyQt6-6.5.1/sip/QtBluetooth/qbluetoothhostinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     2570 2023-06-02 10:41:04.320774 PyQt6-6.5.1/sip/QtBluetooth/qbluetoothlocaldevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3360 2023-06-02 10:41:04.321943 PyQt6-6.5.1/sip/QtBluetooth/qbluetoothserver.sip
--rw-r--r--   0 phil       (501) staff       (20)     2467 2023-06-02 10:41:04.313752 PyQt6-6.5.1/sip/QtBluetooth/qbluetoothservicediscoveryagent.sip
--rw-r--r--   0 phil       (501) staff       (20)     3324 2023-06-02 10:41:04.323391 PyQt6-6.5.1/sip/QtBluetooth/qbluetoothserviceinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     5134 2023-06-02 10:41:04.310337 PyQt6-6.5.1/sip/QtBluetooth/qbluetoothsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     9422 2023-06-02 10:41:04.319054 PyQt6-6.5.1/sip/QtBluetooth/qbluetoothuuid.sip
--rw-r--r--   0 phil       (501) staff       (20)     2334 2023-06-02 10:41:04.308462 PyQt6-6.5.1/sip/QtBluetooth/qlowenergyadvertisingdata.sip
--rw-r--r--   0 phil       (501) staff       (20)     3006 2023-06-02 10:41:04.307804 PyQt6-6.5.1/sip/QtBluetooth/qlowenergyadvertisingparameters.sip
--rw-r--r--   0 phil       (501) staff       (20)     2262 2023-06-02 10:41:04.312266 PyQt6-6.5.1/sip/QtBluetooth/qlowenergycharacteristic.sip
--rw-r--r--   0 phil       (501) staff       (20)     2472 2023-06-02 10:41:04.319795 PyQt6-6.5.1/sip/QtBluetooth/qlowenergycharacteristicdata.sip
--rw-r--r--   0 phil       (501) staff       (20)     1843 2023-06-02 10:41:04.322387 PyQt6-6.5.1/sip/QtBluetooth/qlowenergyconnectionparameters.sip
--rw-r--r--   0 phil       (501) staff       (20)     4355 2023-06-02 10:41:04.311029 PyQt6-6.5.1/sip/QtBluetooth/qlowenergycontroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     1568 2023-06-02 10:41:04.316485 PyQt6-6.5.1/sip/QtBluetooth/qlowenergydescriptor.sip
--rw-r--r--   0 phil       (501) staff       (20)     2201 2023-06-02 10:41:04.317505 PyQt6-6.5.1/sip/QtBluetooth/qlowenergydescriptordata.sip
--rw-r--r--   0 phil       (501) staff       (20)     3661 2023-06-02 10:41:04.314434 PyQt6-6.5.1/sip/QtBluetooth/qlowenergyservice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2201 2023-06-02 10:41:04.316996 PyQt6-6.5.1/sip/QtBluetooth/qlowenergyservicedata.sip
--rw-r--r--   0 phil       (501) staff       (20)     3358 2023-06-02 10:41:04.315371 PyQt6-6.5.1/sip/QtBluetooth/qpybluetooth_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     4039 2023-06-02 10:41:04.313187 PyQt6-6.5.1/sip/QtBluetooth/qpybluetooth_qmultihash.sip
--rw-r--r--   0 phil       (501) staff       (20)     2860 2023-06-02 10:41:04.307088 PyQt6-6.5.1/sip/QtBluetooth/qpybluetooth_quint128.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.066058 PyQt6-6.5.1/sip/QtCore/
--rw-r--r--   0 phil       (501) staff       (20)     6347 2023-06-02 10:41:05.022572 PyQt6-6.5.1/sip/QtCore/QtCoremod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2557 2023-06-02 10:41:05.156292 PyQt6-6.5.1/sip/QtCore/qabstractanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     2449 2023-06-02 10:41:05.113631 PyQt6-6.5.1/sip/QtCore/qabstracteventdispatcher.sip
--rw-r--r--   0 phil       (501) staff       (20)    13972 2023-06-02 10:41:04.971474 PyQt6-6.5.1/sip/QtCore/qabstractitemmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1335 2023-06-02 10:41:05.133678 PyQt6-6.5.1/sip/QtCore/qabstractnativeeventfilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     3493 2023-06-02 10:41:05.119817 PyQt6-6.5.1/sip/QtCore/qabstractproxymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1649 2023-06-02 10:41:04.981335 PyQt6-6.5.1/sip/QtCore/qanimationgroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     2718 2023-06-02 10:41:04.960138 PyQt6-6.5.1/sip/QtCore/qanystringview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1338 2023-06-02 10:41:04.983538 PyQt6-6.5.1/sip/QtCore/qbasictimer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2909 2023-06-02 10:41:05.117309 PyQt6-6.5.1/sip/QtCore/qbitarray.sip
--rw-r--r--   0 phil       (501) staff       (20)     3743 2023-06-02 10:41:04.964919 PyQt6-6.5.1/sip/QtCore/qbuffer.sip
--rw-r--r--   0 phil       (501) staff       (20)    14436 2023-06-02 10:41:05.108444 PyQt6-6.5.1/sip/QtCore/qbytearray.sip
--rw-r--r--   0 phil       (501) staff       (20)     1144 2023-06-02 10:41:04.981822 PyQt6-6.5.1/sip/QtCore/qbytearrayalgorithms.sip
--rw-r--r--   0 phil       (501) staff       (20)     2976 2023-06-02 10:41:04.972313 PyQt6-6.5.1/sip/QtCore/qbytearraylist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1906 2023-06-02 10:41:05.123212 PyQt6-6.5.1/sip/QtCore/qbytearraymatcher.sip
--rw-r--r--   0 phil       (501) staff       (20)     2692 2023-06-02 10:41:05.128395 PyQt6-6.5.1/sip/QtCore/qbytearrayview.sip
--rw-r--r--   0 phil       (501) staff       (20)     3336 2023-06-02 10:41:04.961412 PyQt6-6.5.1/sip/QtCore/qcalendar.sip
--rw-r--r--   0 phil       (501) staff       (20)     2452 2023-06-02 10:41:05.060310 PyQt6-6.5.1/sip/QtCore/qcborcommon.sip
--rw-r--r--   0 phil       (501) staff       (20)     3894 2023-06-02 10:41:05.123938 PyQt6-6.5.1/sip/QtCore/qcborstreamreader.sip
--rw-r--r--   0 phil       (501) staff       (20)     2475 2023-06-02 10:41:05.105512 PyQt6-6.5.1/sip/QtCore/qcborstreamwriter.sip
--rw-r--r--   0 phil       (501) staff       (20)     1591 2023-06-02 10:41:05.026452 PyQt6-6.5.1/sip/QtCore/qchar.sip
--rw-r--r--   0 phil       (501) staff       (20)     2161 2023-06-02 10:41:04.980433 PyQt6-6.5.1/sip/QtCore/qcollator.sip
--rw-r--r--   0 phil       (501) staff       (20)     2203 2023-06-02 10:41:05.108982 PyQt6-6.5.1/sip/QtCore/qcommandlineoption.sip
--rw-r--r--   0 phil       (501) staff       (20)     2825 2023-06-02 10:41:05.118059 PyQt6-6.5.1/sip/QtCore/qcommandlineparser.sip
--rw-r--r--   0 phil       (501) staff       (20)     4086 2023-06-02 10:41:05.116746 PyQt6-6.5.1/sip/QtCore/qconcatenatetablesproxymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)    11852 2023-06-02 10:41:05.008861 PyQt6-6.5.1/sip/QtCore/qcoreapplication.sip
--rw-r--r--   0 phil       (501) staff       (20)     6998 2023-06-02 10:41:05.017321 PyQt6-6.5.1/sip/QtCore/qcoreevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2546 2023-06-02 10:41:05.015453 PyQt6-6.5.1/sip/QtCore/qcryptographichash.sip
--rw-r--r--   0 phil       (501) staff       (20)    11005 2023-06-02 10:41:05.021584 PyQt6-6.5.1/sip/QtCore/qdatastream.sip
--rw-r--r--   0 phil       (501) staff       (20)    15385 2023-06-02 10:41:05.079934 PyQt6-6.5.1/sip/QtCore/qdatetime.sip
--rw-r--r--   0 phil       (501) staff       (20)     2791 2023-06-02 10:41:05.083441 PyQt6-6.5.1/sip/QtCore/qdeadlinetimer.sip
--rw-r--r--   0 phil       (501) staff       (20)     6571 2023-06-02 10:41:05.024140 PyQt6-6.5.1/sip/QtCore/qdir.sip
--rw-r--r--   0 phil       (501) staff       (20)     2019 2023-06-02 10:41:04.963688 PyQt6-6.5.1/sip/QtCore/qdiriterator.sip
--rw-r--r--   0 phil       (501) staff       (20)     6671 2023-06-02 10:41:04.969549 PyQt6-6.5.1/sip/QtCore/qeasingcurve.sip
--rw-r--r--   0 phil       (501) staff       (20)     1833 2023-06-02 10:41:05.019511 PyQt6-6.5.1/sip/QtCore/qelapsedtimer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2197 2023-06-02 10:41:05.115569 PyQt6-6.5.1/sip/QtCore/qeventloop.sip
--rw-r--r--   0 phil       (501) staff       (20)     3031 2023-06-02 10:41:05.126028 PyQt6-6.5.1/sip/QtCore/qfile.sip
--rw-r--r--   0 phil       (501) staff       (20)     6316 2023-06-02 10:41:05.082771 PyQt6-6.5.1/sip/QtCore/qfiledevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3371 2023-06-02 10:41:05.025553 PyQt6-6.5.1/sip/QtCore/qfileinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1365 2023-06-02 10:41:05.072299 PyQt6-6.5.1/sip/QtCore/qfileselector.sip
--rw-r--r--   0 phil       (501) staff       (20)     1597 2023-06-02 10:41:05.072697 PyQt6-6.5.1/sip/QtCore/qfilesystemwatcher.sip
--rw-r--r--   0 phil       (501) staff       (20)     1457 2023-06-02 10:41:04.965410 PyQt6-6.5.1/sip/QtCore/qflags.sip
--rw-r--r--   0 phil       (501) staff       (20)     5036 2023-06-02 10:41:05.080961 PyQt6-6.5.1/sip/QtCore/qglobal.sip
--rw-r--r--   0 phil       (501) staff       (20)     3095 2023-06-02 10:41:05.130586 PyQt6-6.5.1/sip/QtCore/qidentityproxymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)    12510 2023-06-02 10:41:05.059677 PyQt6-6.5.1/sip/QtCore/qiodevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     1380 2023-06-02 10:41:05.110738 PyQt6-6.5.1/sip/QtCore/qiodevicebase.sip
--rw-r--r--   0 phil       (501) staff       (20)     8829 2023-06-02 10:41:05.130148 PyQt6-6.5.1/sip/QtCore/qitemselectionmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     3263 2023-06-02 10:41:05.106390 PyQt6-6.5.1/sip/QtCore/qjsonarray.sip
--rw-r--r--   0 phil       (501) staff       (20)     2862 2023-06-02 10:41:05.056177 PyQt6-6.5.1/sip/QtCore/qjsondocument.sip
--rw-r--r--   0 phil       (501) staff       (20)     3500 2023-06-02 10:41:04.976170 PyQt6-6.5.1/sip/QtCore/qjsonobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2892 2023-06-02 10:41:05.075411 PyQt6-6.5.1/sip/QtCore/qjsonvalue.sip
--rw-r--r--   0 phil       (501) staff       (20)     2418 2023-06-02 10:41:05.036912 PyQt6-6.5.1/sip/QtCore/qlibrary.sip
--rw-r--r--   0 phil       (501) staff       (20)     1661 2023-06-02 10:41:05.057717 PyQt6-6.5.1/sip/QtCore/qlibraryinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     5198 2023-06-02 10:41:05.057111 PyQt6-6.5.1/sip/QtCore/qline.sip
--rw-r--r--   0 phil       (501) staff       (20)    28155 2023-06-02 10:41:05.014816 PyQt6-6.5.1/sip/QtCore/qlocale.sip
--rw-r--r--   0 phil       (501) staff       (20)     1671 2023-06-02 10:41:04.972817 PyQt6-6.5.1/sip/QtCore/qlockfile.sip
--rw-r--r--   0 phil       (501) staff       (20)     6581 2023-06-02 10:41:05.114777 PyQt6-6.5.1/sip/QtCore/qlogging.sip
--rw-r--r--   0 phil       (501) staff       (20)     1612 2023-06-02 10:41:04.966909 PyQt6-6.5.1/sip/QtCore/qloggingcategory.sip
--rw-r--r--   0 phil       (501) staff       (20)     4347 2023-06-02 10:41:05.024939 PyQt6-6.5.1/sip/QtCore/qmargins.sip
--rw-r--r--   0 phil       (501) staff       (20)     1862 2023-06-02 10:41:05.124591 PyQt6-6.5.1/sip/QtCore/qmessageauthenticationcode.sip
--rw-r--r--   0 phil       (501) staff       (20)     9269 2023-06-02 10:41:05.078002 PyQt6-6.5.1/sip/QtCore/qmetaobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     4273 2023-06-02 10:41:05.009900 PyQt6-6.5.1/sip/QtCore/qmetatype.sip
--rw-r--r--   0 phil       (501) staff       (20)     1954 2023-06-02 10:41:04.963162 PyQt6-6.5.1/sip/QtCore/qmimedata.sip
--rw-r--r--   0 phil       (501) staff       (20)     2082 2023-06-02 10:41:05.076298 PyQt6-6.5.1/sip/QtCore/qmimedatabase.sip
--rw-r--r--   0 phil       (501) staff       (20)     1812 2023-06-02 10:41:05.071502 PyQt6-6.5.1/sip/QtCore/qmimetype.sip
--rw-r--r--   0 phil       (501) staff       (20)     1527 2023-06-02 10:41:04.962080 PyQt6-6.5.1/sip/QtCore/qmutex.sip
--rw-r--r--   0 phil       (501) staff       (20)     1961 2023-06-02 10:41:05.157331 PyQt6-6.5.1/sip/QtCore/qmutexlocker.sip
--rw-r--r--   0 phil       (501) staff       (20)    34263 2023-06-02 10:41:05.033792 PyQt6-6.5.1/sip/QtCore/qnamespace.sip
--rw-r--r--   0 phil       (501) staff       (20)     1410 2023-06-02 10:41:05.071922 PyQt6-6.5.1/sip/QtCore/qnumeric.sip
--rw-r--r--   0 phil       (501) staff       (20)    20046 2023-06-02 10:41:04.975372 PyQt6-6.5.1/sip/QtCore/qobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     1248 2023-06-02 10:41:05.113120 PyQt6-6.5.1/sip/QtCore/qobjectcleanuphandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     8135 2023-06-02 10:41:05.111738 PyQt6-6.5.1/sip/QtCore/qobjectdefs.sip
--rw-r--r--   0 phil       (501) staff       (20)     7658 2023-06-02 10:41:04.977188 PyQt6-6.5.1/sip/QtCore/qoperatingsystemversion.sip
--rw-r--r--   0 phil       (501) staff       (20)     1502 2023-06-02 10:41:04.985209 PyQt6-6.5.1/sip/QtCore/qparallelanimationgroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     1373 2023-06-02 10:41:05.076693 PyQt6-6.5.1/sip/QtCore/qpauseanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     7564 2023-06-02 10:41:04.983158 PyQt6-6.5.1/sip/QtCore/qpermissions.sip
--rw-r--r--   0 phil       (501) staff       (20)     1555 2023-06-02 10:41:04.962607 PyQt6-6.5.1/sip/QtCore/qpluginloader.sip
--rw-r--r--   0 phil       (501) staff       (20)     4684 2023-06-02 10:41:05.109832 PyQt6-6.5.1/sip/QtCore/qpoint.sip
--rw-r--r--   0 phil       (501) staff       (20)     7887 2023-06-02 10:41:05.122319 PyQt6-6.5.1/sip/QtCore/qprocess.sip
--rw-r--r--   0 phil       (501) staff       (20)     1695 2023-06-02 10:41:05.070866 PyQt6-6.5.1/sip/QtCore/qpropertyanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)    11135 2023-06-02 10:41:05.132620 PyQt6-6.5.1/sip/QtCore/qpycore_qhash.sip
--rw-r--r--   0 phil       (501) staff       (20)    30380 2023-06-02 10:41:05.066492 PyQt6-6.5.1/sip/QtCore/qpycore_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)    10053 2023-06-02 10:41:05.127826 PyQt6-6.5.1/sip/QtCore/qpycore_qmap.sip
--rw-r--r--   0 phil       (501) staff       (20)     5229 2023-06-02 10:41:04.984660 PyQt6-6.5.1/sip/QtCore/qpycore_qset.sip
--rw-r--r--   0 phil       (501) staff       (20)    11619 2023-06-02 10:41:04.979960 PyQt6-6.5.1/sip/QtCore/qpycore_std_pair.sip
--rw-r--r--   0 phil       (501) staff       (20)      976 2023-06-02 10:41:05.116052 PyQt6-6.5.1/sip/QtCore/qpycore_virtual_error_handler.sip
--rw-r--r--   0 phil       (501) staff       (20)     1863 2023-06-02 10:41:04.985623 PyQt6-6.5.1/sip/QtCore/qrandom.sip
--rw-r--r--   0 phil       (501) staff       (20)     2706 2023-06-02 10:41:05.081728 PyQt6-6.5.1/sip/QtCore/qreadwritelock.sip
--rw-r--r--   0 phil       (501) staff       (20)     9654 2023-06-02 10:41:05.121081 PyQt6-6.5.1/sip/QtCore/qrect.sip
--rw-r--r--   0 phil       (501) staff       (20)     7257 2023-06-02 10:41:05.155698 PyQt6-6.5.1/sip/QtCore/qregularexpression.sip
--rw-r--r--   0 phil       (501) staff       (20)     2661 2023-06-02 10:41:05.017851 PyQt6-6.5.1/sip/QtCore/qresource.sip
--rw-r--r--   0 phil       (501) staff       (20)     1718 2023-06-02 10:41:05.055415 PyQt6-6.5.1/sip/QtCore/qrunnable.sip
--rw-r--r--   0 phil       (501) staff       (20)     2390 2023-06-02 10:41:05.128874 PyQt6-6.5.1/sip/QtCore/qsavefile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1620 2023-06-02 10:41:05.112725 PyQt6-6.5.1/sip/QtCore/qsemaphore.sip
--rw-r--r--   0 phil       (501) staff       (20)     1721 2023-06-02 10:41:05.122754 PyQt6-6.5.1/sip/QtCore/qsequentialanimationgroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     5109 2023-06-02 10:41:05.068246 PyQt6-6.5.1/sip/QtCore/qsettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     2332 2023-06-02 10:41:05.035751 PyQt6-6.5.1/sip/QtCore/qsharedmemory.sip
--rw-r--r--   0 phil       (501) staff       (20)     1641 2023-06-02 10:41:05.110291 PyQt6-6.5.1/sip/QtCore/qsignalmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     5173 2023-06-02 10:41:05.067407 PyQt6-6.5.1/sip/QtCore/qsize.sip
--rw-r--r--   0 phil       (501) staff       (20)     1673 2023-06-02 10:41:04.965902 PyQt6-6.5.1/sip/QtCore/qsocketnotifier.sip
--rw-r--r--   0 phil       (501) staff       (20)     5908 2023-06-02 10:41:05.036454 PyQt6-6.5.1/sip/QtCore/qsortfilterproxymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     2598 2023-06-02 10:41:04.980950 PyQt6-6.5.1/sip/QtCore/qstandardpaths.sip
--rw-r--r--   0 phil       (501) staff       (20)     1966 2023-06-02 10:41:05.018868 PyQt6-6.5.1/sip/QtCore/qstorageinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1485 2023-06-02 10:41:04.968230 PyQt6-6.5.1/sip/QtCore/qstring.sip
--rw-r--r--   0 phil       (501) staff       (20)     3205 2023-06-02 10:41:04.977938 PyQt6-6.5.1/sip/QtCore/qstringconverter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2134 2023-06-02 10:41:05.119323 PyQt6-6.5.1/sip/QtCore/qstringconverter_base.sip
--rw-r--r--   0 phil       (501) staff       (20)     2937 2023-06-02 10:41:05.074874 PyQt6-6.5.1/sip/QtCore/qstringlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     2403 2023-06-02 10:41:05.034728 PyQt6-6.5.1/sip/QtCore/qstringlistmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1537 2023-06-02 10:41:05.007011 PyQt6-6.5.1/sip/QtCore/qstringview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1572 2023-06-02 10:41:04.966437 PyQt6-6.5.1/sip/QtCore/qsysinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1790 2023-06-02 10:41:05.015929 PyQt6-6.5.1/sip/QtCore/qsystemsemaphore.sip
--rw-r--r--   0 phil       (501) staff       (20)     1463 2023-06-02 10:41:05.060736 PyQt6-6.5.1/sip/QtCore/qtemporarydir.sip
--rw-r--r--   0 phil       (501) staff       (20)     1798 2023-06-02 10:41:04.969989 PyQt6-6.5.1/sip/QtCore/qtemporaryfile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1455 2023-06-02 10:41:05.027601 PyQt6-6.5.1/sip/QtCore/qtenvironmentvariables.sip
--rw-r--r--   0 phil       (501) staff       (20)     1998 2023-06-02 10:41:05.112247 PyQt6-6.5.1/sip/QtCore/qtextboundaryfinder.sip
--rw-r--r--   0 phil       (501) staff       (20)     5603 2023-06-02 10:41:05.125452 PyQt6-6.5.1/sip/QtCore/qtextstream.sip
--rw-r--r--   0 phil       (501) staff       (20)     2691 2023-06-02 10:41:05.027084 PyQt6-6.5.1/sip/QtCore/qthread.sip
--rw-r--r--   0 phil       (501) staff       (20)     4994 2023-06-02 10:41:05.005833 PyQt6-6.5.1/sip/QtCore/qthreadpool.sip
--rw-r--r--   0 phil       (501) staff       (20)     2431 2023-06-02 10:41:04.960725 PyQt6-6.5.1/sip/QtCore/qtimeline.sip
--rw-r--r--   0 phil       (501) staff       (20)     2585 2023-06-02 10:41:05.006491 PyQt6-6.5.1/sip/QtCore/qtimer.sip
--rw-r--r--   0 phil       (501) staff       (20)     5446 2023-06-02 10:41:04.967748 PyQt6-6.5.1/sip/QtCore/qtimezone.sip
--rw-r--r--   0 phil       (501) staff       (20)     1837 2023-06-02 10:41:05.035218 PyQt6-6.5.1/sip/QtCore/qtranslator.sip
--rw-r--r--   0 phil       (501) staff       (20)     2945 2023-06-02 10:41:05.025980 PyQt6-6.5.1/sip/QtCore/qtransposeproxymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1057 2023-06-02 10:41:05.075860 PyQt6-6.5.1/sip/QtCore/qtversion.sip
--rw-r--r--   0 phil       (501) staff       (20)     1843 2023-06-02 10:41:04.964235 PyQt6-6.5.1/sip/QtCore/qtypes.sip
--rw-r--r--   0 phil       (501) staff       (20)     7344 2023-06-02 10:41:05.073648 PyQt6-6.5.1/sip/QtCore/qurl.sip
--rw-r--r--   0 phil       (501) staff       (20)     2784 2023-06-02 10:41:05.018338 PyQt6-6.5.1/sip/QtCore/qurlquery.sip
--rw-r--r--   0 phil       (501) staff       (20)     3479 2023-06-02 10:41:05.133296 PyQt6-6.5.1/sip/QtCore/quuid.sip
--rw-r--r--   0 phil       (501) staff       (20)     3169 2023-06-02 10:41:05.023176 PyQt6-6.5.1/sip/QtCore/qvariant.sip
--rw-r--r--   0 phil       (501) staff       (20)     2197 2023-06-02 10:41:05.156774 PyQt6-6.5.1/sip/QtCore/qvariantanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     3856 2023-06-02 10:41:05.118762 PyQt6-6.5.1/sip/QtCore/qversionnumber.sip
--rw-r--r--   0 phil       (501) staff       (20)     1578 2023-06-02 10:41:05.034277 PyQt6-6.5.1/sip/QtCore/qwaitcondition.sip
--rw-r--r--   0 phil       (501) staff       (20)     1577 2023-06-02 10:41:05.074141 PyQt6-6.5.1/sip/QtCore/qwineventnotifier.sip
--rw-r--r--   0 phil       (501) staff       (20)    15570 2023-06-02 10:41:05.070418 PyQt6-6.5.1/sip/QtCore/qxmlstream.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.955080 PyQt6-6.5.1/sip/QtDBus/
--rw-r--r--   0 phil       (501) staff       (20)     2340 2023-06-02 10:41:04.708336 PyQt6-6.5.1/sip/QtDBus/QtDBusmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1271 2023-06-02 10:41:04.678831 PyQt6-6.5.1/sip/QtDBus/qdbusabstractadaptor.sip
--rw-r--r--   0 phil       (501) staff       (20)     7394 2023-06-02 10:41:04.706638 PyQt6-6.5.1/sip/QtDBus/qdbusabstractinterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     4871 2023-06-02 10:41:04.679688 PyQt6-6.5.1/sip/QtDBus/qdbusargument.sip
--rw-r--r--   0 phil       (501) staff       (20)     9428 2023-06-02 10:41:04.677348 PyQt6-6.5.1/sip/QtDBus/qdbusconnection.sip
--rw-r--r--   0 phil       (501) staff       (20)     2976 2023-06-02 10:41:04.680680 PyQt6-6.5.1/sip/QtDBus/qdbusconnectioninterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     1933 2023-06-02 10:41:04.707849 PyQt6-6.5.1/sip/QtDBus/qdbuserror.sip
--rw-r--r--   0 phil       (501) staff       (20)     2507 2023-06-02 10:41:04.677871 PyQt6-6.5.1/sip/QtDBus/qdbusextratypes.sip
--rw-r--r--   0 phil       (501) staff       (20)     1299 2023-06-02 10:41:04.681107 PyQt6-6.5.1/sip/QtDBus/qdbusinterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     3015 2023-06-02 10:41:04.678370 PyQt6-6.5.1/sip/QtDBus/qdbusmessage.sip
--rw-r--r--   0 phil       (501) staff       (20)     1745 2023-06-02 10:41:04.680172 PyQt6-6.5.1/sip/QtDBus/qdbuspendingcall.sip
--rw-r--r--   0 phil       (501) staff       (20)     2225 2023-06-02 10:41:04.707263 PyQt6-6.5.1/sip/QtDBus/qdbusservicewatcher.sip
--rw-r--r--   0 phil       (501) staff       (20)     1450 2023-06-02 10:41:04.675676 PyQt6-6.5.1/sip/QtDBus/qdbusunixfiledescriptor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1739 2023-06-02 10:41:04.676227 PyQt6-6.5.1/sip/QtDBus/qpydbuspendingreply.sip
--rw-r--r--   0 phil       (501) staff       (20)     5291 2023-06-02 10:41:04.675285 PyQt6-6.5.1/sip/QtDBus/qpydbusreply.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.880672 PyQt6-6.5.1/sip/QtDesigner/
--rw-r--r--   0 phil       (501) staff       (20)     2809 2023-06-02 10:41:04.413867 PyQt6-6.5.1/sip/QtDesigner/QtDesignermod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1493 2023-06-02 10:41:04.406058 PyQt6-6.5.1/sip/QtDesigner/abstractactioneditor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1457 2023-06-02 10:41:04.414927 PyQt6-6.5.1/sip/QtDesigner/abstractformbuilder.sip
--rw-r--r--   0 phil       (501) staff       (20)     2021 2023-06-02 10:41:04.412036 PyQt6-6.5.1/sip/QtDesigner/abstractformeditor.sip
--rw-r--r--   0 phil       (501) staff       (20)     4737 2023-06-02 10:41:04.406763 PyQt6-6.5.1/sip/QtDesigner/abstractformwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     2532 2023-06-02 10:41:04.410228 PyQt6-6.5.1/sip/QtDesigner/abstractformwindowcursor.sip
--rw-r--r--   0 phil       (501) staff       (20)     3286 2023-06-02 10:41:04.378970 PyQt6-6.5.1/sip/QtDesigner/abstractformwindowmanager.sip
--rw-r--r--   0 phil       (501) staff       (20)     1402 2023-06-02 10:41:04.412856 PyQt6-6.5.1/sip/QtDesigner/abstractobjectinspector.sip
--rw-r--r--   0 phil       (501) staff       (20)     1736 2023-06-02 10:41:04.413293 PyQt6-6.5.1/sip/QtDesigner/abstractpropertyeditor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1397 2023-06-02 10:41:04.411075 PyQt6-6.5.1/sip/QtDesigner/abstractwidgetbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     1633 2023-06-02 10:41:04.411513 PyQt6-6.5.1/sip/QtDesigner/container.sip
--rw-r--r--   0 phil       (501) staff       (20)     1884 2023-06-02 10:41:04.409151 PyQt6-6.5.1/sip/QtDesigner/customwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1438 2023-06-02 10:41:04.412452 PyQt6-6.5.1/sip/QtDesigner/default_extensionfactory.sip
--rw-r--r--   0 phil       (501) staff       (20)     1571 2023-06-02 10:41:04.409587 PyQt6-6.5.1/sip/QtDesigner/extension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1345 2023-06-02 10:41:04.407614 PyQt6-6.5.1/sip/QtDesigner/formbuilder.sip
--rw-r--r--   0 phil       (501) staff       (20)     1993 2023-06-02 10:41:04.408688 PyQt6-6.5.1/sip/QtDesigner/membersheet.sip
--rw-r--r--   0 phil       (501) staff       (20)     2084 2023-06-02 10:41:04.380368 PyQt6-6.5.1/sip/QtDesigner/propertysheet.sip
--rw-r--r--   0 phil       (501) staff       (20)     3397 2023-06-02 10:41:04.405523 PyQt6-6.5.1/sip/QtDesigner/qextensionmanager.sip
--rw-r--r--   0 phil       (501) staff       (20)     1228 2023-06-02 10:41:04.378412 PyQt6-6.5.1/sip/QtDesigner/qpydesignercontainerextension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1308 2023-06-02 10:41:04.379889 PyQt6-6.5.1/sip/QtDesigner/qpydesignercustomwidgetcollectionplugin.sip
--rw-r--r--   0 phil       (501) staff       (20)     1235 2023-06-02 10:41:04.407209 PyQt6-6.5.1/sip/QtDesigner/qpydesignercustomwidgetplugin.sip
--rw-r--r--   0 phil       (501) staff       (20)     1242 2023-06-02 10:41:04.414433 PyQt6-6.5.1/sip/QtDesigner/qpydesignermembersheetextension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1259 2023-06-02 10:41:04.410672 PyQt6-6.5.1/sip/QtDesigner/qpydesignerpropertysheetextension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1221 2023-06-02 10:41:04.408166 PyQt6-6.5.1/sip/QtDesigner/qpydesignertaskmenuextension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1300 2023-06-02 10:41:04.379340 PyQt6-6.5.1/sip/QtDesigner/taskmenu.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.935972 PyQt6-6.5.1/sip/QtGui/
--rw-r--r--   0 phil       (501) staff       (20)     4178 2023-06-02 10:41:04.608405 PyQt6-6.5.1/sip/QtGui/QtGuimod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1404 2023-06-02 10:41:04.605764 PyQt6-6.5.1/sip/QtGui/opengl_types.sip
--rw-r--r--   0 phil       (501) staff       (20)     1809 2023-06-02 10:41:04.514637 PyQt6-6.5.1/sip/QtGui/qabstractfileiconprovider.sip
--rw-r--r--   0 phil       (501) staff       (20)     3726 2023-06-02 10:41:04.510637 PyQt6-6.5.1/sip/QtGui/qabstracttextdocumentlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     4672 2023-06-02 10:41:04.571118 PyQt6-6.5.1/sip/QtGui/qaction.sip
--rw-r--r--   0 phil       (501) staff       (20)     1946 2023-06-02 10:41:04.516142 PyQt6-6.5.1/sip/QtGui/qactiongroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     1568 2023-06-02 10:41:04.611419 PyQt6-6.5.1/sip/QtGui/qbackingstore.sip
--rw-r--r--   0 phil       (501) staff       (20)     1848 2023-06-02 10:41:04.527847 PyQt6-6.5.1/sip/QtGui/qbitmap.sip
--rw-r--r--   0 phil       (501) staff       (20)    10739 2023-06-02 10:41:04.623499 PyQt6-6.5.1/sip/QtGui/qbrush.sip
--rw-r--r--   0 phil       (501) staff       (20)     3492 2023-06-02 10:41:04.624154 PyQt6-6.5.1/sip/QtGui/qclipboard.sip
--rw-r--r--   0 phil       (501) staff       (20)    12351 2023-06-02 10:41:04.561413 PyQt6-6.5.1/sip/QtGui/qcolor.sip
--rw-r--r--   0 phil       (501) staff       (20)     4476 2023-06-02 10:41:04.519780 PyQt6-6.5.1/sip/QtGui/qcolorspace.sip
--rw-r--r--   0 phil       (501) staff       (20)     1554 2023-06-02 10:41:04.533095 PyQt6-6.5.1/sip/QtGui/qcolortransform.sip
--rw-r--r--   0 phil       (501) staff       (20)     3042 2023-06-02 10:41:04.574224 PyQt6-6.5.1/sip/QtGui/qcursor.sip
--rw-r--r--   0 phil       (501) staff       (20)     2418 2023-06-02 10:41:04.613403 PyQt6-6.5.1/sip/QtGui/qdesktopservices.sip
--rw-r--r--   0 phil       (501) staff       (20)     1971 2023-06-02 10:41:04.619812 PyQt6-6.5.1/sip/QtGui/qdrag.sip
--rw-r--r--   0 phil       (501) staff       (20)    23127 2023-06-02 10:41:04.617406 PyQt6-6.5.1/sip/QtGui/qevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2495 2023-06-02 10:41:04.582306 PyQt6-6.5.1/sip/QtGui/qeventpoint.sip
--rw-r--r--   0 phil       (501) staff       (20)     4840 2023-06-02 10:41:04.536619 PyQt6-6.5.1/sip/QtGui/qfilesystemmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     5846 2023-06-02 10:41:04.518269 PyQt6-6.5.1/sip/QtGui/qfont.sip
--rw-r--r--   0 phil       (501) staff       (20)     3645 2023-06-02 10:41:04.519021 PyQt6-6.5.1/sip/QtGui/qfontdatabase.sip
--rw-r--r--   0 phil       (501) staff       (20)     1495 2023-06-02 10:41:04.522875 PyQt6-6.5.1/sip/QtGui/qfontinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     6681 2023-06-02 10:41:04.556109 PyQt6-6.5.1/sip/QtGui/qfontmetrics.sip
--rw-r--r--   0 phil       (501) staff       (20)    25528 2023-06-02 10:41:04.577911 PyQt6-6.5.1/sip/QtGui/qgenericmatrix.sip
--rw-r--r--   0 phil       (501) staff       (20)     2611 2023-06-02 10:41:04.582896 PyQt6-6.5.1/sip/QtGui/qglyphrun.sip
--rw-r--r--   0 phil       (501) staff       (20)     9603 2023-06-02 10:41:04.621103 PyQt6-6.5.1/sip/QtGui/qguiapplication.sip
--rw-r--r--   0 phil       (501) staff       (20)     4245 2023-06-02 10:41:04.581722 PyQt6-6.5.1/sip/QtGui/qicon.sip
--rw-r--r--   0 phil       (501) staff       (20)     2384 2023-06-02 10:41:04.520377 PyQt6-6.5.1/sip/QtGui/qiconengine.sip
--rw-r--r--   0 phil       (501) staff       (20)    13954 2023-06-02 10:41:04.526315 PyQt6-6.5.1/sip/QtGui/qimage.sip
--rw-r--r--   0 phil       (501) staff       (20)     2751 2023-06-02 10:41:04.566622 PyQt6-6.5.1/sip/QtGui/qimageiohandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     3480 2023-06-02 10:41:04.609109 PyQt6-6.5.1/sip/QtGui/qimagereader.sip
--rw-r--r--   0 phil       (501) staff       (20)     2666 2023-06-02 10:41:04.573667 PyQt6-6.5.1/sip/QtGui/qimagewriter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2591 2023-06-02 10:41:04.524534 PyQt6-6.5.1/sip/QtGui/qinputdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2303 2023-06-02 10:41:04.619305 PyQt6-6.5.1/sip/QtGui/qinputmethod.sip
--rw-r--r--   0 phil       (501) staff       (20)     7031 2023-06-02 10:41:04.584871 PyQt6-6.5.1/sip/QtGui/qkeysequence.sip
--rw-r--r--   0 phil       (501) staff       (20)     9803 2023-06-02 10:41:04.521988 PyQt6-6.5.1/sip/QtGui/qmatrix4x4.sip
--rw-r--r--   0 phil       (501) staff       (20)     2857 2023-06-02 10:41:04.618177 PyQt6-6.5.1/sip/QtGui/qmovie.sip
--rw-r--r--   0 phil       (501) staff       (20)     1585 2023-06-02 10:41:04.580893 PyQt6-6.5.1/sip/QtGui/qoffscreensurface.sip
--rw-r--r--   0 phil       (501) staff       (20)     2580 2023-06-02 10:41:04.529073 PyQt6-6.5.1/sip/QtGui/qopenglcontext.sip
--rw-r--r--   0 phil       (501) staff       (20)     1686 2023-06-02 10:41:04.522425 PyQt6-6.5.1/sip/QtGui/qpagedpaintdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3104 2023-06-02 10:41:04.532264 PyQt6-6.5.1/sip/QtGui/qpagelayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     2145 2023-06-02 10:41:04.569993 PyQt6-6.5.1/sip/QtGui/qpageranges.sip
--rw-r--r--   0 phil       (501) staff       (20)     5591 2023-06-02 10:41:04.566021 PyQt6-6.5.1/sip/QtGui/qpagesize.sip
--rw-r--r--   0 phil       (501) staff       (20)     1994 2023-06-02 10:41:04.556650 PyQt6-6.5.1/sip/QtGui/qpaintdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     1415 2023-06-02 10:41:04.607445 PyQt6-6.5.1/sip/QtGui/qpaintdevicewindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     5665 2023-06-02 10:41:04.610071 PyQt6-6.5.1/sip/QtGui/qpaintengine.sip
--rw-r--r--   0 phil       (501) staff       (20)    20805 2023-06-02 10:41:04.569005 PyQt6-6.5.1/sip/QtGui/qpainter.sip
--rw-r--r--   0 phil       (501) staff       (20)     6554 2023-06-02 10:41:04.578781 PyQt6-6.5.1/sip/QtGui/qpainterpath.sip
--rw-r--r--   0 phil       (501) staff       (20)     4511 2023-06-02 10:41:04.517049 PyQt6-6.5.1/sip/QtGui/qpalette.sip
--rw-r--r--   0 phil       (501) staff       (20)     1885 2023-06-02 10:41:04.563261 PyQt6-6.5.1/sip/QtGui/qpdfwriter.sip
--rw-r--r--   0 phil       (501) staff       (20)     3397 2023-06-02 10:41:04.515504 PyQt6-6.5.1/sip/QtGui/qpen.sip
--rw-r--r--   0 phil       (501) staff       (20)     2021 2023-06-02 10:41:04.586002 PyQt6-6.5.1/sip/QtGui/qpicture.sip
--rw-r--r--   0 phil       (501) staff       (20)     5520 2023-06-02 10:41:04.564926 PyQt6-6.5.1/sip/QtGui/qpixelformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     4917 2023-06-02 10:41:04.506241 PyQt6-6.5.1/sip/QtGui/qpixmap.sip
--rw-r--r--   0 phil       (501) staff       (20)     2240 2023-06-02 10:41:04.562074 PyQt6-6.5.1/sip/QtGui/qpixmapcache.sip
--rw-r--r--   0 phil       (501) staff       (20)     2499 2023-06-02 10:41:04.618760 PyQt6-6.5.1/sip/QtGui/qpointingdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)    11953 2023-06-02 10:41:04.531709 PyQt6-6.5.1/sip/QtGui/qpolygon.sip
--rw-r--r--   0 phil       (501) staff       (20)     2719 2023-06-02 10:41:04.562808 PyQt6-6.5.1/sip/QtGui/qpygui_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     5076 2023-06-02 10:41:04.529754 PyQt6-6.5.1/sip/QtGui/qquaternion.sip
--rw-r--r--   0 phil       (501) staff       (20)     1230 2023-06-02 10:41:04.579225 PyQt6-6.5.1/sip/QtGui/qrasterwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     3616 2023-06-02 10:41:04.528482 PyQt6-6.5.1/sip/QtGui/qrawfont.sip
--rw-r--r--   0 phil       (501) staff       (20)     3768 2023-06-02 10:41:04.583616 PyQt6-6.5.1/sip/QtGui/qregion.sip
--rw-r--r--   0 phil       (501) staff       (20)     1271 2023-06-02 10:41:04.479067 PyQt6-6.5.1/sip/QtGui/qrgb.sip
--rw-r--r--   0 phil       (501) staff       (20)     2141 2023-06-02 10:41:04.612851 PyQt6-6.5.1/sip/QtGui/qrgba64.sip
--rw-r--r--   0 phil       (501) staff       (20)     3073 2023-06-02 10:41:04.526906 PyQt6-6.5.1/sip/QtGui/qscreen.sip
--rw-r--r--   0 phil       (501) staff       (20)     1990 2023-06-02 10:41:04.607016 PyQt6-6.5.1/sip/QtGui/qsessionmanager.sip
--rw-r--r--   0 phil       (501) staff       (20)     6080 2023-06-02 10:41:04.610988 PyQt6-6.5.1/sip/QtGui/qshortcut.sip
--rw-r--r--   0 phil       (501) staff       (20)     9704 2023-06-02 10:41:04.557712 PyQt6-6.5.1/sip/QtGui/qstandarditemmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1953 2023-06-02 10:41:04.532695 PyQt6-6.5.1/sip/QtGui/qstatictext.sip
--rw-r--r--   0 phil       (501) staff       (20)     3060 2023-06-02 10:41:04.612269 PyQt6-6.5.1/sip/QtGui/qstylehints.sip
--rw-r--r--   0 phil       (501) staff       (20)     1634 2023-06-02 10:41:04.527395 PyQt6-6.5.1/sip/QtGui/qsurface.sip
--rw-r--r--   0 phil       (501) staff       (20)     3651 2023-06-02 10:41:04.513999 PyQt6-6.5.1/sip/QtGui/qsurfaceformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     2965 2023-06-02 10:41:04.509788 PyQt6-6.5.1/sip/QtGui/qsyntaxhighlighter.sip
--rw-r--r--   0 phil       (501) staff       (20)     5531 2023-06-02 10:41:04.572427 PyQt6-6.5.1/sip/QtGui/qtextcursor.sip
--rw-r--r--   0 phil       (501) staff       (20)    12118 2023-06-02 10:41:04.559636 PyQt6-6.5.1/sip/QtGui/qtextdocument.sip
--rw-r--r--   0 phil       (501) staff       (20)     1935 2023-06-02 10:41:04.507037 PyQt6-6.5.1/sip/QtGui/qtextdocumentfragment.sip
--rw-r--r--   0 phil       (501) staff       (20)     1714 2023-06-02 10:41:04.613830 PyQt6-6.5.1/sip/QtGui/qtextdocumentwriter.sip
--rw-r--r--   0 phil       (501) staff       (20)    19535 2023-06-02 10:41:04.535921 PyQt6-6.5.1/sip/QtGui/qtextformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     5890 2023-06-02 10:41:04.508993 PyQt6-6.5.1/sip/QtGui/qtextlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     1462 2023-06-02 10:41:04.507592 PyQt6-6.5.1/sip/QtGui/qtextlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     7691 2023-06-02 10:41:04.512468 PyQt6-6.5.1/sip/QtGui/qtextobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2786 2023-06-02 10:41:04.606453 PyQt6-6.5.1/sip/QtGui/qtextoption.sip
--rw-r--r--   0 phil       (501) staff       (20)     2569 2023-06-02 10:41:04.621657 PyQt6-6.5.1/sip/QtGui/qtexttable.sip
--rw-r--r--   0 phil       (501) staff       (20)     5139 2023-06-02 10:41:04.564029 PyQt6-6.5.1/sip/QtGui/qtransform.sip
--rw-r--r--   0 phil       (501) staff       (20)     2042 2023-06-02 10:41:04.513094 PyQt6-6.5.1/sip/QtGui/qundogroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     3004 2023-06-02 10:41:04.573012 PyQt6-6.5.1/sip/QtGui/qundostack.sip
--rw-r--r--   0 phil       (501) staff       (20)     1692 2023-06-02 10:41:04.571587 PyQt6-6.5.1/sip/QtGui/qutimimeconverter.sip
--rw-r--r--   0 phil       (501) staff       (20)     3361 2023-06-02 10:41:04.585558 PyQt6-6.5.1/sip/QtGui/qvalidator.sip
--rw-r--r--   0 phil       (501) staff       (20)     9152 2023-06-02 10:41:04.580474 PyQt6-6.5.1/sip/QtGui/qvectornd.sip
--rw-r--r--   0 phil       (501) staff       (20)     7236 2023-06-02 10:41:04.523945 PyQt6-6.5.1/sip/QtGui/qwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     1009 2023-06-02 10:41:04.569472 PyQt6-6.5.1/sip/QtGui/qwindowdefs.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.886661 PyQt6-6.5.1/sip/QtHelp/
--rw-r--r--   0 phil       (501) staff       (20)     2347 2023-06-02 10:41:04.421274 PyQt6-6.5.1/sip/QtHelp/QtHelpmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1429 2023-06-02 10:41:04.418299 PyQt6-6.5.1/sip/QtHelp/qcompressedhelpinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     2348 2023-06-02 10:41:04.420387 PyQt6-6.5.1/sip/QtHelp/qhelpcontentwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1361 2023-06-02 10:41:04.420839 PyQt6-6.5.1/sip/QtHelp/qhelpengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     4184 2023-06-02 10:41:04.419830 PyQt6-6.5.1/sip/QtHelp/qhelpenginecore.sip
--rw-r--r--   0 phil       (501) staff       (20)     1430 2023-06-02 10:41:04.419112 PyQt6-6.5.1/sip/QtHelp/qhelpfilterdata.sip
--rw-r--r--   0 phil       (501) staff       (20)     1889 2023-06-02 10:41:04.424016 PyQt6-6.5.1/sip/QtHelp/qhelpfilterengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     1457 2023-06-02 10:41:04.423563 PyQt6-6.5.1/sip/QtHelp/qhelpfiltersettingswidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1836 2023-06-02 10:41:04.421750 PyQt6-6.5.1/sip/QtHelp/qhelpindexwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1048 2023-06-02 10:41:04.423170 PyQt6-6.5.1/sip/QtHelp/qhelplink.sip
--rw-r--r--   0 phil       (501) staff       (20)     2399 2023-06-02 10:41:04.422348 PyQt6-6.5.1/sip/QtHelp/qhelpsearchengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     1552 2023-06-02 10:41:04.422792 PyQt6-6.5.1/sip/QtHelp/qhelpsearchquerywidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1222 2023-06-02 10:41:04.418702 PyQt6-6.5.1/sip/QtHelp/qhelpsearchresultwidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.009419 PyQt6-6.5.1/sip/QtMultimedia/
--rw-r--r--   0 phil       (501) staff       (20)     2656 2023-06-02 10:41:04.878588 PyQt6-6.5.1/sip/QtMultimedia/QtMultimediamod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1516 2023-06-02 10:41:04.909668 PyQt6-6.5.1/sip/QtMultimedia/qaudio.sip
--rw-r--r--   0 phil       (501) staff       (20)     1993 2023-06-02 10:41:04.875377 PyQt6-6.5.1/sip/QtMultimedia/qaudiobuffer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2206 2023-06-02 10:41:04.913500 PyQt6-6.5.1/sip/QtMultimedia/qaudiodecoder.sip
--rw-r--r--   0 phil       (501) staff       (20)     1930 2023-06-02 10:41:04.874481 PyQt6-6.5.1/sip/QtMultimedia/qaudiodevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3341 2023-06-02 10:41:04.879374 PyQt6-6.5.1/sip/QtMultimedia/qaudioformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     1565 2023-06-02 10:41:04.911151 PyQt6-6.5.1/sip/QtMultimedia/qaudioinput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1567 2023-06-02 10:41:04.874917 PyQt6-6.5.1/sip/QtMultimedia/qaudiooutput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1838 2023-06-02 10:41:04.876748 PyQt6-6.5.1/sip/QtMultimedia/qaudiosink.sip
--rw-r--r--   0 phil       (501) staff       (20)     1862 2023-06-02 10:41:04.910146 PyQt6-6.5.1/sip/QtMultimedia/qaudiosource.sip
--rw-r--r--   0 phil       (501) staff       (20)     7429 2023-06-02 10:41:04.880457 PyQt6-6.5.1/sip/QtMultimedia/qcamera.sip
--rw-r--r--   0 phil       (501) staff       (20)     2093 2023-06-02 10:41:04.906250 PyQt6-6.5.1/sip/QtMultimedia/qcameradevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3030 2023-06-02 10:41:04.876148 PyQt6-6.5.1/sip/QtMultimedia/qimagecapture.sip
--rw-r--r--   0 phil       (501) staff       (20)     2160 2023-06-02 10:41:04.917043 PyQt6-6.5.1/sip/QtMultimedia/qmediacapturesession.sip
--rw-r--r--   0 phil       (501) staff       (20)     1540 2023-06-02 10:41:04.915485 PyQt6-6.5.1/sip/QtMultimedia/qmediadevices.sip
--rw-r--r--   0 phil       (501) staff       (20)     3349 2023-06-02 10:41:04.914839 PyQt6-6.5.1/sip/QtMultimedia/qmediaformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     2186 2023-06-02 10:41:04.906875 PyQt6-6.5.1/sip/QtMultimedia/qmediametadata.sip
--rw-r--r--   0 phil       (501) staff       (20)     4095 2023-06-02 10:41:04.912742 PyQt6-6.5.1/sip/QtMultimedia/qmediaplayer.sip
--rw-r--r--   0 phil       (501) staff       (20)     3680 2023-06-02 10:41:04.877418 PyQt6-6.5.1/sip/QtMultimedia/qmediarecorder.sip
--rw-r--r--   0 phil       (501) staff       (20)     3046 2023-06-02 10:41:04.905548 PyQt6-6.5.1/sip/QtMultimedia/qmediatimerange.sip
--rw-r--r--   0 phil       (501) staff       (20)    10957 2023-06-02 10:41:04.909167 PyQt6-6.5.1/sip/QtMultimedia/qpymultimedia_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1795 2023-06-02 10:41:04.911675 PyQt6-6.5.1/sip/QtMultimedia/qscreencapture.sip
--rw-r--r--   0 phil       (501) staff       (20)     2198 2023-06-02 10:41:04.910705 PyQt6-6.5.1/sip/QtMultimedia/qsoundeffect.sip
--rw-r--r--   0 phil       (501) staff       (20)     3181 2023-06-02 10:41:04.878090 PyQt6-6.5.1/sip/QtMultimedia/qvideoframe.sip
--rw-r--r--   0 phil       (501) staff       (20)     4710 2023-06-02 10:41:04.916444 PyQt6-6.5.1/sip/QtMultimedia/qvideoframeformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     1508 2023-06-02 10:41:04.914055 PyQt6-6.5.1/sip/QtMultimedia/qvideosink.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.067187 PyQt6-6.5.1/sip/QtMultimediaWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2083 2023-06-02 10:41:05.157804 PyQt6-6.5.1/sip/QtMultimediaWidgets/QtMultimediaWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2007 2023-06-02 10:41:05.158886 PyQt6-6.5.1/sip/QtMultimediaWidgets/qgraphicsvideoitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2399 2023-06-02 10:41:05.158396 PyQt6-6.5.1/sip/QtMultimediaWidgets/qvideowidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.872435 PyQt6-6.5.1/sip/QtNetwork/
--rw-r--r--   0 phil       (501) staff       (20)     3123 2023-06-02 10:41:04.327320 PyQt6-6.5.1/sip/QtNetwork/QtNetworkmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2995 2023-06-02 10:41:04.363999 PyQt6-6.5.1/sip/QtNetwork/qabstractnetworkcache.sip
--rw-r--r--   0 phil       (501) staff       (20)    10970 2023-06-02 10:41:04.365966 PyQt6-6.5.1/sip/QtNetwork/qabstractsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     1584 2023-06-02 10:41:04.362838 PyQt6-6.5.1/sip/QtNetwork/qauthenticator.sip
--rw-r--r--   0 phil       (501) staff       (20)     4595 2023-06-02 10:41:04.328155 PyQt6-6.5.1/sip/QtNetwork/qdnslookup.sip
--rw-r--r--   0 phil       (501) staff       (20)     5644 2023-06-02 10:41:04.355716 PyQt6-6.5.1/sip/QtNetwork/qhostaddress.sip
--rw-r--r--   0 phil       (501) staff       (20)     2987 2023-06-02 10:41:04.356869 PyQt6-6.5.1/sip/QtNetwork/qhostinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1906 2023-06-02 10:41:04.372476 PyQt6-6.5.1/sip/QtNetwork/qhstspolicy.sip
--rw-r--r--   0 phil       (501) staff       (20)     1632 2023-06-02 10:41:04.357327 PyQt6-6.5.1/sip/QtNetwork/qhttp1configuration.sip
--rw-r--r--   0 phil       (501) staff       (20)     1863 2023-06-02 10:41:04.369088 PyQt6-6.5.1/sip/QtNetwork/qhttp2configuration.sip
--rw-r--r--   0 phil       (501) staff       (20)     2111 2023-06-02 10:41:04.376358 PyQt6-6.5.1/sip/QtNetwork/qhttpmultipart.sip
--rw-r--r--   0 phil       (501) staff       (20)     2417 2023-06-02 10:41:04.356284 PyQt6-6.5.1/sip/QtNetwork/qlocalserver.sip
--rw-r--r--   0 phil       (501) staff       (20)     6739 2023-06-02 10:41:04.367306 PyQt6-6.5.1/sip/QtNetwork/qlocalsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     4835 2023-06-02 10:41:04.360396 PyQt6-6.5.1/sip/QtNetwork/qnetworkaccessmanager.sip
--rw-r--r--   0 phil       (501) staff       (20)     2540 2023-06-02 10:41:04.326818 PyQt6-6.5.1/sip/QtNetwork/qnetworkcookie.sip
--rw-r--r--   0 phil       (501) staff       (20)     1719 2023-06-02 10:41:04.375830 PyQt6-6.5.1/sip/QtNetwork/qnetworkcookiejar.sip
--rw-r--r--   0 phil       (501) staff       (20)     1941 2023-06-02 10:41:04.324095 PyQt6-6.5.1/sip/QtNetwork/qnetworkdatagram.sip
--rw-r--r--   0 phil       (501) staff       (20)     1881 2023-06-02 10:41:04.363436 PyQt6-6.5.1/sip/QtNetwork/qnetworkdiskcache.sip
--rw-r--r--   0 phil       (501) staff       (20)     2950 2023-06-02 10:41:04.359725 PyQt6-6.5.1/sip/QtNetwork/qnetworkinformation.sip
--rw-r--r--   0 phil       (501) staff       (20)     3720 2023-06-02 10:41:04.358511 PyQt6-6.5.1/sip/QtNetwork/qnetworkinterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     5091 2023-06-02 10:41:04.377262 PyQt6-6.5.1/sip/QtNetwork/qnetworkproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     5728 2023-06-02 10:41:04.329012 PyQt6-6.5.1/sip/QtNetwork/qnetworkreply.sip
--rw-r--r--   0 phil       (501) staff       (20)     5117 2023-06-02 10:41:04.370069 PyQt6-6.5.1/sip/QtNetwork/qnetworkrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2020 2023-06-02 10:41:04.374667 PyQt6-6.5.1/sip/QtNetwork/qocspresponse.sip
--rw-r--r--   0 phil       (501) staff       (20)     1379 2023-06-02 10:41:04.329465 PyQt6-6.5.1/sip/QtNetwork/qpassworddigestor.sip
--rw-r--r--   0 phil       (501) staff       (20)     3458 2023-06-02 10:41:04.375411 PyQt6-6.5.1/sip/QtNetwork/qpynetwork_qhash.sip
--rw-r--r--   0 phil       (501) staff       (20)     7009 2023-06-02 10:41:04.372062 PyQt6-6.5.1/sip/QtNetwork/qpynetwork_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     4985 2023-06-02 10:41:04.361493 PyQt6-6.5.1/sip/QtNetwork/qpynetwork_qmap.sip
--rw-r--r--   0 phil       (501) staff       (20)     3643 2023-06-02 10:41:04.368198 PyQt6-6.5.1/sip/QtNetwork/qssl.sip
--rw-r--r--   0 phil       (501) staff       (20)     3763 2023-06-02 10:41:04.377912 PyQt6-6.5.1/sip/QtNetwork/qsslcertificate.sip
--rw-r--r--   0 phil       (501) staff       (20)     1426 2023-06-02 10:41:04.368671 PyQt6-6.5.1/sip/QtNetwork/qsslcertificateextension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1694 2023-06-02 10:41:04.357801 PyQt6-6.5.1/sip/QtNetwork/qsslcipher.sip
--rw-r--r--   0 phil       (501) staff       (20)     5201 2023-06-02 10:41:04.326167 PyQt6-6.5.1/sip/QtNetwork/qsslconfiguration.sip
--rw-r--r--   0 phil       (501) staff       (20)     2171 2023-06-02 10:41:04.359010 PyQt6-6.5.1/sip/QtNetwork/qssldiffiehellmanparameters.sip
--rw-r--r--   0 phil       (501) staff       (20)     1594 2023-06-02 10:41:04.362394 PyQt6-6.5.1/sip/QtNetwork/qsslellipticcurve.sip
--rw-r--r--   0 phil       (501) staff       (20)     2803 2023-06-02 10:41:04.364553 PyQt6-6.5.1/sip/QtNetwork/qsslerror.sip
--rw-r--r--   0 phil       (501) staff       (20)     2021 2023-06-02 10:41:04.361943 PyQt6-6.5.1/sip/QtNetwork/qsslkey.sip
--rw-r--r--   0 phil       (501) staff       (20)     1883 2023-06-02 10:41:04.325362 PyQt6-6.5.1/sip/QtNetwork/qsslpresharedkeyauthenticator.sip
--rw-r--r--   0 phil       (501) staff       (20)     2150 2023-06-02 10:41:04.324942 PyQt6-6.5.1/sip/QtNetwork/qsslserver.sip
--rw-r--r--   0 phil       (501) staff       (20)     8621 2023-06-02 10:41:04.373573 PyQt6-6.5.1/sip/QtNetwork/qsslsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     2339 2023-06-02 10:41:04.370559 PyQt6-6.5.1/sip/QtNetwork/qtcpserver.sip
--rw-r--r--   0 phil       (501) staff       (20)     1134 2023-06-02 10:41:04.324458 PyQt6-6.5.1/sip/QtNetwork/qtcpsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     3235 2023-06-02 10:41:04.374141 PyQt6-6.5.1/sip/QtNetwork/qudpsocket.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.939062 PyQt6-6.5.1/sip/QtNfc/
--rw-r--r--   0 phil       (501) staff       (20)     2146 2023-06-02 10:41:04.626981 PyQt6-6.5.1/sip/QtNfc/QtNfcmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1772 2023-06-02 10:41:04.629142 PyQt6-6.5.1/sip/QtNfc/qndeffilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2185 2023-06-02 10:41:04.627507 PyQt6-6.5.1/sip/QtNfc/qndefmessage.sip
--rw-r--r--   0 phil       (501) staff       (20)     3351 2023-06-02 10:41:04.626562 PyQt6-6.5.1/sip/QtNfc/qndefnfcsmartposterrecord.sip
--rw-r--r--   0 phil       (501) staff       (20)     1471 2023-06-02 10:41:04.627956 PyQt6-6.5.1/sip/QtNfc/qndefnfctextrecord.sip
--rw-r--r--   0 phil       (501) staff       (20)     1213 2023-06-02 10:41:04.625937 PyQt6-6.5.1/sip/QtNfc/qndefnfcurirecord.sip
--rw-r--r--   0 phil       (501) staff       (20)     2536 2023-06-02 10:41:04.624856 PyQt6-6.5.1/sip/QtNfc/qndefrecord.sip
--rw-r--r--   0 phil       (501) staff       (20)     3014 2023-06-02 10:41:04.625521 PyQt6-6.5.1/sip/QtNfc/qnearfieldmanager.sip
--rw-r--r--   0 phil       (501) staff       (20)     3250 2023-06-02 10:41:04.628644 PyQt6-6.5.1/sip/QtNfc/qnearfieldtarget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.840068 PyQt6-6.5.1/sip/QtOpenGL/
--rw-r--r--   0 phil       (501) staff       (20)     2618 2023-06-02 10:41:04.257114 PyQt6-6.5.1/sip/QtOpenGL/QtOpenGLmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2645 2023-06-02 10:41:04.256679 PyQt6-6.5.1/sip/QtOpenGL/qopenglbuffer.sip
--rw-r--r--   0 phil       (501) staff       (20)     5913 2023-06-02 10:41:04.256100 PyQt6-6.5.1/sip/QtOpenGL/qopengldebug.sip
--rw-r--r--   0 phil       (501) staff       (20)     5082 2023-06-02 10:41:04.232269 PyQt6-6.5.1/sip/QtOpenGL/qopenglframebufferobject.sip
--rw-r--r--   0 phil       (501) staff       (20)   111265 2023-06-02 10:41:04.243233 PyQt6-6.5.1/sip/QtOpenGL/qopenglfunctions_2_0.sip
--rw-r--r--   0 phil       (501) staff       (20)   111310 2023-06-02 10:41:04.254477 PyQt6-6.5.1/sip/QtOpenGL/qopenglfunctions_2_1.sip
--rw-r--r--   0 phil       (501) staff       (20)    42567 2023-06-02 10:41:04.227483 PyQt6-6.5.1/sip/QtOpenGL/qopenglfunctions_4_1_core.sip
--rw-r--r--   0 phil       (501) staff       (20)    28956 2023-06-02 10:41:04.261155 PyQt6-6.5.1/sip/QtOpenGL/qopenglfunctions_es2.sip
--rw-r--r--   0 phil       (501) staff       (20)     1751 2023-06-02 10:41:04.231536 PyQt6-6.5.1/sip/QtOpenGL/qopenglpaintdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     1865 2023-06-02 10:41:04.261709 PyQt6-6.5.1/sip/QtOpenGL/qopenglpixeltransferoptions.sip
--rw-r--r--   0 phil       (501) staff       (20)    15899 2023-06-02 10:41:04.264325 PyQt6-6.5.1/sip/QtOpenGL/qopenglshaderprogram.sip
--rw-r--r--   0 phil       (501) staff       (20)    14995 2023-06-02 10:41:04.231017 PyQt6-6.5.1/sip/QtOpenGL/qopengltexture.sip
--rw-r--r--   0 phil       (501) staff       (20)     2010 2023-06-02 10:41:04.262832 PyQt6-6.5.1/sip/QtOpenGL/qopengltextureblitter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2095 2023-06-02 10:41:04.228505 PyQt6-6.5.1/sip/QtOpenGL/qopengltimerquery.sip
--rw-r--r--   0 phil       (501) staff       (20)     1168 2023-06-02 10:41:04.228894 PyQt6-6.5.1/sip/QtOpenGL/qopenglversionfunctions.sip
--rw-r--r--   0 phil       (501) staff       (20)     1350 2023-06-02 10:41:04.227952 PyQt6-6.5.1/sip/QtOpenGL/qopenglversionfunctionsfactory.sip
--rw-r--r--   0 phil       (501) staff       (20)     1814 2023-06-02 10:41:04.262188 PyQt6-6.5.1/sip/QtOpenGL/qopenglversionprofile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1909 2023-06-02 10:41:04.264832 PyQt6-6.5.1/sip/QtOpenGL/qopenglvertexarrayobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2173 2023-06-02 10:41:04.255237 PyQt6-6.5.1/sip/QtOpenGL/qopenglwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     2926 2023-06-02 10:41:04.222643 PyQt6-6.5.1/sip/QtOpenGL/qpyopengl_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     3170 2023-06-02 10:41:04.258005 PyQt6-6.5.1/sip/QtOpenGL/qpyopengl_std_pair.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.903685 PyQt6-6.5.1/sip/QtOpenGLWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2059 2023-06-02 10:41:04.477850 PyQt6-6.5.1/sip/QtOpenGLWidgets/QtOpenGLWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3230 2023-06-02 10:41:04.478551 PyQt6-6.5.1/sip/QtOpenGLWidgets/qopenglwidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.902926 PyQt6-6.5.1/sip/QtPdf/
--rw-r--r--   0 phil       (501) staff       (20)     2169 2023-06-02 10:41:04.473343 PyQt6-6.5.1/sip/QtPdf/QtPdfmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1876 2023-06-02 10:41:04.475772 PyQt6-6.5.1/sip/QtPdf/qpdfbookmarkmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     3512 2023-06-02 10:41:04.474903 PyQt6-6.5.1/sip/QtPdf/qpdfdocument.sip
--rw-r--r--   0 phil       (501) staff       (20)     2081 2023-06-02 10:41:04.476233 PyQt6-6.5.1/sip/QtPdf/qpdfdocumentrenderoptions.sip
--rw-r--r--   0 phil       (501) staff       (20)     1460 2023-06-02 10:41:04.473734 PyQt6-6.5.1/sip/QtPdf/qpdflink.sip
--rw-r--r--   0 phil       (501) staff       (20)     1827 2023-06-02 10:41:04.475338 PyQt6-6.5.1/sip/QtPdf/qpdfpagenavigator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1681 2023-06-02 10:41:04.474137 PyQt6-6.5.1/sip/QtPdf/qpdfpagerenderer.sip
--rw-r--r--   0 phil       (501) staff       (20)     1900 2023-06-02 10:41:04.476845 PyQt6-6.5.1/sip/QtPdf/qpdfsearchmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1430 2023-06-02 10:41:04.477293 PyQt6-6.5.1/sip/QtPdf/qpdfselection.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.069956 PyQt6-6.5.1/sip/QtPdfWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2012 2023-06-02 10:41:05.162318 PyQt6-6.5.1/sip/QtPdfWidgets/QtPdfWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2848 2023-06-02 10:41:05.162953 PyQt6-6.5.1/sip/QtPdfWidgets/qpdfview.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.017765 PyQt6-6.5.1/sip/QtPositioning/
--rw-r--r--   0 phil       (501) staff       (20)     2365 2023-06-02 10:41:04.921527 PyQt6-6.5.1/sip/QtPositioning/QtPositioningmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2273 2023-06-02 10:41:04.956358 PyQt6-6.5.1/sip/QtPositioning/qgeoaddress.sip
--rw-r--r--   0 phil       (501) staff       (20)     2226 2023-06-02 10:41:04.928896 PyQt6-6.5.1/sip/QtPositioning/qgeoareamonitorinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     3002 2023-06-02 10:41:04.927129 PyQt6-6.5.1/sip/QtPositioning/qgeoareamonitorsource.sip
--rw-r--r--   0 phil       (501) staff       (20)     1857 2023-06-02 10:41:04.925718 PyQt6-6.5.1/sip/QtPositioning/qgeocircle.sip
--rw-r--r--   0 phil       (501) staff       (20)     2775 2023-06-02 10:41:04.957058 PyQt6-6.5.1/sip/QtPositioning/qgeocoordinate.sip
--rw-r--r--   0 phil       (501) staff       (20)     1850 2023-06-02 10:41:04.929363 PyQt6-6.5.1/sip/QtPositioning/qgeolocation.sip
--rw-r--r--   0 phil       (501) staff       (20)     2370 2023-06-02 10:41:04.927678 PyQt6-6.5.1/sip/QtPositioning/qgeopath.sip
--rw-r--r--   0 phil       (501) staff       (20)     2601 2023-06-02 10:41:04.928308 PyQt6-6.5.1/sip/QtPositioning/qgeopolygon.sip
--rw-r--r--   0 phil       (501) staff       (20)     2502 2023-06-02 10:41:04.921122 PyQt6-6.5.1/sip/QtPositioning/qgeopositioninfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     4135 2023-06-02 10:41:04.926478 PyQt6-6.5.1/sip/QtPositioning/qgeopositioninfosource.sip
--rw-r--r--   0 phil       (501) staff       (20)     2832 2023-06-02 10:41:04.922669 PyQt6-6.5.1/sip/QtPositioning/qgeorectangle.sip
--rw-r--r--   0 phil       (501) staff       (20)     2343 2023-06-02 10:41:04.924527 PyQt6-6.5.1/sip/QtPositioning/qgeosatelliteinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     2640 2023-06-02 10:41:04.955595 PyQt6-6.5.1/sip/QtPositioning/qgeosatelliteinfosource.sip
--rw-r--r--   0 phil       (501) staff       (20)     2434 2023-06-02 10:41:04.925201 PyQt6-6.5.1/sip/QtPositioning/qgeoshape.sip
--rw-r--r--   0 phil       (501) staff       (20)     2205 2023-06-02 10:41:04.923508 PyQt6-6.5.1/sip/QtPositioning/qnmeapositioninfosource.sip
--rw-r--r--   0 phil       (501) staff       (20)     2448 2023-06-02 10:41:04.922074 PyQt6-6.5.1/sip/QtPositioning/qnmeasatelliteinfosource.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.832900 PyQt6-6.5.1/sip/QtPrintSupport/
--rw-r--r--   0 phil       (501) staff       (20)     2261 2023-06-02 10:41:04.216838 PyQt6-6.5.1/sip/QtPrintSupport/QtPrintSupportmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3959 2023-06-02 10:41:04.216342 PyQt6-6.5.1/sip/QtPrintSupport/qabstractprintdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2569 2023-06-02 10:41:04.219424 PyQt6-6.5.1/sip/QtPrintSupport/qpagesetupdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2959 2023-06-02 10:41:04.214904 PyQt6-6.5.1/sip/QtPrintSupport/qprintdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2327 2023-06-02 10:41:04.220630 PyQt6-6.5.1/sip/QtPrintSupport/qprintengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     4672 2023-06-02 10:41:04.221678 PyQt6-6.5.1/sip/QtPrintSupport/qprinter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2194 2023-06-02 10:41:04.220004 PyQt6-6.5.1/sip/QtPrintSupport/qprinterinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     2034 2023-06-02 10:41:04.215462 PyQt6-6.5.1/sip/QtPrintSupport/qprintpreviewdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2558 2023-06-02 10:41:04.217501 PyQt6-6.5.1/sip/QtPrintSupport/qprintpreviewwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     4887 2023-06-02 10:41:04.218840 PyQt6-6.5.1/sip/QtPrintSupport/qpyprintsupport_qlist.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.848935 PyQt6-6.5.1/sip/QtQml/
--rw-r--r--   0 phil       (501) staff       (20)     2708 2023-06-02 10:41:04.271902 PyQt6-6.5.1/sip/QtQml/QtQmlmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     6133 2023-06-02 10:41:04.272859 PyQt6-6.5.1/sip/QtQml/qjsengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     3449 2023-06-02 10:41:04.276957 PyQt6-6.5.1/sip/QtQml/qjsmanagedvalue.sip
--rw-r--r--   0 phil       (501) staff       (20)     3260 2023-06-02 10:41:04.267404 PyQt6-6.5.1/sip/QtQml/qjsprimitivevalue.sip
--rw-r--r--   0 phil       (501) staff       (20)     3624 2023-06-02 10:41:04.270970 PyQt6-6.5.1/sip/QtQml/qjsvalue.sip
--rw-r--r--   0 phil       (501) staff       (20)     1267 2023-06-02 10:41:04.266710 PyQt6-6.5.1/sip/QtQml/qjsvalueiterator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1412 2023-06-02 10:41:04.266270 PyQt6-6.5.1/sip/QtQml/qmlattachedpropertiesobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2851 2023-06-02 10:41:04.275944 PyQt6-6.5.1/sip/QtQml/qmlregistertype.sip
--rw-r--r--   0 phil       (501) staff       (20)     1413 2023-06-02 10:41:04.273878 PyQt6-6.5.1/sip/QtQml/qpyqmllistproperty.sip
--rw-r--r--   0 phil       (501) staff       (20)     1852 2023-06-02 10:41:04.279197 PyQt6-6.5.1/sip/QtQml/qqml.sip
--rw-r--r--   0 phil       (501) staff       (20)     1354 2023-06-02 10:41:04.274702 PyQt6-6.5.1/sip/QtQml/qqmlabstracturlinterceptor.sip
--rw-r--r--   0 phil       (501) staff       (20)     2102 2023-06-02 10:41:04.270020 PyQt6-6.5.1/sip/QtQml/qqmlapplicationengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     3497 2023-06-02 10:41:04.269375 PyQt6-6.5.1/sip/QtQml/qqmlcomponent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2006 2023-06-02 10:41:04.278828 PyQt6-6.5.1/sip/QtQml/qqmlcontext.sip
--rw-r--r--   0 phil       (501) staff       (20)     5776 2023-06-02 10:41:04.305837 PyQt6-6.5.1/sip/QtQml/qqmlengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     1624 2023-06-02 10:41:04.306299 PyQt6-6.5.1/sip/QtQml/qqmlerror.sip
--rw-r--r--   0 phil       (501) staff       (20)     1925 2023-06-02 10:41:04.277887 PyQt6-6.5.1/sip/QtQml/qqmlexpression.sip
--rw-r--r--   0 phil       (501) staff       (20)     1583 2023-06-02 10:41:04.274300 PyQt6-6.5.1/sip/QtQml/qqmlextensionplugin.sip
--rw-r--r--   0 phil       (501) staff       (20)     1303 2023-06-02 10:41:04.268690 PyQt6-6.5.1/sip/QtQml/qqmlfileselector.sip
--rw-r--r--   0 phil       (501) staff       (20)     2332 2023-06-02 10:41:04.268208 PyQt6-6.5.1/sip/QtQml/qqmlincubator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1898 2023-06-02 10:41:04.273297 PyQt6-6.5.1/sip/QtQml/qqmllist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1199 2023-06-02 10:41:04.276354 PyQt6-6.5.1/sip/QtQml/qqmlnetworkaccessmanagerfactory.sip
--rw-r--r--   0 phil       (501) staff       (20)     1235 2023-06-02 10:41:04.277338 PyQt6-6.5.1/sip/QtQml/qqmlparserstatus.sip
--rw-r--r--   0 phil       (501) staff       (20)     4182 2023-06-02 10:41:04.265830 PyQt6-6.5.1/sip/QtQml/qqmlproperty.sip
--rw-r--r--   0 phil       (501) staff       (20)     1769 2023-06-02 10:41:04.271442 PyQt6-6.5.1/sip/QtQml/qqmlpropertymap.sip
--rw-r--r--   0 phil       (501) staff       (20)     1254 2023-06-02 10:41:04.278247 PyQt6-6.5.1/sip/QtQml/qqmlpropertyvaluesource.sip
--rw-r--r--   0 phil       (501) staff       (20)     1457 2023-06-02 10:41:04.275169 PyQt6-6.5.1/sip/QtQml/qqmlscriptstring.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.950190 PyQt6-6.5.1/sip/QtQuick/
--rw-r--r--   0 phil       (501) staff       (20)     2852 2023-06-02 10:41:04.663937 PyQt6-6.5.1/sip/QtQuick/QtQuickmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2548 2023-06-02 10:41:04.660536 PyQt6-6.5.1/sip/QtQuick/qquickframebufferobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2308 2023-06-02 10:41:04.670772 PyQt6-6.5.1/sip/QtQuick/qquickgraphicsconfiguration.sip
--rw-r--r--   0 phil       (501) staff       (20)     1298 2023-06-02 10:41:04.631840 PyQt6-6.5.1/sip/QtQuick/qquickgraphicsdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2820 2023-06-02 10:41:04.669163 PyQt6-6.5.1/sip/QtQuick/qquickimageprovider.sip
--rw-r--r--   0 phil       (501) staff       (20)    10164 2023-06-02 10:41:04.674006 PyQt6-6.5.1/sip/QtQuick/qquickitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     1368 2023-06-02 10:41:04.672634 PyQt6-6.5.1/sip/QtQuick/qquickitemgrabresult.sip
--rw-r--r--   0 phil       (501) staff       (20)     2983 2023-06-02 10:41:04.657525 PyQt6-6.5.1/sip/QtQuick/qquickpainteditem.sip
--rw-r--r--   0 phil       (501) staff       (20)     1662 2023-06-02 10:41:04.663220 PyQt6-6.5.1/sip/QtQuick/qquickrendercontrol.sip
--rw-r--r--   0 phil       (501) staff       (20)     2100 2023-06-02 10:41:04.656957 PyQt6-6.5.1/sip/QtQuick/qquickrendertarget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1160 2023-06-02 10:41:04.666501 PyQt6-6.5.1/sip/QtQuick/qquicktextdocument.sip
--rw-r--r--   0 phil       (501) staff       (20)     2345 2023-06-02 10:41:04.671859 PyQt6-6.5.1/sip/QtQuick/qquickview.sip
--rw-r--r--   0 phil       (501) staff       (20)     6928 2023-06-02 10:41:04.665359 PyQt6-6.5.1/sip/QtQuick/qquickwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     1377 2023-06-02 10:41:04.659371 PyQt6-6.5.1/sip/QtQuick/qsgflatcolormaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)    11740 2023-06-02 10:41:04.662774 PyQt6-6.5.1/sip/QtQuick/qsggeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     2762 2023-06-02 10:41:04.659884 PyQt6-6.5.1/sip/QtQuick/qsgimagenode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1747 2023-06-02 10:41:04.669763 PyQt6-6.5.1/sip/QtQuick/qsgmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     4807 2023-06-02 10:41:04.656490 PyQt6-6.5.1/sip/QtQuick/qsgmaterialshader.sip
--rw-r--r--   0 phil       (501) staff       (20)     1033 2023-06-02 10:41:04.658576 PyQt6-6.5.1/sip/QtQuick/qsgmaterialtype.sip
--rw-r--r--   0 phil       (501) staff       (20)     8652 2023-06-02 10:41:04.668405 PyQt6-6.5.1/sip/QtQuick/qsgnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1343 2023-06-02 10:41:04.672231 PyQt6-6.5.1/sip/QtQuick/qsgrectanglenode.sip
--rw-r--r--   0 phil       (501) staff       (20)     3077 2023-06-02 10:41:04.661167 PyQt6-6.5.1/sip/QtQuick/qsgrendererinterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     2526 2023-06-02 10:41:04.666100 PyQt6-6.5.1/sip/QtQuick/qsgrendernode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1354 2023-06-02 10:41:04.666931 PyQt6-6.5.1/sip/QtQuick/qsgsimplerectnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     2097 2023-06-02 10:41:04.670216 PyQt6-6.5.1/sip/QtQuick/qsgsimpletexturenode.sip
--rw-r--r--   0 phil       (501) staff       (20)     2513 2023-06-02 10:41:04.655633 PyQt6-6.5.1/sip/QtQuick/qsgtexture.sip
--rw-r--r--   0 phil       (501) staff       (20)     1446 2023-06-02 10:41:04.664387 PyQt6-6.5.1/sip/QtQuick/qsgtexture_platform.sip
--rw-r--r--   0 phil       (501) staff       (20)     2207 2023-06-02 10:41:04.658169 PyQt6-6.5.1/sip/QtQuick/qsgtexturematerial.sip
--rw-r--r--   0 phil       (501) staff       (20)     1152 2023-06-02 10:41:04.671311 PyQt6-6.5.1/sip/QtQuick/qsgtextureprovider.sip
--rw-r--r--   0 phil       (501) staff       (20)     1324 2023-06-02 10:41:04.658957 PyQt6-6.5.1/sip/QtQuick/qsgvertexcolormaterial.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.882446 PyQt6-6.5.1/sip/QtQuick3D/
--rw-r--r--   0 phil       (501) staff       (20)     2086 2023-06-02 10:41:04.417300 PyQt6-6.5.1/sip/QtQuick3D/QtQuick3Dmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1086 2023-06-02 10:41:04.416895 PyQt6-6.5.1/sip/QtQuick3D/qquick3d.sip
--rw-r--r--   0 phil       (501) staff       (20)     3758 2023-06-02 10:41:04.416493 PyQt6-6.5.1/sip/QtQuick3D/qquick3dgeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     2159 2023-06-02 10:41:04.417835 PyQt6-6.5.1/sip/QtQuick3D/qquick3dobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2181 2023-06-02 10:41:04.415624 PyQt6-6.5.1/sip/QtQuick3D/qquick3dtexturedata.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.955785 PyQt6-6.5.1/sip/QtQuickWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2080 2023-06-02 10:41:04.708900 PyQt6-6.5.1/sip/QtQuickWidgets/QtQuickWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3345 2023-06-02 10:41:04.709694 PyQt6-6.5.1/sip/QtQuickWidgets/qquickwidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.893501 PyQt6-6.5.1/sip/QtRemoteObjects/
--rw-r--r--   0 phil       (501) staff       (20)     2163 2023-06-02 10:41:04.460946 PyQt6-6.5.1/sip/QtRemoteObjects/QtRemoteObjectsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2298 2023-06-02 10:41:04.458844 PyQt6-6.5.1/sip/QtRemoteObjects/qremoteobjectabstractitemmodelreplica.sip
--rw-r--r--   0 phil       (501) staff       (20)     1221 2023-06-02 10:41:04.457769 PyQt6-6.5.1/sip/QtRemoteObjects/qremoteobjectdynamicreplica.sip
--rw-r--r--   0 phil       (501) staff       (20)     6469 2023-06-02 10:41:04.459859 PyQt6-6.5.1/sip/QtRemoteObjects/qremoteobjectnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1429 2023-06-02 10:41:04.461419 PyQt6-6.5.1/sip/QtRemoteObjects/qremoteobjectregistry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1689 2023-06-02 10:41:04.460304 PyQt6-6.5.1/sip/QtRemoteObjects/qremoteobjectreplica.sip
--rw-r--r--   0 phil       (501) staff       (20)     2093 2023-06-02 10:41:04.458354 PyQt6-6.5.1/sip/QtRemoteObjects/qtremoteobjectglobal.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.899760 PyQt6-6.5.1/sip/QtSensors/
--rw-r--r--   0 phil       (501) staff       (20)     2393 2023-06-02 10:41:04.471714 PyQt6-6.5.1/sip/QtSensors/QtSensorsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2037 2023-06-02 10:41:04.465772 PyQt6-6.5.1/sip/QtSensors/qaccelerometer.sip
--rw-r--r--   0 phil       (501) staff       (20)     1842 2023-06-02 10:41:04.462092 PyQt6-6.5.1/sip/QtSensors/qambientlightsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1726 2023-06-02 10:41:04.467472 PyQt6-6.5.1/sip/QtSensors/qambienttemperaturesensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1641 2023-06-02 10:41:04.471249 PyQt6-6.5.1/sip/QtSensors/qcompass.sip
--rw-r--r--   0 phil       (501) staff       (20)     1645 2023-06-02 10:41:04.468042 PyQt6-6.5.1/sip/QtSensors/qgyroscope.sip
--rw-r--r--   0 phil       (501) staff       (20)     1701 2023-06-02 10:41:04.466924 PyQt6-6.5.1/sip/QtSensors/qhumiditysensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1649 2023-06-02 10:41:04.466240 PyQt6-6.5.1/sip/QtSensors/qirproximitysensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1719 2023-06-02 10:41:04.462582 PyQt6-6.5.1/sip/QtSensors/qlidsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1692 2023-06-02 10:41:04.465006 PyQt6-6.5.1/sip/QtSensors/qlightsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1918 2023-06-02 10:41:04.472374 PyQt6-6.5.1/sip/QtSensors/qmagnetometer.sip
--rw-r--r--   0 phil       (501) staff       (20)     1856 2023-06-02 10:41:04.463394 PyQt6-6.5.1/sip/QtSensors/qorientationsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1682 2023-06-02 10:41:04.464428 PyQt6-6.5.1/sip/QtSensors/qpressuresensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1607 2023-06-02 10:41:04.463927 PyQt6-6.5.1/sip/QtSensors/qproximitysensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1749 2023-06-02 10:41:04.472896 PyQt6-6.5.1/sip/QtSensors/qrotationsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     7556 2023-06-02 10:41:04.470699 PyQt6-6.5.1/sip/QtSensors/qsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     2079 2023-06-02 10:41:04.469348 PyQt6-6.5.1/sip/QtSensors/qtapsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1641 2023-06-02 10:41:04.468516 PyQt6-6.5.1/sip/QtSensors/qtiltsensor.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.940187 PyQt6-6.5.1/sip/QtSerialPort/
--rw-r--r--   0 phil       (501) staff       (20)     1982 2023-06-02 10:41:04.630035 PyQt6-6.5.1/sip/QtSerialPort/QtSerialPortmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     7926 2023-06-02 10:41:04.631387 PyQt6-6.5.1/sip/QtSerialPort/qserialport.sip
--rw-r--r--   0 phil       (501) staff       (20)     1768 2023-06-02 10:41:04.629638 PyQt6-6.5.1/sip/QtSerialPort/qserialportinfo.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.011726 PyQt6-6.5.1/sip/QtSpatialAudio/
--rw-r--r--   0 phil       (501) staff       (20)     2107 2023-06-02 10:41:04.917523 PyQt6-6.5.1/sip/QtSpatialAudio/QtSpatialAudiomod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1672 2023-06-02 10:41:04.918815 PyQt6-6.5.1/sip/QtSpatialAudio/qambientsound.sip
--rw-r--r--   0 phil       (501) staff       (20)     2978 2023-06-02 10:41:04.920373 PyQt6-6.5.1/sip/QtSpatialAudio/qaudioengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     1342 2023-06-02 10:41:04.919189 PyQt6-6.5.1/sip/QtSpatialAudio/qaudiolistener.sip
--rw-r--r--   0 phil       (501) staff       (20)     2771 2023-06-02 10:41:04.919777 PyQt6-6.5.1/sip/QtSpatialAudio/qaudioroom.sip
--rw-r--r--   0 phil       (501) staff       (20)     2891 2023-06-02 10:41:04.918369 PyQt6-6.5.1/sip/QtSpatialAudio/qspatialsound.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.000345 PyQt6-6.5.1/sip/QtSql/
--rw-r--r--   0 phil       (501) staff       (20)     2287 2023-06-02 10:41:04.872826 PyQt6-6.5.1/sip/QtSql/QtSqlmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3746 2023-06-02 10:41:04.872424 PyQt6-6.5.1/sip/QtSql/qsqldatabase.sip
--rw-r--r--   0 phil       (501) staff       (20)     5000 2023-06-02 10:41:04.868037 PyQt6-6.5.1/sip/QtSql/qsqldriver.sip
--rw-r--r--   0 phil       (501) staff       (20)     1749 2023-06-02 10:41:04.866639 PyQt6-6.5.1/sip/QtSql/qsqlerror.sip
--rw-r--r--   0 phil       (501) staff       (20)     2360 2023-06-02 10:41:04.873947 PyQt6-6.5.1/sip/QtSql/qsqlfield.sip
--rw-r--r--   0 phil       (501) staff       (20)     1497 2023-06-02 10:41:04.871823 PyQt6-6.5.1/sip/QtSql/qsqlindex.sip
--rw-r--r--   0 phil       (501) staff       (20)     3080 2023-06-02 10:41:04.869567 PyQt6-6.5.1/sip/QtSql/qsqlquery.sip
--rw-r--r--   0 phil       (501) staff       (20)     3117 2023-06-02 10:41:04.871442 PyQt6-6.5.1/sip/QtSql/qsqlquerymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     2260 2023-06-02 10:41:04.870025 PyQt6-6.5.1/sip/QtSql/qsqlrecord.sip
--rw-r--r--   0 phil       (501) staff       (20)     1542 2023-06-02 10:41:04.869032 PyQt6-6.5.1/sip/QtSql/qsqlrelationaldelegate.sip
--rw-r--r--   0 phil       (501) staff       (20)     2598 2023-06-02 10:41:04.873319 PyQt6-6.5.1/sip/QtSql/qsqlrelationaltablemodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     3175 2023-06-02 10:41:04.867231 PyQt6-6.5.1/sip/QtSql/qsqlresult.sip
--rw-r--r--   0 phil       (501) staff       (20)     3785 2023-06-02 10:41:04.870634 PyQt6-6.5.1/sip/QtSql/qsqltablemodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1512 2023-06-02 10:41:04.868491 PyQt6-6.5.1/sip/QtSql/qtsqlglobal.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.889449 PyQt6-6.5.1/sip/QtSvg/
--rw-r--r--   0 phil       (501) staff       (20)     1987 2023-06-02 10:41:04.428535 PyQt6-6.5.1/sip/QtSvg/QtSvgmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2082 2023-06-02 10:41:04.427509 PyQt6-6.5.1/sip/QtSvg/qsvggenerator.sip
--rw-r--r--   0 phil       (501) staff       (20)     3043 2023-06-02 10:41:04.428126 PyQt6-6.5.1/sip/QtSvg/qsvgrenderer.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.891178 PyQt6-6.5.1/sip/QtSvgWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2071 2023-06-02 10:41:04.456697 PyQt6-6.5.1/sip/QtSvgWidgets/QtSvgWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1911 2023-06-02 10:41:04.456270 PyQt6-6.5.1/sip/QtSvgWidgets/qgraphicssvgitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2035 2023-06-02 10:41:04.457195 PyQt6-6.5.1/sip/QtSvgWidgets/qsvgwidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.069184 PyQt6-6.5.1/sip/QtTest/
--rw-r--r--   0 phil       (501) staff       (20)     2110 2023-06-02 10:41:05.159361 PyQt6-6.5.1/sip/QtTest/QtTestmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1689 2023-06-02 10:41:05.161751 PyQt6-6.5.1/sip/QtTest/qabstractitemmodeltester.sip
--rw-r--r--   0 phil       (501) staff       (20)     3285 2023-06-02 10:41:05.160504 PyQt6-6.5.1/sip/QtTest/qsignalspy.sip
--rw-r--r--   0 phil       (501) staff       (20)     3740 2023-06-02 10:41:05.159858 PyQt6-6.5.1/sip/QtTest/qtestkeyboard.sip
--rw-r--r--   0 phil       (501) staff       (20)     2446 2023-06-02 10:41:05.161298 PyQt6-6.5.1/sip/QtTest/qtestmouse.sip
--rw-r--r--   0 phil       (501) staff       (20)     1381 2023-06-02 10:41:05.160892 PyQt6-6.5.1/sip/QtTest/qtestsystem.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:06.018885 PyQt6-6.5.1/sip/QtTextToSpeech/
--rw-r--r--   0 phil       (501) staff       (20)     1981 2023-06-02 10:41:04.959291 PyQt6-6.5.1/sip/QtTextToSpeech/QtTextToSpeechmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3550 2023-06-02 10:41:04.958045 PyQt6-6.5.1/sip/QtTextToSpeech/qtexttospeech.sip
--rw-r--r--   0 phil       (501) staff       (20)     1760 2023-06-02 10:41:04.958821 PyQt6-6.5.1/sip/QtTextToSpeech/qvoice.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.956847 PyQt6-6.5.1/sip/QtWebChannel/
--rw-r--r--   0 phil       (501) staff       (20)     1995 2023-06-02 10:41:04.710275 PyQt6-6.5.1/sip/QtWebChannel/QtWebChannelmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2363 2023-06-02 10:41:04.711499 PyQt6-6.5.1/sip/QtWebChannel/qwebchannel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1425 2023-06-02 10:41:04.710808 PyQt6-6.5.1/sip/QtWebChannel/qwebchannelabstracttransport.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.829353 PyQt6-6.5.1/sip/QtWebSockets/
--rw-r--r--   0 phil       (501) staff       (20)     2158 2023-06-02 10:41:04.213018 PyQt6-6.5.1/sip/QtWebSockets/QtWebSocketsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1238 2023-06-02 10:41:04.213471 PyQt6-6.5.1/sip/QtWebSockets/qmaskgenerator.sip
--rw-r--r--   0 phil       (501) staff       (20)     6039 2023-06-02 10:41:04.212539 PyQt6-6.5.1/sip/QtWebSockets/qwebsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     1445 2023-06-02 10:41:04.211449 PyQt6-6.5.1/sip/QtWebSockets/qwebsocketcorsauthenticator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1623 2023-06-02 10:41:04.210965 PyQt6-6.5.1/sip/QtWebSockets/qwebsockethandshakeoptions.sip
--rw-r--r--   0 phil       (501) staff       (20)     1741 2023-06-02 10:41:04.210432 PyQt6-6.5.1/sip/QtWebSockets/qwebsocketprotocol.sip
--rw-r--r--   0 phil       (501) staff       (20)     3249 2023-06-02 10:41:04.214190 PyQt6-6.5.1/sip/QtWebSockets/qwebsocketserver.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.995574 PyQt6-6.5.1/sip/QtWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     4913 2023-06-02 10:41:04.815738 PyQt6-6.5.1/sip/QtWidgets/QtWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2732 2023-06-02 10:41:04.857056 PyQt6-6.5.1/sip/QtWidgets/qabstractbutton.sip
--rw-r--r--   0 phil       (501) staff       (20)     2621 2023-06-02 10:41:04.767097 PyQt6-6.5.1/sip/QtWidgets/qabstractitemdelegate.sip
--rw-r--r--   0 phil       (501) staff       (20)    10372 2023-06-02 10:41:04.730292 PyQt6-6.5.1/sip/QtWidgets/qabstractitemview.sip
--rw-r--r--   0 phil       (501) staff       (20)     3459 2023-06-02 10:41:04.857857 PyQt6-6.5.1/sip/QtWidgets/qabstractscrollarea.sip
--rw-r--r--   0 phil       (501) staff       (20)     3009 2023-06-02 10:41:04.716992 PyQt6-6.5.1/sip/QtWidgets/qabstractslider.sip
--rw-r--r--   0 phil       (501) staff       (20)     4021 2023-06-02 10:41:04.814322 PyQt6-6.5.1/sip/QtWidgets/qabstractspinbox.sip
--rw-r--r--   0 phil       (501) staff       (20)    14136 2023-06-02 10:41:04.781595 PyQt6-6.5.1/sip/QtWidgets/qapplication.sip
--rw-r--r--   0 phil       (501) staff       (20)     4795 2023-06-02 10:41:04.731619 PyQt6-6.5.1/sip/QtWidgets/qboxlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     1835 2023-06-02 10:41:04.760935 PyQt6-6.5.1/sip/QtWidgets/qbuttongroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     4043 2023-06-02 10:41:04.830186 PyQt6-6.5.1/sip/QtWidgets/qcalendarwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1799 2023-06-02 10:41:04.765417 PyQt6-6.5.1/sip/QtWidgets/qcheckbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     2995 2023-06-02 10:41:04.785587 PyQt6-6.5.1/sip/QtWidgets/qcolordialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2872 2023-06-02 10:41:04.764205 PyQt6-6.5.1/sip/QtWidgets/qcolumnview.sip
--rw-r--r--   0 phil       (501) staff       (20)     6343 2023-06-02 10:41:04.864285 PyQt6-6.5.1/sip/QtWidgets/qcombobox.sip
--rw-r--r--   0 phil       (501) staff       (20)     1749 2023-06-02 10:41:04.825584 PyQt6-6.5.1/sip/QtWidgets/qcommandlinkbutton.sip
--rw-r--r--   0 phil       (501) staff       (20)     3141 2023-06-02 10:41:04.824595 PyQt6-6.5.1/sip/QtWidgets/qcommonstyle.sip
--rw-r--r--   0 phil       (501) staff       (20)     3315 2023-06-02 10:41:04.757921 PyQt6-6.5.1/sip/QtWidgets/qcompleter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2437 2023-06-02 10:41:04.814823 PyQt6-6.5.1/sip/QtWidgets/qdatawidgetmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     5039 2023-06-02 10:41:04.827000 PyQt6-6.5.1/sip/QtWidgets/qdatetimeedit.sip
--rw-r--r--   0 phil       (501) staff       (20)     1866 2023-06-02 10:41:04.728426 PyQt6-6.5.1/sip/QtWidgets/qdial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2692 2023-06-02 10:41:04.728944 PyQt6-6.5.1/sip/QtWidgets/qdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     3396 2023-06-02 10:41:04.816551 PyQt6-6.5.1/sip/QtWidgets/qdialogbuttonbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     2666 2023-06-02 10:41:04.855498 PyQt6-6.5.1/sip/QtWidgets/qdockwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     2730 2023-06-02 10:41:04.829522 PyQt6-6.5.1/sip/QtWidgets/qdrawutil.sip
--rw-r--r--   0 phil       (501) staff       (20)     1389 2023-06-02 10:41:04.762561 PyQt6-6.5.1/sip/QtWidgets/qerrormessage.sip
--rw-r--r--   0 phil       (501) staff       (20)    12183 2023-06-02 10:41:04.807464 PyQt6-6.5.1/sip/QtWidgets/qfiledialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     1261 2023-06-02 10:41:04.760273 PyQt6-6.5.1/sip/QtWidgets/qfileiconprovider.sip
--rw-r--r--   0 phil       (501) staff       (20)      957 2023-06-02 10:41:04.767471 PyQt6-6.5.1/sip/QtWidgets/qfilesystemmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1392 2023-06-02 10:41:04.862264 PyQt6-6.5.1/sip/QtWidgets/qfocusframe.sip
--rw-r--r--   0 phil       (501) staff       (20)     2764 2023-06-02 10:41:04.730874 PyQt6-6.5.1/sip/QtWidgets/qfontcombobox.sip
--rw-r--r--   0 phil       (501) staff       (20)     2916 2023-06-02 10:41:04.723553 PyQt6-6.5.1/sip/QtWidgets/qfontdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     4981 2023-06-02 10:41:04.722986 PyQt6-6.5.1/sip/QtWidgets/qformlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     2164 2023-06-02 10:41:04.714016 PyQt6-6.5.1/sip/QtWidgets/qframe.sip
--rw-r--r--   0 phil       (501) staff       (20)     5339 2023-06-02 10:41:04.828580 PyQt6-6.5.1/sip/QtWidgets/qgesture.sip
--rw-r--r--   0 phil       (501) staff       (20)     1738 2023-06-02 10:41:04.826019 PyQt6-6.5.1/sip/QtWidgets/qgesturerecognizer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2740 2023-06-02 10:41:04.725456 PyQt6-6.5.1/sip/QtWidgets/qgraphicsanchorlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     5015 2023-06-02 10:41:04.863226 PyQt6-6.5.1/sip/QtWidgets/qgraphicseffect.sip
--rw-r--r--   0 phil       (501) staff       (20)     4207 2023-06-02 10:41:04.864939 PyQt6-6.5.1/sip/QtWidgets/qgraphicsgridlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)    26805 2023-06-02 10:41:04.860739 PyQt6-6.5.1/sip/QtWidgets/qgraphicsitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     1730 2023-06-02 10:41:04.718605 PyQt6-6.5.1/sip/QtWidgets/qgraphicslayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     3128 2023-06-02 10:41:04.725993 PyQt6-6.5.1/sip/QtWidgets/qgraphicslayoutitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     3150 2023-06-02 10:41:04.783045 PyQt6-6.5.1/sip/QtWidgets/qgraphicslinearlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     3920 2023-06-02 10:41:04.766040 PyQt6-6.5.1/sip/QtWidgets/qgraphicsproxywidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     8768 2023-06-02 10:41:04.817447 PyQt6-6.5.1/sip/QtWidgets/qgraphicsscene.sip
--rw-r--r--   0 phil       (501) staff       (20)     6166 2023-06-02 10:41:04.762150 PyQt6-6.5.1/sip/QtWidgets/qgraphicssceneevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2441 2023-06-02 10:41:04.812343 PyQt6-6.5.1/sip/QtWidgets/qgraphicstransform.sip
--rw-r--r--   0 phil       (501) staff       (20)     8125 2023-06-02 10:41:04.865844 PyQt6-6.5.1/sip/QtWidgets/qgraphicsview.sip
--rw-r--r--   0 phil       (501) staff       (20)     5459 2023-06-02 10:41:04.782491 PyQt6-6.5.1/sip/QtWidgets/qgraphicswidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     5537 2023-06-02 10:41:04.757170 PyQt6-6.5.1/sip/QtWidgets/qgridlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     2122 2023-06-02 10:41:04.808627 PyQt6-6.5.1/sip/QtWidgets/qgroupbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     7170 2023-06-02 10:41:04.768399 PyQt6-6.5.1/sip/QtWidgets/qheaderview.sip
--rw-r--r--   0 phil       (501) staff       (20)     5360 2023-06-02 10:41:04.715476 PyQt6-6.5.1/sip/QtWidgets/qinputdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2931 2023-06-02 10:41:04.856504 PyQt6-6.5.1/sip/QtWidgets/qitemdelegate.sip
--rw-r--r--   0 phil       (501) staff       (20)     1812 2023-06-02 10:41:04.777751 PyQt6-6.5.1/sip/QtWidgets/qitemeditorfactory.sip
--rw-r--r--   0 phil       (501) staff       (20)     2219 2023-06-02 10:41:04.714573 PyQt6-6.5.1/sip/QtWidgets/qkeysequenceedit.sip
--rw-r--r--   0 phil       (501) staff       (20)     6063 2023-06-02 10:41:04.809927 PyQt6-6.5.1/sip/QtWidgets/qlabel.sip
--rw-r--r--   0 phil       (501) staff       (20)     5894 2023-06-02 10:41:04.724449 PyQt6-6.5.1/sip/QtWidgets/qlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     3732 2023-06-02 10:41:04.784251 PyQt6-6.5.1/sip/QtWidgets/qlayoutitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2378 2023-06-02 10:41:04.712437 PyQt6-6.5.1/sip/QtWidgets/qlcdnumber.sip
--rw-r--r--   0 phil       (501) staff       (20)     5210 2023-06-02 10:41:04.779162 PyQt6-6.5.1/sip/QtWidgets/qlineedit.sip
--rw-r--r--   0 phil       (501) staff       (20)     4961 2023-06-02 10:41:04.759886 PyQt6-6.5.1/sip/QtWidgets/qlistview.sip
--rw-r--r--   0 phil       (501) staff       (20)     7358 2023-06-02 10:41:04.823799 PyQt6-6.5.1/sip/QtWidgets/qlistwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     4691 2023-06-02 10:41:04.780239 PyQt6-6.5.1/sip/QtWidgets/qmainwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     4174 2023-06-02 10:41:04.716312 PyQt6-6.5.1/sip/QtWidgets/qmdiarea.sip
--rw-r--r--   0 phil       (501) staff       (20)     4054 2023-06-02 10:41:04.830848 PyQt6-6.5.1/sip/QtWidgets/qmdisubwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     5652 2023-06-02 10:41:04.727999 PyQt6-6.5.1/sip/QtWidgets/qmenu.sip
--rw-r--r--   0 phil       (501) staff       (20)     3601 2023-06-02 10:41:04.822873 PyQt6-6.5.1/sip/QtWidgets/qmenubar.sip
--rw-r--r--   0 phil       (501) staff       (20)     6307 2023-06-02 10:41:04.785061 PyQt6-6.5.1/sip/QtWidgets/qmessagebox.sip
--rw-r--r--   0 phil       (501) staff       (20)     7249 2023-06-02 10:41:04.819597 PyQt6-6.5.1/sip/QtWidgets/qplaintextedit.sip
--rw-r--r--   0 phil       (501) staff       (20)     2226 2023-06-02 10:41:04.724969 PyQt6-6.5.1/sip/QtWidgets/qprogressbar.sip
--rw-r--r--   0 phil       (501) staff       (20)     2903 2023-06-02 10:41:04.718139 PyQt6-6.5.1/sip/QtWidgets/qprogressdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     3947 2023-06-02 10:41:04.717519 PyQt6-6.5.1/sip/QtWidgets/qproxystyle.sip
--rw-r--r--   0 phil       (501) staff       (20)     2069 2023-06-02 10:41:04.808126 PyQt6-6.5.1/sip/QtWidgets/qpushbutton.sip
--rw-r--r--   0 phil       (501) staff       (20)     2905 2023-06-02 10:41:04.811372 PyQt6-6.5.1/sip/QtWidgets/qpywidgets_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1555 2023-06-02 10:41:04.825022 PyQt6-6.5.1/sip/QtWidgets/qradiobutton.sip
--rw-r--r--   0 phil       (501) staff       (20)     1794 2023-06-02 10:41:04.783605 PyQt6-6.5.1/sip/QtWidgets/qrubberband.sip
--rw-r--r--   0 phil       (501) staff       (20)     1895 2023-06-02 10:41:04.818534 PyQt6-6.5.1/sip/QtWidgets/qscrollarea.sip
--rw-r--r--   0 phil       (501) staff       (20)     1773 2023-06-02 10:41:04.719067 PyQt6-6.5.1/sip/QtWidgets/qscrollbar.sip
--rw-r--r--   0 phil       (501) staff       (20)     2896 2023-06-02 10:41:04.768991 PyQt6-6.5.1/sip/QtWidgets/qscroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     2485 2023-06-02 10:41:04.778311 PyQt6-6.5.1/sip/QtWidgets/qscrollerproperties.sip
--rw-r--r--   0 phil       (501) staff       (20)     1640 2023-06-02 10:41:04.759110 PyQt6-6.5.1/sip/QtWidgets/qsizegrip.sip
--rw-r--r--   0 phil       (501) staff       (20)     3272 2023-06-02 10:41:04.764881 PyQt6-6.5.1/sip/QtWidgets/qsizepolicy.sip
--rw-r--r--   0 phil       (501) staff       (20)     1921 2023-06-02 10:41:04.822154 PyQt6-6.5.1/sip/QtWidgets/qslider.sip
--rw-r--r--   0 phil       (501) staff       (20)     3301 2023-06-02 10:41:04.805839 PyQt6-6.5.1/sip/QtWidgets/qspinbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     1798 2023-06-02 10:41:04.732838 PyQt6-6.5.1/sip/QtWidgets/qsplashscreen.sip
--rw-r--r--   0 phil       (501) staff       (20)     3429 2023-06-02 10:41:04.818109 PyQt6-6.5.1/sip/QtWidgets/qsplitter.sip
--rw-r--r--   0 phil       (501) staff       (20)     3651 2023-06-02 10:41:04.810602 PyQt6-6.5.1/sip/QtWidgets/qstackedlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     1662 2023-06-02 10:41:04.829011 PyQt6-6.5.1/sip/QtWidgets/qstackedwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1956 2023-06-02 10:41:04.756306 PyQt6-6.5.1/sip/QtWidgets/qstatusbar.sip
--rw-r--r--   0 phil       (501) staff       (20)    22575 2023-06-02 10:41:04.722093 PyQt6-6.5.1/sip/QtWidgets/qstyle.sip
--rw-r--r--   0 phil       (501) staff       (20)     2426 2023-06-02 10:41:04.811784 PyQt6-6.5.1/sip/QtWidgets/qstyleditemdelegate.sip
--rw-r--r--   0 phil       (501) staff       (20)     1122 2023-06-02 10:41:04.755752 PyQt6-6.5.1/sip/QtWidgets/qstylefactory.sip
--rw-r--r--   0 phil       (501) staff       (20)    20087 2023-06-02 10:41:04.773282 PyQt6-6.5.1/sip/QtWidgets/qstyleoption.sip
--rw-r--r--   0 phil       (501) staff       (20)     1732 2023-06-02 10:41:04.855955 PyQt6-6.5.1/sip/QtWidgets/qstylepainter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2317 2023-06-02 10:41:04.766597 PyQt6-6.5.1/sip/QtWidgets/qsystemtrayicon.sip
--rw-r--r--   0 phil       (501) staff       (20)     5251 2023-06-02 10:41:04.774209 PyQt6-6.5.1/sip/QtWidgets/qtabbar.sip
--rw-r--r--   0 phil       (501) staff       (20)     4837 2023-06-02 10:41:04.827666 PyQt6-6.5.1/sip/QtWidgets/qtableview.sip
--rw-r--r--   0 phil       (501) staff       (20)     9246 2023-06-02 10:41:04.727237 PyQt6-6.5.1/sip/QtWidgets/qtablewidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     4240 2023-06-02 10:41:04.774984 PyQt6-6.5.1/sip/QtWidgets/qtabwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     2740 2023-06-02 10:41:04.763623 PyQt6-6.5.1/sip/QtWidgets/qtextbrowser.sip
--rw-r--r--   0 phil       (501) staff       (20)     7388 2023-06-02 10:41:04.821700 PyQt6-6.5.1/sip/QtWidgets/qtextedit.sip
--rw-r--r--   0 phil       (501) staff       (20)     4343 2023-06-02 10:41:04.732293 PyQt6-6.5.1/sip/QtWidgets/qtoolbar.sip
--rw-r--r--   0 phil       (501) staff       (20)     2421 2023-06-02 10:41:04.758592 PyQt6-6.5.1/sip/QtWidgets/qtoolbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     2556 2023-06-02 10:41:04.813549 PyQt6-6.5.1/sip/QtWidgets/qtoolbutton.sip
--rw-r--r--   0 phil       (501) staff       (20)     1399 2023-06-02 10:41:04.779555 PyQt6-6.5.1/sip/QtWidgets/qtooltip.sip
--rw-r--r--   0 phil       (501) staff       (20)     6474 2023-06-02 10:41:04.713444 PyQt6-6.5.1/sip/QtWidgets/qtreeview.sip
--rw-r--r--   0 phil       (501) staff       (20)    10328 2023-06-02 10:41:04.820742 PyQt6-6.5.1/sip/QtWidgets/qtreewidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     2195 2023-06-02 10:41:04.813037 PyQt6-6.5.1/sip/QtWidgets/qtreewidgetitemiterator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1597 2023-06-02 10:41:04.762977 PyQt6-6.5.1/sip/QtWidgets/qundoview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1353 2023-06-02 10:41:04.824173 PyQt6-6.5.1/sip/QtWidgets/qwhatsthis.sip
--rw-r--r--   0 phil       (501) staff       (20)    18362 2023-06-02 10:41:04.777240 PyQt6-6.5.1/sip/QtWidgets/qwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1627 2023-06-02 10:41:04.755356 PyQt6-6.5.1/sip/QtWidgets/qwidgetaction.sip
--rw-r--r--   0 phil       (501) staff       (20)     7633 2023-06-02 10:41:04.861872 PyQt6-6.5.1/sip/QtWidgets/qwizard.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.890179 PyQt6-6.5.1/sip/QtXml/
--rw-r--r--   0 phil       (501) staff       (20)     1925 2023-06-02 10:41:04.455589 PyQt6-6.5.1/sip/QtXml/QtXmlmod.sip
--rw-r--r--   0 phil       (501) staff       (20)    16807 2023-06-02 10:41:04.430736 PyQt6-6.5.1/sip/QtXml/qdom.sip
--rw-r--r--   0 phil       (501) staff       (20)       22 2023-06-02 10:41:04.209768 PyQt6-6.5.1/sip/pyqt-gpl.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.713040 PyQt6-6.5.1/uic/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.715436 PyQt6-6.5.1/uic/Compiler/
--rw-r--r--   0 phil       (501) staff       (20)     1004 2023-06-02 10:40:57.534130 PyQt6-6.5.1/uic/Compiler/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     1412 2023-06-02 10:40:57.536594 PyQt6-6.5.1/uic/Compiler/as_string.py
--rw-r--r--   0 phil       (501) staff       (20)     3934 2023-06-02 10:40:57.533798 PyQt6-6.5.1/uic/Compiler/compiler.py
--rw-r--r--   0 phil       (501) staff       (20)     2742 2023-06-02 10:40:57.534653 PyQt6-6.5.1/uic/Compiler/indenter.py
--rw-r--r--   0 phil       (501) staff       (20)     2374 2023-06-02 10:40:57.533133 PyQt6-6.5.1/uic/Compiler/misc.py
--rw-r--r--   0 phil       (501) staff       (20)     4324 2023-06-02 10:40:57.536258 PyQt6-6.5.1/uic/Compiler/proxy_metaclass.py
--rw-r--r--   0 phil       (501) staff       (20)     5839 2023-06-02 10:40:57.535513 PyQt6-6.5.1/uic/Compiler/qobjectcreator.py
--rw-r--r--   0 phil       (501) staff       (20)    16164 2023-06-02 10:40:57.538739 PyQt6-6.5.1/uic/Compiler/qtproxies.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.712684 PyQt6-6.5.1/uic/Loader/
--rw-r--r--   0 phil       (501) staff       (20)     1004 2023-06-02 10:40:57.527421 PyQt6-6.5.1/uic/Loader/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2625 2023-06-02 10:40:57.529078 PyQt6-6.5.1/uic/Loader/loader.py
--rw-r--r--   0 phil       (501) staff       (20)     5187 2023-06-02 10:40:57.528580 PyQt6-6.5.1/uic/Loader/qobjectcreator.py
--rw-r--r--   0 phil       (501) staff       (20)     1003 2023-06-02 10:40:57.526996 PyQt6-6.5.1/uic/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     6103 2023-06-02 10:40:57.539929 PyQt6-6.5.1/uic/compile_ui.py
--rw-r--r--   0 phil       (501) staff       (20)    31764 2023-06-02 10:40:57.526431 PyQt6-6.5.1/uic/enum_map.py
--rw-r--r--   0 phil       (501) staff       (20)     2609 2023-06-02 10:40:57.531302 PyQt6-6.5.1/uic/exceptions.py
--rw-r--r--   0 phil       (501) staff       (20)     5047 2023-06-02 10:40:57.530102 PyQt6-6.5.1/uic/icon_cache.py
--rw-r--r--   0 phil       (501) staff       (20)     3327 2023-06-02 10:40:57.530729 PyQt6-6.5.1/uic/load_ui.py
--rw-r--r--   0 phil       (501) staff       (20)     6097 2023-06-02 10:40:57.518617 PyQt6-6.5.1/uic/objcreator.py
--rw-r--r--   0 phil       (501) staff       (20)    18275 2023-06-02 10:40:57.521407 PyQt6-6.5.1/uic/properties.py
--rw-r--r--   0 phil       (501) staff       (20)     5850 2023-06-02 10:40:57.532554 PyQt6-6.5.1/uic/pyuic.py
--rw-r--r--   0 phil       (501) staff       (20)     3213 2023-06-02 10:40:57.512857 PyQt6-6.5.1/uic/ui_file.py
--rw-r--r--   0 phil       (501) staff       (20)    37502 2023-06-02 10:40:57.517481 PyQt6-6.5.1/uic/uiparser.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 10:41:05.711573 PyQt6-6.5.1/uic/widget-plugins/
--rw-r--r--   0 phil       (501) staff       (20)     1557 2023-06-02 10:40:57.524014 PyQt6-6.5.1/uic/widget-plugins/qaxcontainer.py
--rw-r--r--   0 phil       (501) staff       (20)     1553 2023-06-02 10:40:57.522126 PyQt6-6.5.1/uic/widget-plugins/qscintilla.py
--rw-r--r--   0 phil       (501) staff       (20)     1562 2023-06-02 10:40:57.522852 PyQt6-6.5.1/uic/widget-plugins/qtcharts.py
--rw-r--r--   0 phil       (501) staff       (20)     1588 2023-06-02 10:40:57.523271 PyQt6-6.5.1/uic/widget-plugins/qtprintsupport.py
--rw-r--r--   0 phil       (501) staff       (20)     1562 2023-06-02 10:40:57.523625 PyQt6-6.5.1/uic/widget-plugins/qtquickwidgets.py
--rw-r--r--   0 phil       (501) staff       (20)     1568 2023-06-02 10:40:57.522418 PyQt6-6.5.1/uic/widget-plugins/qtwebenginewidgets.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.899028 PyQt6-6.5.2/
+-rw-r--r--   0 phil       (501) staff       (20)   122192 2023-07-22 15:08:24.134214 PyQt6-6.5.2/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2023-07-22 15:08:23.578918 PyQt6-6.5.2/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)     3804 2023-07-22 15:08:24.136437 PyQt6-6.5.2/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     2075 2023-07-22 15:08:32.899154 PyQt6-6.5.2/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1735 2023-07-22 15:08:24.372580 PyQt6-6.5.2/README
+-rw-r--r--   0 phil       (501) staff       (20)      960 2023-07-22 15:08:24.146517 PyQt6-6.5.2/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.543949 PyQt6-6.5.2/config-tests/
+-rw-r--r--   0 phil       (501) staff       (20)      848 2023-07-22 15:08:24.145340 PyQt6-6.5.2/config-tests/cfgtest_QtCore.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      813 2023-07-22 15:08:24.144381 PyQt6-6.5.2/config-tests/cfgtest_QtGui.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      569 2023-07-22 15:08:24.145790 PyQt6-6.5.2/config-tests/cfgtest_QtNetwork.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      752 2023-07-22 15:08:24.144923 PyQt6-6.5.2/config-tests/cfgtest_QtPrintSupport.cpp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.542250 PyQt6-6.5.2/dbus/
+-rw-r--r--   0 phil       (501) staff       (20)    11344 2023-07-22 15:08:24.366728 PyQt6-6.5.2/dbus/dbus.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2067 2023-07-22 15:08:24.364784 PyQt6-6.5.2/dbus/helper.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.657671 PyQt6-6.5.2/designer/
+-rw-r--r--   0 phil       (501) staff       (20)      435 2023-07-22 15:08:24.367257 PyQt6-6.5.2/designer/designer.pro-in
+-rw-r--r--   0 phil       (501) staff       (20)     9229 2023-07-22 15:08:24.368860 PyQt6-6.5.2/designer/pluginloader.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1982 2023-07-22 15:08:24.369407 PyQt6-6.5.2/designer/pluginloader.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.656036 PyQt6-6.5.2/examples/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.647741 PyQt6-6.5.2/examples/designer/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.648790 PyQt6-6.5.2/examples/designer/calculatorform/
+-rw-r--r--   0 phil       (501) staff       (20)     2805 2023-07-22 14:17:55.678222 PyQt6-6.5.2/examples/designer/calculatorform/calculatorform.py
+-rw-r--r--   0 phil       (501) staff       (20)     7150 2023-07-22 14:17:55.679884 PyQt6-6.5.2/examples/designer/calculatorform/calculatorform.ui
+-rw-r--r--   0 phil       (501) staff       (20)     5538 2023-07-22 14:17:55.680893 PyQt6-6.5.2/examples/designer/calculatorform/ui_calculatorform.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.644602 PyQt6-6.5.2/examples/designer/plugins/
+-rw-r--r--   0 phil       (501) staff       (20)     3578 2023-07-22 14:17:55.673432 PyQt6-6.5.2/examples/designer/plugins/plugins.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.644223 PyQt6-6.5.2/examples/designer/plugins/python/
+-rw-r--r--   0 phil       (501) staff       (20)     5548 2023-07-22 14:17:55.673467 PyQt6-6.5.2/examples/designer/plugins/python/analogclockplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     5106 2023-07-22 14:17:55.674903 PyQt6-6.5.2/examples/designer/plugins/python/bubbleswidgetplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     3447 2023-07-22 14:17:55.810430 PyQt6-6.5.2/examples/designer/plugins/python/counterlabelplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     4401 2023-07-22 14:17:55.674975 PyQt6-6.5.2/examples/designer/plugins/python/datetimeeditplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     3566 2023-07-22 14:17:55.675682 PyQt6-6.5.2/examples/designer/plugins/python/helloglwidgetplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     5126 2023-07-22 14:17:55.677685 PyQt6-6.5.2/examples/designer/plugins/python/multipagewidgetplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     4714 2023-07-22 14:17:55.677378 PyQt6-6.5.2/examples/designer/plugins/python/polygonwidgetplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     4184 2023-07-22 14:17:55.677865 PyQt6-6.5.2/examples/designer/plugins/python/pydemoplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     4612 2023-07-22 14:17:55.679510 PyQt6-6.5.2/examples/designer/plugins/python/pythonconsoleplugin.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.647356 PyQt6-6.5.2/examples/designer/plugins/widgets/
+-rw-r--r--   0 phil       (501) staff       (20)     6253 2023-07-22 14:17:55.681303 PyQt6-6.5.2/examples/designer/plugins/widgets/analogclock.py
+-rw-r--r--   0 phil       (501) staff       (20)    10365 2023-07-22 14:17:55.682898 PyQt6-6.5.2/examples/designer/plugins/widgets/bubbleswidget.py
+-rw-r--r--   0 phil       (501) staff       (20)     5187 2023-07-22 14:17:55.675429 PyQt6-6.5.2/examples/designer/plugins/widgets/counterlabel.py
+-rw-r--r--   0 phil       (501) staff       (20)    16152 2023-07-22 14:17:55.675368 PyQt6-6.5.2/examples/designer/plugins/widgets/datetimeedit.py
+-rw-r--r--   0 phil       (501) staff       (20)     8302 2023-07-22 14:17:55.676689 PyQt6-6.5.2/examples/designer/plugins/widgets/helloglwidget.py
+-rw-r--r--   0 phil       (501) staff       (20)     3985 2023-07-22 14:17:55.811041 PyQt6-6.5.2/examples/designer/plugins/widgets/multipagewidget.py
+-rw-r--r--   0 phil       (501) staff       (20)     5827 2023-07-22 14:17:55.676726 PyQt6-6.5.2/examples/designer/plugins/widgets/polygonwidget.py
+-rw-r--r--   0 phil       (501) staff       (20)     5619 2023-07-22 14:17:55.676809 PyQt6-6.5.2/examples/designer/plugins/widgets/pydemo.py
+-rw-r--r--   0 phil       (501) staff       (20)     3016 2023-07-22 14:17:55.678941 PyQt6-6.5.2/examples/designer/plugins/widgets/pythonconsolewidget.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.637156 PyQt6-6.5.2/examples/desktop/
+-rw-r--r--   0 phil       (501) staff       (20)     6605 2023-07-22 14:17:55.678673 PyQt6-6.5.2/examples/desktop/screenshot.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.637542 PyQt6-6.5.2/examples/desktop/systray/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.638555 PyQt6-6.5.2/examples/desktop/systray/images/
+-rw-r--r--   0 phil       (501) staff       (20)     2496 2023-07-22 14:17:55.679585 PyQt6-6.5.2/examples/desktop/systray/images/bad.png
+-rw-r--r--   0 phil       (501) staff       (20)    25780 2023-07-22 14:17:55.681552 PyQt6-6.5.2/examples/desktop/systray/images/heart.png
+-rw-r--r--   0 phil       (501) staff       (20)    12128 2023-07-22 14:17:55.683634 PyQt6-6.5.2/examples/desktop/systray/images/trash.png
+-rw-r--r--   0 phil       (501) staff       (20)     9595 2023-07-22 14:17:55.685186 PyQt6-6.5.2/examples/desktop/systray/systray.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.654369 PyQt6-6.5.2/examples/dialogs/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.651487 PyQt6-6.5.2/examples/dialogs/classwizard/
+-rw-r--r--   0 phil       (501) staff       (20)    15515 2023-07-22 14:17:55.677019 PyQt6-6.5.2/examples/dialogs/classwizard/classwizard.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.654008 PyQt6-6.5.2/examples/dialogs/classwizard/images/
+-rw-r--r--   0 phil       (501) staff       (20)    22578 2023-07-22 14:17:55.677421 PyQt6-6.5.2/examples/dialogs/classwizard/images/background.png
+-rw-r--r--   0 phil       (501) staff       (20)     3947 2023-07-22 14:17:55.678182 PyQt6-6.5.2/examples/dialogs/classwizard/images/banner.png
+-rw-r--r--   0 phil       (501) staff       (20)     1619 2023-07-22 14:17:55.811640 PyQt6-6.5.2/examples/dialogs/classwizard/images/logo1.png
+-rw-r--r--   0 phil       (501) staff       (20)     1619 2023-07-22 14:17:55.678362 PyQt6-6.5.2/examples/dialogs/classwizard/images/logo2.png
+-rw-r--r--   0 phil       (501) staff       (20)     1619 2023-07-22 14:17:55.678531 PyQt6-6.5.2/examples/dialogs/classwizard/images/logo3.png
+-rw-r--r--   0 phil       (501) staff       (20)    14516 2023-07-22 14:17:55.680520 PyQt6-6.5.2/examples/dialogs/classwizard/images/watermark1.png
+-rw-r--r--   0 phil       (501) staff       (20)    14912 2023-07-22 14:17:55.680123 PyQt6-6.5.2/examples/dialogs/classwizard/images/watermark2.png
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.654847 PyQt6-6.5.2/examples/dialogs/configdialog/
+-rw-r--r--   0 phil       (501) staff       (20)     8989 2023-07-22 14:17:55.681040 PyQt6-6.5.2/examples/dialogs/configdialog/configdialog.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.655589 PyQt6-6.5.2/examples/dialogs/configdialog/images/
+-rw-r--r--   0 phil       (501) staff       (20)     7059 2023-07-22 14:17:55.683376 PyQt6-6.5.2/examples/dialogs/configdialog/images/config.png
+-rw-r--r--   0 phil       (501) staff       (20)     2269 2023-07-22 14:17:55.685827 PyQt6-6.5.2/examples/dialogs/configdialog/images/query.png
+-rw-r--r--   0 phil       (501) staff       (20)     8296 2023-07-22 14:17:55.687485 PyQt6-6.5.2/examples/dialogs/configdialog/images/update.png
+-rw-r--r--   0 phil       (501) staff       (20)     4434 2023-07-22 14:17:55.678259 PyQt6-6.5.2/examples/dialogs/extension.py
+-rw-r--r--   0 phil       (501) staff       (20)     8264 2023-07-22 14:17:55.678614 PyQt6-6.5.2/examples/dialogs/findfiles.py
+-rw-r--r--   0 phil       (501) staff       (20)    13995 2023-07-22 14:17:55.679411 PyQt6-6.5.2/examples/dialogs/standarddialogs.py
+-rw-r--r--   0 phil       (501) staff       (20)     7401 2023-07-22 14:17:55.812214 PyQt6-6.5.2/examples/dialogs/tabdialog.py
+-rw-r--r--   0 phil       (501) staff       (20)     3603 2023-07-22 14:17:55.679336 PyQt6-6.5.2/examples/dialogs/trivialwizard.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.596634 PyQt6-6.5.2/examples/draganddrop/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.595664 PyQt6-6.5.2/examples/draganddrop/delayedencoding/
+-rw-r--r--   0 phil       (501) staff       (20)     4979 2023-07-22 14:17:55.679947 PyQt6-6.5.2/examples/draganddrop/delayedencoding/delayedencoding.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.596248 PyQt6-6.5.2/examples/draganddrop/delayedencoding/images/
+-rw-r--r--   0 phil       (501) staff       (20)      977 2023-07-22 14:17:55.682793 PyQt6-6.5.2/examples/draganddrop/delayedencoding/images/drag.png
+-rw-r--r--   0 phil       (501) staff       (20)     2689 2023-07-22 14:17:55.681842 PyQt6-6.5.2/examples/draganddrop/delayedencoding/images/example.svg
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.593160 PyQt6-6.5.2/examples/draganddrop/draggableicons/
+-rw-r--r--   0 phil       (501) staff       (20)     5975 2023-07-22 14:17:55.682733 PyQt6-6.5.2/examples/draganddrop/draggableicons/draggableicons.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.594096 PyQt6-6.5.2/examples/draganddrop/draggableicons/images/
+-rw-r--r--   0 phil       (501) staff       (20)     2772 2023-07-22 14:17:55.685258 PyQt6-6.5.2/examples/draganddrop/draggableicons/images/boat.png
+-rw-r--r--   0 phil       (501) staff       (20)     2963 2023-07-22 14:17:55.687782 PyQt6-6.5.2/examples/draganddrop/draggableicons/images/car.png
+-rw-r--r--   0 phil       (501) staff       (20)     3292 2023-07-22 14:17:55.688938 PyQt6-6.5.2/examples/draganddrop/draggableicons/images/house.png
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.594998 PyQt6-6.5.2/examples/draganddrop/draggabletext/
+-rw-r--r--   0 phil       (501) staff       (20)     5414 2023-07-22 14:17:55.679885 PyQt6-6.5.2/examples/draganddrop/draggabletext/draggabletext.py
+-rw-r--r--   0 phil       (501) staff       (20)      247 2023-07-22 14:17:55.679877 PyQt6-6.5.2/examples/draganddrop/draggabletext/words.txt
+-rw-r--r--   0 phil       (501) staff       (20)     6826 2023-07-22 14:17:55.680743 PyQt6-6.5.2/examples/draganddrop/dropsite.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.597189 PyQt6-6.5.2/examples/draganddrop/fridgemagnets/
+-rw-r--r--   0 phil       (501) staff       (20)     6903 2023-07-22 14:17:55.812862 PyQt6-6.5.2/examples/draganddrop/fridgemagnets/fridgemagnets.py
+-rw-r--r--   0 phil       (501) staff       (20)      278 2023-07-22 14:17:55.681263 PyQt6-6.5.2/examples/draganddrop/fridgemagnets/words.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.592220 PyQt6-6.5.2/examples/draganddrop/puzzle/
+-rw-r--r--   0 phil       (501) staff       (20)    42654 2023-07-22 14:17:55.682866 PyQt6-6.5.2/examples/draganddrop/puzzle/example.jpg
+-rw-r--r--   0 phil       (501) staff       (20)    12900 2023-07-22 14:17:55.684309 PyQt6-6.5.2/examples/draganddrop/puzzle/puzzle.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.639499 PyQt6-6.5.2/examples/multimedia/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.640325 PyQt6-6.5.2/examples/multimedia/audiodevices/
+-rw-r--r--   0 phil       (501) staff       (20)     7889 2023-07-22 14:17:55.684403 PyQt6-6.5.2/examples/multimedia/audiodevices/audiodevices.py
+-rw-r--r--   0 phil       (501) staff       (20)    11927 2023-07-22 14:17:55.684263 PyQt6-6.5.2/examples/multimedia/audiodevices/audiodevicesbase.ui
+-rw-r--r--   0 phil       (501) staff       (20)    12232 2023-07-22 14:17:55.687056 PyQt6-6.5.2/examples/multimedia/audiodevices/ui_audiodevicesbase.py
+-rw-r--r--   0 phil       (501) staff       (20)     9047 2023-07-22 14:17:55.689087 PyQt6-6.5.2/examples/multimedia/audiooutput.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.602513 PyQt6-6.5.2/examples/multimediawidgets/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.605448 PyQt6-6.5.2/examples/multimediawidgets/camera/
+-rw-r--r--   0 phil       (501) staff       (20)    21481 2023-07-22 14:17:55.691856 PyQt6-6.5.2/examples/multimediawidgets/camera/camera.py
+-rw-r--r--   0 phil       (501) staff       (20)    13064 2023-07-22 14:17:55.681755 PyQt6-6.5.2/examples/multimediawidgets/camera/camera.ui
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.605551 PyQt6-6.5.2/examples/multimediawidgets/camera/images/
+-rw-r--r--   0 phil       (501) staff       (20)     1491 2023-07-22 14:17:55.682189 PyQt6-6.5.2/examples/multimediawidgets/camera/images/shutter.svg
+-rw-r--r--   0 phil       (501) staff       (20)     3290 2023-07-22 14:17:55.682722 PyQt6-6.5.2/examples/multimediawidgets/camera/imagesettings.ui
+-rw-r--r--   0 phil       (501) staff       (20)    10689 2023-07-22 14:17:55.813536 PyQt6-6.5.2/examples/multimediawidgets/camera/ui_camera.py
+-rw-r--r--   0 phil       (501) staff       (20)     3453 2023-07-22 14:17:55.683590 PyQt6-6.5.2/examples/multimediawidgets/camera/ui_imagesettings.py
+-rw-r--r--   0 phil       (501) staff       (20)     6492 2023-07-22 14:17:55.685014 PyQt6-6.5.2/examples/multimediawidgets/camera/ui_videosettings.py
+-rw-r--r--   0 phil       (501) staff       (20)     5727 2023-07-22 14:17:55.686343 PyQt6-6.5.2/examples/multimediawidgets/camera/videosettings.ui
+-rw-r--r--   0 phil       (501) staff       (20)     6277 2023-07-22 14:17:55.686604 PyQt6-6.5.2/examples/multimediawidgets/videographicsitem.py
+-rw-r--r--   0 phil       (501) staff       (20)     5857 2023-07-22 14:17:55.686157 PyQt6-6.5.2/examples/multimediawidgets/videowidget.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.597600 PyQt6-6.5.2/examples/qml/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.601178 PyQt6-6.5.2/examples/qml/referenceexamples/
+-rwxr-xr-x   0 phil       (501) staff       (20)     3228 2023-07-22 14:17:55.688693 PyQt6-6.5.2/examples/qml/referenceexamples/adding.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     6032 2023-07-22 14:17:55.691047 PyQt6-6.5.2/examples/qml/referenceexamples/attached.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     8823 2023-07-22 14:17:55.693847 PyQt6-6.5.2/examples/qml/referenceexamples/binding.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     4133 2023-07-22 14:17:55.684437 PyQt6-6.5.2/examples/qml/referenceexamples/coercion.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     4168 2023-07-22 14:17:55.683985 PyQt6-6.5.2/examples/qml/referenceexamples/default.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     5630 2023-07-22 14:17:55.684147 PyQt6-6.5.2/examples/qml/referenceexamples/grouped.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     4157 2023-07-22 14:17:55.814154 PyQt6-6.5.2/examples/qml/referenceexamples/methods.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     3945 2023-07-22 14:17:55.685347 PyQt6-6.5.2/examples/qml/referenceexamples/properties.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     6504 2023-07-22 14:17:55.686786 PyQt6-6.5.2/examples/qml/referenceexamples/signal.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     8821 2023-07-22 14:17:55.688214 PyQt6-6.5.2/examples/qml/referenceexamples/valuesource.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.635857 PyQt6-6.5.2/examples/quick/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.612334 PyQt6-6.5.2/examples/quick/animation/
+-rw-r--r--   0 phil       (501) staff       (20)     2415 2023-07-22 14:17:55.688367 PyQt6-6.5.2/examples/quick/animation/animation.py
+-rw-r--r--   0 phil       (501) staff       (20)     3371 2023-07-22 14:17:55.688115 PyQt6-6.5.2/examples/quick/animation/animation.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.607822 PyQt6-6.5.2/examples/quick/animation/basics/
+-rw-r--r--   0 phil       (501) staff       (20)     4957 2023-07-22 14:17:55.690328 PyQt6-6.5.2/examples/quick/animation/basics/color-animation.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.609286 PyQt6-6.5.2/examples/quick/animation/basics/images/
+-rw-r--r--   0 phil       (501) staff       (20)    15408 2023-07-22 14:17:55.693269 PyQt6-6.5.2/examples/quick/animation/basics/images/face-smile.png
+-rw-r--r--   0 phil       (501) staff       (20)     2433 2023-07-22 14:17:55.695790 PyQt6-6.5.2/examples/quick/animation/basics/images/moon.png
+-rw-r--r--   0 phil       (501) staff       (20)      425 2023-07-22 14:17:55.686725 PyQt6-6.5.2/examples/quick/animation/basics/images/shadow.png
+-rw-r--r--   0 phil       (501) staff       (20)      349 2023-07-22 14:17:55.686783 PyQt6-6.5.2/examples/quick/animation/basics/images/star.png
+-rw-r--r--   0 phil       (501) staff       (20)     8153 2023-07-22 14:17:55.687168 PyQt6-6.5.2/examples/quick/animation/basics/images/sun.png
+-rw-r--r--   0 phil       (501) staff       (20)     4187 2023-07-22 14:17:55.814803 PyQt6-6.5.2/examples/quick/animation/basics/property-animation.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.612042 PyQt6-6.5.2/examples/quick/animation/behaviors/
+-rw-r--r--   0 phil       (501) staff       (20)     2401 2023-07-22 14:17:55.687374 PyQt6-6.5.2/examples/quick/animation/behaviors/SideRect.qml
+-rw-r--r--   0 phil       (501) staff       (20)     4444 2023-07-22 14:17:55.688638 PyQt6-6.5.2/examples/quick/animation/behaviors/behavior-example.qml
+-rw-r--r--   0 phil       (501) staff       (20)     4376 2023-07-22 14:17:55.690113 PyQt6-6.5.2/examples/quick/animation/behaviors/tvtennis.qml
+-rw-r--r--   0 phil       (501) staff       (20)     4090 2023-07-22 14:17:55.690379 PyQt6-6.5.2/examples/quick/animation/behaviors/wigglytext.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.609700 PyQt6-6.5.2/examples/quick/animation/easing/
+-rw-r--r--   0 phil       (501) staff       (20)     8398 2023-07-22 14:17:55.690152 PyQt6-6.5.2/examples/quick/animation/easing/easing.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.610546 PyQt6-6.5.2/examples/quick/animation/pathanimation/
+-rw-r--r--   0 phil       (501) staff       (20)     3407 2023-07-22 14:17:55.691934 PyQt6-6.5.2/examples/quick/animation/pathanimation/pathanimation.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.610121 PyQt6-6.5.2/examples/quick/animation/pathinterpolator/
+-rw-r--r--   0 phil       (501) staff       (20)     3596 2023-07-22 14:17:55.695309 PyQt6-6.5.2/examples/quick/animation/pathinterpolator/pathinterpolator.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.613073 PyQt6-6.5.2/examples/quick/animation/states/
+-rw-r--r--   0 phil       (501) staff       (20)     5149 2023-07-22 14:17:55.697244 PyQt6-6.5.2/examples/quick/animation/states/qt-logo.png
+-rw-r--r--   0 phil       (501) staff       (20)     3876 2023-07-22 14:17:55.688383 PyQt6-6.5.2/examples/quick/animation/states/states.qml
+-rw-r--r--   0 phil       (501) staff       (20)     4932 2023-07-22 14:17:55.689197 PyQt6-6.5.2/examples/quick/animation/states/transitions.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.629094 PyQt6-6.5.2/examples/quick/canvas/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.628759 PyQt6-6.5.2/examples/quick/canvas/bezierCurve/
+-rw-r--r--   0 phil       (501) staff       (20)     4728 2023-07-22 14:17:55.689238 PyQt6-6.5.2/examples/quick/canvas/bezierCurve/bezierCurve.qml
+-rw-r--r--   0 phil       (501) staff       (20)     2412 2023-07-22 14:17:55.815628 PyQt6-6.5.2/examples/quick/canvas/canvas.py
+-rw-r--r--   0 phil       (501) staff       (20)     3069 2023-07-22 14:17:55.688857 PyQt6-6.5.2/examples/quick/canvas/canvas.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.625813 PyQt6-6.5.2/examples/quick/canvas/clip/
+-rw-r--r--   0 phil       (501) staff       (20)     5037 2023-07-22 14:17:55.691431 PyQt6-6.5.2/examples/quick/canvas/clip/clip.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.621138 PyQt6-6.5.2/examples/quick/canvas/contents/
+-rw-r--r--   0 phil       (501) staff       (20)     3026 2023-07-22 14:17:55.692322 PyQt6-6.5.2/examples/quick/canvas/contents/Button.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3391 2023-07-22 14:17:55.691891 PyQt6-6.5.2/examples/quick/canvas/contents/ScrollBar.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3915 2023-07-22 14:17:55.691551 PyQt6-6.5.2/examples/quick/canvas/contents/Slider.qml
+-rw-r--r--   0 phil       (501) staff       (20)     2826 2023-07-22 14:17:55.693861 PyQt6-6.5.2/examples/quick/canvas/contents/TitleBar.qml
+-rw-r--r--   0 phil       (501) staff       (20)     2564 2023-07-22 14:17:55.696692 PyQt6-6.5.2/examples/quick/canvas/contents/ToolBar.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.625326 PyQt6-6.5.2/examples/quick/canvas/contents/images/
+-rw-r--r--   0 phil       (501) staff       (20)      571 2023-07-22 14:17:55.698769 PyQt6-6.5.2/examples/quick/canvas/contents/images/button-pressed.png
+-rw-r--r--   0 phil       (501) staff       (20)      564 2023-07-22 14:17:55.690157 PyQt6-6.5.2/examples/quick/canvas/contents/images/button.png
+-rw-r--r--   0 phil       (501) staff       (20)     7458 2023-07-22 14:17:55.691569 PyQt6-6.5.2/examples/quick/canvas/contents/images/default.svg
+-rw-r--r--   0 phil       (501) staff       (20)     1236 2023-07-22 14:17:55.691442 PyQt6-6.5.2/examples/quick/canvas/contents/images/gloss.png
+-rw-r--r--   0 phil       (501) staff       (20)     1415 2023-07-22 14:17:55.816200 PyQt6-6.5.2/examples/quick/canvas/contents/images/lineedit.png
+-rw-r--r--   0 phil       (501) staff       (20)       87 2023-07-22 14:17:55.691225 PyQt6-6.5.2/examples/quick/canvas/contents/images/lineedit.sci
+-rw-r--r--   0 phil       (501) staff       (20)     2369 2023-07-22 14:17:55.693109 PyQt6-6.5.2/examples/quick/canvas/contents/images/quit.png
+-rw-r--r--   0 phil       (501) staff       (20)      257 2023-07-22 14:17:55.693986 PyQt6-6.5.2/examples/quick/canvas/contents/images/stripes.png
+-rw-r--r--   0 phil       (501) staff       (20)     1436 2023-07-22 14:17:55.693441 PyQt6-6.5.2/examples/quick/canvas/contents/images/titlebar.png
+-rw-r--r--   0 phil       (501) staff       (20)       87 2023-07-22 14:17:55.693736 PyQt6-6.5.2/examples/quick/canvas/contents/images/titlebar.sci
+-rw-r--r--   0 phil       (501) staff       (20)     2550 2023-07-22 14:17:55.695394 PyQt6-6.5.2/examples/quick/canvas/contents/images/toolbutton.png
+-rw-r--r--   0 phil       (501) staff       (20)       87 2023-07-22 14:17:55.698228 PyQt6-6.5.2/examples/quick/canvas/contents/images/toolbutton.sci
+-rw-r--r--   0 phil       (501) staff       (20)    23519 2023-07-22 14:17:55.700539 PyQt6-6.5.2/examples/quick/canvas/contents/qt-logo.png
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.627357 PyQt6-6.5.2/examples/quick/canvas/quadraticCurveTo/
+-rw-r--r--   0 phil       (501) staff       (20)     4992 2023-07-22 14:17:55.691992 PyQt6-6.5.2/examples/quick/canvas/quadraticCurveTo/quadraticCurveTo.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.618483 PyQt6-6.5.2/examples/quick/canvas/roundedrect/
+-rw-r--r--   0 phil       (501) staff       (20)     5070 2023-07-22 14:17:55.693284 PyQt6-6.5.2/examples/quick/canvas/roundedrect/roundedrect.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.629200 PyQt6-6.5.2/examples/quick/canvas/smile/
+-rw-r--r--   0 phil       (501) staff       (20)     5063 2023-07-22 14:17:55.693489 PyQt6-6.5.2/examples/quick/canvas/smile/smile.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.628277 PyQt6-6.5.2/examples/quick/canvas/squircle/
+-rw-r--r--   0 phil       (501) staff       (20)      771 2023-07-22 14:17:55.816796 PyQt6-6.5.2/examples/quick/canvas/squircle/squircle.png
+-rw-r--r--   0 phil       (501) staff       (20)     5379 2023-07-22 14:17:55.692882 PyQt6-6.5.2/examples/quick/canvas/squircle/squircle.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.626647 PyQt6-6.5.2/examples/quick/canvas/tiger/
+-rw-r--r--   0 phil       (501) staff       (20)    93676 2023-07-22 14:17:55.696465 PyQt6-6.5.2/examples/quick/canvas/tiger/tiger.js
+-rw-r--r--   0 phil       (501) staff       (20)     4864 2023-07-22 14:17:55.695628 PyQt6-6.5.2/examples/quick/canvas/tiger/tiger.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.616871 PyQt6-6.5.2/examples/quick/models/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.616539 PyQt6-6.5.2/examples/quick/models/abstractitemmodel/
+-rw-r--r--   0 phil       (501) staff       (20)     4051 2023-07-22 14:17:55.695379 PyQt6-6.5.2/examples/quick/models/abstractitemmodel/abstractitemmodel.py
+-rw-r--r--   0 phil       (501) staff       (20)     2151 2023-07-22 14:17:55.695161 PyQt6-6.5.2/examples/quick/models/abstractitemmodel/view.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.615819 PyQt6-6.5.2/examples/quick/models/objectlistmodel/
+-rw-r--r--   0 phil       (501) staff       (20)     3630 2023-07-22 14:17:55.697068 PyQt6-6.5.2/examples/quick/models/objectlistmodel/objectlistmodel.py
+-rw-r--r--   0 phil       (501) staff       (20)     2784 2023-07-22 14:17:55.699787 PyQt6-6.5.2/examples/quick/models/objectlistmodel/view.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.617290 PyQt6-6.5.2/examples/quick/models/stringlistmodel/
+-rw-r--r--   0 phil       (501) staff       (20)     2607 2023-07-22 14:17:55.701974 PyQt6-6.5.2/examples/quick/models/stringlistmodel/stringlistmodel.py
+-rw-r--r--   0 phil       (501) staff       (20)     2772 2023-07-22 14:17:55.694283 PyQt6-6.5.2/examples/quick/models/stringlistmodel/view.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.635911 PyQt6-6.5.2/examples/quick/scenegraph/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.636408 PyQt6-6.5.2/examples/quick/scenegraph/customgeometry/
+-rw-r--r--   0 phil       (501) staff       (20)     5922 2023-07-22 14:17:55.695380 PyQt6-6.5.2/examples/quick/scenegraph/customgeometry/customgeometry.py
+-rw-r--r--   0 phil       (501) staff       (20)     2732 2023-07-22 14:17:55.695284 PyQt6-6.5.2/examples/quick/scenegraph/customgeometry/main.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.614498 PyQt6-6.5.2/examples/quick/shared/
+-rw-r--r--   0 phil       (501) staff       (20)     3291 2023-07-22 14:17:55.817310 PyQt6-6.5.2/examples/quick/shared/Button.qml
+-rw-r--r--   0 phil       (501) staff       (20)     5174 2023-07-22 14:17:55.694891 PyQt6-6.5.2/examples/quick/shared/LauncherList.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3287 2023-07-22 14:17:55.697985 PyQt6-6.5.2/examples/quick/shared/SimpleLauncherDelegate.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.614956 PyQt6-6.5.2/examples/quick/shared/images/
+-rw-r--r--   0 phil       (501) staff       (20)     1590 2023-07-22 14:17:55.697110 PyQt6-6.5.2/examples/quick/shared/images/back.png
+-rw-r--r--   0 phil       (501) staff       (20)     1371 2023-07-22 14:17:55.697043 PyQt6-6.5.2/examples/quick/shared/images/next.png
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.629716 PyQt6-6.5.2/examples/quick/tutorials/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.635070 PyQt6-6.5.2/examples/quick/tutorials/extending/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.635517 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter1-basics/
+-rw-r--r--   0 phil       (501) staff       (20)     2385 2023-07-22 14:17:55.696899 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter1-basics/app.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3492 2023-07-22 14:17:55.698489 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter1-basics/chapter1-basics.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.630178 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter2-methods/
+-rw-r--r--   0 phil       (501) staff       (20)     2532 2023-07-22 14:17:55.701401 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter2-methods/app.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3538 2023-07-22 14:17:55.703378 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter2-methods/chapter2-methods.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.630973 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter3-bindings/
+-rw-r--r--   0 phil       (501) staff       (20)     2650 2023-07-22 14:17:55.696437 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter3-bindings/app.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3625 2023-07-22 14:17:55.697043 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter3-bindings/chapter3-bindings.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.632664 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter4-customPropertyTypes/
+-rw-r--r--   0 phil       (501) staff       (20)     2361 2023-07-22 14:17:55.696946 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter4-customPropertyTypes/app.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3724 2023-07-22 14:17:55.817936 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter4-customPropertyTypes/chapter4-customPropertyTypes.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.631816 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter5-listproperties/
+-rw-r--r--   0 phil       (501) staff       (20)     2643 2023-07-22 14:17:55.696548 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter5-listproperties/app.qml
+-rw-r--r--   0 phil       (501) staff       (20)     4116 2023-07-22 14:17:55.699886 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter5-listproperties/chapter5-listproperties.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.633486 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.634612 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/
+-rw-r--r--   0 phil       (501) staff       (20)     2292 2023-07-22 14:17:55.699022 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/chartsplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     2587 2023-07-22 14:17:55.698782 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/piechart.py
+-rw-r--r--   0 phil       (501) staff       (20)     3132 2023-07-22 14:17:55.698770 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/pieslice.py
+-rw-r--r--   0 phil       (501) staff       (20)       36 2023-07-22 14:17:55.700053 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/qmldir
+-rw-r--r--   0 phil       (501) staff       (20)     2643 2023-07-22 14:17:55.702740 PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/app.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.656084 PyQt6-6.5.2/examples/richtext/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.656502 PyQt6-6.5.2/examples/richtext/textobject/
+-rw-r--r--   0 phil       (501) staff       (20)     3873 2023-07-22 14:17:55.704564 PyQt6-6.5.2/examples/richtext/textobject/heart.svg
+-rw-r--r--   0 phil       (501) staff       (20)     4491 2023-07-22 14:17:55.697921 PyQt6-6.5.2/examples/richtext/textobject/textobject.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.529780 PyQt6-6.5.2/lupdate/
+-rw-r--r--   0 phil       (501) staff       (20)      875 2023-07-22 15:08:24.331868 PyQt6-6.5.2/lupdate/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2479 2023-07-22 15:08:24.332980 PyQt6-6.5.2/lupdate/designer_source.py
+-rw-r--r--   0 phil       (501) staff       (20)     3416 2023-07-22 15:08:24.335368 PyQt6-6.5.2/lupdate/lupdate.py
+-rw-r--r--   0 phil       (501) staff       (20)     3062 2023-07-22 15:08:24.328772 PyQt6-6.5.2/lupdate/pylupdate.py
+-rw-r--r--   0 phil       (501) staff       (20)    11253 2023-07-22 15:08:24.334739 PyQt6-6.5.2/lupdate/python_source.py
+-rw-r--r--   0 phil       (501) staff       (20)     1114 2023-07-22 15:08:24.332388 PyQt6-6.5.2/lupdate/source_file.py
+-rw-r--r--   0 phil       (501) staff       (20)    14976 2023-07-22 15:08:24.331027 PyQt6-6.5.2/lupdate/translation_file.py
+-rw-r--r--   0 phil       (501) staff       (20)     1633 2023-07-22 15:08:24.331543 PyQt6-6.5.2/lupdate/translations.py
+-rw-r--r--   0 phil       (501) staff       (20)     1504 2023-07-22 15:08:24.327895 PyQt6-6.5.2/lupdate/user.py
+-rw-r--r--   0 phil       (501) staff       (20)    29993 2023-07-22 15:08:24.376157 PyQt6-6.5.2/project.py
+-rw-r--r--   0 phil       (501) staff       (20)      546 2023-07-22 15:08:24.376478 PyQt6-6.5.2/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.898796 PyQt6-6.5.2/qmlscene/
+-rw-r--r--   0 phil       (501) staff       (20)     9302 2023-07-22 15:08:24.371641 PyQt6-6.5.2/qmlscene/pluginloader.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1670 2023-07-22 15:08:24.372052 PyQt6-6.5.2/qmlscene/pluginloader.h
+-rw-r--r--   0 phil       (501) staff       (20)      451 2023-07-22 15:08:24.370021 PyQt6-6.5.2/qmlscene/qmlscene.pro-in
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.570015 PyQt6-6.5.2/qpy/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.590584 PyQt6-6.5.2/qpy/QtCore/
+-rw-r--r--   0 phil       (501) staff       (20)     3878 2023-07-22 15:08:24.236143 PyQt6-6.5.2/qpy/QtCore/qpycore_api.h
+-rw-r--r--   0 phil       (501) staff       (20)    49695 2023-07-22 15:08:24.187986 PyQt6-6.5.2/qpy/QtCore/qpycore_chimera.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9586 2023-07-22 15:08:24.201516 PyQt6-6.5.2/qpy/QtCore/qpycore_chimera.h
+-rw-r--r--   0 phil       (501) staff       (20)     2557 2023-07-22 15:08:24.223179 PyQt6-6.5.2/qpy/QtCore/qpycore_chimera_signature.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3515 2023-07-22 15:08:24.220874 PyQt6-6.5.2/qpy/QtCore/qpycore_chimera_storage.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3077 2023-07-22 15:08:24.224261 PyQt6-6.5.2/qpy/QtCore/qpycore_classinfo.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1089 2023-07-22 15:08:24.151337 PyQt6-6.5.2/qpy/QtCore/qpycore_classinfo.h
+-rw-r--r--   0 phil       (501) staff       (20)     4385 2023-07-22 15:08:24.180008 PyQt6-6.5.2/qpy/QtCore/qpycore_decorators.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5930 2023-07-22 15:08:24.174800 PyQt6-6.5.2/qpy/QtCore/qpycore_enums_flags.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1261 2023-07-22 15:08:24.222473 PyQt6-6.5.2/qpy/QtCore/qpycore_enums_flags.h
+-rw-r--r--   0 phil       (501) staff       (20)     4006 2023-07-22 15:08:24.156255 PyQt6-6.5.2/qpy/QtCore/qpycore_event_handlers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1376 2023-07-22 15:08:24.225530 PyQt6-6.5.2/qpy/QtCore/qpycore_event_handlers.h
+-rw-r--r--   0 phil       (501) staff       (20)     3908 2023-07-22 15:08:24.176071 PyQt6-6.5.2/qpy/QtCore/qpycore_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1815 2023-07-22 15:08:24.203097 PyQt6-6.5.2/qpy/QtCore/qpycore_misc.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1136 2023-07-22 15:08:24.163577 PyQt6-6.5.2/qpy/QtCore/qpycore_misc.h
+-rw-r--r--   0 phil       (501) staff       (20)     1136 2023-07-22 15:08:24.177912 PyQt6-6.5.2/qpy/QtCore/qpycore_namespace.h
+-rw-r--r--   0 phil       (501) staff       (20)     1183 2023-07-22 15:08:24.206936 PyQt6-6.5.2/qpy/QtCore/qpycore_objectified_strings.h
+-rw-r--r--   0 phil       (501) staff       (20)     4375 2023-07-22 15:08:24.157818 PyQt6-6.5.2/qpy/QtCore/qpycore_post_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12835 2023-07-22 15:08:24.228835 PyQt6-6.5.2/qpy/QtCore/qpycore_public_api.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4908 2023-07-22 15:08:24.226193 PyQt6-6.5.2/qpy/QtCore/qpycore_public_api.h
+-rw-r--r--   0 phil       (501) staff       (20)    29685 2023-07-22 15:08:24.214613 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtboundsignal.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2023 2023-07-22 15:08:24.230274 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtboundsignal.h
+-rw-r--r--   0 phil       (501) staff       (20)     6090 2023-07-22 15:08:24.215897 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtconfigure.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7424 2023-07-22 15:08:24.210162 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtmethodproxy.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1769 2023-07-22 15:08:24.178969 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtmethodproxy.h
+-rw-r--r--   0 phil       (501) staff       (20)     2072 2023-07-22 15:08:24.222073 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtmutexlocker.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1438 2023-07-22 15:08:24.197734 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtmutexlocker.h
+-rw-r--r--   0 phil       (501) staff       (20)    15571 2023-07-22 15:08:24.172698 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtproperty.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2076 2023-07-22 15:08:24.173444 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtproperty.h
+-rw-r--r--   0 phil       (501) staff       (20)     4765 2023-07-22 15:08:24.204781 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtpyobject.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1742 2023-07-22 15:08:24.178381 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtpyobject.h
+-rw-r--r--   0 phil       (501) staff       (20)    20440 2023-07-22 15:08:24.155332 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtsignal.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2537 2023-07-22 15:08:24.203666 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtsignal.h
+-rw-r--r--   0 phil       (501) staff       (20)     9102 2023-07-22 15:08:24.189948 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtslot.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2284 2023-07-22 15:08:24.226828 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtslot.h
+-rw-r--r--   0 phil       (501) staff       (20)    10864 2023-07-22 15:08:24.218174 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtslotproxy.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3552 2023-07-22 15:08:24.207707 PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtslotproxy.h
+-rw-r--r--   0 phil       (501) staff       (20)     4375 2023-07-22 15:08:24.229678 PyQt6-6.5.2/qpy/QtCore/qpycore_qjsonvalue.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3016 2023-07-22 15:08:24.224934 PyQt6-6.5.2/qpy/QtCore/qpycore_qmessagelogger.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4296 2023-07-22 15:08:24.198571 PyQt6-6.5.2/qpy/QtCore/qpycore_qmetaobject.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4569 2023-07-22 15:08:24.220140 PyQt6-6.5.2/qpy/QtCore/qpycore_qmetaobject_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3505 2023-07-22 15:08:24.199951 PyQt6-6.5.2/qpy/QtCore/qpycore_qmetaobjectbuilder.h
+-rw-r--r--   0 phil       (501) staff       (20)     4273 2023-07-22 15:08:24.208524 PyQt6-6.5.2/qpy/QtCore/qpycore_qobject_getattr.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8681 2023-07-22 15:08:24.206359 PyQt6-6.5.2/qpy/QtCore/qpycore_qobject_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1408 2023-07-22 15:08:24.230779 PyQt6-6.5.2/qpy/QtCore/qpycore_qobject_helpers.h
+-rw-r--r--   0 phil       (501) staff       (20)     4181 2023-07-22 15:08:24.190846 PyQt6-6.5.2/qpy/QtCore/qpycore_qstring.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3178 2023-07-22 15:08:24.165811 PyQt6-6.5.2/qpy/QtCore/qpycore_qt_conf.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2535 2023-07-22 15:08:24.221509 PyQt6-6.5.2/qpy/QtCore/qpycore_qvariant.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6459 2023-07-22 15:08:24.177416 PyQt6-6.5.2/qpy/QtCore/qpycore_qvariant_value.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    17334 2023-07-22 15:08:24.169333 PyQt6-6.5.2/qpy/QtCore/qpycore_types.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1576 2023-07-22 15:08:24.169875 PyQt6-6.5.2/qpy/QtCore/qpycore_types.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.567104 PyQt6-6.5.2/qpy/QtDBus/
+-rw-r--r--   0 phil       (501) staff       (20)      999 2023-07-22 15:08:24.239601 PyQt6-6.5.2/qpy/QtDBus/qpydbus_api.h
+-rw-r--r--   0 phil       (501) staff       (20)     5739 2023-07-22 15:08:24.242944 PyQt6-6.5.2/qpy/QtDBus/qpydbus_chimera_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1236 2023-07-22 15:08:24.241691 PyQt6-6.5.2/qpy/QtDBus/qpydbus_chimera_helpers.h
+-rw-r--r--   0 phil       (501) staff       (20)     1471 2023-07-22 15:08:24.238863 PyQt6-6.5.2/qpy/QtDBus/qpydbus_post_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1865 2023-07-22 15:08:24.239294 PyQt6-6.5.2/qpy/QtDBus/qpydbuspendingreply.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1340 2023-07-22 15:08:24.241350 PyQt6-6.5.2/qpy/QtDBus/qpydbuspendingreply.h
+-rw-r--r--   0 phil       (501) staff       (20)     3583 2023-07-22 15:08:24.240812 PyQt6-6.5.2/qpy/QtDBus/qpydbusreply.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1788 2023-07-22 15:08:24.238518 PyQt6-6.5.2/qpy/QtDBus/qpydbusreply.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.557511 PyQt6-6.5.2/qpy/QtDesigner/
+-rw-r--r--   0 phil       (501) staff       (20)     1410 2023-07-22 15:08:24.244724 PyQt6-6.5.2/qpy/QtDesigner/qpydesignercontainerextension.h
+-rw-r--r--   0 phil       (501) staff       (20)     1492 2023-07-22 15:08:24.246709 PyQt6-6.5.2/qpy/QtDesigner/qpydesignercustomwidgetcollectionplugin.h
+-rw-r--r--   0 phil       (501) staff       (20)     1402 2023-07-22 15:08:24.246048 PyQt6-6.5.2/qpy/QtDesigner/qpydesignercustomwidgetplugin.h
+-rw-r--r--   0 phil       (501) staff       (20)     1430 2023-07-22 15:08:24.243895 PyQt6-6.5.2/qpy/QtDesigner/qpydesignermembersheetextension.h
+-rw-r--r--   0 phil       (501) staff       (20)     1450 2023-07-22 15:08:24.245386 PyQt6-6.5.2/qpy/QtDesigner/qpydesignerpropertysheetextension.h
+-rw-r--r--   0 phil       (501) staff       (20)     1400 2023-07-22 15:08:24.247510 PyQt6-6.5.2/qpy/QtDesigner/qpydesignertaskmenuextension.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.548711 PyQt6-6.5.2/qpy/QtOpenGL/
+-rw-r--r--   0 phil       (501) staff       (20)   209932 2023-07-22 15:08:24.281380 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_add_constants.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2585 2023-07-22 15:08:24.288509 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_api.h
+-rw-r--r--   0 phil       (501) staff       (20)     4002 2023-07-22 15:08:24.286394 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_array_convertors.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7165 2023-07-22 15:08:24.283879 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_attribute_array.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5002 2023-07-22 15:08:24.287657 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_data_cache.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2413 2023-07-22 15:08:24.257205 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_data_cache.h
+-rw-r--r--   0 phil       (501) staff       (20)     4686 2023-07-22 15:08:24.282471 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_get.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1228 2023-07-22 15:08:24.288910 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1261 2023-07-22 15:08:24.257670 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_misc.h
+-rw-r--r--   0 phil       (501) staff       (20)    12637 2023-07-22 15:08:24.259452 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_uniform_value_array.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9947 2023-07-22 15:08:24.261349 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_value_array.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3103 2023-07-22 15:08:24.284724 PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_version_functions.cpp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.555050 PyQt6-6.5.2/qpy/QtQml/
+-rw-r--r--   0 phil       (501) staff       (20)     2279 2023-07-22 15:08:24.300339 PyQt6-6.5.2/qpy/QtQml/qpyqml_api.h
+-rw-r--r--   0 phil       (501) staff       (20)     1799 2023-07-22 15:08:24.305045 PyQt6-6.5.2/qpy/QtQml/qpyqml_listdata.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1431 2023-07-22 15:08:24.310249 PyQt6-6.5.2/qpy/QtQml/qpyqml_listdata.h
+-rw-r--r--   0 phil       (501) staff       (20)     2595 2023-07-22 15:08:24.306059 PyQt6-6.5.2/qpy/QtQml/qpyqml_post_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3089 2023-07-22 15:08:24.304376 PyQt6-6.5.2/qpy/QtQml/qpyqml_qjsvalue.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5283 2023-07-22 15:08:24.296897 PyQt6-6.5.2/qpy/QtQml/qpyqml_register_singleton_type.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12648 2023-07-22 15:08:24.307976 PyQt6-6.5.2/qpy/QtQml/qpyqml_register_type.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9495 2023-07-22 15:08:24.309804 PyQt6-6.5.2/qpy/QtQml/qpyqmllistproperty.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1118 2023-07-22 15:08:24.303741 PyQt6-6.5.2/qpy/QtQml/qpyqmllistproperty.h
+-rw-r--r--   0 phil       (501) staff       (20)     6171 2023-07-22 15:08:24.302063 PyQt6-6.5.2/qpy/QtQml/qpyqmllistpropertywrapper.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1884 2023-07-22 15:08:24.300807 PyQt6-6.5.2/qpy/QtQml/qpyqmllistpropertywrapper.h
+-rw-r--r--   0 phil       (501) staff       (20)    17618 2023-07-22 15:08:24.299740 PyQt6-6.5.2/qpy/QtQml/qpyqmlobject.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7477 2023-07-22 15:08:24.292448 PyQt6-6.5.2/qpy/QtQml/qpyqmlobject.h
+-rw-r--r--   0 phil       (501) staff       (20)     3201 2023-07-22 15:08:24.302805 PyQt6-6.5.2/qpy/QtQml/qpyqmlsingletonobject.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3097 2023-07-22 15:08:24.293218 PyQt6-6.5.2/qpy/QtQml/qpyqmlsingletonobject.h
+-rw-r--r--   0 phil       (501) staff       (20)    10140 2023-07-22 15:08:24.295847 PyQt6-6.5.2/qpy/QtQml/qpyqmlvalidator.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3440 2023-07-22 15:08:24.294083 PyQt6-6.5.2/qpy/QtQml/qpyqmlvalidator.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.563695 PyQt6-6.5.2/qpy/QtQuick/
+-rw-r--r--   0 phil       (501) staff       (20)     1136 2023-07-22 15:08:24.314320 PyQt6-6.5.2/qpy/QtQuick/qpyquick_api.h
+-rw-r--r--   0 phil       (501) staff       (20)     4162 2023-07-22 15:08:24.315416 PyQt6-6.5.2/qpy/QtQuick/qpyquick_chimera_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1601 2023-07-22 15:08:24.312977 PyQt6-6.5.2/qpy/QtQuick/qpyquick_chimera_helpers.h
+-rw-r--r--   0 phil       (501) staff       (20)     2528 2023-07-22 15:08:24.311196 PyQt6-6.5.2/qpy/QtQuick/qpyquick_post_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2490 2023-07-22 15:08:24.312414 PyQt6-6.5.2/qpy/QtQuick/qpyquick_register_type.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1297 2023-07-22 15:08:24.318689 PyQt6-6.5.2/qpy/QtQuick/qpyquick_register_type.h
+-rw-r--r--   0 phil       (501) staff       (20)     6763 2023-07-22 15:08:24.316318 PyQt6-6.5.2/qpy/QtQuick/qpyquickframebufferobject.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3136 2023-07-22 15:08:24.311982 PyQt6-6.5.2/qpy/QtQuick/qpyquickframebufferobject.h
+-rw-r--r--   0 phil       (501) staff       (20)     7803 2023-07-22 15:08:24.319856 PyQt6-6.5.2/qpy/QtQuick/qpyquickitem.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3255 2023-07-22 15:08:24.320642 PyQt6-6.5.2/qpy/QtQuick/qpyquickitem.h
+-rw-r--r--   0 phil       (501) staff       (20)     6215 2023-07-22 15:08:24.313957 PyQt6-6.5.2/qpy/QtQuick/qpyquickpainteditem.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2873 2023-07-22 15:08:24.316964 PyQt6-6.5.2/qpy/QtQuick/qpyquickpainteditem.h
+-rw-r--r--   0 phil       (501) staff       (20)     5020 2023-07-22 15:08:24.317789 PyQt6-6.5.2/qpy/QtQuick/qpyquickview.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2326 2023-07-22 15:08:24.322203 PyQt6-6.5.2/qpy/QtQuick/qpyquickview.h
+-rw-r--r--   0 phil       (501) staff       (20)     5160 2023-07-22 15:08:24.321445 PyQt6-6.5.2/qpy/QtQuick/qpyquickwindow.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2396 2023-07-22 15:08:24.318324 PyQt6-6.5.2/qpy/QtQuick/qpyquickwindow.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.569551 PyQt6-6.5.2/qpy/QtWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     1008 2023-07-22 15:08:24.322783 PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_api.h
+-rw-r--r--   0 phil       (501) staff       (20)     1805 2023-07-22 15:08:24.323604 PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_chimera_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1247 2023-07-22 15:08:24.324683 PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_chimera_helpers.h
+-rw-r--r--   0 phil       (501) staff       (20)     1703 2023-07-22 15:08:24.325794 PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_post_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1195 2023-07-22 15:08:24.323158 PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_qaction_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1147 2023-07-22 15:08:24.325049 PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_qaction_helpers.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.897258 PyQt6-6.5.2/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.721011 PyQt6-6.5.2/sip/QAxContainer/
+-rw-r--r--   0 phil       (501) staff       (20)     1998 2023-07-22 15:08:31.295246 PyQt6-6.5.2/sip/QAxContainer/QAxContainermod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4938 2023-07-22 15:08:31.296014 PyQt6-6.5.2/sip/QAxContainer/qaxbase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2540 2023-07-22 15:08:31.297526 PyQt6-6.5.2/sip/QAxContainer/qaxobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1251 2023-07-22 15:08:31.296484 PyQt6-6.5.2/sip/QAxContainer/qaxobjectinterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2350 2023-07-22 15:08:31.296977 PyQt6-6.5.2/sip/QAxContainer/qaxwidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.689928 PyQt6-6.5.2/sip/QtBluetooth/
+-rw-r--r--   0 phil       (501) staff       (20)     2777 2023-07-22 15:08:31.191485 PyQt6-6.5.2/sip/QtBluetooth/QtBluetoothmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1559 2023-07-22 15:08:31.190450 PyQt6-6.5.2/sip/QtBluetooth/qbluetooth.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1673 2023-07-22 15:08:31.181963 PyQt6-6.5.2/sip/QtBluetooth/qbluetoothaddress.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2670 2023-07-22 15:08:31.186349 PyQt6-6.5.2/sip/QtBluetooth/qbluetoothdevicediscoveryagent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6598 2023-07-22 15:08:31.179954 PyQt6-6.5.2/sip/QtBluetooth/qbluetoothdeviceinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1541 2023-07-22 15:08:31.193031 PyQt6-6.5.2/sip/QtBluetooth/qbluetoothhostinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2570 2023-07-22 15:08:31.191012 PyQt6-6.5.2/sip/QtBluetooth/qbluetoothlocaldevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3360 2023-07-22 15:08:31.192134 PyQt6-6.5.2/sip/QtBluetooth/qbluetoothserver.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2467 2023-07-22 15:08:31.184159 PyQt6-6.5.2/sip/QtBluetooth/qbluetoothservicediscoveryagent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3324 2023-07-22 15:08:31.193643 PyQt6-6.5.2/sip/QtBluetooth/qbluetoothserviceinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5134 2023-07-22 15:08:31.180753 PyQt6-6.5.2/sip/QtBluetooth/qbluetoothsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9422 2023-07-22 15:08:31.189448 PyQt6-6.5.2/sip/QtBluetooth/qbluetoothuuid.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2334 2023-07-22 15:08:31.178770 PyQt6-6.5.2/sip/QtBluetooth/qlowenergyadvertisingdata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3006 2023-07-22 15:08:31.178239 PyQt6-6.5.2/sip/QtBluetooth/qlowenergyadvertisingparameters.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2262 2023-07-22 15:08:31.182491 PyQt6-6.5.2/sip/QtBluetooth/qlowenergycharacteristic.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2472 2023-07-22 15:08:31.189943 PyQt6-6.5.2/sip/QtBluetooth/qlowenergycharacteristicdata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1843 2023-07-22 15:08:31.192584 PyQt6-6.5.2/sip/QtBluetooth/qlowenergyconnectionparameters.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4355 2023-07-22 15:08:31.181479 PyQt6-6.5.2/sip/QtBluetooth/qlowenergycontroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1568 2023-07-22 15:08:31.186802 PyQt6-6.5.2/sip/QtBluetooth/qlowenergydescriptor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2201 2023-07-22 15:08:31.187820 PyQt6-6.5.2/sip/QtBluetooth/qlowenergydescriptordata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3661 2023-07-22 15:08:31.184824 PyQt6-6.5.2/sip/QtBluetooth/qlowenergyservice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2201 2023-07-22 15:08:31.187297 PyQt6-6.5.2/sip/QtBluetooth/qlowenergyservicedata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3358 2023-07-22 15:08:31.185673 PyQt6-6.5.2/sip/QtBluetooth/qpybluetooth_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4039 2023-07-22 15:08:31.183612 PyQt6-6.5.2/sip/QtBluetooth/qpybluetooth_qmultihash.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2860 2023-07-22 15:08:31.177494 PyQt6-6.5.2/sip/QtBluetooth/qpybluetooth_quint128.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.893801 PyQt6-6.5.2/sip/QtCore/
+-rw-r--r--   0 phil       (501) staff       (20)     6347 2023-07-22 15:08:31.887981 PyQt6-6.5.2/sip/QtCore/QtCoremod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2557 2023-07-22 15:08:31.999871 PyQt6-6.5.2/sip/QtCore/qabstractanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2449 2023-07-22 15:08:31.977951 PyQt6-6.5.2/sip/QtCore/qabstracteventdispatcher.sip
+-rw-r--r--   0 phil       (501) staff       (20)    13972 2023-07-22 15:08:31.835343 PyQt6-6.5.2/sip/QtCore/qabstractitemmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1335 2023-07-22 15:08:31.998407 PyQt6-6.5.2/sip/QtCore/qabstractnativeeventfilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3493 2023-07-22 15:08:31.983595 PyQt6-6.5.2/sip/QtCore/qabstractproxymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1649 2023-07-22 15:08:31.845575 PyQt6-6.5.2/sip/QtCore/qanimationgroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2718 2023-07-22 15:08:31.799084 PyQt6-6.5.2/sip/QtCore/qanystringview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1338 2023-07-22 15:08:31.847734 PyQt6-6.5.2/sip/QtCore/qbasictimer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2909 2023-07-22 15:08:31.981220 PyQt6-6.5.2/sip/QtCore/qbitarray.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3743 2023-07-22 15:08:31.828837 PyQt6-6.5.2/sip/QtCore/qbuffer.sip
+-rw-r--r--   0 phil       (501) staff       (20)    14499 2023-07-22 15:08:31.952804 PyQt6-6.5.2/sip/QtCore/qbytearray.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1144 2023-07-22 15:08:31.846074 PyQt6-6.5.2/sip/QtCore/qbytearrayalgorithms.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2976 2023-07-22 15:08:31.836312 PyQt6-6.5.2/sip/QtCore/qbytearraylist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1906 2023-07-22 15:08:31.987224 PyQt6-6.5.2/sip/QtCore/qbytearraymatcher.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2399 2023-07-22 15:08:31.992654 PyQt6-6.5.2/sip/QtCore/qbytearrayview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3336 2023-07-22 15:08:31.825751 PyQt6-6.5.2/sip/QtCore/qcalendar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2452 2023-07-22 15:08:31.925365 PyQt6-6.5.2/sip/QtCore/qcborcommon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3894 2023-07-22 15:08:31.987921 PyQt6-6.5.2/sip/QtCore/qcborstreamreader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2475 2023-07-22 15:08:31.950180 PyQt6-6.5.2/sip/QtCore/qcborstreamwriter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1591 2023-07-22 15:08:31.892072 PyQt6-6.5.2/sip/QtCore/qchar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2161 2023-07-22 15:08:31.844664 PyQt6-6.5.2/sip/QtCore/qcollator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2203 2023-07-22 15:08:31.953300 PyQt6-6.5.2/sip/QtCore/qcommandlineoption.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2825 2023-07-22 15:08:31.981750 PyQt6-6.5.2/sip/QtCore/qcommandlineparser.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4086 2023-07-22 15:08:31.980633 PyQt6-6.5.2/sip/QtCore/qconcatenatetablesproxymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)    12147 2023-07-22 15:08:31.853528 PyQt6-6.5.2/sip/QtCore/qcoreapplication.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7083 2023-07-22 15:08:31.882551 PyQt6-6.5.2/sip/QtCore/qcoreevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2546 2023-07-22 15:08:31.880547 PyQt6-6.5.2/sip/QtCore/qcryptographichash.sip
+-rw-r--r--   0 phil       (501) staff       (20)    11005 2023-07-22 15:08:31.886943 PyQt6-6.5.2/sip/QtCore/qdatastream.sip
+-rw-r--r--   0 phil       (501) staff       (20)    15385 2023-07-22 15:08:31.946324 PyQt6-6.5.2/sip/QtCore/qdatetime.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2791 2023-07-22 15:08:31.949604 PyQt6-6.5.2/sip/QtCore/qdeadlinetimer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6571 2023-07-22 15:08:31.889639 PyQt6-6.5.2/sip/QtCore/qdir.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2019 2023-07-22 15:08:31.827606 PyQt6-6.5.2/sip/QtCore/qdiriterator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6671 2023-07-22 15:08:31.833519 PyQt6-6.5.2/sip/QtCore/qeasingcurve.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1833 2023-07-22 15:08:31.884735 PyQt6-6.5.2/sip/QtCore/qelapsedtimer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2197 2023-07-22 15:08:31.979618 PyQt6-6.5.2/sip/QtCore/qeventloop.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3031 2023-07-22 15:08:31.990122 PyQt6-6.5.2/sip/QtCore/qfile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6316 2023-07-22 15:08:31.949123 PyQt6-6.5.2/sip/QtCore/qfiledevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3371 2023-07-22 15:08:31.891123 PyQt6-6.5.2/sip/QtCore/qfileinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1365 2023-07-22 15:08:31.938442 PyQt6-6.5.2/sip/QtCore/qfileselector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1597 2023-07-22 15:08:31.938878 PyQt6-6.5.2/sip/QtCore/qfilesystemwatcher.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1457 2023-07-22 15:08:31.829326 PyQt6-6.5.2/sip/QtCore/qflags.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5036 2023-07-22 15:08:31.947358 PyQt6-6.5.2/sip/QtCore/qglobal.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3095 2023-07-22 15:08:31.995078 PyQt6-6.5.2/sip/QtCore/qidentityproxymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)    12510 2023-07-22 15:08:31.906901 PyQt6-6.5.2/sip/QtCore/qiodevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1380 2023-07-22 15:08:31.974970 PyQt6-6.5.2/sip/QtCore/qiodevicebase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8829 2023-07-22 15:08:31.994524 PyQt6-6.5.2/sip/QtCore/qitemselectionmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3263 2023-07-22 15:08:31.950916 PyQt6-6.5.2/sip/QtCore/qjsonarray.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2862 2023-07-22 15:08:31.903625 PyQt6-6.5.2/sip/QtCore/qjsondocument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3500 2023-07-22 15:08:31.840227 PyQt6-6.5.2/sip/QtCore/qjsonobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2892 2023-07-22 15:08:31.941708 PyQt6-6.5.2/sip/QtCore/qjsonvalue.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2418 2023-07-22 15:08:31.902646 PyQt6-6.5.2/sip/QtCore/qlibrary.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1661 2023-07-22 15:08:31.905125 PyQt6-6.5.2/sip/QtCore/qlibraryinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5198 2023-07-22 15:08:31.904597 PyQt6-6.5.2/sip/QtCore/qline.sip
+-rw-r--r--   0 phil       (501) staff       (20)    28155 2023-07-22 15:08:31.879818 PyQt6-6.5.2/sip/QtCore/qlocale.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1671 2023-07-22 15:08:31.836824 PyQt6-6.5.2/sip/QtCore/qlockfile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6581 2023-07-22 15:08:31.979090 PyQt6-6.5.2/sip/QtCore/qlogging.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1612 2023-07-22 15:08:31.830690 PyQt6-6.5.2/sip/QtCore/qloggingcategory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4347 2023-07-22 15:08:31.890382 PyQt6-6.5.2/sip/QtCore/qmargins.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1862 2023-07-22 15:08:31.988644 PyQt6-6.5.2/sip/QtCore/qmessageauthenticationcode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9269 2023-07-22 15:08:31.944266 PyQt6-6.5.2/sip/QtCore/qmetaobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4273 2023-07-22 15:08:31.854440 PyQt6-6.5.2/sip/QtCore/qmetatype.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1954 2023-07-22 15:08:31.827142 PyQt6-6.5.2/sip/QtCore/qmimedata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2082 2023-07-22 15:08:31.942546 PyQt6-6.5.2/sip/QtCore/qmimedatabase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1812 2023-07-22 15:08:31.937510 PyQt6-6.5.2/sip/QtCore/qmimetype.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1527 2023-07-22 15:08:31.826230 PyQt6-6.5.2/sip/QtCore/qmutex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1961 2023-07-22 15:08:32.000950 PyQt6-6.5.2/sip/QtCore/qmutexlocker.sip
+-rw-r--r--   0 phil       (501) staff       (20)    34263 2023-07-22 15:08:31.899148 PyQt6-6.5.2/sip/QtCore/qnamespace.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1410 2023-07-22 15:08:31.938003 PyQt6-6.5.2/sip/QtCore/qnumeric.sip
+-rw-r--r--   0 phil       (501) staff       (20)    20265 2023-07-22 15:08:31.839393 PyQt6-6.5.2/sip/QtCore/qobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1248 2023-07-22 15:08:31.977439 PyQt6-6.5.2/sip/QtCore/qobjectcleanuphandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8135 2023-07-22 15:08:31.976019 PyQt6-6.5.2/sip/QtCore/qobjectdefs.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7658 2023-07-22 15:08:31.841291 PyQt6-6.5.2/sip/QtCore/qoperatingsystemversion.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1502 2023-07-22 15:08:31.849388 PyQt6-6.5.2/sip/QtCore/qparallelanimationgroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1373 2023-07-22 15:08:31.942953 PyQt6-6.5.2/sip/QtCore/qpauseanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7564 2023-07-22 15:08:31.847335 PyQt6-6.5.2/sip/QtCore/qpermissions.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1555 2023-07-22 15:08:31.826666 PyQt6-6.5.2/sip/QtCore/qpluginloader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4684 2023-07-22 15:08:31.954088 PyQt6-6.5.2/sip/QtCore/qpoint.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7887 2023-07-22 15:08:31.986314 PyQt6-6.5.2/sip/QtCore/qprocess.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1695 2023-07-22 15:08:31.937037 PyQt6-6.5.2/sip/QtCore/qpropertyanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)    11135 2023-07-22 15:08:31.997371 PyQt6-6.5.2/sip/QtCore/qpycore_qhash.sip
+-rw-r--r--   0 phil       (501) staff       (20)    30380 2023-07-22 15:08:31.932235 PyQt6-6.5.2/sip/QtCore/qpycore_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10053 2023-07-22 15:08:31.991947 PyQt6-6.5.2/sip/QtCore/qpycore_qmap.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5229 2023-07-22 15:08:31.848881 PyQt6-6.5.2/sip/QtCore/qpycore_qset.sip
+-rw-r--r--   0 phil       (501) staff       (20)    11619 2023-07-22 15:08:31.844173 PyQt6-6.5.2/sip/QtCore/qpycore_std_pair.sip
+-rw-r--r--   0 phil       (501) staff       (20)      976 2023-07-22 15:08:31.980024 PyQt6-6.5.2/sip/QtCore/qpycore_virtual_error_handler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1863 2023-07-22 15:08:31.849817 PyQt6-6.5.2/sip/QtCore/qrandom.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2706 2023-07-22 15:08:31.948007 PyQt6-6.5.2/sip/QtCore/qreadwritelock.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9654 2023-07-22 15:08:31.985178 PyQt6-6.5.2/sip/QtCore/qrect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7257 2023-07-22 15:08:31.999311 PyQt6-6.5.2/sip/QtCore/qregularexpression.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2661 2023-07-22 15:08:31.883122 PyQt6-6.5.2/sip/QtCore/qresource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1718 2023-07-22 15:08:31.903067 PyQt6-6.5.2/sip/QtCore/qrunnable.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2390 2023-07-22 15:08:31.993277 PyQt6-6.5.2/sip/QtCore/qsavefile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1620 2023-07-22 15:08:31.977028 PyQt6-6.5.2/sip/QtCore/qsemaphore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1721 2023-07-22 15:08:31.986738 PyQt6-6.5.2/sip/QtCore/qsequentialanimationgroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5109 2023-07-22 15:08:31.934005 PyQt6-6.5.2/sip/QtCore/qsettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2332 2023-07-22 15:08:31.901216 PyQt6-6.5.2/sip/QtCore/qsharedmemory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1641 2023-07-22 15:08:31.954500 PyQt6-6.5.2/sip/QtCore/qsignalmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5173 2023-07-22 15:08:31.933148 PyQt6-6.5.2/sip/QtCore/qsize.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1673 2023-07-22 15:08:31.829805 PyQt6-6.5.2/sip/QtCore/qsocketnotifier.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5908 2023-07-22 15:08:31.902156 PyQt6-6.5.2/sip/QtCore/qsortfilterproxymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2598 2023-07-22 15:08:31.845185 PyQt6-6.5.2/sip/QtCore/qstandardpaths.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1966 2023-07-22 15:08:31.884227 PyQt6-6.5.2/sip/QtCore/qstorageinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1518 2023-07-22 15:08:31.832251 PyQt6-6.5.2/sip/QtCore/qstring.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3205 2023-07-22 15:08:31.841942 PyQt6-6.5.2/sip/QtCore/qstringconverter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2134 2023-07-22 15:08:31.983108 PyQt6-6.5.2/sip/QtCore/qstringconverter_base.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2937 2023-07-22 15:08:31.941138 PyQt6-6.5.2/sip/QtCore/qstringlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2403 2023-07-22 15:08:31.900157 PyQt6-6.5.2/sip/QtCore/qstringlistmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1537 2023-07-22 15:08:31.851786 PyQt6-6.5.2/sip/QtCore/qstringview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1572 2023-07-22 15:08:31.830263 PyQt6-6.5.2/sip/QtCore/qsysinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1790 2023-07-22 15:08:31.881143 PyQt6-6.5.2/sip/QtCore/qsystemsemaphore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1463 2023-07-22 15:08:31.926033 PyQt6-6.5.2/sip/QtCore/qtemporarydir.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1798 2023-07-22 15:08:31.833934 PyQt6-6.5.2/sip/QtCore/qtemporaryfile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1455 2023-07-22 15:08:31.893157 PyQt6-6.5.2/sip/QtCore/qtenvironmentvariables.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1998 2023-07-22 15:08:31.976556 PyQt6-6.5.2/sip/QtCore/qtextboundaryfinder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5603 2023-07-22 15:08:31.989550 PyQt6-6.5.2/sip/QtCore/qtextstream.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2691 2023-07-22 15:08:31.892614 PyQt6-6.5.2/sip/QtCore/qthread.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4994 2023-07-22 15:08:31.850687 PyQt6-6.5.2/sip/QtCore/qthreadpool.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2431 2023-07-22 15:08:31.825109 PyQt6-6.5.2/sip/QtCore/qtimeline.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2585 2023-07-22 15:08:31.851229 PyQt6-6.5.2/sip/QtCore/qtimer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5446 2023-07-22 15:08:31.831549 PyQt6-6.5.2/sip/QtCore/qtimezone.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1837 2023-07-22 15:08:31.900535 PyQt6-6.5.2/sip/QtCore/qtranslator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2945 2023-07-22 15:08:31.891570 PyQt6-6.5.2/sip/QtCore/qtransposeproxymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1057 2023-07-22 15:08:31.942084 PyQt6-6.5.2/sip/QtCore/qtversion.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1843 2023-07-22 15:08:31.828155 PyQt6-6.5.2/sip/QtCore/qtypes.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7344 2023-07-22 15:08:31.939844 PyQt6-6.5.2/sip/QtCore/qurl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2784 2023-07-22 15:08:31.883704 PyQt6-6.5.2/sip/QtCore/qurlquery.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3479 2023-07-22 15:08:31.998030 PyQt6-6.5.2/sip/QtCore/quuid.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3169 2023-07-22 15:08:31.888622 PyQt6-6.5.2/sip/QtCore/qvariant.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2197 2023-07-22 15:08:32.000430 PyQt6-6.5.2/sip/QtCore/qvariantanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3856 2023-07-22 15:08:31.982416 PyQt6-6.5.2/sip/QtCore/qversionnumber.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1578 2023-07-22 15:08:31.899741 PyQt6-6.5.2/sip/QtCore/qwaitcondition.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1577 2023-07-22 15:08:31.940366 PyQt6-6.5.2/sip/QtCore/qwineventnotifier.sip
+-rw-r--r--   0 phil       (501) staff       (20)    15570 2023-07-22 15:08:31.936549 PyQt6-6.5.2/sip/QtCore/qxmlstream.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.786784 PyQt6-6.5.2/sip/QtDBus/
+-rw-r--r--   0 phil       (501) staff       (20)     2340 2023-07-22 15:08:31.574998 PyQt6-6.5.2/sip/QtDBus/QtDBusmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1271 2023-07-22 15:08:31.547300 PyQt6-6.5.2/sip/QtDBus/qdbusabstractadaptor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7394 2023-07-22 15:08:31.550643 PyQt6-6.5.2/sip/QtDBus/qdbusabstractinterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4871 2023-07-22 15:08:31.548258 PyQt6-6.5.2/sip/QtDBus/qdbusargument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9428 2023-07-22 15:08:31.545897 PyQt6-6.5.2/sip/QtDBus/qdbusconnection.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2976 2023-07-22 15:08:31.549210 PyQt6-6.5.2/sip/QtDBus/qdbusconnectioninterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1933 2023-07-22 15:08:31.551656 PyQt6-6.5.2/sip/QtDBus/qdbuserror.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2507 2023-07-22 15:08:31.546444 PyQt6-6.5.2/sip/QtDBus/qdbusextratypes.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1299 2023-07-22 15:08:31.549566 PyQt6-6.5.2/sip/QtDBus/qdbusinterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3015 2023-07-22 15:08:31.546936 PyQt6-6.5.2/sip/QtDBus/qdbusmessage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1745 2023-07-22 15:08:31.548697 PyQt6-6.5.2/sip/QtDBus/qdbuspendingcall.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2225 2023-07-22 15:08:31.551181 PyQt6-6.5.2/sip/QtDBus/qdbusservicewatcher.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1450 2023-07-22 15:08:31.544219 PyQt6-6.5.2/sip/QtDBus/qdbusunixfiledescriptor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1739 2023-07-22 15:08:31.544668 PyQt6-6.5.2/sip/QtDBus/qpydbuspendingreply.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5291 2023-07-22 15:08:31.543844 PyQt6-6.5.2/sip/QtDBus/qpydbusreply.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.712965 PyQt6-6.5.2/sip/QtDesigner/
+-rw-r--r--   0 phil       (501) staff       (20)     2809 2023-07-22 15:08:31.284492 PyQt6-6.5.2/sip/QtDesigner/QtDesignermod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1493 2023-07-22 15:08:31.276822 PyQt6-6.5.2/sip/QtDesigner/abstractactioneditor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1457 2023-07-22 15:08:31.285433 PyQt6-6.5.2/sip/QtDesigner/abstractformbuilder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2021 2023-07-22 15:08:31.282649 PyQt6-6.5.2/sip/QtDesigner/abstractformeditor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4737 2023-07-22 15:08:31.277528 PyQt6-6.5.2/sip/QtDesigner/abstractformwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2532 2023-07-22 15:08:31.280852 PyQt6-6.5.2/sip/QtDesigner/abstractformwindowcursor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3286 2023-07-22 15:08:31.251174 PyQt6-6.5.2/sip/QtDesigner/abstractformwindowmanager.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1402 2023-07-22 15:08:31.283576 PyQt6-6.5.2/sip/QtDesigner/abstractobjectinspector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1736 2023-07-22 15:08:31.284024 PyQt6-6.5.2/sip/QtDesigner/abstractpropertyeditor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1397 2023-07-22 15:08:31.281738 PyQt6-6.5.2/sip/QtDesigner/abstractwidgetbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1633 2023-07-22 15:08:31.282203 PyQt6-6.5.2/sip/QtDesigner/container.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1884 2023-07-22 15:08:31.279857 PyQt6-6.5.2/sip/QtDesigner/customwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1438 2023-07-22 15:08:31.283057 PyQt6-6.5.2/sip/QtDesigner/default_extensionfactory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1571 2023-07-22 15:08:31.280305 PyQt6-6.5.2/sip/QtDesigner/extension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1345 2023-07-22 15:08:31.278432 PyQt6-6.5.2/sip/QtDesigner/formbuilder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1993 2023-07-22 15:08:31.279373 PyQt6-6.5.2/sip/QtDesigner/membersheet.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2084 2023-07-22 15:08:31.275731 PyQt6-6.5.2/sip/QtDesigner/propertysheet.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3397 2023-07-22 15:08:31.276380 PyQt6-6.5.2/sip/QtDesigner/qextensionmanager.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1228 2023-07-22 15:08:31.250610 PyQt6-6.5.2/sip/QtDesigner/qpydesignercontainerextension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1308 2023-07-22 15:08:31.275108 PyQt6-6.5.2/sip/QtDesigner/qpydesignercustomwidgetcollectionplugin.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1235 2023-07-22 15:08:31.278002 PyQt6-6.5.2/sip/QtDesigner/qpydesignercustomwidgetplugin.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1242 2023-07-22 15:08:31.284928 PyQt6-6.5.2/sip/QtDesigner/qpydesignermembersheetextension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1259 2023-07-22 15:08:31.281314 PyQt6-6.5.2/sip/QtDesigner/qpydesignerpropertysheetextension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1221 2023-07-22 15:08:31.278901 PyQt6-6.5.2/sip/QtDesigner/qpydesignertaskmenuextension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1300 2023-07-22 15:08:31.251556 PyQt6-6.5.2/sip/QtDesigner/taskmenu.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.767410 PyQt6-6.5.2/sip/QtGui/
+-rw-r--r--   0 phil       (501) staff       (20)     4178 2023-07-22 15:08:31.476347 PyQt6-6.5.2/sip/QtGui/QtGuimod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1404 2023-07-22 15:08:31.455758 PyQt6-6.5.2/sip/QtGui/opengl_types.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1809 2023-07-22 15:08:31.384263 PyQt6-6.5.2/sip/QtGui/qabstractfileiconprovider.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3726 2023-07-22 15:08:31.380759 PyQt6-6.5.2/sip/QtGui/qabstracttextdocumentlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4672 2023-07-22 15:08:31.440147 PyQt6-6.5.2/sip/QtGui/qaction.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1946 2023-07-22 15:08:31.385469 PyQt6-6.5.2/sip/QtGui/qactiongroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1568 2023-07-22 15:08:31.479422 PyQt6-6.5.2/sip/QtGui/qbackingstore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1848 2023-07-22 15:08:31.396404 PyQt6-6.5.2/sip/QtGui/qbitmap.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10739 2023-07-22 15:08:31.491187 PyQt6-6.5.2/sip/QtGui/qbrush.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3492 2023-07-22 15:08:31.491768 PyQt6-6.5.2/sip/QtGui/qclipboard.sip
+-rw-r--r--   0 phil       (501) staff       (20)    12351 2023-07-22 15:08:31.430051 PyQt6-6.5.2/sip/QtGui/qcolor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4476 2023-07-22 15:08:31.388674 PyQt6-6.5.2/sip/QtGui/qcolorspace.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1554 2023-07-22 15:08:31.401699 PyQt6-6.5.2/sip/QtGui/qcolortransform.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3042 2023-07-22 15:08:31.443327 PyQt6-6.5.2/sip/QtGui/qcursor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2418 2023-07-22 15:08:31.481106 PyQt6-6.5.2/sip/QtGui/qdesktopservices.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1971 2023-07-22 15:08:31.487417 PyQt6-6.5.2/sip/QtGui/qdrag.sip
+-rw-r--r--   0 phil       (501) staff       (20)    23127 2023-07-22 15:08:31.485051 PyQt6-6.5.2/sip/QtGui/qevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2495 2023-07-22 15:08:31.451707 PyQt6-6.5.2/sip/QtGui/qeventpoint.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4840 2023-07-22 15:08:31.405227 PyQt6-6.5.2/sip/QtGui/qfilesystemmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5846 2023-07-22 15:08:31.387318 PyQt6-6.5.2/sip/QtGui/qfont.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3645 2023-07-22 15:08:31.387996 PyQt6-6.5.2/sip/QtGui/qfontdatabase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1495 2023-07-22 15:08:31.391478 PyQt6-6.5.2/sip/QtGui/qfontinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6681 2023-07-22 15:08:31.406173 PyQt6-6.5.2/sip/QtGui/qfontmetrics.sip
+-rw-r--r--   0 phil       (501) staff       (20)    25528 2023-07-22 15:08:31.447160 PyQt6-6.5.2/sip/QtGui/qgenericmatrix.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2611 2023-07-22 15:08:31.452256 PyQt6-6.5.2/sip/QtGui/qglyphrun.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9603 2023-07-22 15:08:31.488683 PyQt6-6.5.2/sip/QtGui/qguiapplication.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4245 2023-07-22 15:08:31.451107 PyQt6-6.5.2/sip/QtGui/qicon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2384 2023-07-22 15:08:31.389273 PyQt6-6.5.2/sip/QtGui/qiconengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)    13954 2023-07-22 15:08:31.394825 PyQt6-6.5.2/sip/QtGui/qimage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2751 2023-07-22 15:08:31.435783 PyQt6-6.5.2/sip/QtGui/qimageiohandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3480 2023-07-22 15:08:31.477073 PyQt6-6.5.2/sip/QtGui/qimagereader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2666 2023-07-22 15:08:31.442732 PyQt6-6.5.2/sip/QtGui/qimagewriter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2591 2023-07-22 15:08:31.393154 PyQt6-6.5.2/sip/QtGui/qinputdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2303 2023-07-22 15:08:31.486951 PyQt6-6.5.2/sip/QtGui/qinputmethod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7031 2023-07-22 15:08:31.454217 PyQt6-6.5.2/sip/QtGui/qkeysequence.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9803 2023-07-22 15:08:31.390618 PyQt6-6.5.2/sip/QtGui/qmatrix4x4.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2857 2023-07-22 15:08:31.485732 PyQt6-6.5.2/sip/QtGui/qmovie.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1585 2023-07-22 15:08:31.450415 PyQt6-6.5.2/sip/QtGui/qoffscreensurface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2580 2023-07-22 15:08:31.397528 PyQt6-6.5.2/sip/QtGui/qopenglcontext.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1686 2023-07-22 15:08:31.391041 PyQt6-6.5.2/sip/QtGui/qpagedpaintdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3104 2023-07-22 15:08:31.400697 PyQt6-6.5.2/sip/QtGui/qpagelayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2145 2023-07-22 15:08:31.439256 PyQt6-6.5.2/sip/QtGui/qpageranges.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5591 2023-07-22 15:08:31.435102 PyQt6-6.5.2/sip/QtGui/qpagesize.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1994 2023-07-22 15:08:31.425192 PyQt6-6.5.2/sip/QtGui/qpaintdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1415 2023-07-22 15:08:31.475524 PyQt6-6.5.2/sip/QtGui/qpaintdevicewindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5665 2023-07-22 15:08:31.478063 PyQt6-6.5.2/sip/QtGui/qpaintengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)    21088 2023-07-22 15:08:31.438242 PyQt6-6.5.2/sip/QtGui/qpainter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6554 2023-07-22 15:08:31.448130 PyQt6-6.5.2/sip/QtGui/qpainterpath.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4511 2023-07-22 15:08:31.386238 PyQt6-6.5.2/sip/QtGui/qpalette.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1885 2023-07-22 15:08:31.432082 PyQt6-6.5.2/sip/QtGui/qpdfwriter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3397 2023-07-22 15:08:31.384946 PyQt6-6.5.2/sip/QtGui/qpen.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2021 2023-07-22 15:08:31.455311 PyQt6-6.5.2/sip/QtGui/qpicture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5520 2023-07-22 15:08:31.433860 PyQt6-6.5.2/sip/QtGui/qpixelformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4917 2023-07-22 15:08:31.377338 PyQt6-6.5.2/sip/QtGui/qpixmap.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2240 2023-07-22 15:08:31.430734 PyQt6-6.5.2/sip/QtGui/qpixmapcache.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2499 2023-07-22 15:08:31.486271 PyQt6-6.5.2/sip/QtGui/qpointingdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)    11987 2023-07-22 15:08:31.400129 PyQt6-6.5.2/sip/QtGui/qpolygon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2719 2023-07-22 15:08:31.431542 PyQt6-6.5.2/sip/QtGui/qpygui_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5076 2023-07-22 15:08:31.398276 PyQt6-6.5.2/sip/QtGui/qquaternion.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1230 2023-07-22 15:08:31.448548 PyQt6-6.5.2/sip/QtGui/qrasterwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3616 2023-07-22 15:08:31.396964 PyQt6-6.5.2/sip/QtGui/qrawfont.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3768 2023-07-22 15:08:31.452945 PyQt6-6.5.2/sip/QtGui/qregion.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1271 2023-07-22 15:08:31.376569 PyQt6-6.5.2/sip/QtGui/qrgb.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2141 2023-07-22 15:08:31.480585 PyQt6-6.5.2/sip/QtGui/qrgba64.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3073 2023-07-22 15:08:31.395388 PyQt6-6.5.2/sip/QtGui/qscreen.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1990 2023-07-22 15:08:31.475093 PyQt6-6.5.2/sip/QtGui/qsessionmanager.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6080 2023-07-22 15:08:31.478992 PyQt6-6.5.2/sip/QtGui/qshortcut.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9704 2023-07-22 15:08:31.426411 PyQt6-6.5.2/sip/QtGui/qstandarditemmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1953 2023-07-22 15:08:31.401129 PyQt6-6.5.2/sip/QtGui/qstatictext.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3060 2023-07-22 15:08:31.480072 PyQt6-6.5.2/sip/QtGui/qstylehints.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1634 2023-07-22 15:08:31.395954 PyQt6-6.5.2/sip/QtGui/qsurface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3651 2023-07-22 15:08:31.383771 PyQt6-6.5.2/sip/QtGui/qsurfaceformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2965 2023-07-22 15:08:31.380130 PyQt6-6.5.2/sip/QtGui/qsyntaxhighlighter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5531 2023-07-22 15:08:31.441559 PyQt6-6.5.2/sip/QtGui/qtextcursor.sip
+-rw-r--r--   0 phil       (501) staff       (20)    12118 2023-07-22 15:08:31.428215 PyQt6-6.5.2/sip/QtGui/qtextdocument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1935 2023-07-22 15:08:31.377883 PyQt6-6.5.2/sip/QtGui/qtextdocumentfragment.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1714 2023-07-22 15:08:31.481555 PyQt6-6.5.2/sip/QtGui/qtextdocumentwriter.sip
+-rw-r--r--   0 phil       (501) staff       (20)    19535 2023-07-22 15:08:31.404390 PyQt6-6.5.2/sip/QtGui/qtextformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5890 2023-07-22 15:08:31.379461 PyQt6-6.5.2/sip/QtGui/qtextlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1462 2023-07-22 15:08:31.378447 PyQt6-6.5.2/sip/QtGui/qtextlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7691 2023-07-22 15:08:31.382546 PyQt6-6.5.2/sip/QtGui/qtextobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2786 2023-07-22 15:08:31.456403 PyQt6-6.5.2/sip/QtGui/qtextoption.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2569 2023-07-22 15:08:31.489241 PyQt6-6.5.2/sip/QtGui/qtexttable.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5139 2023-07-22 15:08:31.432950 PyQt6-6.5.2/sip/QtGui/qtransform.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2042 2023-07-22 15:08:31.383073 PyQt6-6.5.2/sip/QtGui/qundogroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3004 2023-07-22 15:08:31.442192 PyQt6-6.5.2/sip/QtGui/qundostack.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1692 2023-07-22 15:08:31.440639 PyQt6-6.5.2/sip/QtGui/qutimimeconverter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3361 2023-07-22 15:08:31.454871 PyQt6-6.5.2/sip/QtGui/qvalidator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9152 2023-07-22 15:08:31.449778 PyQt6-6.5.2/sip/QtGui/qvectornd.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7236 2023-07-22 15:08:31.392601 PyQt6-6.5.2/sip/QtGui/qwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1009 2023-07-22 15:08:31.438715 PyQt6-6.5.2/sip/QtGui/qwindowdefs.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.719353 PyQt6-6.5.2/sip/QtHelp/
+-rw-r--r--   0 phil       (501) staff       (20)     2347 2023-07-22 15:08:31.291997 PyQt6-6.5.2/sip/QtHelp/QtHelpmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1429 2023-07-22 15:08:31.288891 PyQt6-6.5.2/sip/QtHelp/qcompressedhelpinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2348 2023-07-22 15:08:31.291140 PyQt6-6.5.2/sip/QtHelp/qhelpcontentwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1361 2023-07-22 15:08:31.291557 PyQt6-6.5.2/sip/QtHelp/qhelpengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4184 2023-07-22 15:08:31.290571 PyQt6-6.5.2/sip/QtHelp/qhelpenginecore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1430 2023-07-22 15:08:31.289802 PyQt6-6.5.2/sip/QtHelp/qhelpfilterdata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1889 2023-07-22 15:08:31.294814 PyQt6-6.5.2/sip/QtHelp/qhelpfilterengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1457 2023-07-22 15:08:31.294309 PyQt6-6.5.2/sip/QtHelp/qhelpfiltersettingswidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1836 2023-07-22 15:08:31.292481 PyQt6-6.5.2/sip/QtHelp/qhelpindexwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1048 2023-07-22 15:08:31.293921 PyQt6-6.5.2/sip/QtHelp/qhelplink.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2399 2023-07-22 15:08:31.293122 PyQt6-6.5.2/sip/QtHelp/qhelpsearchengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1552 2023-07-22 15:08:31.293562 PyQt6-6.5.2/sip/QtHelp/qhelpsearchquerywidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1222 2023-07-22 15:08:31.289331 PyQt6-6.5.2/sip/QtHelp/qhelpsearchresultwidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.840581 PyQt6-6.5.2/sip/QtMultimedia/
+-rw-r--r--   0 phil       (501) staff       (20)     2656 2023-07-22 15:08:31.746233 PyQt6-6.5.2/sip/QtMultimedia/QtMultimediamod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1516 2023-07-22 15:08:31.775513 PyQt6-6.5.2/sip/QtMultimedia/qaudio.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1993 2023-07-22 15:08:31.743251 PyQt6-6.5.2/sip/QtMultimedia/qaudiobuffer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2206 2023-07-22 15:08:31.779993 PyQt6-6.5.2/sip/QtMultimedia/qaudiodecoder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1930 2023-07-22 15:08:31.742262 PyQt6-6.5.2/sip/QtMultimedia/qaudiodevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3341 2023-07-22 15:08:31.746873 PyQt6-6.5.2/sip/QtMultimedia/qaudioformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1565 2023-07-22 15:08:31.777509 PyQt6-6.5.2/sip/QtMultimedia/qaudioinput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1567 2023-07-22 15:08:31.742805 PyQt6-6.5.2/sip/QtMultimedia/qaudiooutput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1838 2023-07-22 15:08:31.744276 PyQt6-6.5.2/sip/QtMultimedia/qaudiosink.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1862 2023-07-22 15:08:31.776321 PyQt6-6.5.2/sip/QtMultimedia/qaudiosource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7429 2023-07-22 15:08:31.748107 PyQt6-6.5.2/sip/QtMultimedia/qcamera.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2093 2023-07-22 15:08:31.749161 PyQt6-6.5.2/sip/QtMultimedia/qcameradevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3030 2023-07-22 15:08:31.743835 PyQt6-6.5.2/sip/QtMultimedia/qimagecapture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2160 2023-07-22 15:08:31.783601 PyQt6-6.5.2/sip/QtMultimedia/qmediacapturesession.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1540 2023-07-22 15:08:31.782097 PyQt6-6.5.2/sip/QtMultimedia/qmediadevices.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3349 2023-07-22 15:08:31.781448 PyQt6-6.5.2/sip/QtMultimedia/qmediaformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2186 2023-07-22 15:08:31.749690 PyQt6-6.5.2/sip/QtMultimedia/qmediametadata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4095 2023-07-22 15:08:31.779273 PyQt6-6.5.2/sip/QtMultimedia/qmediaplayer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3680 2023-07-22 15:08:31.745092 PyQt6-6.5.2/sip/QtMultimedia/qmediarecorder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3046 2023-07-22 15:08:31.748668 PyQt6-6.5.2/sip/QtMultimedia/qmediatimerange.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10957 2023-07-22 15:08:31.751807 PyQt6-6.5.2/sip/QtMultimedia/qpymultimedia_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1795 2023-07-22 15:08:31.778322 PyQt6-6.5.2/sip/QtMultimedia/qscreencapture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2198 2023-07-22 15:08:31.777049 PyQt6-6.5.2/sip/QtMultimedia/qsoundeffect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3181 2023-07-22 15:08:31.745755 PyQt6-6.5.2/sip/QtMultimedia/qvideoframe.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4710 2023-07-22 15:08:31.783062 PyQt6-6.5.2/sip/QtMultimedia/qvideoframeformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1508 2023-07-22 15:08:31.780609 PyQt6-6.5.2/sip/QtMultimedia/qvideosink.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.894869 PyQt6-6.5.2/sip/QtMultimediaWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2083 2023-07-22 15:08:32.001379 PyQt6-6.5.2/sip/QtMultimediaWidgets/QtMultimediaWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2007 2023-07-22 15:08:32.002478 PyQt6-6.5.2/sip/QtMultimediaWidgets/qgraphicsvideoitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2399 2023-07-22 15:08:32.001918 PyQt6-6.5.2/sip/QtMultimediaWidgets/qvideowidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.704651 PyQt6-6.5.2/sip/QtNetwork/
+-rw-r--r--   0 phil       (501) staff       (20)     3123 2023-07-22 15:08:31.197341 PyQt6-6.5.2/sip/QtNetwork/QtNetworkmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2995 2023-07-22 15:08:31.235162 PyQt6-6.5.2/sip/QtNetwork/qabstractnetworkcache.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10970 2023-07-22 15:08:31.237493 PyQt6-6.5.2/sip/QtNetwork/qabstractsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1584 2023-07-22 15:08:31.234084 PyQt6-6.5.2/sip/QtNetwork/qauthenticator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4595 2023-07-22 15:08:31.198326 PyQt6-6.5.2/sip/QtNetwork/qdnslookup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5644 2023-07-22 15:08:31.226331 PyQt6-6.5.2/sip/QtNetwork/qhostaddress.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2987 2023-07-22 15:08:31.227649 PyQt6-6.5.2/sip/QtNetwork/qhostinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1906 2023-07-22 15:08:31.243933 PyQt6-6.5.2/sip/QtNetwork/qhstspolicy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1632 2023-07-22 15:08:31.228177 PyQt6-6.5.2/sip/QtNetwork/qhttp1configuration.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1863 2023-07-22 15:08:31.240457 PyQt6-6.5.2/sip/QtNetwork/qhttp2configuration.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2111 2023-07-22 15:08:31.248290 PyQt6-6.5.2/sip/QtNetwork/qhttpmultipart.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2417 2023-07-22 15:08:31.226995 PyQt6-6.5.2/sip/QtNetwork/qlocalserver.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6739 2023-07-22 15:08:31.238583 PyQt6-6.5.2/sip/QtNetwork/qlocalsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4835 2023-07-22 15:08:31.231520 PyQt6-6.5.2/sip/QtNetwork/qnetworkaccessmanager.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2540 2023-07-22 15:08:31.196801 PyQt6-6.5.2/sip/QtNetwork/qnetworkcookie.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1719 2023-07-22 15:08:31.247677 PyQt6-6.5.2/sip/QtNetwork/qnetworkcookiejar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1941 2023-07-22 15:08:31.194199 PyQt6-6.5.2/sip/QtNetwork/qnetworkdatagram.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1881 2023-07-22 15:08:31.234568 PyQt6-6.5.2/sip/QtNetwork/qnetworkdiskcache.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2950 2023-07-22 15:08:31.230795 PyQt6-6.5.2/sip/QtNetwork/qnetworkinformation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3720 2023-07-22 15:08:31.229467 PyQt6-6.5.2/sip/QtNetwork/qnetworkinterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5091 2023-07-22 15:08:31.249309 PyQt6-6.5.2/sip/QtNetwork/qnetworkproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5728 2023-07-22 15:08:31.199233 PyQt6-6.5.2/sip/QtNetwork/qnetworkreply.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5117 2023-07-22 15:08:31.241351 PyQt6-6.5.2/sip/QtNetwork/qnetworkrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2020 2023-07-22 15:08:31.246229 PyQt6-6.5.2/sip/QtNetwork/qocspresponse.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1379 2023-07-22 15:08:31.225107 PyQt6-6.5.2/sip/QtNetwork/qpassworddigestor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3458 2023-07-22 15:08:31.247161 PyQt6-6.5.2/sip/QtNetwork/qpynetwork_qhash.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7009 2023-07-22 15:08:31.243514 PyQt6-6.5.2/sip/QtNetwork/qpynetwork_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4985 2023-07-22 15:08:31.232665 PyQt6-6.5.2/sip/QtNetwork/qpynetwork_qmap.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3643 2023-07-22 15:08:31.239455 PyQt6-6.5.2/sip/QtNetwork/qssl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3763 2023-07-22 15:08:31.250011 PyQt6-6.5.2/sip/QtNetwork/qsslcertificate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1426 2023-07-22 15:08:31.239993 PyQt6-6.5.2/sip/QtNetwork/qsslcertificateextension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1694 2023-07-22 15:08:31.228689 PyQt6-6.5.2/sip/QtNetwork/qsslcipher.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5201 2023-07-22 15:08:31.196229 PyQt6-6.5.2/sip/QtNetwork/qsslconfiguration.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2171 2023-07-22 15:08:31.230031 PyQt6-6.5.2/sip/QtNetwork/qssldiffiehellmanparameters.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1594 2023-07-22 15:08:31.233626 PyQt6-6.5.2/sip/QtNetwork/qsslellipticcurve.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2803 2023-07-22 15:08:31.235922 PyQt6-6.5.2/sip/QtNetwork/qsslerror.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2021 2023-07-22 15:08:31.233147 PyQt6-6.5.2/sip/QtNetwork/qsslkey.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1883 2023-07-22 15:08:31.195484 PyQt6-6.5.2/sip/QtNetwork/qsslpresharedkeyauthenticator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2150 2023-07-22 15:08:31.195035 PyQt6-6.5.2/sip/QtNetwork/qsslserver.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8621 2023-07-22 15:08:31.244974 PyQt6-6.5.2/sip/QtNetwork/qsslsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2339 2023-07-22 15:08:31.241893 PyQt6-6.5.2/sip/QtNetwork/qtcpserver.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1134 2023-07-22 15:08:31.194572 PyQt6-6.5.2/sip/QtNetwork/qtcpsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3235 2023-07-22 15:08:31.245563 PyQt6-6.5.2/sip/QtNetwork/qudpsocket.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.770372 PyQt6-6.5.2/sip/QtNfc/
+-rw-r--r--   0 phil       (501) staff       (20)     2146 2023-07-22 15:08:31.494515 PyQt6-6.5.2/sip/QtNfc/QtNfcmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1772 2023-07-22 15:08:31.496650 PyQt6-6.5.2/sip/QtNfc/qndeffilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2185 2023-07-22 15:08:31.495025 PyQt6-6.5.2/sip/QtNfc/qndefmessage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3351 2023-07-22 15:08:31.494124 PyQt6-6.5.2/sip/QtNfc/qndefnfcsmartposterrecord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1471 2023-07-22 15:08:31.495453 PyQt6-6.5.2/sip/QtNfc/qndefnfctextrecord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1213 2023-07-22 15:08:31.493428 PyQt6-6.5.2/sip/QtNfc/qndefnfcurirecord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2536 2023-07-22 15:08:31.492404 PyQt6-6.5.2/sip/QtNfc/qndefrecord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3014 2023-07-22 15:08:31.493037 PyQt6-6.5.2/sip/QtNfc/qnearfieldmanager.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3250 2023-07-22 15:08:31.496186 PyQt6-6.5.2/sip/QtNfc/qnearfieldtarget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.672043 PyQt6-6.5.2/sip/QtOpenGL/
+-rw-r--r--   0 phil       (501) staff       (20)     2618 2023-07-22 15:08:31.128038 PyQt6-6.5.2/sip/QtOpenGL/QtOpenGLmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2645 2023-07-22 15:08:31.127596 PyQt6-6.5.2/sip/QtOpenGL/qopenglbuffer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5913 2023-07-22 15:08:31.126995 PyQt6-6.5.2/sip/QtOpenGL/qopengldebug.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5082 2023-07-22 15:08:31.102819 PyQt6-6.5.2/sip/QtOpenGL/qopenglframebufferobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)   111265 2023-07-22 15:08:31.114386 PyQt6-6.5.2/sip/QtOpenGL/qopenglfunctions_2_0.sip
+-rw-r--r--   0 phil       (501) staff       (20)   111310 2023-07-22 15:08:31.125595 PyQt6-6.5.2/sip/QtOpenGL/qopenglfunctions_2_1.sip
+-rw-r--r--   0 phil       (501) staff       (20)    42567 2023-07-22 15:08:31.097895 PyQt6-6.5.2/sip/QtOpenGL/qopenglfunctions_4_1_core.sip
+-rw-r--r--   0 phil       (501) staff       (20)    28956 2023-07-22 15:08:31.132073 PyQt6-6.5.2/sip/QtOpenGL/qopenglfunctions_es2.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1751 2023-07-22 15:08:31.102062 PyQt6-6.5.2/sip/QtOpenGL/qopenglpaintdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1865 2023-07-22 15:08:31.132784 PyQt6-6.5.2/sip/QtOpenGL/qopenglpixeltransferoptions.sip
+-rw-r--r--   0 phil       (501) staff       (20)    15899 2023-07-22 15:08:31.135272 PyQt6-6.5.2/sip/QtOpenGL/qopenglshaderprogram.sip
+-rw-r--r--   0 phil       (501) staff       (20)    14995 2023-07-22 15:08:31.101542 PyQt6-6.5.2/sip/QtOpenGL/qopengltexture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2010 2023-07-22 15:08:31.133823 PyQt6-6.5.2/sip/QtOpenGL/qopengltextureblitter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2095 2023-07-22 15:08:31.098940 PyQt6-6.5.2/sip/QtOpenGL/qopengltimerquery.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1168 2023-07-22 15:08:31.099360 PyQt6-6.5.2/sip/QtOpenGL/qopenglversionfunctions.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1350 2023-07-22 15:08:31.098368 PyQt6-6.5.2/sip/QtOpenGL/qopenglversionfunctionsfactory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1814 2023-07-22 15:08:31.133223 PyQt6-6.5.2/sip/QtOpenGL/qopenglversionprofile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1909 2023-07-22 15:08:31.135827 PyQt6-6.5.2/sip/QtOpenGL/qopenglvertexarrayobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2173 2023-07-22 15:08:31.126123 PyQt6-6.5.2/sip/QtOpenGL/qopenglwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2926 2023-07-22 15:08:31.093046 PyQt6-6.5.2/sip/QtOpenGL/qpyopengl_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3170 2023-07-22 15:08:31.128925 PyQt6-6.5.2/sip/QtOpenGL/qpyopengl_std_pair.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.736528 PyQt6-6.5.2/sip/QtOpenGLWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2059 2023-07-22 15:08:31.375182 PyQt6-6.5.2/sip/QtOpenGLWidgets/QtOpenGLWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3230 2023-07-22 15:08:31.376014 PyQt6-6.5.2/sip/QtOpenGLWidgets/qopenglwidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.735799 PyQt6-6.5.2/sip/QtPdf/
+-rw-r--r--   0 phil       (501) staff       (20)     2169 2023-07-22 15:08:31.345534 PyQt6-6.5.2/sip/QtPdf/QtPdfmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1876 2023-07-22 15:08:31.347992 PyQt6-6.5.2/sip/QtPdf/qpdfbookmarkmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3512 2023-07-22 15:08:31.347090 PyQt6-6.5.2/sip/QtPdf/qpdfdocument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2081 2023-07-22 15:08:31.348518 PyQt6-6.5.2/sip/QtPdf/qpdfdocumentrenderoptions.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1460 2023-07-22 15:08:31.345950 PyQt6-6.5.2/sip/QtPdf/qpdflink.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1827 2023-07-22 15:08:31.347542 PyQt6-6.5.2/sip/QtPdf/qpdfpagenavigator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1681 2023-07-22 15:08:31.346379 PyQt6-6.5.2/sip/QtPdf/qpdfpagerenderer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1900 2023-07-22 15:08:31.348993 PyQt6-6.5.2/sip/QtPdf/qpdfsearchmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1430 2023-07-22 15:08:31.349381 PyQt6-6.5.2/sip/QtPdf/qpdfselection.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.897671 PyQt6-6.5.2/sip/QtPdfWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2012 2023-07-22 15:08:32.028016 PyQt6-6.5.2/sip/QtPdfWidgets/QtPdfWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2848 2023-07-22 15:08:32.028871 PyQt6-6.5.2/sip/QtPdfWidgets/qpdfview.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.848074 PyQt6-6.5.2/sip/QtPositioning/
+-rw-r--r--   0 phil       (501) staff       (20)     2365 2023-07-22 15:08:31.788556 PyQt6-6.5.2/sip/QtPositioning/QtPositioningmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2273 2023-07-22 15:08:31.796034 PyQt6-6.5.2/sip/QtPositioning/qgeoaddress.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2226 2023-07-22 15:08:31.794452 PyQt6-6.5.2/sip/QtPositioning/qgeoareamonitorinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3002 2023-07-22 15:08:31.792999 PyQt6-6.5.2/sip/QtPositioning/qgeoareamonitorsource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1857 2023-07-22 15:08:31.791735 PyQt6-6.5.2/sip/QtPositioning/qgeocircle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2775 2023-07-22 15:08:31.796592 PyQt6-6.5.2/sip/QtPositioning/qgeocoordinate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1850 2023-07-22 15:08:31.794935 PyQt6-6.5.2/sip/QtPositioning/qgeolocation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2370 2023-07-22 15:08:31.793466 PyQt6-6.5.2/sip/QtPositioning/qgeopath.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2601 2023-07-22 15:08:31.793939 PyQt6-6.5.2/sip/QtPositioning/qgeopolygon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2502 2023-07-22 15:08:31.787955 PyQt6-6.5.2/sip/QtPositioning/qgeopositioninfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4135 2023-07-22 15:08:31.792385 PyQt6-6.5.2/sip/QtPositioning/qgeopositioninfosource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2832 2023-07-22 15:08:31.789539 PyQt6-6.5.2/sip/QtPositioning/qgeorectangle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2343 2023-07-22 15:08:31.790646 PyQt6-6.5.2/sip/QtPositioning/qgeosatelliteinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2640 2023-07-22 15:08:31.795539 PyQt6-6.5.2/sip/QtPositioning/qgeosatelliteinfosource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2434 2023-07-22 15:08:31.791267 PyQt6-6.5.2/sip/QtPositioning/qgeoshape.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2205 2023-07-22 15:08:31.789997 PyQt6-6.5.2/sip/QtPositioning/qnmeapositioninfosource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2448 2023-07-22 15:08:31.789041 PyQt6-6.5.2/sip/QtPositioning/qnmeasatelliteinfosource.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.663859 PyQt6-6.5.2/sip/QtPrintSupport/
+-rw-r--r--   0 phil       (501) staff       (20)     2261 2023-07-22 15:08:31.087185 PyQt6-6.5.2/sip/QtPrintSupport/QtPrintSupportmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3959 2023-07-22 15:08:31.086669 PyQt6-6.5.2/sip/QtPrintSupport/qabstractprintdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2569 2023-07-22 15:08:31.089820 PyQt6-6.5.2/sip/QtPrintSupport/qpagesetupdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2959 2023-07-22 15:08:31.085211 PyQt6-6.5.2/sip/QtPrintSupport/qprintdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2327 2023-07-22 15:08:31.091021 PyQt6-6.5.2/sip/QtPrintSupport/qprintengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4672 2023-07-22 15:08:31.092077 PyQt6-6.5.2/sip/QtPrintSupport/qprinter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2194 2023-07-22 15:08:31.090387 PyQt6-6.5.2/sip/QtPrintSupport/qprinterinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2034 2023-07-22 15:08:31.085785 PyQt6-6.5.2/sip/QtPrintSupport/qprintpreviewdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2558 2023-07-22 15:08:31.087843 PyQt6-6.5.2/sip/QtPrintSupport/qprintpreviewwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4887 2023-07-22 15:08:31.089208 PyQt6-6.5.2/sip/QtPrintSupport/qpyprintsupport_qlist.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.681306 PyQt6-6.5.2/sip/QtQml/
+-rw-r--r--   0 phil       (501) staff       (20)     2708 2023-07-22 15:08:31.142179 PyQt6-6.5.2/sip/QtQml/QtQmlmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6133 2023-07-22 15:08:31.143156 PyQt6-6.5.2/sip/QtQml/qjsengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3449 2023-07-22 15:08:31.147375 PyQt6-6.5.2/sip/QtQml/qjsmanagedvalue.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3260 2023-07-22 15:08:31.138275 PyQt6-6.5.2/sip/QtQml/qjsprimitivevalue.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3624 2023-07-22 15:08:31.141223 PyQt6-6.5.2/sip/QtQml/qjsvalue.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1267 2023-07-22 15:08:31.137609 PyQt6-6.5.2/sip/QtQml/qjsvalueiterator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1412 2023-07-22 15:08:31.137217 PyQt6-6.5.2/sip/QtQml/qmlattachedpropertiesobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2851 2023-07-22 15:08:31.146212 PyQt6-6.5.2/sip/QtQml/qmlregistertype.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1413 2023-07-22 15:08:31.144178 PyQt6-6.5.2/sip/QtQml/qpyqmllistproperty.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1852 2023-07-22 15:08:31.175064 PyQt6-6.5.2/sip/QtQml/qqml.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1354 2023-07-22 15:08:31.145041 PyQt6-6.5.2/sip/QtQml/qqmlabstracturlinterceptor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2102 2023-07-22 15:08:31.140420 PyQt6-6.5.2/sip/QtQml/qqmlapplicationengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3497 2023-07-22 15:08:31.139987 PyQt6-6.5.2/sip/QtQml/qqmlcomponent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2006 2023-07-22 15:08:31.149125 PyQt6-6.5.2/sip/QtQml/qqmlcontext.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5776 2023-07-22 15:08:31.176200 PyQt6-6.5.2/sip/QtQml/qqmlengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1624 2023-07-22 15:08:31.176663 PyQt6-6.5.2/sip/QtQml/qqmlerror.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1925 2023-07-22 15:08:31.148179 PyQt6-6.5.2/sip/QtQml/qqmlexpression.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1583 2023-07-22 15:08:31.144597 PyQt6-6.5.2/sip/QtQml/qqmlextensionplugin.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1303 2023-07-22 15:08:31.139386 PyQt6-6.5.2/sip/QtQml/qqmlfileselector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2332 2023-07-22 15:08:31.138959 PyQt6-6.5.2/sip/QtQml/qqmlincubator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1898 2023-07-22 15:08:31.143686 PyQt6-6.5.2/sip/QtQml/qqmllist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1199 2023-07-22 15:08:31.146771 PyQt6-6.5.2/sip/QtQml/qqmlnetworkaccessmanagerfactory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1235 2023-07-22 15:08:31.147748 PyQt6-6.5.2/sip/QtQml/qqmlparserstatus.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4182 2023-07-22 15:08:31.136775 PyQt6-6.5.2/sip/QtQml/qqmlproperty.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1769 2023-07-22 15:08:31.141694 PyQt6-6.5.2/sip/QtQml/qqmlpropertymap.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1254 2023-07-22 15:08:31.148665 PyQt6-6.5.2/sip/QtQml/qqmlpropertyvaluesource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1457 2023-07-22 15:08:31.145438 PyQt6-6.5.2/sip/QtQml/qqmlscriptstring.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.781791 PyQt6-6.5.2/sip/QtQuick/
+-rw-r--r--   0 phil       (501) staff       (20)     2852 2023-07-22 15:08:31.532359 PyQt6-6.5.2/sip/QtQuick/QtQuickmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2548 2023-07-22 15:08:31.529148 PyQt6-6.5.2/sip/QtQuick/qquickframebufferobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2308 2023-07-22 15:08:31.539193 PyQt6-6.5.2/sip/QtQuick/qquickgraphicsconfiguration.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1298 2023-07-22 15:08:31.499420 PyQt6-6.5.2/sip/QtQuick/qquickgraphicsdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2820 2023-07-22 15:08:31.537567 PyQt6-6.5.2/sip/QtQuick/qquickimageprovider.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10164 2023-07-22 15:08:31.542666 PyQt6-6.5.2/sip/QtQuick/qquickitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1368 2023-07-22 15:08:31.541125 PyQt6-6.5.2/sip/QtQuick/qquickitemgrabresult.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2983 2023-07-22 15:08:31.526471 PyQt6-6.5.2/sip/QtQuick/qquickpainteditem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1662 2023-07-22 15:08:31.531884 PyQt6-6.5.2/sip/QtQuick/qquickrendercontrol.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2100 2023-07-22 15:08:31.525864 PyQt6-6.5.2/sip/QtQuick/qquickrendertarget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1160 2023-07-22 15:08:31.534721 PyQt6-6.5.2/sip/QtQuick/qquicktextdocument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2345 2023-07-22 15:08:31.540362 PyQt6-6.5.2/sip/QtQuick/qquickview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6928 2023-07-22 15:08:31.533842 PyQt6-6.5.2/sip/QtQuick/qquickwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1377 2023-07-22 15:08:31.528090 PyQt6-6.5.2/sip/QtQuick/qsgflatcolormaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)    11740 2023-07-22 15:08:31.531427 PyQt6-6.5.2/sip/QtQuick/qsggeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2762 2023-07-22 15:08:31.528595 PyQt6-6.5.2/sip/QtQuick/qsgimagenode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1747 2023-07-22 15:08:31.538053 PyQt6-6.5.2/sip/QtQuick/qsgmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4807 2023-07-22 15:08:31.525360 PyQt6-6.5.2/sip/QtQuick/qsgmaterialshader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1033 2023-07-22 15:08:31.527307 PyQt6-6.5.2/sip/QtQuick/qsgmaterialtype.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8652 2023-07-22 15:08:31.536950 PyQt6-6.5.2/sip/QtQuick/qsgnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1343 2023-07-22 15:08:31.540730 PyQt6-6.5.2/sip/QtQuick/qsgrectanglenode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3077 2023-07-22 15:08:31.529816 PyQt6-6.5.2/sip/QtQuick/qsgrendererinterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2526 2023-07-22 15:08:31.534373 PyQt6-6.5.2/sip/QtQuick/qsgrendernode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1354 2023-07-22 15:08:31.535398 PyQt6-6.5.2/sip/QtQuick/qsgsimplerectnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2097 2023-07-22 15:08:31.538573 PyQt6-6.5.2/sip/QtQuick/qsgsimpletexturenode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2513 2023-07-22 15:08:31.500033 PyQt6-6.5.2/sip/QtQuick/qsgtexture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1446 2023-07-22 15:08:31.532856 PyQt6-6.5.2/sip/QtQuick/qsgtexture_platform.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2207 2023-07-22 15:08:31.526941 PyQt6-6.5.2/sip/QtQuick/qsgtexturematerial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1152 2023-07-22 15:08:31.539864 PyQt6-6.5.2/sip/QtQuick/qsgtextureprovider.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1324 2023-07-22 15:08:31.527698 PyQt6-6.5.2/sip/QtQuick/qsgvertexcolormaterial.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.714701 PyQt6-6.5.2/sip/QtQuick3D/
+-rw-r--r--   0 phil       (501) staff       (20)     2086 2023-07-22 15:08:31.287750 PyQt6-6.5.2/sip/QtQuick3D/QtQuick3Dmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1086 2023-07-22 15:08:31.287358 PyQt6-6.5.2/sip/QtQuick3D/qquick3d.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3758 2023-07-22 15:08:31.287006 PyQt6-6.5.2/sip/QtQuick3D/qquick3dgeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2159 2023-07-22 15:08:31.288352 PyQt6-6.5.2/sip/QtQuick3D/qquick3dobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2181 2023-07-22 15:08:31.286274 PyQt6-6.5.2/sip/QtQuick3D/qquick3dtexturedata.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.787522 PyQt6-6.5.2/sip/QtQuickWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2080 2023-07-22 15:08:31.575525 PyQt6-6.5.2/sip/QtQuickWidgets/QtQuickWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3345 2023-07-22 15:08:31.576191 PyQt6-6.5.2/sip/QtQuickWidgets/qquickwidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.726536 PyQt6-6.5.2/sip/QtRemoteObjects/
+-rw-r--r--   0 phil       (501) staff       (20)     2163 2023-07-22 15:08:31.334121 PyQt6-6.5.2/sip/QtRemoteObjects/QtRemoteObjectsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2298 2023-07-22 15:08:31.332007 PyQt6-6.5.2/sip/QtRemoteObjects/qremoteobjectabstractitemmodelreplica.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1221 2023-07-22 15:08:31.330642 PyQt6-6.5.2/sip/QtRemoteObjects/qremoteobjectdynamicreplica.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6469 2023-07-22 15:08:31.333144 PyQt6-6.5.2/sip/QtRemoteObjects/qremoteobjectnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1429 2023-07-22 15:08:31.334605 PyQt6-6.5.2/sip/QtRemoteObjects/qremoteobjectregistry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1689 2023-07-22 15:08:31.333702 PyQt6-6.5.2/sip/QtRemoteObjects/qremoteobjectreplica.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2093 2023-07-22 15:08:31.331285 PyQt6-6.5.2/sip/QtRemoteObjects/qtremoteobjectglobal.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.732779 PyQt6-6.5.2/sip/QtSensors/
+-rw-r--r--   0 phil       (501) staff       (20)     2393 2023-07-22 15:08:31.344006 PyQt6-6.5.2/sip/QtSensors/QtSensorsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2037 2023-07-22 15:08:31.338591 PyQt6-6.5.2/sip/QtSensors/qaccelerometer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1842 2023-07-22 15:08:31.335330 PyQt6-6.5.2/sip/QtSensors/qambientlightsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1726 2023-07-22 15:08:31.340107 PyQt6-6.5.2/sip/QtSensors/qambienttemperaturesensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1641 2023-07-22 15:08:31.343555 PyQt6-6.5.2/sip/QtSensors/qcompass.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1645 2023-07-22 15:08:31.340664 PyQt6-6.5.2/sip/QtSensors/qgyroscope.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1701 2023-07-22 15:08:31.339620 PyQt6-6.5.2/sip/QtSensors/qhumiditysensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1649 2023-07-22 15:08:31.339082 PyQt6-6.5.2/sip/QtSensors/qirproximitysensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1719 2023-07-22 15:08:31.335916 PyQt6-6.5.2/sip/QtSensors/qlidsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1692 2023-07-22 15:08:31.338038 PyQt6-6.5.2/sip/QtSensors/qlightsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1918 2023-07-22 15:08:31.344547 PyQt6-6.5.2/sip/QtSensors/qmagnetometer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1856 2023-07-22 15:08:31.336515 PyQt6-6.5.2/sip/QtSensors/qorientationsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1682 2023-07-22 15:08:31.337533 PyQt6-6.5.2/sip/QtSensors/qpressuresensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1607 2023-07-22 15:08:31.337035 PyQt6-6.5.2/sip/QtSensors/qproximitysensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1749 2023-07-22 15:08:31.345057 PyQt6-6.5.2/sip/QtSensors/qrotationsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7556 2023-07-22 15:08:31.343010 PyQt6-6.5.2/sip/QtSensors/qsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2079 2023-07-22 15:08:31.341860 PyQt6-6.5.2/sip/QtSensors/qtapsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1641 2023-07-22 15:08:31.341260 PyQt6-6.5.2/sip/QtSensors/qtiltsensor.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.771587 PyQt6-6.5.2/sip/QtSerialPort/
+-rw-r--r--   0 phil       (501) staff       (20)     1982 2023-07-22 15:08:31.497745 PyQt6-6.5.2/sip/QtSerialPort/QtSerialPortmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7926 2023-07-22 15:08:31.498973 PyQt6-6.5.2/sip/QtSerialPort/qserialport.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1768 2023-07-22 15:08:31.497366 PyQt6-6.5.2/sip/QtSerialPort/qserialportinfo.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.842581 PyQt6-6.5.2/sip/QtSpatialAudio/
+-rw-r--r--   0 phil       (501) staff       (20)     2107 2023-07-22 15:08:31.784047 PyQt6-6.5.2/sip/QtSpatialAudio/QtSpatialAudiomod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1672 2023-07-22 15:08:31.785406 PyQt6-6.5.2/sip/QtSpatialAudio/qambientsound.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2978 2023-07-22 15:08:31.787322 PyQt6-6.5.2/sip/QtSpatialAudio/qaudioengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1342 2023-07-22 15:08:31.786008 PyQt6-6.5.2/sip/QtSpatialAudio/qaudiolistener.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2771 2023-07-22 15:08:31.786708 PyQt6-6.5.2/sip/QtSpatialAudio/qaudioroom.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2891 2023-07-22 15:08:31.784807 PyQt6-6.5.2/sip/QtSpatialAudio/qspatialsound.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.832050 PyQt6-6.5.2/sip/QtSql/
+-rw-r--r--   0 phil       (501) staff       (20)     2287 2023-07-22 15:08:31.740720 PyQt6-6.5.2/sip/QtSql/QtSqlmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3746 2023-07-22 15:08:31.740090 PyQt6-6.5.2/sip/QtSql/qsqldatabase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5000 2023-07-22 15:08:31.735634 PyQt6-6.5.2/sip/QtSql/qsqldriver.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1749 2023-07-22 15:08:31.733575 PyQt6-6.5.2/sip/QtSql/qsqlerror.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2360 2023-07-22 15:08:31.741744 PyQt6-6.5.2/sip/QtSql/qsqlfield.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1497 2023-07-22 15:08:31.739393 PyQt6-6.5.2/sip/QtSql/qsqlindex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3080 2023-07-22 15:08:31.737140 PyQt6-6.5.2/sip/QtSql/qsqlquery.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3117 2023-07-22 15:08:31.738951 PyQt6-6.5.2/sip/QtSql/qsqlquerymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2260 2023-07-22 15:08:31.737598 PyQt6-6.5.2/sip/QtSql/qsqlrecord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1542 2023-07-22 15:08:31.736530 PyQt6-6.5.2/sip/QtSql/qsqlrelationaldelegate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2598 2023-07-22 15:08:31.741254 PyQt6-6.5.2/sip/QtSql/qsqlrelationaltablemodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3175 2023-07-22 15:08:31.734351 PyQt6-6.5.2/sip/QtSql/qsqlresult.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3785 2023-07-22 15:08:31.738397 PyQt6-6.5.2/sip/QtSql/qsqltablemodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1512 2023-07-22 15:08:31.736125 PyQt6-6.5.2/sip/QtSql/qtsqlglobal.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.722138 PyQt6-6.5.2/sip/QtSvg/
+-rw-r--r--   0 phil       (501) staff       (20)     1987 2023-07-22 15:08:31.325258 PyQt6-6.5.2/sip/QtSvg/QtSvgmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2082 2023-07-22 15:08:31.298057 PyQt6-6.5.2/sip/QtSvg/qsvggenerator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3043 2023-07-22 15:08:31.298747 PyQt6-6.5.2/sip/QtSvg/qsvgrenderer.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.723970 PyQt6-6.5.2/sip/QtSvgWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2071 2023-07-22 15:08:31.329664 PyQt6-6.5.2/sip/QtSvgWidgets/QtSvgWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1911 2023-07-22 15:08:31.329253 PyQt6-6.5.2/sip/QtSvgWidgets/qgraphicssvgitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2035 2023-07-22 15:08:31.330190 PyQt6-6.5.2/sip/QtSvgWidgets/qsvgwidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.896964 PyQt6-6.5.2/sip/QtTest/
+-rw-r--r--   0 phil       (501) staff       (20)     2110 2023-07-22 15:08:32.002918 PyQt6-6.5.2/sip/QtTest/QtTestmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1689 2023-07-22 15:08:32.027351 PyQt6-6.5.2/sip/QtTest/qabstractitemmodeltester.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3285 2023-07-22 15:08:32.025922 PyQt6-6.5.2/sip/QtTest/qsignalspy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3740 2023-07-22 15:08:32.025140 PyQt6-6.5.2/sip/QtTest/qtestkeyboard.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2446 2023-07-22 15:08:32.026917 PyQt6-6.5.2/sip/QtTest/qtestmouse.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1381 2023-07-22 15:08:32.026418 PyQt6-6.5.2/sip/QtTest/qtestsystem.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.849073 PyQt6-6.5.2/sip/QtTextToSpeech/
+-rw-r--r--   0 phil       (501) staff       (20)     1981 2023-07-22 15:08:31.798258 PyQt6-6.5.2/sip/QtTextToSpeech/QtTextToSpeechmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3550 2023-07-22 15:08:31.797305 PyQt6-6.5.2/sip/QtTextToSpeech/qtexttospeech.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1760 2023-07-22 15:08:31.797878 PyQt6-6.5.2/sip/QtTextToSpeech/qvoice.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.788612 PyQt6-6.5.2/sip/QtWebChannel/
+-rw-r--r--   0 phil       (501) staff       (20)     1995 2023-07-22 15:08:31.576666 PyQt6-6.5.2/sip/QtWebChannel/QtWebChannelmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2363 2023-07-22 15:08:31.577682 PyQt6-6.5.2/sip/QtWebChannel/qwebchannel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1425 2023-07-22 15:08:31.577108 PyQt6-6.5.2/sip/QtWebChannel/qwebchannelabstracttransport.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.660431 PyQt6-6.5.2/sip/QtWebSockets/
+-rw-r--r--   0 phil       (501) staff       (20)     2158 2023-07-22 15:08:31.083278 PyQt6-6.5.2/sip/QtWebSockets/QtWebSocketsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1238 2023-07-22 15:08:31.083749 PyQt6-6.5.2/sip/QtWebSockets/qmaskgenerator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6039 2023-07-22 15:08:31.082780 PyQt6-6.5.2/sip/QtWebSockets/qwebsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1445 2023-07-22 15:08:31.081651 PyQt6-6.5.2/sip/QtWebSockets/qwebsocketcorsauthenticator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1623 2023-07-22 15:08:31.081138 PyQt6-6.5.2/sip/QtWebSockets/qwebsockethandshakeoptions.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1741 2023-07-22 15:08:31.080601 PyQt6-6.5.2/sip/QtWebSockets/qwebsocketprotocol.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3249 2023-07-22 15:08:31.084484 PyQt6-6.5.2/sip/QtWebSockets/qwebsocketserver.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.827031 PyQt6-6.5.2/sip/QtWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     4913 2023-07-22 15:08:31.681901 PyQt6-6.5.2/sip/QtWidgets/QtWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2732 2023-07-22 15:08:31.699175 PyQt6-6.5.2/sip/QtWidgets/qabstractbutton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2621 2023-07-22 15:08:31.632693 PyQt6-6.5.2/sip/QtWidgets/qabstractitemdelegate.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10372 2023-07-22 15:08:31.595889 PyQt6-6.5.2/sip/QtWidgets/qabstractitemview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3459 2023-07-22 15:08:31.699836 PyQt6-6.5.2/sip/QtWidgets/qabstractscrollarea.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3009 2023-07-22 15:08:31.582541 PyQt6-6.5.2/sip/QtWidgets/qabstractslider.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4021 2023-07-22 15:08:31.680524 PyQt6-6.5.2/sip/QtWidgets/qabstractspinbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)    14136 2023-07-22 15:08:31.647151 PyQt6-6.5.2/sip/QtWidgets/qapplication.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4795 2023-07-22 15:08:31.597355 PyQt6-6.5.2/sip/QtWidgets/qboxlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1835 2023-07-22 15:08:31.626706 PyQt6-6.5.2/sip/QtWidgets/qbuttongroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4043 2023-07-22 15:08:31.696429 PyQt6-6.5.2/sip/QtWidgets/qcalendarwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1799 2023-07-22 15:08:31.630965 PyQt6-6.5.2/sip/QtWidgets/qcheckbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2995 2023-07-22 15:08:31.651321 PyQt6-6.5.2/sip/QtWidgets/qcolordialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2872 2023-07-22 15:08:31.629803 PyQt6-6.5.2/sip/QtWidgets/qcolumnview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6343 2023-07-22 15:08:31.731340 PyQt6-6.5.2/sip/QtWidgets/qcombobox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1749 2023-07-22 15:08:31.692002 PyQt6-6.5.2/sip/QtWidgets/qcommandlinkbutton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3141 2023-07-22 15:08:31.691036 PyQt6-6.5.2/sip/QtWidgets/qcommonstyle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3315 2023-07-22 15:08:31.601301 PyQt6-6.5.2/sip/QtWidgets/qcompleter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2437 2023-07-22 15:08:31.681060 PyQt6-6.5.2/sip/QtWidgets/qdatawidgetmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5039 2023-07-22 15:08:31.693200 PyQt6-6.5.2/sip/QtWidgets/qdatetimeedit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1866 2023-07-22 15:08:31.594057 PyQt6-6.5.2/sip/QtWidgets/qdial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2692 2023-07-22 15:08:31.594596 PyQt6-6.5.2/sip/QtWidgets/qdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3396 2023-07-22 15:08:31.682588 PyQt6-6.5.2/sip/QtWidgets/qdialogbuttonbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2666 2023-07-22 15:08:31.697794 PyQt6-6.5.2/sip/QtWidgets/qdockwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2730 2023-07-22 15:08:31.695754 PyQt6-6.5.2/sip/QtWidgets/qdrawutil.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1389 2023-07-22 15:08:31.628279 PyQt6-6.5.2/sip/QtWidgets/qerrormessage.sip
+-rw-r--r--   0 phil       (501) staff       (20)    12183 2023-07-22 15:08:31.653913 PyQt6-6.5.2/sip/QtWidgets/qfiledialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1261 2023-07-22 15:08:31.626237 PyQt6-6.5.2/sip/QtWidgets/qfileiconprovider.sip
+-rw-r--r--   0 phil       (501) staff       (20)      957 2023-07-22 15:08:31.633107 PyQt6-6.5.2/sip/QtWidgets/qfilesystemmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1392 2023-07-22 15:08:31.729424 PyQt6-6.5.2/sip/QtWidgets/qfocusframe.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2764 2023-07-22 15:08:31.596476 PyQt6-6.5.2/sip/QtWidgets/qfontcombobox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2916 2023-07-22 15:08:31.588899 PyQt6-6.5.2/sip/QtWidgets/qfontdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4981 2023-07-22 15:08:31.588266 PyQt6-6.5.2/sip/QtWidgets/qformlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2164 2023-07-22 15:08:31.579908 PyQt6-6.5.2/sip/QtWidgets/qframe.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5339 2023-07-22 15:08:31.694908 PyQt6-6.5.2/sip/QtWidgets/qgesture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1738 2023-07-22 15:08:31.692423 PyQt6-6.5.2/sip/QtWidgets/qgesturerecognizer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2740 2023-07-22 15:08:31.591033 PyQt6-6.5.2/sip/QtWidgets/qgraphicsanchorlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5015 2023-07-22 15:08:31.730396 PyQt6-6.5.2/sip/QtWidgets/qgraphicseffect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4207 2023-07-22 15:08:31.732041 PyQt6-6.5.2/sip/QtWidgets/qgraphicsgridlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)    26805 2023-07-22 15:08:31.727664 PyQt6-6.5.2/sip/QtWidgets/qgraphicsitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1730 2023-07-22 15:08:31.584145 PyQt6-6.5.2/sip/QtWidgets/qgraphicslayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3128 2023-07-22 15:08:31.591606 PyQt6-6.5.2/sip/QtWidgets/qgraphicslayoutitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3150 2023-07-22 15:08:31.648476 PyQt6-6.5.2/sip/QtWidgets/qgraphicslinearlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3920 2023-07-22 15:08:31.631595 PyQt6-6.5.2/sip/QtWidgets/qgraphicsproxywidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8768 2023-07-22 15:08:31.683544 PyQt6-6.5.2/sip/QtWidgets/qgraphicsscene.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6166 2023-07-22 15:08:31.627856 PyQt6-6.5.2/sip/QtWidgets/qgraphicssceneevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2441 2023-07-22 15:08:31.678708 PyQt6-6.5.2/sip/QtWidgets/qgraphicstransform.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8125 2023-07-22 15:08:31.733015 PyQt6-6.5.2/sip/QtWidgets/qgraphicsview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5459 2023-07-22 15:08:31.647940 PyQt6-6.5.2/sip/QtWidgets/qgraphicswidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5537 2023-07-22 15:08:31.600691 PyQt6-6.5.2/sip/QtWidgets/qgridlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2122 2023-07-22 15:08:31.675081 PyQt6-6.5.2/sip/QtWidgets/qgroupbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7170 2023-07-22 15:08:31.634052 PyQt6-6.5.2/sip/QtWidgets/qheaderview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5360 2023-07-22 15:08:31.581197 PyQt6-6.5.2/sip/QtWidgets/qinputdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2931 2023-07-22 15:08:31.698628 PyQt6-6.5.2/sip/QtWidgets/qitemdelegate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1812 2023-07-22 15:08:31.643142 PyQt6-6.5.2/sip/QtWidgets/qitemeditorfactory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2219 2023-07-22 15:08:31.580451 PyQt6-6.5.2/sip/QtWidgets/qkeysequenceedit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6063 2023-07-22 15:08:31.676081 PyQt6-6.5.2/sip/QtWidgets/qlabel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5894 2023-07-22 15:08:31.589739 PyQt6-6.5.2/sip/QtWidgets/qlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3732 2023-07-22 15:08:31.649756 PyQt6-6.5.2/sip/QtWidgets/qlayoutitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2378 2023-07-22 15:08:31.578426 PyQt6-6.5.2/sip/QtWidgets/qlcdnumber.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5210 2023-07-22 15:08:31.644598 PyQt6-6.5.2/sip/QtWidgets/qlineedit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4961 2023-07-22 15:08:31.625825 PyQt6-6.5.2/sip/QtWidgets/qlistview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7358 2023-07-22 15:08:31.690193 PyQt6-6.5.2/sip/QtWidgets/qlistwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4691 2023-07-22 15:08:31.645639 PyQt6-6.5.2/sip/QtWidgets/qmainwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4174 2023-07-22 15:08:31.581936 PyQt6-6.5.2/sip/QtWidgets/qmdiarea.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4054 2023-07-22 15:08:31.697295 PyQt6-6.5.2/sip/QtWidgets/qmdisubwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5652 2023-07-22 15:08:31.593540 PyQt6-6.5.2/sip/QtWidgets/qmenu.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3601 2023-07-22 15:08:31.689225 PyQt6-6.5.2/sip/QtWidgets/qmenubar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6307 2023-07-22 15:08:31.650570 PyQt6-6.5.2/sip/QtWidgets/qmessagebox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7249 2023-07-22 15:08:31.685810 PyQt6-6.5.2/sip/QtWidgets/qplaintextedit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2226 2023-07-22 15:08:31.590277 PyQt6-6.5.2/sip/QtWidgets/qprogressbar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2903 2023-07-22 15:08:31.583751 PyQt6-6.5.2/sip/QtWidgets/qprogressdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3947 2023-07-22 15:08:31.583184 PyQt6-6.5.2/sip/QtWidgets/qproxystyle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2069 2023-07-22 15:08:31.654437 PyQt6-6.5.2/sip/QtWidgets/qpushbutton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2905 2023-07-22 15:08:31.677587 PyQt6-6.5.2/sip/QtWidgets/qpywidgets_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1555 2023-07-22 15:08:31.691497 PyQt6-6.5.2/sip/QtWidgets/qradiobutton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1794 2023-07-22 15:08:31.648919 PyQt6-6.5.2/sip/QtWidgets/qrubberband.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1895 2023-07-22 15:08:31.684676 PyQt6-6.5.2/sip/QtWidgets/qscrollarea.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1773 2023-07-22 15:08:31.584543 PyQt6-6.5.2/sip/QtWidgets/qscrollbar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2896 2023-07-22 15:08:31.634622 PyQt6-6.5.2/sip/QtWidgets/qscroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2485 2023-07-22 15:08:31.643792 PyQt6-6.5.2/sip/QtWidgets/qscrollerproperties.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1640 2023-07-22 15:08:31.624979 PyQt6-6.5.2/sip/QtWidgets/qsizegrip.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3272 2023-07-22 15:08:31.630493 PyQt6-6.5.2/sip/QtWidgets/qsizepolicy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1921 2023-07-22 15:08:31.688466 PyQt6-6.5.2/sip/QtWidgets/qslider.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3301 2023-07-22 15:08:31.652272 PyQt6-6.5.2/sip/QtWidgets/qspinbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1798 2023-07-22 15:08:31.598513 PyQt6-6.5.2/sip/QtWidgets/qsplashscreen.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3429 2023-07-22 15:08:31.684196 PyQt6-6.5.2/sip/QtWidgets/qsplitter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3651 2023-07-22 15:08:31.676769 PyQt6-6.5.2/sip/QtWidgets/qstackedlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1662 2023-07-22 15:08:31.695360 PyQt6-6.5.2/sip/QtWidgets/qstackedwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1956 2023-07-22 15:08:31.599949 PyQt6-6.5.2/sip/QtWidgets/qstatusbar.sip
+-rw-r--r--   0 phil       (501) staff       (20)    22575 2023-07-22 15:08:31.587430 PyQt6-6.5.2/sip/QtWidgets/qstyle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2426 2023-07-22 15:08:31.678071 PyQt6-6.5.2/sip/QtWidgets/qstyleditemdelegate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1122 2023-07-22 15:08:31.599372 PyQt6-6.5.2/sip/QtWidgets/qstylefactory.sip
+-rw-r--r--   0 phil       (501) staff       (20)    20087 2023-07-22 15:08:31.638840 PyQt6-6.5.2/sip/QtWidgets/qstyleoption.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1732 2023-07-22 15:08:31.698197 PyQt6-6.5.2/sip/QtWidgets/qstylepainter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2317 2023-07-22 15:08:31.632159 PyQt6-6.5.2/sip/QtWidgets/qsystemtrayicon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5251 2023-07-22 15:08:31.639808 PyQt6-6.5.2/sip/QtWidgets/qtabbar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4837 2023-07-22 15:08:31.693871 PyQt6-6.5.2/sip/QtWidgets/qtableview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9246 2023-07-22 15:08:31.592773 PyQt6-6.5.2/sip/QtWidgets/qtablewidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4240 2023-07-22 15:08:31.640537 PyQt6-6.5.2/sip/QtWidgets/qtabwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2740 2023-07-22 15:08:31.629290 PyQt6-6.5.2/sip/QtWidgets/qtextbrowser.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7388 2023-07-22 15:08:31.687996 PyQt6-6.5.2/sip/QtWidgets/qtextedit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4343 2023-07-22 15:08:31.598098 PyQt6-6.5.2/sip/QtWidgets/qtoolbar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2421 2023-07-22 15:08:31.601810 PyQt6-6.5.2/sip/QtWidgets/qtoolbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2556 2023-07-22 15:08:31.679790 PyQt6-6.5.2/sip/QtWidgets/qtoolbutton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1399 2023-07-22 15:08:31.644997 PyQt6-6.5.2/sip/QtWidgets/qtooltip.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6474 2023-07-22 15:08:31.579323 PyQt6-6.5.2/sip/QtWidgets/qtreeview.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10328 2023-07-22 15:08:31.687001 PyQt6-6.5.2/sip/QtWidgets/qtreewidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2195 2023-07-22 15:08:31.679238 PyQt6-6.5.2/sip/QtWidgets/qtreewidgetitemiterator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1597 2023-07-22 15:08:31.628715 PyQt6-6.5.2/sip/QtWidgets/qundoview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1353 2023-07-22 15:08:31.690570 PyQt6-6.5.2/sip/QtWidgets/qwhatsthis.sip
+-rw-r--r--   0 phil       (501) staff       (20)    18362 2023-07-22 15:08:31.642657 PyQt6-6.5.2/sip/QtWidgets/qwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1627 2023-07-22 15:08:31.598918 PyQt6-6.5.2/sip/QtWidgets/qwidgetaction.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7633 2023-07-22 15:08:31.728987 PyQt6-6.5.2/sip/QtWidgets/qwizard.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.722859 PyQt6-6.5.2/sip/QtXml/
+-rw-r--r--   0 phil       (501) staff       (20)     1925 2023-07-22 15:08:31.328635 PyQt6-6.5.2/sip/QtXml/QtXmlmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)    16807 2023-07-22 15:08:31.327979 PyQt6-6.5.2/sip/QtXml/qdom.sip
+-rw-r--r--   0 phil       (501) staff       (20)       22 2023-07-22 15:08:31.079909 PyQt6-6.5.2/sip/pyqt-gpl.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.538577 PyQt6-6.5.2/uic/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.541307 PyQt6-6.5.2/uic/Compiler/
+-rw-r--r--   0 phil       (501) staff       (20)     1004 2023-07-22 15:08:24.358123 PyQt6-6.5.2/uic/Compiler/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     1412 2023-07-22 15:08:24.360725 PyQt6-6.5.2/uic/Compiler/as_string.py
+-rw-r--r--   0 phil       (501) staff       (20)     3934 2023-07-22 15:08:24.357756 PyQt6-6.5.2/uic/Compiler/compiler.py
+-rw-r--r--   0 phil       (501) staff       (20)     2742 2023-07-22 15:08:24.358684 PyQt6-6.5.2/uic/Compiler/indenter.py
+-rw-r--r--   0 phil       (501) staff       (20)     2374 2023-07-22 15:08:24.356909 PyQt6-6.5.2/uic/Compiler/misc.py
+-rw-r--r--   0 phil       (501) staff       (20)     4324 2023-07-22 15:08:24.360248 PyQt6-6.5.2/uic/Compiler/proxy_metaclass.py
+-rw-r--r--   0 phil       (501) staff       (20)     5839 2023-07-22 15:08:24.359599 PyQt6-6.5.2/uic/Compiler/qobjectcreator.py
+-rw-r--r--   0 phil       (501) staff       (20)    16164 2023-07-22 15:08:24.362874 PyQt6-6.5.2/uic/Compiler/qtproxies.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.538263 PyQt6-6.5.2/uic/Loader/
+-rw-r--r--   0 phil       (501) staff       (20)     1004 2023-07-22 15:08:24.351405 PyQt6-6.5.2/uic/Loader/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2625 2023-07-22 15:08:24.352917 PyQt6-6.5.2/uic/Loader/loader.py
+-rw-r--r--   0 phil       (501) staff       (20)     5187 2023-07-22 15:08:24.352421 PyQt6-6.5.2/uic/Loader/qobjectcreator.py
+-rw-r--r--   0 phil       (501) staff       (20)     1003 2023-07-22 15:08:24.350839 PyQt6-6.5.2/uic/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     6103 2023-07-22 15:08:24.364059 PyQt6-6.5.2/uic/compile_ui.py
+-rw-r--r--   0 phil       (501) staff       (20)    31764 2023-07-22 15:08:24.350248 PyQt6-6.5.2/uic/enum_map.py
+-rw-r--r--   0 phil       (501) staff       (20)     2609 2023-07-22 15:08:24.355238 PyQt6-6.5.2/uic/exceptions.py
+-rw-r--r--   0 phil       (501) staff       (20)     5047 2023-07-22 15:08:24.353968 PyQt6-6.5.2/uic/icon_cache.py
+-rw-r--r--   0 phil       (501) staff       (20)     3327 2023-07-22 15:08:24.354723 PyQt6-6.5.2/uic/load_ui.py
+-rw-r--r--   0 phil       (501) staff       (20)     6097 2023-07-22 15:08:24.342310 PyQt6-6.5.2/uic/objcreator.py
+-rw-r--r--   0 phil       (501) staff       (20)    18275 2023-07-22 15:08:24.345306 PyQt6-6.5.2/uic/properties.py
+-rw-r--r--   0 phil       (501) staff       (20)     5850 2023-07-22 15:08:24.356286 PyQt6-6.5.2/uic/pyuic.py
+-rw-r--r--   0 phil       (501) staff       (20)     3213 2023-07-22 15:08:24.336506 PyQt6-6.5.2/uic/ui_file.py
+-rw-r--r--   0 phil       (501) staff       (20)    37502 2023-07-22 15:08:24.341264 PyQt6-6.5.2/uic/uiparser.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-22 15:08:32.537070 PyQt6-6.5.2/uic/widget-plugins/
+-rw-r--r--   0 phil       (501) staff       (20)     1557 2023-07-22 15:08:24.347839 PyQt6-6.5.2/uic/widget-plugins/qaxcontainer.py
+-rw-r--r--   0 phil       (501) staff       (20)     1553 2023-07-22 15:08:24.345768 PyQt6-6.5.2/uic/widget-plugins/qscintilla.py
+-rw-r--r--   0 phil       (501) staff       (20)     1562 2023-07-22 15:08:24.346551 PyQt6-6.5.2/uic/widget-plugins/qtcharts.py
+-rw-r--r--   0 phil       (501) staff       (20)     1588 2023-07-22 15:08:24.346938 PyQt6-6.5.2/uic/widget-plugins/qtprintsupport.py
+-rw-r--r--   0 phil       (501) staff       (20)     1562 2023-07-22 15:08:24.347334 PyQt6-6.5.2/uic/widget-plugins/qtquickwidgets.py
+-rw-r--r--   0 phil       (501) staff       (20)     1568 2023-07-22 15:08:24.346197 PyQt6-6.5.2/uic/widget-plugins/qtwebenginewidgets.py
```

### Comparing `PyQt6-6.5.1/ChangeLog` & `PyQt6-6.5.2/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,99 @@
+2023-07-22  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, extras/lupdate/python_source.py:
+	Fixed an exception in pylupdate.
+	[38c17a29338d] [6.5.2] <6.5-maint>
+
+2023-07-21  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, qpy/QtCore/qstring.sip:
+	Fixed a regression in using None as a QString.
+	[6089948fc034] <6.5-maint>
+
+2023-07-15  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6.msp:
+	Fixed the type hints for all ellipsis arguments.
+	[dc5cc8a6f07d] <6.5-maint>
+
+2023-07-14  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* qpy/QtCore/qstring.sip:
+	Further fix fro QString's type hint.
+	[5c0f11c46cb1] <6.5-maint>
+
+	* NEWS, qpy/QtCore/qstring.sip:
+	Fixed the type hint for QString.
+	[2857fd3946c7] <6.5-maint>
+
+2023-07-12  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* PyQt6.msp:
+	Another type hint fix for QObject.findChild().
+	[dd57f73873eb] <6.5-maint>
+
+	* PyQt6.msp:
+	Fixed the type hints fro QObject.findChild() and
+	QObject.findChildren().
+	[b088d75e77d6] <6.5-maint>
+
+2023-07-09  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6.msp:
+	Fixed PYQT_SLOT for the QtCore module.
+	[f5cb0b97d94e] <6.5-maint>
+
+2023-07-05  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* extras/lupdate/python_source.py:
+	pylupdate will now look for tr() and translate() as a function as
+	well as a method.
+	[a0230e25929a] <6.5-maint>
+
+	* PyQt6.msp:
+	Fixed the type hint for pyqtSlot().
+	[b8e51995b3c5] <6.5-maint>
+
+	* PyQt6.msp:
+	Fixed the type hint for PYQT_SLOT.
+	[8c73a0c3dd1f] <6.5-maint>
+
+	* NEWS, PyQt6.msp, qpy/QtCore/qbytearrayview.sip:
+	Fixed the type hints for QByteArray and QByteArrayView.
+	[f631f8e6cc3e] <6.5-maint>
+
+2023-06-08  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6.msp, project.py:
+	Added the missing QEvent.Type.EnterEditFocus and
+	QEvent.Type.LeaveEditFocus enum members.
+	[a8d9583f33d9] <6.5-maint>
+
+	* NEWS, PyQt6.msp:
+	Added the missing QEvent.Type.NativeGesture and QEvent.Type.Quit
+	enum members.
+	[ebd0738bb268] <6.5-maint>
+
+2023-06-04  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS:
+	Updated the NEWS file.
+	[6590e301a19c] <6.5-maint>
+
+	* config-tests/cfgtest_QtCore.cpp:
+	Fixed building against Qt older than v6.5.
+	[4860e1d699d4] <6.5-maint>
+
+2023-06-02  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* .hgtags:
+	Added tag 6.5.1 for changeset 443f350df939
+	[9d6e72a95cae] <6.5-maint>
+
 2023-05-26  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, qpy/QtCore/qpycore_pyqtboundsignal.cpp:
 	Fixed a regression that broke pyqtSlot arguments that where
 	typedefs.
 	[443f350df939] [6.5.1] <6.5-maint>
```

### Comparing `PyQt6-6.5.1/LICENSE` & `PyQt6-6.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/NEWS` & `PyQt6-6.5.2/NEWS`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v6.5.2 22nd July 2023
+  - Added the missing NativeGesture, Quit, EnterEditFocus and LeaveEditFocus
+    members of QEventType.
+  - Bug fixes.
+
 v6.5.1 26th May 2023
   - Added support for QPermission and related classes and methods.
   - Added the max_workers argument to uic.compileUiDir() to specifiy the
     maximum number of worker processes to use when compiling the .ui files in a
     directory.
   - pyuic6 will now compile all the .ui files in a directory if the name of the
     directory is passed instead of a .ui file.
```

### Comparing `PyQt6-6.5.1/PKG-INFO` & `PyQt6-6.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6
-Version: 6.5.1
+Version: 6.5.2
 Requires-Python: >=3.6.1
 Summary: Python bindings for the Qt cross platform application toolkit
 Home-Page: https://www.riverbankcomputing.com/software/pyqt/
 Author: Riverbank Computing Limited
 Author-Email: info@riverbankcomputing.com
 License: GPL v3
 Requires-Dist: PyQt6-sip (>=13.4, <14)
```

### Comparing `PyQt6-6.5.1/README` & `PyQt6-6.5.2/README`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/__init__.py` & `PyQt6-6.5.2/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/config-tests/cfgtest_QtCore.cpp` & `PyQt6-6.5.2/config-tests/cfgtest_QtCore.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -27,13 +27,13 @@
     out << "PyQt_Process\n";
 #endif
 
     // qreal is double unless QT_COORD_TYPE is defined.
     if (sizeof (qreal) != sizeof (double))
         out << "PyQt_qreal_double\n";
 
-#if !QT_CONFIG(permissions)
+#if QT_VERSION < 0x060500 || !QT_CONFIG(permissions)
     out << "PyQt_Permissions";
 #endif
 
     return 0;
 }
```

### Comparing `PyQt6-6.5.1/config-tests/cfgtest_QtGui.cpp` & `PyQt6-6.5.2/config-tests/cfgtest_QtGui.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/config-tests/cfgtest_QtNetwork.cpp` & `PyQt6-6.5.2/config-tests/cfgtest_QtNetwork.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/config-tests/cfgtest_QtPrintSupport.cpp` & `PyQt6-6.5.2/config-tests/cfgtest_QtPrintSupport.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/dbus/dbus.cpp` & `PyQt6-6.5.2/dbus/dbus.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/dbus/helper.h` & `PyQt6-6.5.2/dbus/helper.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/designer/pluginloader.cpp` & `PyQt6-6.5.2/designer/pluginloader.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/designer/pluginloader.h` & `PyQt6-6.5.2/designer/pluginloader.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/calculatorform/calculatorform.py` & `PyQt6-6.5.2/examples/designer/calculatorform/calculatorform.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/calculatorform/calculatorform.ui` & `PyQt6-6.5.2/examples/designer/calculatorform/calculatorform.ui`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/calculatorform/ui_calculatorform.py` & `PyQt6-6.5.2/examples/designer/calculatorform/ui_calculatorform.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/plugins.py` & `PyQt6-6.5.2/examples/designer/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/python/analogclockplugin.py` & `PyQt6-6.5.2/examples/designer/plugins/python/analogclockplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/python/bubbleswidgetplugin.py` & `PyQt6-6.5.2/examples/designer/plugins/python/bubbleswidgetplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/python/counterlabelplugin.py` & `PyQt6-6.5.2/examples/designer/plugins/python/counterlabelplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/python/datetimeeditplugin.py` & `PyQt6-6.5.2/examples/designer/plugins/python/datetimeeditplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/python/helloglwidgetplugin.py` & `PyQt6-6.5.2/examples/designer/plugins/python/helloglwidgetplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/python/multipagewidgetplugin.py` & `PyQt6-6.5.2/examples/designer/plugins/python/multipagewidgetplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/python/polygonwidgetplugin.py` & `PyQt6-6.5.2/examples/designer/plugins/python/polygonwidgetplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/python/pydemoplugin.py` & `PyQt6-6.5.2/examples/designer/plugins/python/pydemoplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/python/pythonconsoleplugin.py` & `PyQt6-6.5.2/examples/designer/plugins/python/pythonconsoleplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/widgets/analogclock.py` & `PyQt6-6.5.2/examples/designer/plugins/widgets/analogclock.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/widgets/bubbleswidget.py` & `PyQt6-6.5.2/examples/designer/plugins/widgets/bubbleswidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/widgets/counterlabel.py` & `PyQt6-6.5.2/examples/designer/plugins/widgets/counterlabel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/widgets/datetimeedit.py` & `PyQt6-6.5.2/examples/designer/plugins/widgets/datetimeedit.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/widgets/helloglwidget.py` & `PyQt6-6.5.2/examples/designer/plugins/widgets/helloglwidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/widgets/multipagewidget.py` & `PyQt6-6.5.2/examples/designer/plugins/widgets/multipagewidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/widgets/polygonwidget.py` & `PyQt6-6.5.2/examples/designer/plugins/widgets/polygonwidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/widgets/pydemo.py` & `PyQt6-6.5.2/examples/designer/plugins/widgets/pydemo.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/designer/plugins/widgets/pythonconsolewidget.py` & `PyQt6-6.5.2/examples/designer/plugins/widgets/pythonconsolewidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/desktop/screenshot.py` & `PyQt6-6.5.2/examples/desktop/screenshot.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/desktop/systray/images/bad.png` & `PyQt6-6.5.2/examples/desktop/systray/images/bad.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/desktop/systray/images/heart.png` & `PyQt6-6.5.2/examples/desktop/systray/images/heart.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/desktop/systray/images/trash.png` & `PyQt6-6.5.2/examples/desktop/systray/images/trash.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/desktop/systray/systray.py` & `PyQt6-6.5.2/examples/desktop/systray/systray.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/classwizard/classwizard.py` & `PyQt6-6.5.2/examples/dialogs/classwizard/classwizard.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/classwizard/images/background.png` & `PyQt6-6.5.2/examples/dialogs/classwizard/images/background.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/classwizard/images/banner.png` & `PyQt6-6.5.2/examples/dialogs/classwizard/images/banner.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/classwizard/images/logo1.png` & `PyQt6-6.5.2/examples/dialogs/classwizard/images/logo1.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/classwizard/images/logo2.png` & `PyQt6-6.5.2/examples/dialogs/classwizard/images/logo2.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/classwizard/images/logo3.png` & `PyQt6-6.5.2/examples/dialogs/classwizard/images/logo3.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/classwizard/images/watermark1.png` & `PyQt6-6.5.2/examples/dialogs/classwizard/images/watermark1.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/classwizard/images/watermark2.png` & `PyQt6-6.5.2/examples/dialogs/classwizard/images/watermark2.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/configdialog/configdialog.py` & `PyQt6-6.5.2/examples/dialogs/configdialog/configdialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/configdialog/images/config.png` & `PyQt6-6.5.2/examples/dialogs/configdialog/images/config.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/configdialog/images/query.png` & `PyQt6-6.5.2/examples/dialogs/configdialog/images/query.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/configdialog/images/update.png` & `PyQt6-6.5.2/examples/dialogs/configdialog/images/update.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/extension.py` & `PyQt6-6.5.2/examples/dialogs/extension.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/findfiles.py` & `PyQt6-6.5.2/examples/dialogs/findfiles.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/standarddialogs.py` & `PyQt6-6.5.2/examples/dialogs/standarddialogs.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/tabdialog.py` & `PyQt6-6.5.2/examples/dialogs/tabdialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/dialogs/trivialwizard.py` & `PyQt6-6.5.2/examples/dialogs/trivialwizard.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/delayedencoding/delayedencoding.py` & `PyQt6-6.5.2/examples/draganddrop/delayedencoding/delayedencoding.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/delayedencoding/images/drag.png` & `PyQt6-6.5.2/examples/draganddrop/delayedencoding/images/drag.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/delayedencoding/images/example.svg` & `PyQt6-6.5.2/examples/draganddrop/delayedencoding/images/example.svg`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/draggableicons/draggableicons.py` & `PyQt6-6.5.2/examples/draganddrop/draggableicons/draggableicons.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/draggableicons/images/boat.png` & `PyQt6-6.5.2/examples/draganddrop/draggableicons/images/boat.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/draggableicons/images/car.png` & `PyQt6-6.5.2/examples/draganddrop/draggableicons/images/car.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/draggableicons/images/house.png` & `PyQt6-6.5.2/examples/draganddrop/draggableicons/images/house.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/draggabletext/draggabletext.py` & `PyQt6-6.5.2/examples/draganddrop/draggabletext/draggabletext.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/dropsite.py` & `PyQt6-6.5.2/examples/draganddrop/dropsite.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/fridgemagnets/fridgemagnets.py` & `PyQt6-6.5.2/examples/draganddrop/fridgemagnets/fridgemagnets.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/puzzle/example.jpg` & `PyQt6-6.5.2/examples/draganddrop/puzzle/example.jpg`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/draganddrop/puzzle/puzzle.py` & `PyQt6-6.5.2/examples/draganddrop/puzzle/puzzle.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimedia/audiodevices/audiodevices.py` & `PyQt6-6.5.2/examples/multimedia/audiodevices/audiodevices.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimedia/audiodevices/audiodevicesbase.ui` & `PyQt6-6.5.2/examples/multimedia/audiodevices/audiodevicesbase.ui`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimedia/audiodevices/ui_audiodevicesbase.py` & `PyQt6-6.5.2/examples/multimedia/audiodevices/ui_audiodevicesbase.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimedia/audiooutput.py` & `PyQt6-6.5.2/examples/multimedia/audiooutput.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimediawidgets/camera/camera.py` & `PyQt6-6.5.2/examples/multimediawidgets/camera/camera.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimediawidgets/camera/camera.ui` & `PyQt6-6.5.2/examples/multimediawidgets/camera/camera.ui`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimediawidgets/camera/images/shutter.svg` & `PyQt6-6.5.2/examples/multimediawidgets/camera/images/shutter.svg`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimediawidgets/camera/imagesettings.ui` & `PyQt6-6.5.2/examples/multimediawidgets/camera/imagesettings.ui`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimediawidgets/camera/ui_camera.py` & `PyQt6-6.5.2/examples/multimediawidgets/camera/ui_camera.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimediawidgets/camera/ui_imagesettings.py` & `PyQt6-6.5.2/examples/multimediawidgets/camera/ui_imagesettings.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimediawidgets/camera/ui_videosettings.py` & `PyQt6-6.5.2/examples/multimediawidgets/camera/ui_videosettings.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimediawidgets/camera/videosettings.ui` & `PyQt6-6.5.2/examples/multimediawidgets/camera/videosettings.ui`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimediawidgets/videographicsitem.py` & `PyQt6-6.5.2/examples/multimediawidgets/videographicsitem.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/multimediawidgets/videowidget.py` & `PyQt6-6.5.2/examples/multimediawidgets/videowidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/qml/referenceexamples/adding.py` & `PyQt6-6.5.2/examples/qml/referenceexamples/adding.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/qml/referenceexamples/attached.py` & `PyQt6-6.5.2/examples/qml/referenceexamples/attached.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/qml/referenceexamples/binding.py` & `PyQt6-6.5.2/examples/qml/referenceexamples/binding.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/qml/referenceexamples/coercion.py` & `PyQt6-6.5.2/examples/qml/referenceexamples/coercion.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/qml/referenceexamples/default.py` & `PyQt6-6.5.2/examples/qml/referenceexamples/default.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/qml/referenceexamples/grouped.py` & `PyQt6-6.5.2/examples/qml/referenceexamples/grouped.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/qml/referenceexamples/methods.py` & `PyQt6-6.5.2/examples/qml/referenceexamples/methods.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/qml/referenceexamples/properties.py` & `PyQt6-6.5.2/examples/qml/referenceexamples/properties.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/qml/referenceexamples/signal.py` & `PyQt6-6.5.2/examples/qml/referenceexamples/signal.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/qml/referenceexamples/valuesource.py` & `PyQt6-6.5.2/examples/qml/referenceexamples/valuesource.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/animation.py` & `PyQt6-6.5.2/examples/quick/animation/animation.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/animation.qml` & `PyQt6-6.5.2/examples/quick/animation/animation.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/basics/color-animation.qml` & `PyQt6-6.5.2/examples/quick/animation/basics/color-animation.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/basics/images/face-smile.png` & `PyQt6-6.5.2/examples/quick/animation/basics/images/face-smile.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/basics/images/moon.png` & `PyQt6-6.5.2/examples/quick/animation/basics/images/moon.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/basics/images/sun.png` & `PyQt6-6.5.2/examples/quick/animation/basics/images/sun.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/basics/property-animation.qml` & `PyQt6-6.5.2/examples/quick/animation/basics/property-animation.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/behaviors/SideRect.qml` & `PyQt6-6.5.2/examples/quick/animation/behaviors/SideRect.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/behaviors/behavior-example.qml` & `PyQt6-6.5.2/examples/quick/animation/behaviors/behavior-example.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/behaviors/tvtennis.qml` & `PyQt6-6.5.2/examples/quick/animation/behaviors/tvtennis.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/behaviors/wigglytext.qml` & `PyQt6-6.5.2/examples/quick/animation/behaviors/wigglytext.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/easing/easing.qml` & `PyQt6-6.5.2/examples/quick/animation/easing/easing.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/pathanimation/pathanimation.qml` & `PyQt6-6.5.2/examples/quick/animation/pathanimation/pathanimation.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/pathinterpolator/pathinterpolator.qml` & `PyQt6-6.5.2/examples/quick/animation/pathinterpolator/pathinterpolator.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/states/qt-logo.png` & `PyQt6-6.5.2/examples/quick/animation/states/qt-logo.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/states/states.qml` & `PyQt6-6.5.2/examples/quick/animation/states/states.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/animation/states/transitions.qml` & `PyQt6-6.5.2/examples/quick/animation/states/transitions.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/bezierCurve/bezierCurve.qml` & `PyQt6-6.5.2/examples/quick/canvas/bezierCurve/bezierCurve.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/canvas.py` & `PyQt6-6.5.2/examples/quick/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/canvas.qml` & `PyQt6-6.5.2/examples/quick/canvas/canvas.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/clip/clip.qml` & `PyQt6-6.5.2/examples/quick/canvas/clip/clip.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/Button.qml` & `PyQt6-6.5.2/examples/quick/canvas/contents/Button.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/ScrollBar.qml` & `PyQt6-6.5.2/examples/quick/canvas/contents/ScrollBar.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/Slider.qml` & `PyQt6-6.5.2/examples/quick/canvas/contents/Slider.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/TitleBar.qml` & `PyQt6-6.5.2/examples/quick/canvas/contents/TitleBar.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/ToolBar.qml` & `PyQt6-6.5.2/examples/quick/canvas/contents/ToolBar.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/images/button-pressed.png` & `PyQt6-6.5.2/examples/quick/canvas/contents/images/button-pressed.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/images/button.png` & `PyQt6-6.5.2/examples/quick/canvas/contents/images/button.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/images/default.svg` & `PyQt6-6.5.2/examples/quick/canvas/contents/images/default.svg`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/images/gloss.png` & `PyQt6-6.5.2/examples/quick/canvas/contents/images/gloss.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/images/lineedit.png` & `PyQt6-6.5.2/examples/quick/canvas/contents/images/lineedit.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/images/quit.png` & `PyQt6-6.5.2/examples/quick/canvas/contents/images/quit.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/images/titlebar.png` & `PyQt6-6.5.2/examples/quick/canvas/contents/images/titlebar.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/images/toolbutton.png` & `PyQt6-6.5.2/examples/quick/canvas/contents/images/toolbutton.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/contents/qt-logo.png` & `PyQt6-6.5.2/examples/quick/canvas/contents/qt-logo.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/quadraticCurveTo/quadraticCurveTo.qml` & `PyQt6-6.5.2/examples/quick/canvas/quadraticCurveTo/quadraticCurveTo.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/roundedrect/roundedrect.qml` & `PyQt6-6.5.2/examples/quick/canvas/roundedrect/roundedrect.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/smile/smile.qml` & `PyQt6-6.5.2/examples/quick/canvas/smile/smile.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/squircle/squircle.png` & `PyQt6-6.5.2/examples/quick/canvas/squircle/squircle.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/squircle/squircle.qml` & `PyQt6-6.5.2/examples/quick/canvas/squircle/squircle.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/tiger/tiger.js` & `PyQt6-6.5.2/examples/quick/canvas/tiger/tiger.js`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/canvas/tiger/tiger.qml` & `PyQt6-6.5.2/examples/quick/canvas/tiger/tiger.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/models/abstractitemmodel/abstractitemmodel.py` & `PyQt6-6.5.2/examples/quick/models/abstractitemmodel/abstractitemmodel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/models/abstractitemmodel/view.qml` & `PyQt6-6.5.2/examples/quick/models/abstractitemmodel/view.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/models/objectlistmodel/objectlistmodel.py` & `PyQt6-6.5.2/examples/quick/models/objectlistmodel/objectlistmodel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/models/objectlistmodel/view.qml` & `PyQt6-6.5.2/examples/quick/models/objectlistmodel/view.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/models/stringlistmodel/stringlistmodel.py` & `PyQt6-6.5.2/examples/quick/models/stringlistmodel/stringlistmodel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/models/stringlistmodel/view.qml` & `PyQt6-6.5.2/examples/quick/models/stringlistmodel/view.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/scenegraph/customgeometry/customgeometry.py` & `PyQt6-6.5.2/examples/quick/scenegraph/customgeometry/customgeometry.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/scenegraph/customgeometry/main.qml` & `PyQt6-6.5.2/examples/quick/scenegraph/customgeometry/main.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/shared/Button.qml` & `PyQt6-6.5.2/examples/quick/shared/Button.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/shared/LauncherList.qml` & `PyQt6-6.5.2/examples/quick/shared/LauncherList.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/shared/SimpleLauncherDelegate.qml` & `PyQt6-6.5.2/examples/quick/shared/SimpleLauncherDelegate.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/shared/images/back.png` & `PyQt6-6.5.2/examples/quick/shared/images/back.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/shared/images/next.png` & `PyQt6-6.5.2/examples/quick/shared/images/next.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter1-basics/app.qml` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter1-basics/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter1-basics/chapter1-basics.py` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter1-basics/chapter1-basics.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter2-methods/app.qml` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter2-methods/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter2-methods/chapter2-methods.py` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter2-methods/chapter2-methods.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter3-bindings/app.qml` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter3-bindings/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter3-bindings/chapter3-bindings.py` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter3-bindings/chapter3-bindings.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter4-customPropertyTypes/app.qml` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter4-customPropertyTypes/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter4-customPropertyTypes/chapter4-customPropertyTypes.py` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter4-customPropertyTypes/chapter4-customPropertyTypes.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter5-listproperties/app.qml` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter5-listproperties/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter5-listproperties/chapter5-listproperties.py` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter5-listproperties/chapter5-listproperties.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/Charts/chartsplugin.py` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/chartsplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/Charts/piechart.py` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/piechart.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/Charts/pieslice.py` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/pieslice.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/quick/tutorials/extending/chapter6-plugins/app.qml` & `PyQt6-6.5.2/examples/quick/tutorials/extending/chapter6-plugins/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/richtext/textobject/heart.svg` & `PyQt6-6.5.2/examples/richtext/textobject/heart.svg`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/examples/richtext/textobject/textobject.py` & `PyQt6-6.5.2/examples/richtext/textobject/textobject.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/lupdate/__init__.py` & `PyQt6-6.5.2/lupdate/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/lupdate/designer_source.py` & `PyQt6-6.5.2/lupdate/designer_source.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/lupdate/lupdate.py` & `PyQt6-6.5.2/lupdate/lupdate.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/lupdate/pylupdate.py` & `PyQt6-6.5.2/lupdate/pylupdate.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/lupdate/python_source.py` & `PyQt6-6.5.2/lupdate/python_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,26 +145,29 @@
 
         # Parse the arguments if a translation function is being called.
         call_args = None
 
         if isinstance(node.func, ast.Attribute):
             name = node.func.attr
 
-            if name == 'tr':
-                call_args = self._parse_tr(node)
-            elif name == 'translate':
-                call_args = self._parse_translate(node)
-
         elif isinstance(node.func, ast.Name):
             name = node.func.id
 
             if name == 'QT_TR_NOOP':
                 call_args = self._parse_QT_TR_NOOP(node)
             elif name == 'QT_TRANSLATE_NOOP':
                 call_args = self._parse_QT_TRANSLATE_NOOP(node)
+        else:
+            name = ''
+
+        # Allow these to be either methods or functions.
+        if name == 'tr':
+            call_args = self._parse_tr(node)
+        elif name == 'translate':
+            call_args = self._parse_translate(node)
 
         # Update the context if the arguments are usable.
         if call_args is not None and call_args.source != '':
             call_args.context.messages.append(
                     Message(self._source.filename, node.lineno,
                             call_args.source, call_args.disambiguation,
                             (call_args.numerus)))
```

### Comparing `PyQt6-6.5.1/lupdate/source_file.py` & `PyQt6-6.5.2/lupdate/source_file.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/lupdate/translation_file.py` & `PyQt6-6.5.2/lupdate/translation_file.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/lupdate/translations.py` & `PyQt6-6.5.2/lupdate/translations.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/lupdate/user.py` & `PyQt6-6.5.2/lupdate/user.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/project.py` & `PyQt6-6.5.2/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,15 +501,16 @@
 
 class QtCore(PyQtBindings):
     """ The QtCore bindings. """
 
     def __init__(self, project):
         """ Initialise the bindings. """
 
-        super().__init__(project, 'QtCore', qmake_QT=['-gui'])
+        super().__init__(project, 'QtCore', qmake_QT=['-gui'],
+                define_macros=['QT_KEYPAD_NAVIGATION'])
 
     def handle_test_output(self, test_output):
         """ Handle the output from the external test program and return True if
         the bindings are buildable.
         """
 
         project = self.project
```

### Comparing `PyQt6-6.5.1/pyproject.toml` & `PyQt6-6.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["sip >=6.5, <7", "PyQt-builder >=1.15, <2"]
 build-backend = "sipbuild.api"
 
 # Specify the PEP 566 metadata for the project.
 [tool.sip.metadata]
 name = "PyQt6"
-version = "6.5.1"
+version = "6.5.2"
 summary = "Python bindings for the Qt cross platform application toolkit"
 home-page = "https://www.riverbankcomputing.com/software/pyqt/"
 author = "Riverbank Computing Limited"
 author-email = "info@riverbankcomputing.com"
 license = "GPL v3"
 description-file = "README"
 requires-python = ">=3.6.1"
```

### Comparing `PyQt6-6.5.1/qmlscene/pluginloader.cpp` & `PyQt6-6.5.2/qmlscene/pluginloader.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qmlscene/pluginloader.h` & `PyQt6-6.5.2/qmlscene/pluginloader.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_api.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_chimera.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_chimera.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_chimera.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_chimera.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_chimera_signature.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_chimera_signature.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_chimera_storage.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_chimera_storage.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_classinfo.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_classinfo.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_classinfo.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_classinfo.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_decorators.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_decorators.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_enums_flags.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_enums_flags.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_enums_flags.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_enums_flags.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_event_handlers.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_event_handlers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_event_handlers.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_event_handlers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_init.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_misc.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_misc.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_misc.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_misc.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_namespace.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_namespace.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_objectified_strings.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_objectified_strings.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_post_init.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_post_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_public_api.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_public_api.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_public_api.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_public_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtboundsignal.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtboundsignal.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtboundsignal.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtboundsignal.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtconfigure.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtconfigure.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtmethodproxy.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtmethodproxy.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtmethodproxy.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtmethodproxy.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtmutexlocker.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtmutexlocker.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtmutexlocker.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtmutexlocker.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtproperty.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtproperty.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtproperty.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtproperty.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtpyobject.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtpyobject.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtpyobject.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtpyobject.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtsignal.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtsignal.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtsignal.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtsignal.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtslot.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtslot.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtslot.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtslot.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtslotproxy.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtslotproxy.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_pyqtslotproxy.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_pyqtslotproxy.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qjsonvalue.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qjsonvalue.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qmessagelogger.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qmessagelogger.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qmetaobject.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qmetaobject.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qmetaobject_helpers.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qmetaobject_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qmetaobjectbuilder.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qmetaobjectbuilder.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qobject_getattr.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qobject_getattr.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qobject_helpers.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qobject_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qobject_helpers.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qobject_helpers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qstring.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qstring.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qt_conf.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qt_conf.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qvariant.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qvariant.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_qvariant_value.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_qvariant_value.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_types.cpp` & `PyQt6-6.5.2/qpy/QtCore/qpycore_types.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtCore/qpycore_types.h` & `PyQt6-6.5.2/qpy/QtCore/qpycore_types.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDBus/qpydbus_api.h` & `PyQt6-6.5.2/qpy/QtDBus/qpydbus_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDBus/qpydbus_chimera_helpers.cpp` & `PyQt6-6.5.2/qpy/QtDBus/qpydbus_chimera_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDBus/qpydbus_chimera_helpers.h` & `PyQt6-6.5.2/qpy/QtDBus/qpydbus_chimera_helpers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDBus/qpydbus_post_init.cpp` & `PyQt6-6.5.2/qpy/QtDBus/qpydbus_post_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDBus/qpydbuspendingreply.cpp` & `PyQt6-6.5.2/qpy/QtDBus/qpydbuspendingreply.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDBus/qpydbuspendingreply.h` & `PyQt6-6.5.2/qpy/QtDBus/qpydbuspendingreply.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDBus/qpydbusreply.cpp` & `PyQt6-6.5.2/qpy/QtDBus/qpydbusreply.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDBus/qpydbusreply.h` & `PyQt6-6.5.2/qpy/QtDBus/qpydbusreply.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDesigner/qpydesignercontainerextension.h` & `PyQt6-6.5.2/qpy/QtDesigner/qpydesignercontainerextension.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDesigner/qpydesignercustomwidgetcollectionplugin.h` & `PyQt6-6.5.2/qpy/QtDesigner/qpydesignercustomwidgetcollectionplugin.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDesigner/qpydesignercustomwidgetplugin.h` & `PyQt6-6.5.2/qpy/QtDesigner/qpydesignercustomwidgetplugin.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDesigner/qpydesignermembersheetextension.h` & `PyQt6-6.5.2/qpy/QtDesigner/qpydesignermembersheetextension.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDesigner/qpydesignerpropertysheetextension.h` & `PyQt6-6.5.2/qpy/QtDesigner/qpydesignerpropertysheetextension.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtDesigner/qpydesignertaskmenuextension.h` & `PyQt6-6.5.2/qpy/QtDesigner/qpydesignertaskmenuextension.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_add_constants.cpp` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_add_constants.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_api.h` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_array_convertors.cpp` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_array_convertors.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_attribute_array.cpp` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_attribute_array.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_data_cache.cpp` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_data_cache.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_data_cache.h` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_data_cache.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_get.cpp` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_get.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_init.cpp` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_misc.h` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_misc.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_uniform_value_array.cpp` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_uniform_value_array.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_value_array.cpp` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_value_array.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtOpenGL/qpyopengl_version_functions.cpp` & `PyQt6-6.5.2/qpy/QtOpenGL/qpyopengl_version_functions.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqml_api.h` & `PyQt6-6.5.2/qpy/QtQml/qpyqml_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqml_listdata.cpp` & `PyQt6-6.5.2/qpy/QtQml/qpyqml_listdata.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqml_listdata.h` & `PyQt6-6.5.2/qpy/QtQml/qpyqml_listdata.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqml_post_init.cpp` & `PyQt6-6.5.2/qpy/QtQml/qpyqml_post_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqml_qjsvalue.cpp` & `PyQt6-6.5.2/qpy/QtQml/qpyqml_qjsvalue.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqml_register_singleton_type.cpp` & `PyQt6-6.5.2/qpy/QtQml/qpyqml_register_singleton_type.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqml_register_type.cpp` & `PyQt6-6.5.2/qpy/QtQml/qpyqml_register_type.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqmllistproperty.cpp` & `PyQt6-6.5.2/qpy/QtQml/qpyqmllistproperty.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqmllistproperty.h` & `PyQt6-6.5.2/qpy/QtQml/qpyqmllistproperty.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqmllistpropertywrapper.cpp` & `PyQt6-6.5.2/qpy/QtQml/qpyqmllistpropertywrapper.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqmllistpropertywrapper.h` & `PyQt6-6.5.2/qpy/QtQml/qpyqmllistpropertywrapper.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqmlobject.cpp` & `PyQt6-6.5.2/qpy/QtQml/qpyqmlobject.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqmlobject.h` & `PyQt6-6.5.2/qpy/QtQml/qpyqmlobject.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqmlsingletonobject.cpp` & `PyQt6-6.5.2/qpy/QtQml/qpyqmlsingletonobject.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqmlsingletonobject.h` & `PyQt6-6.5.2/qpy/QtQml/qpyqmlsingletonobject.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqmlvalidator.cpp` & `PyQt6-6.5.2/qpy/QtQml/qpyqmlvalidator.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQml/qpyqmlvalidator.h` & `PyQt6-6.5.2/qpy/QtQml/qpyqmlvalidator.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquick_api.h` & `PyQt6-6.5.2/qpy/QtQuick/qpyquick_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquick_chimera_helpers.cpp` & `PyQt6-6.5.2/qpy/QtQuick/qpyquick_chimera_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquick_chimera_helpers.h` & `PyQt6-6.5.2/qpy/QtQuick/qpyquick_chimera_helpers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquick_post_init.cpp` & `PyQt6-6.5.2/qpy/QtQuick/qpyquick_post_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquick_register_type.cpp` & `PyQt6-6.5.2/qpy/QtQuick/qpyquick_register_type.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquick_register_type.h` & `PyQt6-6.5.2/qpy/QtQuick/qpyquick_register_type.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquickframebufferobject.cpp` & `PyQt6-6.5.2/qpy/QtQuick/qpyquickframebufferobject.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquickframebufferobject.h` & `PyQt6-6.5.2/qpy/QtQuick/qpyquickframebufferobject.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquickitem.cpp` & `PyQt6-6.5.2/qpy/QtQuick/qpyquickitem.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquickitem.h` & `PyQt6-6.5.2/qpy/QtQuick/qpyquickitem.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquickpainteditem.cpp` & `PyQt6-6.5.2/qpy/QtQuick/qpyquickpainteditem.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquickpainteditem.h` & `PyQt6-6.5.2/qpy/QtQuick/qpyquickpainteditem.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquickview.cpp` & `PyQt6-6.5.2/qpy/QtQuick/qpyquickview.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquickview.h` & `PyQt6-6.5.2/qpy/QtQuick/qpyquickview.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquickwindow.cpp` & `PyQt6-6.5.2/qpy/QtQuick/qpyquickwindow.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtQuick/qpyquickwindow.h` & `PyQt6-6.5.2/qpy/QtQuick/qpyquickwindow.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_api.h` & `PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_chimera_helpers.cpp` & `PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_chimera_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_chimera_helpers.h` & `PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_chimera_helpers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_post_init.cpp` & `PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_post_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_qaction_helpers.cpp` & `PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_qaction_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/qpy/QtWidgets/qpywidgets_qaction_helpers.h` & `PyQt6-6.5.2/qpy/QtWidgets/qpywidgets_qaction_helpers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QAxContainer/QAxContainermod.sip` & `PyQt6-6.5.2/sip/QAxContainer/QAxContainermod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QAxContainer/qaxbase.sip` & `PyQt6-6.5.2/sip/QAxContainer/qaxbase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QAxContainer/qaxobject.sip` & `PyQt6-6.5.2/sip/QAxContainer/qaxobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QAxContainer/qaxobjectinterface.sip` & `PyQt6-6.5.2/sip/QAxContainer/qaxobjectinterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QAxContainer/qaxwidget.sip` & `PyQt6-6.5.2/sip/QAxContainer/qaxwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/QtBluetoothmod.sip` & `PyQt6-6.5.2/sip/QtBluetooth/QtBluetoothmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetooth.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetooth.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetoothaddress.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetoothaddress.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetoothdevicediscoveryagent.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetoothdevicediscoveryagent.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetoothdeviceinfo.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetoothdeviceinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetoothhostinfo.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetoothhostinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetoothlocaldevice.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetoothlocaldevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetoothserver.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetoothserver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetoothservicediscoveryagent.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetoothservicediscoveryagent.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetoothserviceinfo.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetoothserviceinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetoothsocket.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetoothsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qbluetoothuuid.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qbluetoothuuid.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qlowenergyadvertisingdata.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qlowenergyadvertisingdata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qlowenergyadvertisingparameters.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qlowenergyadvertisingparameters.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qlowenergycharacteristic.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qlowenergycharacteristic.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qlowenergycharacteristicdata.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qlowenergycharacteristicdata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qlowenergyconnectionparameters.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qlowenergyconnectionparameters.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qlowenergycontroller.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qlowenergycontroller.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qlowenergydescriptor.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qlowenergydescriptor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qlowenergydescriptordata.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qlowenergydescriptordata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qlowenergyservice.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qlowenergyservice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qlowenergyservicedata.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qlowenergyservicedata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qpybluetooth_qlist.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qpybluetooth_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qpybluetooth_qmultihash.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qpybluetooth_qmultihash.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtBluetooth/qpybluetooth_quint128.sip` & `PyQt6-6.5.2/sip/QtBluetooth/qpybluetooth_quint128.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/QtCoremod.sip` & `PyQt6-6.5.2/sip/QtCore/QtCoremod.sip`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 
 %DefaultSupertype PyQt6.sip.simplewrapper
 
 int PYQT_VERSION;
 const char *PYQT_VERSION_STR;
 
 %ModuleCode
-static int PYQT_VERSION = 0x060501;
-static const char *PYQT_VERSION_STR = "6.5.1";
+static int PYQT_VERSION = 0x060502;
+static const char *PYQT_VERSION_STR = "6.5.2";
 %End
 
 %Include qglobal.sip
 %Include qtenvironmentvariables.sip
 %Include qtversion.sip
 %Include qnamespace.sip
 %Include qabstractanimation.sip
```

### Comparing `PyQt6-6.5.1/sip/QtCore/qabstractanimation.sip` & `PyQt6-6.5.2/sip/QtCore/qabstractanimation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qabstracteventdispatcher.sip` & `PyQt6-6.5.2/sip/QtCore/qabstracteventdispatcher.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qabstractitemmodel.sip` & `PyQt6-6.5.2/sip/QtCore/qabstractitemmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qabstractnativeeventfilter.sip` & `PyQt6-6.5.2/sip/QtCore/qabstractnativeeventfilter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qabstractproxymodel.sip` & `PyQt6-6.5.2/sip/QtCore/qabstractproxymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qanimationgroup.sip` & `PyQt6-6.5.2/sip/QtCore/qanimationgroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qanystringview.sip` & `PyQt6-6.5.2/sip/QtCore/qanystringview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qbasictimer.sip` & `PyQt6-6.5.2/sip/QtCore/qbasictimer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qbitarray.sip` & `PyQt6-6.5.2/sip/QtCore/qbitarray.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qbuffer.sip` & `PyQt6-6.5.2/sip/QtCore/qbuffer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qbytearray.sip` & `PyQt6-6.5.2/sip/QtCore/qbytearray.sip`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 %ModuleCode
 #include <qbytearray.h>
 %End
 
-class QByteArray
+class QByteArray /TypeHintIn="Union[QByteArray, bytes, bytearray, memoryview]"/
 {
 %TypeHeaderCode
 #include <qbytearray.h>
 %End
 
 %TypeCode
 // This is needed by __hash__().
```

### Comparing `PyQt6-6.5.1/sip/QtCore/qbytearrayalgorithms.sip` & `PyQt6-6.5.2/sip/QtCore/qbytearrayalgorithms.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qbytearraylist.sip` & `PyQt6-6.5.2/sip/QtCore/qbytearraylist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qbytearraymatcher.sip` & `PyQt6-6.5.2/sip/QtCore/qbytearraymatcher.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qbytearrayview.sip` & `PyQt6-6.5.2/sip/QtCore/qbytearrayview.sip`

 * *Files 9% similar despite different names*

```diff
@@ -14,19 +14,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-// Note that the typing module doesn't have the means for describing objects
-// that implement the buffer protocol.  We therefore just document the common
-// cases for documentation purposes even though all of them are accessed via
-// the buffer protocol.
-%MappedType QByteArrayView /TypeHint="Union[QByteArray, bytes, bytearray, memoryview]"/
+%MappedType QByteArrayView /TypeHint="QByteArray"/
 {
 %TypeHeaderCode
 #include <qbytearrayview.h>
 %End
 
 %ConvertToTypeCode
 if (sipIsErr == NULL)
```

### Comparing `PyQt6-6.5.1/sip/QtCore/qcalendar.sip` & `PyQt6-6.5.2/sip/QtCore/qcalendar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qcborcommon.sip` & `PyQt6-6.5.2/sip/QtCore/qcborcommon.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qcborstreamreader.sip` & `PyQt6-6.5.2/sip/QtCore/qcborstreamreader.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qcborstreamwriter.sip` & `PyQt6-6.5.2/sip/QtCore/qcborstreamwriter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qchar.sip` & `PyQt6-6.5.2/sip/QtCore/qchar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qcollator.sip` & `PyQt6-6.5.2/sip/QtCore/qcollator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qcommandlineoption.sip` & `PyQt6-6.5.2/sip/QtCore/qcommandlineoption.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qcommandlineparser.sip` & `PyQt6-6.5.2/sip/QtCore/qcommandlineparser.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qconcatenatetablesproxymodel.sip` & `PyQt6-6.5.2/sip/QtCore/qconcatenatetablesproxymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qcoreapplication.sip` & `PyQt6-6.5.2/sip/QtCore/qcoreapplication.sip`

 * *Files 6% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 
 %ExportedTypeHintCode
 # Support for QDate, QDateTime and QTime.
 import datetime
 
 # Convenient type aliases.
 PYQT_SIGNAL = typing.Union[QtCore.pyqtSignal, QtCore.pyqtBoundSignal]
-PYQT_SLOT = typing.Union[typing.Callable[..., None], QtCore.pyqtBoundSignal]
+PYQT_SLOT = typing.Union[typing.Callable[..., Any], QtCore.pyqtBoundSignal]
 %End
 
 %TypeHintCode
 # Support for QDate, QDateTime and QTime.
 import datetime
 
 
@@ -389,11 +389,19 @@
 
     @typing.overload
     def disconnect(self, slot: typing.Union['PYQT_SLOT', 'QMetaObject.Connection']) -> None: ...
 
     def emit(self, *args: typing.Any) -> None: ...
 
 
+FuncT = typing.TypeVar('FuncT', bound=typing.Callable)
+def pyqtSlot(*types, name: typing.Optional[str] = ..., result: typing.Optional[str] = ...) -> typing.Callable[[FuncT], FuncT]: ...
+
+
+# For QObject.findChild() and QObject.findChildren().
+QObjectT = typing.TypeVar('QObjectT', bound=QObject)
+
+
 # Convenient type aliases.
 PYQT_SIGNAL = typing.Union[pyqtSignal, pyqtBoundSignal]
-PYQT_SLOT = typing.Union[typing.Callable[..., None], pyqtBoundSignal]
+PYQT_SLOT = typing.Union[typing.Callable[..., Any], pyqtBoundSignal]
 %End
```

### Comparing `PyQt6-6.5.1/sip/QtCore/qcoreevent.sip` & `PyQt6-6.5.2/sip/QtCore/qcoreevent.sip`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         Leave,
         Paint,
         Move,
         Resize,
         Show,
         Hide,
         Close,
+        Quit,
         ParentChange,
         ParentAboutToChange,
         ThreadChange,
         WindowActivate,
         WindowDeactivate,
         ShowToParent,
         HideToParent,
@@ -176,14 +177,15 @@
         GrabKeyboard,
         UngrabKeyboard,
         StateMachineSignal,
         StateMachineWrapped,
         TouchBegin,
         TouchUpdate,
         TouchEnd,
+        NativeGesture,
         RequestSoftwareInputPanel,
         CloseSoftwareInputPanel,
         WinIdChange,
         Gesture,
         GestureOverride,
         FocusAboutToChange,
         ScrollPrepare,
@@ -194,14 +196,16 @@
         TouchCancel,
         PlatformPanel,
         ApplicationStateChange,
         ReadOnlyChange,
         PlatformSurface,
         TabletTrackingChange,
         GraphicsSceneLeave,
+        EnterEditFocus,
+        LeaveEditFocus,
         User,
         MaxUser,
     };
 
     explicit QEvent(QEvent::Type type);
     QEvent(int type) /Deprecated, NoDerived/;
 %MethodCode
```

### Comparing `PyQt6-6.5.1/sip/QtCore/qcryptographichash.sip` & `PyQt6-6.5.2/sip/QtCore/qcryptographichash.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qdatastream.sip` & `PyQt6-6.5.2/sip/QtCore/qdatastream.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qdatetime.sip` & `PyQt6-6.5.2/sip/QtCore/qdatetime.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qdeadlinetimer.sip` & `PyQt6-6.5.2/sip/QtCore/qdeadlinetimer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qdir.sip` & `PyQt6-6.5.2/sip/QtCore/qdir.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qdiriterator.sip` & `PyQt6-6.5.2/sip/QtCore/qdiriterator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qeasingcurve.sip` & `PyQt6-6.5.2/sip/QtCore/qeasingcurve.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qelapsedtimer.sip` & `PyQt6-6.5.2/sip/QtCore/qelapsedtimer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qeventloop.sip` & `PyQt6-6.5.2/sip/QtCore/qeventloop.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qfile.sip` & `PyQt6-6.5.2/sip/QtCore/qfile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qfiledevice.sip` & `PyQt6-6.5.2/sip/QtCore/qfiledevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qfileinfo.sip` & `PyQt6-6.5.2/sip/QtCore/qfileinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qfileselector.sip` & `PyQt6-6.5.2/sip/QtCore/qfileselector.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qfilesystemwatcher.sip` & `PyQt6-6.5.2/sip/QtCore/qfilesystemwatcher.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qflags.sip` & `PyQt6-6.5.2/sip/QtCore/qflags.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qglobal.sip` & `PyQt6-6.5.2/sip/QtCore/qglobal.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qidentityproxymodel.sip` & `PyQt6-6.5.2/sip/QtCore/qidentityproxymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qiodevice.sip` & `PyQt6-6.5.2/sip/QtCore/qiodevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qiodevicebase.sip` & `PyQt6-6.5.2/sip/QtCore/qiodevicebase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qitemselectionmodel.sip` & `PyQt6-6.5.2/sip/QtCore/qitemselectionmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qjsonarray.sip` & `PyQt6-6.5.2/sip/QtCore/qjsonarray.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qjsondocument.sip` & `PyQt6-6.5.2/sip/QtCore/qjsondocument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qjsonobject.sip` & `PyQt6-6.5.2/sip/QtCore/qjsonobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qjsonvalue.sip` & `PyQt6-6.5.2/sip/QtCore/qjsonvalue.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qlibrary.sip` & `PyQt6-6.5.2/sip/QtCore/qlibrary.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qlibraryinfo.sip` & `PyQt6-6.5.2/sip/QtCore/qlibraryinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qline.sip` & `PyQt6-6.5.2/sip/QtCore/qline.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qlocale.sip` & `PyQt6-6.5.2/sip/QtCore/qlocale.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qlockfile.sip` & `PyQt6-6.5.2/sip/QtCore/qlockfile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qlogging.sip` & `PyQt6-6.5.2/sip/QtCore/qlogging.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qloggingcategory.sip` & `PyQt6-6.5.2/sip/QtCore/qloggingcategory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qmargins.sip` & `PyQt6-6.5.2/sip/QtCore/qmargins.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qmessageauthenticationcode.sip` & `PyQt6-6.5.2/sip/QtCore/qmessageauthenticationcode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qmetaobject.sip` & `PyQt6-6.5.2/sip/QtCore/qmetaobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qmetatype.sip` & `PyQt6-6.5.2/sip/QtCore/qmetatype.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qmimedata.sip` & `PyQt6-6.5.2/sip/QtCore/qmimedata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qmimedatabase.sip` & `PyQt6-6.5.2/sip/QtCore/qmimedatabase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qmimetype.sip` & `PyQt6-6.5.2/sip/QtCore/qmimetype.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qmutex.sip` & `PyQt6-6.5.2/sip/QtCore/qmutex.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qmutexlocker.sip` & `PyQt6-6.5.2/sip/QtCore/qmutexlocker.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qnamespace.sip` & `PyQt6-6.5.2/sip/QtCore/qnamespace.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qnumeric.sip` & `PyQt6-6.5.2/sip/QtCore/qnumeric.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qobject.sip` & `PyQt6-6.5.2/sip/QtCore/qobject.sip`

 * *Files 2% similar despite different names*

```diff
@@ -370,55 +370,55 @@
     virtual bool event(QEvent *);
     virtual bool eventFilter(QObject *, QEvent *);
     static QString tr(const char *sourceText /Encoding="UTF-8"/, const char *disambiguation = 0, int n = -1);
 %MethodCode
         sipRes = new QString(QCoreApplication::translate(sipPyTypeName((PyTypeObject *)sipSelf), a0, a1, a2));
 %End
 
-    SIP_PYOBJECT findChild(SIP_PYTYPE type, const QString &name = QString(), Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="QObject"/;
+    SIP_PYOBJECT findChild(SIP_PYTYPE type /TypeHint="Type[QObjectT]"/, const QString &name = QString(), Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="QObjectT"/;
 %MethodCode
         sipRes = qtcore_FindChild(sipCpp, qtcore_type_to_tuple(a0), *a1, *a2);
         
         if (!sipRes)
             sipIsErr = 1;
 %End
 
-    SIP_PYOBJECT findChild(SIP_PYTUPLE types /TypeHintValue="()"/, const QString &name = QString(), Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="QObject"/;
+    SIP_PYOBJECT findChild(SIP_PYTUPLE types /TypeHint="Tuple[Type[QObjectT], ...]", TypeHintValue="()"/, const QString &name = QString(), Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="QObjectT"/;
 %MethodCode
         sipRes = qtcore_FindChild(sipCpp, qtcore_check_tuple_types(a0), *a1, *a2);
         
         if (!sipRes)
             sipIsErr = 1;
 %End
 
-    SIP_PYLIST findChildren(SIP_PYTYPE type, const QString &name = QString(), Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="List[QObject]"/;
+    SIP_PYLIST findChildren(SIP_PYTYPE type /TypeHint="Type[QObjectT]"/, const QString &name = QString(), Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="List[QObjectT]"/;
 %MethodCode
         sipRes = qtcore_FindChildren(sipCpp, qtcore_type_to_tuple(a0), *a1, *a2);
         
         if (!sipRes)
             sipIsErr = 1;
 %End
 
-    SIP_PYLIST findChildren(SIP_PYTUPLE types /TypeHintValue="()"/, const QString &name = QString(), Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="List[QObject]"/;
+    SIP_PYLIST findChildren(SIP_PYTUPLE types /TypeHint="Tuple[Type[QObjectT], ...]", TypeHintValue="()"/, const QString &name = QString(), Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="List[QObjectT]"/;
 %MethodCode
         sipRes = qtcore_FindChildren(sipCpp, qtcore_check_tuple_types(a0), *a1, *a2);
         
         if (!sipRes)
             sipIsErr = 1;
 %End
 
-    SIP_PYLIST findChildren(SIP_PYTYPE type, const QRegularExpression &re, Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="List[QObject]"/;
+    SIP_PYLIST findChildren(SIP_PYTYPE type /TypeHint="Type[QObjectT]"/, const QRegularExpression &re, Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="List[QObjectT]"/;
 %MethodCode
         sipRes = qtcore_FindChildren(sipCpp, qtcore_type_to_tuple(a0), *a1, *a2);
         
         if (!sipRes)
             sipIsErr = 1;
 %End
 
-    SIP_PYLIST findChildren(SIP_PYTUPLE types /TypeHintValue="()"/, const QRegularExpression &re, Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="List[QObject]"/;
+    SIP_PYLIST findChildren(SIP_PYTUPLE types /TypeHint="Tuple[Type[QObjectT], ...]", TypeHintValue="()"/, const QRegularExpression &re, Qt::FindChildOptions options = Qt::FindChildrenRecursively) const /TypeHint="List[QObjectT]"/;
 %MethodCode
         sipRes = qtcore_FindChildren(sipCpp, qtcore_check_tuple_types(a0), *a1, *a2);
         
         if (!sipRes)
             sipIsErr = 1;
 %End
 
@@ -552,15 +552,15 @@
 %End
 
 SIP_PYOBJECT pyqtEnum(SIP_PYENUM = 0) /TypeHint=""/;
 %MethodCode
     sipRes = qpycore_pyqtEnum(a0);
 %End
 
-SIP_PYOBJECT pyqtSlot(... types, const char *name = 0, const char *result = 0) /NoArgParser/;
+SIP_PYOBJECT pyqtSlot(... types, const char *name = 0, const char *result = 0) /NoArgParser, NoTypeHint/;
 %Docstring
 @pyqtSlot(*types, name: typing.Optional[str], result: typing.Optional[str])
 
 This is a decorator applied to Python methods of a QObject that marks them
 as Qt slots.
 The non-keyword arguments are the types of the slot arguments and each may
 be a Python type object or a string specifying a C++ type.
```

### Comparing `PyQt6-6.5.1/sip/QtCore/qobjectcleanuphandler.sip` & `PyQt6-6.5.2/sip/QtCore/qobjectcleanuphandler.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qobjectdefs.sip` & `PyQt6-6.5.2/sip/QtCore/qobjectdefs.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qoperatingsystemversion.sip` & `PyQt6-6.5.2/sip/QtCore/qoperatingsystemversion.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qparallelanimationgroup.sip` & `PyQt6-6.5.2/sip/QtCore/qparallelanimationgroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpauseanimation.sip` & `PyQt6-6.5.2/sip/QtCore/qpauseanimation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpermissions.sip` & `PyQt6-6.5.2/sip/QtCore/qpermissions.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpluginloader.sip` & `PyQt6-6.5.2/sip/QtCore/qpluginloader.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpoint.sip` & `PyQt6-6.5.2/sip/QtCore/qpoint.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qprocess.sip` & `PyQt6-6.5.2/sip/QtCore/qprocess.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpropertyanimation.sip` & `PyQt6-6.5.2/sip/QtCore/qpropertyanimation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpycore_qhash.sip` & `PyQt6-6.5.2/sip/QtCore/qpycore_qhash.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpycore_qlist.sip` & `PyQt6-6.5.2/sip/QtCore/qpycore_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpycore_qmap.sip` & `PyQt6-6.5.2/sip/QtCore/qpycore_qmap.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpycore_qset.sip` & `PyQt6-6.5.2/sip/QtCore/qpycore_qset.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpycore_std_pair.sip` & `PyQt6-6.5.2/sip/QtCore/qpycore_std_pair.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qpycore_virtual_error_handler.sip` & `PyQt6-6.5.2/sip/QtCore/qpycore_virtual_error_handler.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qrandom.sip` & `PyQt6-6.5.2/sip/QtCore/qrandom.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qreadwritelock.sip` & `PyQt6-6.5.2/sip/QtCore/qreadwritelock.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qrect.sip` & `PyQt6-6.5.2/sip/QtCore/qrect.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qregularexpression.sip` & `PyQt6-6.5.2/sip/QtCore/qregularexpression.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qresource.sip` & `PyQt6-6.5.2/sip/QtCore/qresource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qrunnable.sip` & `PyQt6-6.5.2/sip/QtCore/qrunnable.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsavefile.sip` & `PyQt6-6.5.2/sip/QtCore/qsavefile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsemaphore.sip` & `PyQt6-6.5.2/sip/QtCore/qsemaphore.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsequentialanimationgroup.sip` & `PyQt6-6.5.2/sip/QtCore/qsequentialanimationgroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsettings.sip` & `PyQt6-6.5.2/sip/QtCore/qsettings.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsharedmemory.sip` & `PyQt6-6.5.2/sip/QtCore/qsharedmemory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsignalmapper.sip` & `PyQt6-6.5.2/sip/QtCore/qsignalmapper.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsize.sip` & `PyQt6-6.5.2/sip/QtCore/qsize.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsocketnotifier.sip` & `PyQt6-6.5.2/sip/QtCore/qsocketnotifier.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsortfilterproxymodel.sip` & `PyQt6-6.5.2/sip/QtCore/qsortfilterproxymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qstandardpaths.sip` & `PyQt6-6.5.2/sip/QtCore/qstandardpaths.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qstorageinfo.sip` & `PyQt6-6.5.2/sip/QtCore/qstorageinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qstring.sip` & `PyQt6-6.5.2/sip/QtCore/qstring.sip`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-%MappedType QString /AllowNone,TypeHint="str",TypeHintValue="''"/
+%MappedType QString /AllowNone, TypeHintIn="Optional[str]", TypeHintOut="str", TypeHintValue="''"/
 {
 %TypeHeaderCode
 #include <qstring.h>
 %End
 
 %ConvertToTypeCode
 if (sipIsErr == NULL)
```

### Comparing `PyQt6-6.5.1/sip/QtCore/qstringconverter.sip` & `PyQt6-6.5.2/sip/QtCore/qstringconverter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qstringconverter_base.sip` & `PyQt6-6.5.2/sip/QtCore/qstringconverter_base.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qstringlist.sip` & `PyQt6-6.5.2/sip/QtCore/qstringlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qstringlistmodel.sip` & `PyQt6-6.5.2/sip/QtCore/qstringlistmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qstringview.sip` & `PyQt6-6.5.2/sip/QtCore/qstringview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsysinfo.sip` & `PyQt6-6.5.2/sip/QtCore/qsysinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qsystemsemaphore.sip` & `PyQt6-6.5.2/sip/QtCore/qsystemsemaphore.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtemporarydir.sip` & `PyQt6-6.5.2/sip/QtCore/qtemporarydir.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtemporaryfile.sip` & `PyQt6-6.5.2/sip/QtCore/qtemporaryfile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtenvironmentvariables.sip` & `PyQt6-6.5.2/sip/QtCore/qtenvironmentvariables.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtextboundaryfinder.sip` & `PyQt6-6.5.2/sip/QtCore/qtextboundaryfinder.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtextstream.sip` & `PyQt6-6.5.2/sip/QtCore/qtextstream.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qthread.sip` & `PyQt6-6.5.2/sip/QtCore/qthread.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qthreadpool.sip` & `PyQt6-6.5.2/sip/QtCore/qthreadpool.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtimeline.sip` & `PyQt6-6.5.2/sip/QtCore/qtimeline.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtimer.sip` & `PyQt6-6.5.2/sip/QtCore/qtimer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtimezone.sip` & `PyQt6-6.5.2/sip/QtCore/qtimezone.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtranslator.sip` & `PyQt6-6.5.2/sip/QtCore/qtranslator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtransposeproxymodel.sip` & `PyQt6-6.5.2/sip/QtCore/qtransposeproxymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtversion.sip` & `PyQt6-6.5.2/sip/QtCore/qtversion.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qtypes.sip` & `PyQt6-6.5.2/sip/QtCore/qtypes.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qurl.sip` & `PyQt6-6.5.2/sip/QtCore/qurl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qurlquery.sip` & `PyQt6-6.5.2/sip/QtCore/qurlquery.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/quuid.sip` & `PyQt6-6.5.2/sip/QtCore/quuid.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qvariant.sip` & `PyQt6-6.5.2/sip/QtCore/qvariant.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qvariantanimation.sip` & `PyQt6-6.5.2/sip/QtCore/qvariantanimation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qversionnumber.sip` & `PyQt6-6.5.2/sip/QtCore/qversionnumber.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qwaitcondition.sip` & `PyQt6-6.5.2/sip/QtCore/qwaitcondition.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qwineventnotifier.sip` & `PyQt6-6.5.2/sip/QtCore/qwineventnotifier.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtCore/qxmlstream.sip` & `PyQt6-6.5.2/sip/QtCore/qxmlstream.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/QtDBusmod.sip` & `PyQt6-6.5.2/sip/QtDBus/QtDBusmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbusabstractadaptor.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbusabstractadaptor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbusabstractinterface.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbusabstractinterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbusargument.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbusargument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbusconnection.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbusconnection.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbusconnectioninterface.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbusconnectioninterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbuserror.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbuserror.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbusextratypes.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbusextratypes.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbusinterface.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbusinterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbusmessage.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbusmessage.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbuspendingcall.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbuspendingcall.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbusservicewatcher.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbusservicewatcher.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qdbusunixfiledescriptor.sip` & `PyQt6-6.5.2/sip/QtDBus/qdbusunixfiledescriptor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qpydbuspendingreply.sip` & `PyQt6-6.5.2/sip/QtDBus/qpydbuspendingreply.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDBus/qpydbusreply.sip` & `PyQt6-6.5.2/sip/QtDBus/qpydbusreply.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/QtDesignermod.sip` & `PyQt6-6.5.2/sip/QtDesigner/QtDesignermod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/abstractactioneditor.sip` & `PyQt6-6.5.2/sip/QtDesigner/abstractactioneditor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/abstractformbuilder.sip` & `PyQt6-6.5.2/sip/QtDesigner/abstractformbuilder.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/abstractformeditor.sip` & `PyQt6-6.5.2/sip/QtDesigner/abstractformeditor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/abstractformwindow.sip` & `PyQt6-6.5.2/sip/QtDesigner/abstractformwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/abstractformwindowcursor.sip` & `PyQt6-6.5.2/sip/QtDesigner/abstractformwindowcursor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/abstractformwindowmanager.sip` & `PyQt6-6.5.2/sip/QtDesigner/abstractformwindowmanager.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/abstractobjectinspector.sip` & `PyQt6-6.5.2/sip/QtDesigner/abstractobjectinspector.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/abstractpropertyeditor.sip` & `PyQt6-6.5.2/sip/QtDesigner/abstractpropertyeditor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/abstractwidgetbox.sip` & `PyQt6-6.5.2/sip/QtDesigner/abstractwidgetbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/container.sip` & `PyQt6-6.5.2/sip/QtDesigner/container.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/customwidget.sip` & `PyQt6-6.5.2/sip/QtDesigner/customwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/default_extensionfactory.sip` & `PyQt6-6.5.2/sip/QtDesigner/default_extensionfactory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/extension.sip` & `PyQt6-6.5.2/sip/QtDesigner/extension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/formbuilder.sip` & `PyQt6-6.5.2/sip/QtDesigner/formbuilder.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/membersheet.sip` & `PyQt6-6.5.2/sip/QtDesigner/membersheet.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/propertysheet.sip` & `PyQt6-6.5.2/sip/QtDesigner/propertysheet.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/qextensionmanager.sip` & `PyQt6-6.5.2/sip/QtDesigner/qextensionmanager.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/qpydesignercontainerextension.sip` & `PyQt6-6.5.2/sip/QtDesigner/qpydesignercontainerextension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/qpydesignercustomwidgetcollectionplugin.sip` & `PyQt6-6.5.2/sip/QtDesigner/qpydesignercustomwidgetcollectionplugin.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/qpydesignercustomwidgetplugin.sip` & `PyQt6-6.5.2/sip/QtDesigner/qpydesignercustomwidgetplugin.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/qpydesignermembersheetextension.sip` & `PyQt6-6.5.2/sip/QtDesigner/qpydesignermembersheetextension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/qpydesignerpropertysheetextension.sip` & `PyQt6-6.5.2/sip/QtDesigner/qpydesignerpropertysheetextension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/qpydesignertaskmenuextension.sip` & `PyQt6-6.5.2/sip/QtDesigner/qpydesignertaskmenuextension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtDesigner/taskmenu.sip` & `PyQt6-6.5.2/sip/QtDesigner/taskmenu.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/QtGuimod.sip` & `PyQt6-6.5.2/sip/QtGui/QtGuimod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/opengl_types.sip` & `PyQt6-6.5.2/sip/QtGui/opengl_types.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qabstractfileiconprovider.sip` & `PyQt6-6.5.2/sip/QtGui/qabstractfileiconprovider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qabstracttextdocumentlayout.sip` & `PyQt6-6.5.2/sip/QtGui/qabstracttextdocumentlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qaction.sip` & `PyQt6-6.5.2/sip/QtGui/qaction.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qactiongroup.sip` & `PyQt6-6.5.2/sip/QtGui/qactiongroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qbackingstore.sip` & `PyQt6-6.5.2/sip/QtGui/qbackingstore.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qbitmap.sip` & `PyQt6-6.5.2/sip/QtGui/qbitmap.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qbrush.sip` & `PyQt6-6.5.2/sip/QtGui/qbrush.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qclipboard.sip` & `PyQt6-6.5.2/sip/QtGui/qclipboard.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qcolor.sip` & `PyQt6-6.5.2/sip/QtGui/qcolor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qcolorspace.sip` & `PyQt6-6.5.2/sip/QtGui/qcolorspace.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qcolortransform.sip` & `PyQt6-6.5.2/sip/QtGui/qcolortransform.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qcursor.sip` & `PyQt6-6.5.2/sip/QtGui/qcursor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qdesktopservices.sip` & `PyQt6-6.5.2/sip/QtGui/qdesktopservices.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qdrag.sip` & `PyQt6-6.5.2/sip/QtGui/qdrag.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qevent.sip` & `PyQt6-6.5.2/sip/QtGui/qevent.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qeventpoint.sip` & `PyQt6-6.5.2/sip/QtGui/qeventpoint.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qfilesystemmodel.sip` & `PyQt6-6.5.2/sip/QtGui/qfilesystemmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qfont.sip` & `PyQt6-6.5.2/sip/QtGui/qfont.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qfontdatabase.sip` & `PyQt6-6.5.2/sip/QtGui/qfontdatabase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qfontinfo.sip` & `PyQt6-6.5.2/sip/QtGui/qfontinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qfontmetrics.sip` & `PyQt6-6.5.2/sip/QtGui/qfontmetrics.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qgenericmatrix.sip` & `PyQt6-6.5.2/sip/QtGui/qgenericmatrix.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qglyphrun.sip` & `PyQt6-6.5.2/sip/QtGui/qglyphrun.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qguiapplication.sip` & `PyQt6-6.5.2/sip/QtGui/qguiapplication.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qicon.sip` & `PyQt6-6.5.2/sip/QtGui/qicon.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qiconengine.sip` & `PyQt6-6.5.2/sip/QtGui/qiconengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qimage.sip` & `PyQt6-6.5.2/sip/QtGui/qimage.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qimageiohandler.sip` & `PyQt6-6.5.2/sip/QtGui/qimageiohandler.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qimagereader.sip` & `PyQt6-6.5.2/sip/QtGui/qimagereader.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qimagewriter.sip` & `PyQt6-6.5.2/sip/QtGui/qimagewriter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qinputdevice.sip` & `PyQt6-6.5.2/sip/QtGui/qinputdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qinputmethod.sip` & `PyQt6-6.5.2/sip/QtGui/qinputmethod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qkeysequence.sip` & `PyQt6-6.5.2/sip/QtGui/qkeysequence.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qmatrix4x4.sip` & `PyQt6-6.5.2/sip/QtGui/qmatrix4x4.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qmovie.sip` & `PyQt6-6.5.2/sip/QtGui/qmovie.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qoffscreensurface.sip` & `PyQt6-6.5.2/sip/QtGui/qoffscreensurface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qopenglcontext.sip` & `PyQt6-6.5.2/sip/QtGui/qopenglcontext.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpagedpaintdevice.sip` & `PyQt6-6.5.2/sip/QtGui/qpagedpaintdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpagelayout.sip` & `PyQt6-6.5.2/sip/QtGui/qpagelayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpageranges.sip` & `PyQt6-6.5.2/sip/QtGui/qpageranges.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpagesize.sip` & `PyQt6-6.5.2/sip/QtGui/qpagesize.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpaintdevice.sip` & `PyQt6-6.5.2/sip/QtGui/qpaintdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpaintdevicewindow.sip` & `PyQt6-6.5.2/sip/QtGui/qpaintdevicewindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpaintengine.sip` & `PyQt6-6.5.2/sip/QtGui/qpaintengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpainter.sip` & `PyQt6-6.5.2/sip/QtGui/qpainter.sip`

 * *Files 2% similar despite different names*

```diff
@@ -189,43 +189,43 @@
     bool viewTransformEnabled() const;
     void strokePath(const QPainterPath &path, const QPen &pen);
     void fillPath(const QPainterPath &path, const QBrush &brush);
     void drawPath(const QPainterPath &path);
     void drawPoints(const QPolygonF &points);
     void drawPoints(const QPolygon &points);
     void drawPoints(const QPointF *points /Array/, int pointCount /ArraySize/);
-    void drawPoints(const QPointF *point, ...);
+    void drawPoints(const QPointF *point, ... /TypeHint="QPointF"/);
 %MethodCode
         QPointF *points = qtgui_inst_array<QPointF>(a0, a1, sipType_QPointF);
         
         if (points)
         {
             sipCpp->drawPoints(points, 1 + PyTuple_Size(a1));
             delete[] points;
         }
         else
             sipIsErr = 1;
 %End
 
     void drawPoints(const QPoint *points /Array/, int pointCount /ArraySize/);
-    void drawPoints(const QPoint *point, ...);
+    void drawPoints(const QPoint *point, ... /TypeHint="QPoint"/);
 %MethodCode
         QPoint *points = qtgui_inst_array<QPoint>(a0, a1, sipType_QPoint);
         
         if (points)
         {
             sipCpp->drawPoints(points, 1 + PyTuple_Size(a1));
             delete[] points;
         }
         else
             sipIsErr = 1;
 %End
 
     void drawLines(const QLineF *lines /Array/, int lineCount /ArraySize/);
-    void drawLines(const QLineF *line, ...);
+    void drawLines(const QLineF *line, ... /TypeHint="QLineF"/);
 %MethodCode
         QLineF *lines = qtgui_inst_array<QLineF>(a0, a1, sipType_QLineF);
         
         if (lines)
         {
             sipCpp->drawLines(lines, 1 + PyTuple_Size(a1));
             delete[] lines;
@@ -235,29 +235,29 @@
 %End
 
     void drawLines(const QPointF *pointPairs /Array/, int lineCount /ArraySize/);
 %MethodCode
         sipCpp->drawLines(a0, a1 / 2);
 %End
 
-    void drawLines(const QPointF *pointPair, ...);
+    void drawLines(const QPointF *pointPair, ... /TypeHint="QPointF"/);
 %MethodCode
         QPointF *pairs = qtgui_inst_array<QPointF>(a0, a1, sipType_QPointF);
         
         if (pairs)
         {
             sipCpp->drawLines(pairs, (1 + PyTuple_Size(a1)) / 2);
             delete[] pairs;
         }
         else
             sipIsErr = 1;
 %End
 
     void drawLines(const QLine *lines /Array/, int lineCount /ArraySize/);
-    void drawLines(const QLine *line, ...);
+    void drawLines(const QLine *line, ... /TypeHint="QLine"/);
 %MethodCode
         QLine *lines = qtgui_inst_array<QLine>(a0, a1, sipType_QLine);
         
         if (lines)
         {
             sipCpp->drawLines(lines, 1 + PyTuple_Size(a1));
             delete[] lines;
@@ -267,43 +267,43 @@
 %End
 
     void drawLines(const QPoint *pointPairs /Array/, int lineCount /ArraySize/);
 %MethodCode
         sipCpp->drawLines(a0, a1 / 2);
 %End
 
-    void drawLines(const QPoint *pointPair, ...);
+    void drawLines(const QPoint *pointPair, ... /TypeHint="QPoint"/);
 %MethodCode
         QPoint *pairs = qtgui_inst_array<QPoint>(a0, a1, sipType_QPoint);
         
         if (pairs)
         {
             sipCpp->drawLines(pairs, (1 + PyTuple_Size(a1)) / 2);
             delete[] pairs;
         }
         else
             sipIsErr = 1;
 %End
 
     void drawRects(const QRectF *rects /Array/, int rectCount /ArraySize/);
-    void drawRects(const QRectF *rect, ...);
+    void drawRects(const QRectF *rect, ... /TypeHint="QRectF"/);
 %MethodCode
         QRectF *rects = qtgui_inst_array<QRectF>(a0, a1, sipType_QRectF);
         
         if (rects)
         {
             sipCpp->drawRects(rects, 1 + PyTuple_Size(a1));
             delete[] rects;
         }
         else
             sipIsErr = 1;
 %End
 
     void drawRects(const QRect *rects /Array/, int rectCount /ArraySize/);
-    void drawRects(const QRect *rect, ...);
+    void drawRects(const QRect *rect, ... /TypeHint="QRect"/);
 %MethodCode
         QRect *rects = qtgui_inst_array<QRect>(a0, a1, sipType_QRect);
         
         if (rects)
         {
             sipCpp->drawRects(rects, 1 + PyTuple_Size(a1));
             delete[] rects;
@@ -313,29 +313,29 @@
 %End
 
     void drawEllipse(const QRectF &r);
     void drawEllipse(const QRect &r);
     void drawPolyline(const QPolygonF &polyline);
     void drawPolyline(const QPolygon &polyline);
     void drawPolyline(const QPointF *points /Array/, int pointCount /ArraySize/);
-    void drawPolyline(const QPointF *point, ...);
+    void drawPolyline(const QPointF *point, ... /TypeHint="QPointF"/);
 %MethodCode
         QPointF *points = qtgui_inst_array<QPointF>(a0, a1, sipType_QPointF);
         
         if (points)
         {
             sipCpp->drawPolyline(points, 1 + PyTuple_Size(a1));
             delete[] points;
         }
         else
             sipIsErr = 1;
 %End
 
     void drawPolyline(const QPoint *points /Array/, int pointCount /ArraySize/);
-    void drawPolyline(const QPoint *point, ...);
+    void drawPolyline(const QPoint *point, ... /TypeHint="QPoint"/);
 %MethodCode
         QPoint *points = qtgui_inst_array<QPoint>(a0, a1, sipType_QPoint);
         
         if (points)
         {
             sipCpp->drawPolyline(points, 1 + PyTuple_Size(a1));
             delete[] points;
@@ -343,29 +343,29 @@
         else
             sipIsErr = 1;
 %End
 
     void drawPolygon(const QPolygonF &points, Qt::FillRule fillRule = Qt::OddEvenFill);
     void drawPolygon(const QPolygon &points, Qt::FillRule fillRule = Qt::OddEvenFill);
     void drawPolygon(const QPointF *points /Array/, int pointCount /ArraySize/, Qt::FillRule fillRule = Qt::OddEvenFill);
-    void drawPolygon(const QPointF *point, ...);
+    void drawPolygon(const QPointF *point, ... /TypeHint="QPointF"/);
 %MethodCode
         QPointF *points = qtgui_inst_array<QPointF>(a0, a1, sipType_QPointF);
         
         if (points)
         {
             sipCpp->drawPolygon(points, 1 + PyTuple_Size(a1));
             delete[] points;
         }
         else
             sipIsErr = 1;
 %End
 
     void drawPolygon(const QPoint *points /Array/, int pointCount /ArraySize/, Qt::FillRule fillRule = Qt::OddEvenFill);
-    void drawPolygon(const QPoint *point, ...);
+    void drawPolygon(const QPoint *point, ... /TypeHint="QPoint"/);
 %MethodCode
         QPoint *points = qtgui_inst_array<QPoint>(a0, a1, sipType_QPoint);
         
         if (points)
         {
             sipCpp->drawPolygon(points, 1 + PyTuple_Size(a1));
             delete[] points;
@@ -373,29 +373,29 @@
         else
             sipIsErr = 1;
 %End
 
     void drawConvexPolygon(const QPolygonF &poly);
     void drawConvexPolygon(const QPolygon &poly);
     void drawConvexPolygon(const QPointF *points /Array/, int pointCount /ArraySize/);
-    void drawConvexPolygon(const QPointF *point, ...);
+    void drawConvexPolygon(const QPointF *point, ... /TypeHint="QPointF"/);
 %MethodCode
         QPointF *points = qtgui_inst_array<QPointF>(a0, a1, sipType_QPointF);
         
         if (points)
         {
             sipCpp->drawConvexPolygon(points, 1 + PyTuple_Size(a1));
             delete[] points;
         }
         else
             sipIsErr = 1;
 %End
 
     void drawConvexPolygon(const QPoint *points /Array/, int pointCount /ArraySize/);
-    void drawConvexPolygon(const QPoint *point, ...);
+    void drawConvexPolygon(const QPoint *point, ... /TypeHint="QPoint"/);
 %MethodCode
         QPoint *points = qtgui_inst_array<QPoint>(a0, a1, sipType_QPoint);
         
         if (points)
         {
             sipCpp->drawConvexPolygon(points, 1 + PyTuple_Size(a1));
             delete[] points;
```

### Comparing `PyQt6-6.5.1/sip/QtGui/qpainterpath.sip` & `PyQt6-6.5.2/sip/QtGui/qpainterpath.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpalette.sip` & `PyQt6-6.5.2/sip/QtGui/qpalette.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpdfwriter.sip` & `PyQt6-6.5.2/sip/QtGui/qpdfwriter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpen.sip` & `PyQt6-6.5.2/sip/QtGui/qpen.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpicture.sip` & `PyQt6-6.5.2/sip/QtGui/qpicture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpixelformat.sip` & `PyQt6-6.5.2/sip/QtGui/qpixelformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpixmap.sip` & `PyQt6-6.5.2/sip/QtGui/qpixmap.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpixmapcache.sip` & `PyQt6-6.5.2/sip/QtGui/qpixmapcache.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpointingdevice.sip` & `PyQt6-6.5.2/sip/QtGui/qpointingdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qpolygon.sip` & `PyQt6-6.5.2/sip/QtGui/qpolygon.sip`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     void translate(const QPoint &offset);
     QPolygon translated(int dx, int dy) const;
     QPolygon translated(const QPoint &offset) const;
     QRect boundingRect() const;
     QPoint point(int i) const;
     void setPoint(int index, int x, int y);
     void setPoint(int index, const QPoint &p);
-    void setPoints(int firstx, int firsty, ...);
+    void setPoints(int firstx, int firsty, ... /TypeHint="int"/);
 %MethodCode
         // Accept at least one pair of integer coordinates.
         int nPoints = 1 + ((PyTuple_Size(a2) + 1) >> 1);
         
         int *points = new int[nPoints * 2];
         
         points[0] = a0;
@@ -77,15 +77,15 @@
             points[2 + i] = PyLong_AsLong(PyTuple_GetItem(a2, i));
         
         sipCpp->setPoints(nPoints, points);
         
         delete[] points;
 %End
 
-    void putPoints(int index, int firstx, int firsty, ...);
+    void putPoints(int index, int firstx, int firsty, ... /TypeHint="int"/);
 %MethodCode
         // Accept at least one pair of integer coordinates.
         int nPoints = 1 + ((PyTuple_Size(a3) + 1) >> 1);
         
         int *points = new int[nPoints * 2];
         
         points[0] = a1;
```

### Comparing `PyQt6-6.5.1/sip/QtGui/qpygui_qlist.sip` & `PyQt6-6.5.2/sip/QtGui/qpygui_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qquaternion.sip` & `PyQt6-6.5.2/sip/QtGui/qquaternion.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qrasterwindow.sip` & `PyQt6-6.5.2/sip/QtGui/qrasterwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qrawfont.sip` & `PyQt6-6.5.2/sip/QtGui/qrawfont.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qregion.sip` & `PyQt6-6.5.2/sip/QtGui/qregion.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qrgb.sip` & `PyQt6-6.5.2/sip/QtGui/qrgb.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qrgba64.sip` & `PyQt6-6.5.2/sip/QtGui/qrgba64.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qscreen.sip` & `PyQt6-6.5.2/sip/QtGui/qscreen.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qsessionmanager.sip` & `PyQt6-6.5.2/sip/QtGui/qsessionmanager.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qshortcut.sip` & `PyQt6-6.5.2/sip/QtGui/qshortcut.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qstandarditemmodel.sip` & `PyQt6-6.5.2/sip/QtGui/qstandarditemmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qstatictext.sip` & `PyQt6-6.5.2/sip/QtGui/qstatictext.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qstylehints.sip` & `PyQt6-6.5.2/sip/QtGui/qstylehints.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qsurface.sip` & `PyQt6-6.5.2/sip/QtGui/qsurface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qsurfaceformat.sip` & `PyQt6-6.5.2/sip/QtGui/qsurfaceformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qsyntaxhighlighter.sip` & `PyQt6-6.5.2/sip/QtGui/qsyntaxhighlighter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtextcursor.sip` & `PyQt6-6.5.2/sip/QtGui/qtextcursor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtextdocument.sip` & `PyQt6-6.5.2/sip/QtGui/qtextdocument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtextdocumentfragment.sip` & `PyQt6-6.5.2/sip/QtGui/qtextdocumentfragment.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtextdocumentwriter.sip` & `PyQt6-6.5.2/sip/QtGui/qtextdocumentwriter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtextformat.sip` & `PyQt6-6.5.2/sip/QtGui/qtextformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtextlayout.sip` & `PyQt6-6.5.2/sip/QtGui/qtextlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtextlist.sip` & `PyQt6-6.5.2/sip/QtGui/qtextlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtextobject.sip` & `PyQt6-6.5.2/sip/QtGui/qtextobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtextoption.sip` & `PyQt6-6.5.2/sip/QtGui/qtextoption.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtexttable.sip` & `PyQt6-6.5.2/sip/QtGui/qtexttable.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qtransform.sip` & `PyQt6-6.5.2/sip/QtGui/qtransform.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qundogroup.sip` & `PyQt6-6.5.2/sip/QtGui/qundogroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qundostack.sip` & `PyQt6-6.5.2/sip/QtGui/qundostack.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qutimimeconverter.sip` & `PyQt6-6.5.2/sip/QtGui/qutimimeconverter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qvalidator.sip` & `PyQt6-6.5.2/sip/QtGui/qvalidator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qvectornd.sip` & `PyQt6-6.5.2/sip/QtGui/qvectornd.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qwindow.sip` & `PyQt6-6.5.2/sip/QtGui/qwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtGui/qwindowdefs.sip` & `PyQt6-6.5.2/sip/QtGui/qwindowdefs.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/QtHelpmod.sip` & `PyQt6-6.5.2/sip/QtHelp/QtHelpmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qcompressedhelpinfo.sip` & `PyQt6-6.5.2/sip/QtHelp/qcompressedhelpinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelpcontentwidget.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelpcontentwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelpengine.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelpengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelpenginecore.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelpenginecore.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelpfilterdata.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelpfilterdata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelpfilterengine.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelpfilterengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelpfiltersettingswidget.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelpfiltersettingswidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelpindexwidget.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelpindexwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelplink.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelplink.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelpsearchengine.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelpsearchengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelpsearchquerywidget.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelpsearchquerywidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtHelp/qhelpsearchresultwidget.sip` & `PyQt6-6.5.2/sip/QtHelp/qhelpsearchresultwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/QtMultimediamod.sip` & `PyQt6-6.5.2/sip/QtMultimedia/QtMultimediamod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qaudio.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qaudio.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qaudiobuffer.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qaudiobuffer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qaudiodecoder.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qaudiodecoder.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qaudiodevice.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qaudiodevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qaudioformat.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qaudioformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qaudioinput.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qaudioinput.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qaudiooutput.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qaudiooutput.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qaudiosink.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qaudiosink.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qaudiosource.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qaudiosource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qcamera.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qcamera.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qcameradevice.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qcameradevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qimagecapture.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qimagecapture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qmediacapturesession.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qmediacapturesession.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qmediadevices.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qmediadevices.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qmediaformat.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qmediaformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qmediametadata.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qmediametadata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qmediaplayer.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qmediaplayer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qmediarecorder.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qmediarecorder.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qmediatimerange.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qmediatimerange.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qpymultimedia_qlist.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qpymultimedia_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qscreencapture.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qscreencapture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qsoundeffect.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qsoundeffect.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qvideoframe.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qvideoframe.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qvideoframeformat.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qvideoframeformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimedia/qvideosink.sip` & `PyQt6-6.5.2/sip/QtMultimedia/qvideosink.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimediaWidgets/QtMultimediaWidgetsmod.sip` & `PyQt6-6.5.2/sip/QtMultimediaWidgets/QtMultimediaWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimediaWidgets/qgraphicsvideoitem.sip` & `PyQt6-6.5.2/sip/QtMultimediaWidgets/qgraphicsvideoitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtMultimediaWidgets/qvideowidget.sip` & `PyQt6-6.5.2/sip/QtMultimediaWidgets/qvideowidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/QtNetworkmod.sip` & `PyQt6-6.5.2/sip/QtNetwork/QtNetworkmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qabstractnetworkcache.sip` & `PyQt6-6.5.2/sip/QtNetwork/qabstractnetworkcache.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qabstractsocket.sip` & `PyQt6-6.5.2/sip/QtNetwork/qabstractsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qauthenticator.sip` & `PyQt6-6.5.2/sip/QtNetwork/qauthenticator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qdnslookup.sip` & `PyQt6-6.5.2/sip/QtNetwork/qdnslookup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qhostaddress.sip` & `PyQt6-6.5.2/sip/QtNetwork/qhostaddress.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qhostinfo.sip` & `PyQt6-6.5.2/sip/QtNetwork/qhostinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qhstspolicy.sip` & `PyQt6-6.5.2/sip/QtNetwork/qhstspolicy.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qhttp1configuration.sip` & `PyQt6-6.5.2/sip/QtNetwork/qhttp1configuration.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qhttp2configuration.sip` & `PyQt6-6.5.2/sip/QtNetwork/qhttp2configuration.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qhttpmultipart.sip` & `PyQt6-6.5.2/sip/QtNetwork/qhttpmultipart.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qlocalserver.sip` & `PyQt6-6.5.2/sip/QtNetwork/qlocalserver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qlocalsocket.sip` & `PyQt6-6.5.2/sip/QtNetwork/qlocalsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qnetworkaccessmanager.sip` & `PyQt6-6.5.2/sip/QtNetwork/qnetworkaccessmanager.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qnetworkcookie.sip` & `PyQt6-6.5.2/sip/QtNetwork/qnetworkcookie.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qnetworkcookiejar.sip` & `PyQt6-6.5.2/sip/QtNetwork/qnetworkcookiejar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qnetworkdatagram.sip` & `PyQt6-6.5.2/sip/QtNetwork/qnetworkdatagram.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qnetworkdiskcache.sip` & `PyQt6-6.5.2/sip/QtNetwork/qnetworkdiskcache.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qnetworkinformation.sip` & `PyQt6-6.5.2/sip/QtNetwork/qnetworkinformation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qnetworkinterface.sip` & `PyQt6-6.5.2/sip/QtNetwork/qnetworkinterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qnetworkproxy.sip` & `PyQt6-6.5.2/sip/QtNetwork/qnetworkproxy.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qnetworkreply.sip` & `PyQt6-6.5.2/sip/QtNetwork/qnetworkreply.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qnetworkrequest.sip` & `PyQt6-6.5.2/sip/QtNetwork/qnetworkrequest.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qocspresponse.sip` & `PyQt6-6.5.2/sip/QtNetwork/qocspresponse.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qpassworddigestor.sip` & `PyQt6-6.5.2/sip/QtNetwork/qpassworddigestor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qpynetwork_qhash.sip` & `PyQt6-6.5.2/sip/QtNetwork/qpynetwork_qhash.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qpynetwork_qlist.sip` & `PyQt6-6.5.2/sip/QtNetwork/qpynetwork_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qpynetwork_qmap.sip` & `PyQt6-6.5.2/sip/QtNetwork/qpynetwork_qmap.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qssl.sip` & `PyQt6-6.5.2/sip/QtNetwork/qssl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qsslcertificate.sip` & `PyQt6-6.5.2/sip/QtNetwork/qsslcertificate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qsslcertificateextension.sip` & `PyQt6-6.5.2/sip/QtNetwork/qsslcertificateextension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qsslcipher.sip` & `PyQt6-6.5.2/sip/QtNetwork/qsslcipher.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qsslconfiguration.sip` & `PyQt6-6.5.2/sip/QtNetwork/qsslconfiguration.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qssldiffiehellmanparameters.sip` & `PyQt6-6.5.2/sip/QtNetwork/qssldiffiehellmanparameters.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qsslellipticcurve.sip` & `PyQt6-6.5.2/sip/QtNetwork/qsslellipticcurve.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qsslerror.sip` & `PyQt6-6.5.2/sip/QtNetwork/qsslerror.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qsslkey.sip` & `PyQt6-6.5.2/sip/QtNetwork/qsslkey.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qsslpresharedkeyauthenticator.sip` & `PyQt6-6.5.2/sip/QtNetwork/qsslpresharedkeyauthenticator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qsslserver.sip` & `PyQt6-6.5.2/sip/QtNetwork/qsslserver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qsslsocket.sip` & `PyQt6-6.5.2/sip/QtNetwork/qsslsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qtcpserver.sip` & `PyQt6-6.5.2/sip/QtNetwork/qtcpserver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qtcpsocket.sip` & `PyQt6-6.5.2/sip/QtNetwork/qtcpsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNetwork/qudpsocket.sip` & `PyQt6-6.5.2/sip/QtNetwork/qudpsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNfc/QtNfcmod.sip` & `PyQt6-6.5.2/sip/QtNfc/QtNfcmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNfc/qndeffilter.sip` & `PyQt6-6.5.2/sip/QtNfc/qndeffilter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNfc/qndefmessage.sip` & `PyQt6-6.5.2/sip/QtNfc/qndefmessage.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNfc/qndefnfcsmartposterrecord.sip` & `PyQt6-6.5.2/sip/QtNfc/qndefnfcsmartposterrecord.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNfc/qndefnfctextrecord.sip` & `PyQt6-6.5.2/sip/QtNfc/qndefnfctextrecord.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNfc/qndefnfcurirecord.sip` & `PyQt6-6.5.2/sip/QtNfc/qndefnfcurirecord.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNfc/qndefrecord.sip` & `PyQt6-6.5.2/sip/QtNfc/qndefrecord.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNfc/qnearfieldmanager.sip` & `PyQt6-6.5.2/sip/QtNfc/qnearfieldmanager.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtNfc/qnearfieldtarget.sip` & `PyQt6-6.5.2/sip/QtNfc/qnearfieldtarget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/QtOpenGLmod.sip` & `PyQt6-6.5.2/sip/QtOpenGL/QtOpenGLmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglbuffer.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglbuffer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopengldebug.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopengldebug.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglframebufferobject.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglframebufferobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglfunctions_2_0.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglfunctions_2_0.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglfunctions_2_1.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglfunctions_2_1.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglfunctions_4_1_core.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglfunctions_4_1_core.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglfunctions_es2.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglfunctions_es2.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglpaintdevice.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglpaintdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglpixeltransferoptions.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglpixeltransferoptions.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglshaderprogram.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglshaderprogram.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopengltexture.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopengltexture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopengltextureblitter.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopengltextureblitter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopengltimerquery.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopengltimerquery.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglversionfunctions.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglversionfunctions.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglversionfunctionsfactory.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglversionfunctionsfactory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglversionprofile.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglversionprofile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglvertexarrayobject.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglvertexarrayobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qopenglwindow.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qopenglwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qpyopengl_qlist.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qpyopengl_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGL/qpyopengl_std_pair.sip` & `PyQt6-6.5.2/sip/QtOpenGL/qpyopengl_std_pair.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGLWidgets/QtOpenGLWidgetsmod.sip` & `PyQt6-6.5.2/sip/QtOpenGLWidgets/QtOpenGLWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtOpenGLWidgets/qopenglwidget.sip` & `PyQt6-6.5.2/sip/QtOpenGLWidgets/qopenglwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdf/QtPdfmod.sip` & `PyQt6-6.5.2/sip/QtPdf/QtPdfmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdf/qpdfbookmarkmodel.sip` & `PyQt6-6.5.2/sip/QtPdf/qpdfbookmarkmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdf/qpdfdocument.sip` & `PyQt6-6.5.2/sip/QtPdf/qpdfdocument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdf/qpdfdocumentrenderoptions.sip` & `PyQt6-6.5.2/sip/QtPdf/qpdfdocumentrenderoptions.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdf/qpdflink.sip` & `PyQt6-6.5.2/sip/QtPdf/qpdflink.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdf/qpdfpagenavigator.sip` & `PyQt6-6.5.2/sip/QtPdf/qpdfpagenavigator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdf/qpdfpagerenderer.sip` & `PyQt6-6.5.2/sip/QtPdf/qpdfpagerenderer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdf/qpdfsearchmodel.sip` & `PyQt6-6.5.2/sip/QtPdf/qpdfsearchmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdf/qpdfselection.sip` & `PyQt6-6.5.2/sip/QtPdf/qpdfselection.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdfWidgets/QtPdfWidgetsmod.sip` & `PyQt6-6.5.2/sip/QtPdfWidgets/QtPdfWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPdfWidgets/qpdfview.sip` & `PyQt6-6.5.2/sip/QtPdfWidgets/qpdfview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/QtPositioningmod.sip` & `PyQt6-6.5.2/sip/QtPositioning/QtPositioningmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeoaddress.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeoaddress.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeoareamonitorinfo.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeoareamonitorinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeoareamonitorsource.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeoareamonitorsource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeocircle.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeocircle.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeocoordinate.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeocoordinate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeolocation.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeolocation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeopath.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeopath.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeopolygon.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeopolygon.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeopositioninfo.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeopositioninfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeopositioninfosource.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeopositioninfosource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeorectangle.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeorectangle.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeosatelliteinfo.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeosatelliteinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeosatelliteinfosource.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeosatelliteinfosource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qgeoshape.sip` & `PyQt6-6.5.2/sip/QtPositioning/qgeoshape.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qnmeapositioninfosource.sip` & `PyQt6-6.5.2/sip/QtPositioning/qnmeapositioninfosource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPositioning/qnmeasatelliteinfosource.sip` & `PyQt6-6.5.2/sip/QtPositioning/qnmeasatelliteinfosource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPrintSupport/QtPrintSupportmod.sip` & `PyQt6-6.5.2/sip/QtPrintSupport/QtPrintSupportmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPrintSupport/qabstractprintdialog.sip` & `PyQt6-6.5.2/sip/QtPrintSupport/qabstractprintdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPrintSupport/qpagesetupdialog.sip` & `PyQt6-6.5.2/sip/QtPrintSupport/qpagesetupdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPrintSupport/qprintdialog.sip` & `PyQt6-6.5.2/sip/QtPrintSupport/qprintdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPrintSupport/qprintengine.sip` & `PyQt6-6.5.2/sip/QtPrintSupport/qprintengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPrintSupport/qprinter.sip` & `PyQt6-6.5.2/sip/QtPrintSupport/qprinter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPrintSupport/qprinterinfo.sip` & `PyQt6-6.5.2/sip/QtPrintSupport/qprinterinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPrintSupport/qprintpreviewdialog.sip` & `PyQt6-6.5.2/sip/QtPrintSupport/qprintpreviewdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPrintSupport/qprintpreviewwidget.sip` & `PyQt6-6.5.2/sip/QtPrintSupport/qprintpreviewwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtPrintSupport/qpyprintsupport_qlist.sip` & `PyQt6-6.5.2/sip/QtPrintSupport/qpyprintsupport_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/QtQmlmod.sip` & `PyQt6-6.5.2/sip/QtQml/QtQmlmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qjsengine.sip` & `PyQt6-6.5.2/sip/QtQml/qjsengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qjsmanagedvalue.sip` & `PyQt6-6.5.2/sip/QtQml/qjsmanagedvalue.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qjsprimitivevalue.sip` & `PyQt6-6.5.2/sip/QtQml/qjsprimitivevalue.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qjsvalue.sip` & `PyQt6-6.5.2/sip/QtQml/qjsvalue.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qjsvalueiterator.sip` & `PyQt6-6.5.2/sip/QtQml/qjsvalueiterator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qmlattachedpropertiesobject.sip` & `PyQt6-6.5.2/sip/QtQml/qmlattachedpropertiesobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qmlregistertype.sip` & `PyQt6-6.5.2/sip/QtQml/qmlregistertype.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qpyqmllistproperty.sip` & `PyQt6-6.5.2/sip/QtQml/qpyqmllistproperty.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqml.sip` & `PyQt6-6.5.2/sip/QtQml/qqml.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlabstracturlinterceptor.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlabstracturlinterceptor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlapplicationengine.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlapplicationengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlcomponent.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlcomponent.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlcontext.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlcontext.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlengine.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlerror.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlerror.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlexpression.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlexpression.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlextensionplugin.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlextensionplugin.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlfileselector.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlfileselector.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlincubator.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlincubator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmllist.sip` & `PyQt6-6.5.2/sip/QtQml/qqmllist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlnetworkaccessmanagerfactory.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlnetworkaccessmanagerfactory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlparserstatus.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlparserstatus.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlproperty.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlproperty.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlpropertymap.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlpropertymap.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlpropertyvaluesource.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlpropertyvaluesource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQml/qqmlscriptstring.sip` & `PyQt6-6.5.2/sip/QtQml/qqmlscriptstring.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/QtQuickmod.sip` & `PyQt6-6.5.2/sip/QtQuick/QtQuickmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickframebufferobject.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickframebufferobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickgraphicsconfiguration.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickgraphicsconfiguration.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickgraphicsdevice.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickgraphicsdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickimageprovider.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickimageprovider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickitem.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickitemgrabresult.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickitemgrabresult.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickpainteditem.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickpainteditem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickrendercontrol.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickrendercontrol.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickrendertarget.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickrendertarget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquicktextdocument.sip` & `PyQt6-6.5.2/sip/QtQuick/qquicktextdocument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickview.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qquickwindow.sip` & `PyQt6-6.5.2/sip/QtQuick/qquickwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgflatcolormaterial.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgflatcolormaterial.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsggeometry.sip` & `PyQt6-6.5.2/sip/QtQuick/qsggeometry.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgimagenode.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgimagenode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgmaterial.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgmaterial.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgmaterialshader.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgmaterialshader.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgmaterialtype.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgmaterialtype.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgnode.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgnode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgrectanglenode.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgrectanglenode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgrendererinterface.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgrendererinterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgrendernode.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgrendernode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgsimplerectnode.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgsimplerectnode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgsimpletexturenode.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgsimpletexturenode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgtexture.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgtexture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgtexture_platform.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgtexture_platform.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgtexturematerial.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgtexturematerial.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgtextureprovider.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgtextureprovider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick/qsgvertexcolormaterial.sip` & `PyQt6-6.5.2/sip/QtQuick/qsgvertexcolormaterial.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick3D/QtQuick3Dmod.sip` & `PyQt6-6.5.2/sip/QtQuick3D/QtQuick3Dmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick3D/qquick3d.sip` & `PyQt6-6.5.2/sip/QtQuick3D/qquick3d.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick3D/qquick3dgeometry.sip` & `PyQt6-6.5.2/sip/QtQuick3D/qquick3dgeometry.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick3D/qquick3dobject.sip` & `PyQt6-6.5.2/sip/QtQuick3D/qquick3dobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuick3D/qquick3dtexturedata.sip` & `PyQt6-6.5.2/sip/QtQuick3D/qquick3dtexturedata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuickWidgets/QtQuickWidgetsmod.sip` & `PyQt6-6.5.2/sip/QtQuickWidgets/QtQuickWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtQuickWidgets/qquickwidget.sip` & `PyQt6-6.5.2/sip/QtQuickWidgets/qquickwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtRemoteObjects/QtRemoteObjectsmod.sip` & `PyQt6-6.5.2/sip/QtRemoteObjects/QtRemoteObjectsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtRemoteObjects/qremoteobjectabstractitemmodelreplica.sip` & `PyQt6-6.5.2/sip/QtRemoteObjects/qremoteobjectabstractitemmodelreplica.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtRemoteObjects/qremoteobjectdynamicreplica.sip` & `PyQt6-6.5.2/sip/QtRemoteObjects/qremoteobjectdynamicreplica.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtRemoteObjects/qremoteobjectnode.sip` & `PyQt6-6.5.2/sip/QtRemoteObjects/qremoteobjectnode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtRemoteObjects/qremoteobjectregistry.sip` & `PyQt6-6.5.2/sip/QtRemoteObjects/qremoteobjectregistry.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtRemoteObjects/qremoteobjectreplica.sip` & `PyQt6-6.5.2/sip/QtRemoteObjects/qremoteobjectreplica.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtRemoteObjects/qtremoteobjectglobal.sip` & `PyQt6-6.5.2/sip/QtRemoteObjects/qtremoteobjectglobal.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/QtSensorsmod.sip` & `PyQt6-6.5.2/sip/QtSensors/QtSensorsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qaccelerometer.sip` & `PyQt6-6.5.2/sip/QtSensors/qaccelerometer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qambientlightsensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qambientlightsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qambienttemperaturesensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qambienttemperaturesensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qcompass.sip` & `PyQt6-6.5.2/sip/QtSensors/qcompass.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qgyroscope.sip` & `PyQt6-6.5.2/sip/QtSensors/qgyroscope.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qhumiditysensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qhumiditysensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qirproximitysensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qirproximitysensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qlidsensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qlidsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qlightsensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qlightsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qmagnetometer.sip` & `PyQt6-6.5.2/sip/QtSensors/qmagnetometer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qorientationsensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qorientationsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qpressuresensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qpressuresensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qproximitysensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qproximitysensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qrotationsensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qrotationsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qsensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qtapsensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qtapsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSensors/qtiltsensor.sip` & `PyQt6-6.5.2/sip/QtSensors/qtiltsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSerialPort/QtSerialPortmod.sip` & `PyQt6-6.5.2/sip/QtSerialPort/QtSerialPortmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSerialPort/qserialport.sip` & `PyQt6-6.5.2/sip/QtSerialPort/qserialport.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSerialPort/qserialportinfo.sip` & `PyQt6-6.5.2/sip/QtSerialPort/qserialportinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSpatialAudio/QtSpatialAudiomod.sip` & `PyQt6-6.5.2/sip/QtSpatialAudio/QtSpatialAudiomod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSpatialAudio/qambientsound.sip` & `PyQt6-6.5.2/sip/QtSpatialAudio/qambientsound.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSpatialAudio/qaudioengine.sip` & `PyQt6-6.5.2/sip/QtSpatialAudio/qaudioengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSpatialAudio/qaudiolistener.sip` & `PyQt6-6.5.2/sip/QtSpatialAudio/qaudiolistener.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSpatialAudio/qaudioroom.sip` & `PyQt6-6.5.2/sip/QtSpatialAudio/qaudioroom.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSpatialAudio/qspatialsound.sip` & `PyQt6-6.5.2/sip/QtSpatialAudio/qspatialsound.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/QtSqlmod.sip` & `PyQt6-6.5.2/sip/QtSql/QtSqlmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqldatabase.sip` & `PyQt6-6.5.2/sip/QtSql/qsqldatabase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqldriver.sip` & `PyQt6-6.5.2/sip/QtSql/qsqldriver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqlerror.sip` & `PyQt6-6.5.2/sip/QtSql/qsqlerror.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqlfield.sip` & `PyQt6-6.5.2/sip/QtSql/qsqlfield.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqlindex.sip` & `PyQt6-6.5.2/sip/QtSql/qsqlindex.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqlquery.sip` & `PyQt6-6.5.2/sip/QtSql/qsqlquery.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqlquerymodel.sip` & `PyQt6-6.5.2/sip/QtSql/qsqlquerymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqlrecord.sip` & `PyQt6-6.5.2/sip/QtSql/qsqlrecord.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqlrelationaldelegate.sip` & `PyQt6-6.5.2/sip/QtSql/qsqlrelationaldelegate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqlrelationaltablemodel.sip` & `PyQt6-6.5.2/sip/QtSql/qsqlrelationaltablemodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqlresult.sip` & `PyQt6-6.5.2/sip/QtSql/qsqlresult.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qsqltablemodel.sip` & `PyQt6-6.5.2/sip/QtSql/qsqltablemodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSql/qtsqlglobal.sip` & `PyQt6-6.5.2/sip/QtSql/qtsqlglobal.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSvg/QtSvgmod.sip` & `PyQt6-6.5.2/sip/QtSvg/QtSvgmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSvg/qsvggenerator.sip` & `PyQt6-6.5.2/sip/QtSvg/qsvggenerator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSvg/qsvgrenderer.sip` & `PyQt6-6.5.2/sip/QtSvg/qsvgrenderer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSvgWidgets/QtSvgWidgetsmod.sip` & `PyQt6-6.5.2/sip/QtSvgWidgets/QtSvgWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSvgWidgets/qgraphicssvgitem.sip` & `PyQt6-6.5.2/sip/QtSvgWidgets/qgraphicssvgitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtSvgWidgets/qsvgwidget.sip` & `PyQt6-6.5.2/sip/QtSvgWidgets/qsvgwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtTest/QtTestmod.sip` & `PyQt6-6.5.2/sip/QtTest/QtTestmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtTest/qabstractitemmodeltester.sip` & `PyQt6-6.5.2/sip/QtTest/qabstractitemmodeltester.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtTest/qsignalspy.sip` & `PyQt6-6.5.2/sip/QtTest/qsignalspy.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtTest/qtestkeyboard.sip` & `PyQt6-6.5.2/sip/QtTest/qtestkeyboard.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtTest/qtestmouse.sip` & `PyQt6-6.5.2/sip/QtTest/qtestmouse.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtTest/qtestsystem.sip` & `PyQt6-6.5.2/sip/QtTest/qtestsystem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtTextToSpeech/QtTextToSpeechmod.sip` & `PyQt6-6.5.2/sip/QtTextToSpeech/QtTextToSpeechmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtTextToSpeech/qtexttospeech.sip` & `PyQt6-6.5.2/sip/QtTextToSpeech/qtexttospeech.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtTextToSpeech/qvoice.sip` & `PyQt6-6.5.2/sip/QtTextToSpeech/qvoice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWebChannel/QtWebChannelmod.sip` & `PyQt6-6.5.2/sip/QtWebChannel/QtWebChannelmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWebChannel/qwebchannel.sip` & `PyQt6-6.5.2/sip/QtWebChannel/qwebchannel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWebChannel/qwebchannelabstracttransport.sip` & `PyQt6-6.5.2/sip/QtWebChannel/qwebchannelabstracttransport.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWebSockets/QtWebSocketsmod.sip` & `PyQt6-6.5.2/sip/QtWebSockets/QtWebSocketsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWebSockets/qmaskgenerator.sip` & `PyQt6-6.5.2/sip/QtWebSockets/qmaskgenerator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWebSockets/qwebsocket.sip` & `PyQt6-6.5.2/sip/QtWebSockets/qwebsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWebSockets/qwebsocketcorsauthenticator.sip` & `PyQt6-6.5.2/sip/QtWebSockets/qwebsocketcorsauthenticator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWebSockets/qwebsockethandshakeoptions.sip` & `PyQt6-6.5.2/sip/QtWebSockets/qwebsockethandshakeoptions.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWebSockets/qwebsocketprotocol.sip` & `PyQt6-6.5.2/sip/QtWebSockets/qwebsocketprotocol.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWebSockets/qwebsocketserver.sip` & `PyQt6-6.5.2/sip/QtWebSockets/qwebsocketserver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/QtWidgetsmod.sip` & `PyQt6-6.5.2/sip/QtWidgets/QtWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qabstractbutton.sip` & `PyQt6-6.5.2/sip/QtWidgets/qabstractbutton.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qabstractitemdelegate.sip` & `PyQt6-6.5.2/sip/QtWidgets/qabstractitemdelegate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qabstractitemview.sip` & `PyQt6-6.5.2/sip/QtWidgets/qabstractitemview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qabstractscrollarea.sip` & `PyQt6-6.5.2/sip/QtWidgets/qabstractscrollarea.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qabstractslider.sip` & `PyQt6-6.5.2/sip/QtWidgets/qabstractslider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qabstractspinbox.sip` & `PyQt6-6.5.2/sip/QtWidgets/qabstractspinbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qapplication.sip` & `PyQt6-6.5.2/sip/QtWidgets/qapplication.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qboxlayout.sip` & `PyQt6-6.5.2/sip/QtWidgets/qboxlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qbuttongroup.sip` & `PyQt6-6.5.2/sip/QtWidgets/qbuttongroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qcalendarwidget.sip` & `PyQt6-6.5.2/sip/QtWidgets/qcalendarwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qcheckbox.sip` & `PyQt6-6.5.2/sip/QtWidgets/qcheckbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qcolordialog.sip` & `PyQt6-6.5.2/sip/QtWidgets/qcolordialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qcolumnview.sip` & `PyQt6-6.5.2/sip/QtWidgets/qcolumnview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qcombobox.sip` & `PyQt6-6.5.2/sip/QtWidgets/qcombobox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qcommandlinkbutton.sip` & `PyQt6-6.5.2/sip/QtWidgets/qcommandlinkbutton.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qcommonstyle.sip` & `PyQt6-6.5.2/sip/QtWidgets/qcommonstyle.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qcompleter.sip` & `PyQt6-6.5.2/sip/QtWidgets/qcompleter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qdatawidgetmapper.sip` & `PyQt6-6.5.2/sip/QtWidgets/qdatawidgetmapper.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qdatetimeedit.sip` & `PyQt6-6.5.2/sip/QtWidgets/qdatetimeedit.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qdial.sip` & `PyQt6-6.5.2/sip/QtWidgets/qdial.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qdialog.sip` & `PyQt6-6.5.2/sip/QtWidgets/qdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qdialogbuttonbox.sip` & `PyQt6-6.5.2/sip/QtWidgets/qdialogbuttonbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qdockwidget.sip` & `PyQt6-6.5.2/sip/QtWidgets/qdockwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qdrawutil.sip` & `PyQt6-6.5.2/sip/QtWidgets/qdrawutil.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qerrormessage.sip` & `PyQt6-6.5.2/sip/QtWidgets/qerrormessage.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qfiledialog.sip` & `PyQt6-6.5.2/sip/QtWidgets/qfiledialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qfileiconprovider.sip` & `PyQt6-6.5.2/sip/QtWidgets/qfileiconprovider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qfilesystemmodel.sip` & `PyQt6-6.5.2/sip/QtWidgets/qfilesystemmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qfocusframe.sip` & `PyQt6-6.5.2/sip/QtWidgets/qfocusframe.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qfontcombobox.sip` & `PyQt6-6.5.2/sip/QtWidgets/qfontcombobox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qfontdialog.sip` & `PyQt6-6.5.2/sip/QtWidgets/qfontdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qformlayout.sip` & `PyQt6-6.5.2/sip/QtWidgets/qformlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qframe.sip` & `PyQt6-6.5.2/sip/QtWidgets/qframe.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgesture.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgesture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgesturerecognizer.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgesturerecognizer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicsanchorlayout.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicsanchorlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicseffect.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicseffect.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicsgridlayout.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicsgridlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicsitem.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicsitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicslayout.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicslayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicslayoutitem.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicslayoutitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicslinearlayout.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicslinearlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicsproxywidget.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicsproxywidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicsscene.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicsscene.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicssceneevent.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicssceneevent.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicstransform.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicstransform.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicsview.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicsview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgraphicswidget.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgraphicswidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgridlayout.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgridlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qgroupbox.sip` & `PyQt6-6.5.2/sip/QtWidgets/qgroupbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qheaderview.sip` & `PyQt6-6.5.2/sip/QtWidgets/qheaderview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qinputdialog.sip` & `PyQt6-6.5.2/sip/QtWidgets/qinputdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qitemdelegate.sip` & `PyQt6-6.5.2/sip/QtWidgets/qitemdelegate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qitemeditorfactory.sip` & `PyQt6-6.5.2/sip/QtWidgets/qitemeditorfactory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qkeysequenceedit.sip` & `PyQt6-6.5.2/sip/QtWidgets/qkeysequenceedit.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qlabel.sip` & `PyQt6-6.5.2/sip/QtWidgets/qlabel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qlayout.sip` & `PyQt6-6.5.2/sip/QtWidgets/qlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qlayoutitem.sip` & `PyQt6-6.5.2/sip/QtWidgets/qlayoutitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qlcdnumber.sip` & `PyQt6-6.5.2/sip/QtWidgets/qlcdnumber.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qlineedit.sip` & `PyQt6-6.5.2/sip/QtWidgets/qlineedit.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qlistview.sip` & `PyQt6-6.5.2/sip/QtWidgets/qlistview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qlistwidget.sip` & `PyQt6-6.5.2/sip/QtWidgets/qlistwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qmainwindow.sip` & `PyQt6-6.5.2/sip/QtWidgets/qmainwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qmdiarea.sip` & `PyQt6-6.5.2/sip/QtWidgets/qmdiarea.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qmdisubwindow.sip` & `PyQt6-6.5.2/sip/QtWidgets/qmdisubwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qmenu.sip` & `PyQt6-6.5.2/sip/QtWidgets/qmenu.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qmenubar.sip` & `PyQt6-6.5.2/sip/QtWidgets/qmenubar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qmessagebox.sip` & `PyQt6-6.5.2/sip/QtWidgets/qmessagebox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qplaintextedit.sip` & `PyQt6-6.5.2/sip/QtWidgets/qplaintextedit.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qprogressbar.sip` & `PyQt6-6.5.2/sip/QtWidgets/qprogressbar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qprogressdialog.sip` & `PyQt6-6.5.2/sip/QtWidgets/qprogressdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qproxystyle.sip` & `PyQt6-6.5.2/sip/QtWidgets/qproxystyle.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qpushbutton.sip` & `PyQt6-6.5.2/sip/QtWidgets/qpushbutton.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qpywidgets_qlist.sip` & `PyQt6-6.5.2/sip/QtWidgets/qpywidgets_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qradiobutton.sip` & `PyQt6-6.5.2/sip/QtWidgets/qradiobutton.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qrubberband.sip` & `PyQt6-6.5.2/sip/QtWidgets/qrubberband.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qscrollarea.sip` & `PyQt6-6.5.2/sip/QtWidgets/qscrollarea.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qscrollbar.sip` & `PyQt6-6.5.2/sip/QtWidgets/qscrollbar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qscroller.sip` & `PyQt6-6.5.2/sip/QtWidgets/qscroller.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qscrollerproperties.sip` & `PyQt6-6.5.2/sip/QtWidgets/qscrollerproperties.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qsizegrip.sip` & `PyQt6-6.5.2/sip/QtWidgets/qsizegrip.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qsizepolicy.sip` & `PyQt6-6.5.2/sip/QtWidgets/qsizepolicy.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qslider.sip` & `PyQt6-6.5.2/sip/QtWidgets/qslider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qspinbox.sip` & `PyQt6-6.5.2/sip/QtWidgets/qspinbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qsplashscreen.sip` & `PyQt6-6.5.2/sip/QtWidgets/qsplashscreen.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qsplitter.sip` & `PyQt6-6.5.2/sip/QtWidgets/qsplitter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qstackedlayout.sip` & `PyQt6-6.5.2/sip/QtWidgets/qstackedlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qstackedwidget.sip` & `PyQt6-6.5.2/sip/QtWidgets/qstackedwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qstatusbar.sip` & `PyQt6-6.5.2/sip/QtWidgets/qstatusbar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qstyle.sip` & `PyQt6-6.5.2/sip/QtWidgets/qstyle.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qstyleditemdelegate.sip` & `PyQt6-6.5.2/sip/QtWidgets/qstyleditemdelegate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qstylefactory.sip` & `PyQt6-6.5.2/sip/QtWidgets/qstylefactory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qstyleoption.sip` & `PyQt6-6.5.2/sip/QtWidgets/qstyleoption.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qstylepainter.sip` & `PyQt6-6.5.2/sip/QtWidgets/qstylepainter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qsystemtrayicon.sip` & `PyQt6-6.5.2/sip/QtWidgets/qsystemtrayicon.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtabbar.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtabbar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtableview.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtableview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtablewidget.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtablewidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtabwidget.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtabwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtextbrowser.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtextbrowser.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtextedit.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtextedit.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtoolbar.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtoolbar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtoolbox.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtoolbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtoolbutton.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtoolbutton.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtooltip.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtooltip.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtreeview.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtreeview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtreewidget.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtreewidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qtreewidgetitemiterator.sip` & `PyQt6-6.5.2/sip/QtWidgets/qtreewidgetitemiterator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qundoview.sip` & `PyQt6-6.5.2/sip/QtWidgets/qundoview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qwhatsthis.sip` & `PyQt6-6.5.2/sip/QtWidgets/qwhatsthis.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qwidget.sip` & `PyQt6-6.5.2/sip/QtWidgets/qwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qwidgetaction.sip` & `PyQt6-6.5.2/sip/QtWidgets/qwidgetaction.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtWidgets/qwizard.sip` & `PyQt6-6.5.2/sip/QtWidgets/qwizard.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtXml/QtXmlmod.sip` & `PyQt6-6.5.2/sip/QtXml/QtXmlmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/sip/QtXml/qdom.sip` & `PyQt6-6.5.2/sip/QtXml/qdom.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Compiler/__init__.py` & `PyQt6-6.5.2/uic/Compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Compiler/as_string.py` & `PyQt6-6.5.2/uic/Compiler/as_string.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Compiler/compiler.py` & `PyQt6-6.5.2/uic/Compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Compiler/indenter.py` & `PyQt6-6.5.2/uic/Compiler/indenter.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Compiler/misc.py` & `PyQt6-6.5.2/uic/Compiler/misc.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Compiler/proxy_metaclass.py` & `PyQt6-6.5.2/uic/Compiler/proxy_metaclass.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Compiler/qobjectcreator.py` & `PyQt6-6.5.2/uic/Compiler/qobjectcreator.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Compiler/qtproxies.py` & `PyQt6-6.5.2/uic/Compiler/qtproxies.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Loader/__init__.py` & `PyQt6-6.5.2/uic/Loader/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Loader/loader.py` & `PyQt6-6.5.2/uic/Loader/loader.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/Loader/qobjectcreator.py` & `PyQt6-6.5.2/uic/Loader/qobjectcreator.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/__init__.py` & `PyQt6-6.5.2/uic/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/compile_ui.py` & `PyQt6-6.5.2/uic/compile_ui.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/enum_map.py` & `PyQt6-6.5.2/uic/enum_map.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/exceptions.py` & `PyQt6-6.5.2/uic/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/icon_cache.py` & `PyQt6-6.5.2/uic/icon_cache.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/load_ui.py` & `PyQt6-6.5.2/uic/load_ui.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/objcreator.py` & `PyQt6-6.5.2/uic/objcreator.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/properties.py` & `PyQt6-6.5.2/uic/properties.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/pyuic.py` & `PyQt6-6.5.2/uic/pyuic.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/ui_file.py` & `PyQt6-6.5.2/uic/ui_file.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/uiparser.py` & `PyQt6-6.5.2/uic/uiparser.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/widget-plugins/qaxcontainer.py` & `PyQt6-6.5.2/uic/widget-plugins/qaxcontainer.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/widget-plugins/qscintilla.py` & `PyQt6-6.5.2/uic/widget-plugins/qscintilla.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/widget-plugins/qtcharts.py` & `PyQt6-6.5.2/uic/widget-plugins/qtcharts.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/widget-plugins/qtprintsupport.py` & `PyQt6-6.5.2/uic/widget-plugins/qtprintsupport.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/widget-plugins/qtquickwidgets.py` & `PyQt6-6.5.2/uic/widget-plugins/qtquickwidgets.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.5.1/uic/widget-plugins/qtwebenginewidgets.py` & `PyQt6-6.5.2/uic/widget-plugins/qtwebenginewidgets.py`

 * *Files identical despite different names*

