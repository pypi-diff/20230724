# Comparing `tmp/windeklar-0.2.6.tar.gz` & `tmp/windeklar-0.3.0.tar.gz`

## Comparing `windeklar-0.2.6.tar` & `windeklar-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.6/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.6/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/__init__.py
--rwxr-xr-x   0        0        0    16332 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    45955 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.6/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.6/LICENSE
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 windeklar-0.2.6/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 windeklar-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.3.0/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.3.0/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.3.0/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.3.0/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.3.0/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.3.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.3.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/__init__.py
+-rwxr-xr-x   0        0        0    16521 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    47364 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.3.0/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 windeklar-0.3.0/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 windeklar-0.3.0/PKG-INFO
```

### Comparing `windeklar-0.2.6/.github/workflows/python-publish.yml` & `windeklar-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.3.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/src/WinDeklar/QTAux.py` & `windeklar-0.3.0/src/WinDeklar/QTAux.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,134 +54,141 @@
     x.setMaximumSize(QtCore.QSize(width, height))
 
 
 def set_progress_bar(host):
     return QtWidgets.QProgressBar(host)
 
 
-class ScreenControl(object):
+class ScreenWidget(object):
     """
-    Abstract class for any kind of input control like Sliders and Combos
+    Abstract class for any kind of screen widget like Sliders and Combos
     """
 
     def __init__(self, name, title, bound, action, layout, tooltip=None, label_height=20):
         # bound is the object responsible to keep the value, must implement:
-        #     get_control_value
-        #     set_control_value
+        #     get_value
+        #     set_widget_value
         self.name    = name
         self.ename   = title
         self.bounded = bound
         self.action  = action
         self.label   = None
 
-        # print('control:%s bound:%s, action:%s' % (name, bound, action))
+        # print('widget:%s bound:%s, action:%s' % (name, bound, action))
 
         self.bounded_name = 'self.bounded.'
  
-        is_widget, widget = self.get_widget()
-        if is_widget and layout is not None:
+        widget = self.get_widget()
+        if widget is not None and layout is not None:
             title = self.title()
             if title != '':
                 self.label = set_label(title, layout, height=label_height)  # must go after slider (see title())
             layout.addWidget(widget)
             if tooltip is not None:
                 widget.setToolTip(tooltip)
 
         self.refresh_others = False
         self.refresh()
 
     def current_value(self):
-        return self.bounded.get_control_value(self.name)
+        return self.bounded.get_value(self.name)
 
     def title(self):
         return self.ename
 
     def changed(self):
+        """
+        Internal event triggered when user changes the widget on the form, does the following things:
+            - updates the internal value
+            - trigger any user defined action (useful for recalculate other values for example)
+        :return:
+        """
         # print('%s changed to %s (bounded:%s)' % (self.name, self.value(), self.bounded))
-        self.bounded.set_control_value(self.name, self.value())
+        self.bounded.set_value(self.name, self.value())
         self.exec_action()
 
     def exec_action(self):
         self.exec_bounded_method(self.action)
 
     def exec_bounded_method(self, method_name):
         if method_name is None or method_name == '':
             return
         return getattr(self.bounded, method_name)()
 
     def get_widget(self):
         # abstract method
-        return False, None
+        return None
 
     def value(self):
         # abstract method
         return 0
 
     def refresh(self):
         # abstract method
         pass
 
     def set_ename(self, new_ename):
         self.ename = new_ename
 
     def set_fixed_width(self, width):
-        _, widget = self.get_widget()
+        widget = self.get_widget()
         if widget is not None:
             widget.setFixedWidth(width)
 
     def set_visible(self, is_visible):
-        valid, widget = self.get_widget()
-        if valid:
-            widget.setVisible(is_visible)
-            if self.label is not None:
-                self.label.setVisible(is_visible)
+        widget = self.get_widget()
+        if widget is None:
+            return
+        widget.setVisible(is_visible)
+        if self.label is not None:
+            self.label.setVisible(is_visible)
 
 
-class EnumCombo(ScreenControl):
+class EnumCombo(ScreenWidget):
     def __init__(self, name, title, bound, enum, action, layout, tooltip=None):
     
         self.enum  = enum
         self.combo = QtWidgets.QComboBox(None)
         for member in self.enum:
             self.combo.addItem(member.name)
 
         self.combo.currentIndexChanged.connect(self.changed_combo)
 
         super(EnumCombo, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
 
     def current_value(self):
-        e = self.bounded.get_control_value(self.name)
+        e = self.bounded.get_value(self.name)
         return e  # e.value
 
     def value(self):
         value = self.enum(self.combo.currentIndex())
         return value
 
     def refresh(self):
         self.combo.setCurrentIndex(self.current_value())
 
     def changed_combo(self, i):
-        self.bounded.set_control_value(self.name, self.enum(i))
+        self.bounded.set_value(self.name, self.enum(i))
         self.exec_action()
 
     def get_widget(self):
-        return True, self.combo
+        return self.combo
 
 
-class Combo(ScreenControl):
-    def __init__(self, name, title, bound, action, layout, control_def, tooltip=None, values_key='values'):
+class Combo(ScreenWidget):
+    def __init__(self, name, title, bound, action, layout, widget_def, tooltip=None, values_key='values'):
         self.combo = QtWidgets.QComboBox(None)
 
         self.combo.currentTextChanged.connect(self.changed)
         super(Combo, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
 
         original_values         = []
         self.load_values_action = None
-        if values_key in control_def:
-            values1 = control_def[values_key]
+        if values_key in widget_def:
+            values1 = widget_def[values_key]
             if isinstance(values1, list):
                 original_values = values1
             else:
                 load_function = string_to_eval(values1)
                 if load_function is not None:
                     self.load_values_action = load_function
         self.set_values(original_values)  # must go after definition so self.bounded_name exists
@@ -191,22 +198,22 @@
         values1 = self.exec_bounded_method(self.load_values_action) if self.load_values_action is not None else values
         self.combo.addItems(values1)
 
     def value(self):
         return self.combo.currentText()
 
     def get_widget(self):
-        return True, self.combo
+        return self.combo
 
     def refresh(self):
         # print('current value: %s of %s' % (self.current_value(), self.name))
         self.combo.setCurrentText(self.current_value())
 
 
-class Slider(ScreenControl):
+class Slider(ScreenWidget):
     def __init__(self, name, title, bound, min_value, max_value, action, layout, tooltip=None, scale=1):
 
         # Widget must be created before calling super
         self.slider = QtWidgets.QSlider(QtCore.Qt.Horizontal)
         self.set_min_max(min_value, max_value)
         self.vfactor = scale
         self.action  = action
@@ -220,57 +227,57 @@
         super(Slider, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
 
     def title(self):
         return '%s(%s)' % (self.ename, self.value())
 
     def changed(self):
         # print('set %s' % self.name)
-        self.bounded.set_control_value(self.name, self.value())
+        self.bounded.set_value(self.name, self.value())
         self.label.setText(self.title())
         self.exec_action()
 
     def get_widget(self):
-        return True, self.slider
+        return self.slider
 
     def value(self):
         value = float(self.slider.value())/self.vfactor  # integer to float scaling (slider only accept integers)
         return value
 
     def refresh(self):
         self.slider.setValue(self.current_value()*self.vfactor)
 
     def set_min_max(self, min_value, max_value):
         # print('set min:%s max:%s' % (min_value, max_value))
         self.slider.setMinimum(min_value)
         self.slider.setMaximum(max_value)
 
 
-class Button(ScreenControl):
+class Button(ScreenWidget):
     def __init__(self, name, title, bound, action, layout, tooltip=None, width=50, length=100):
 
         # Widget must be created before calling super
         self.button = set_button(title, length, width, layout, self.changed)
         super(Button, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
 
     def title(self):
         return ''  # button don't have title label
 
     def changed(self):
         # print '%s clicked (%s)' %(self.name, self.event)
         self.exec_action()
 
     def get_widget(self):
-        return True, self.button
+        return self.button
 
     def set_ename(self, new_ename):
         self.ename = new_ename
         self.button.setText(self.ename)
 
 
-class CheckButton(ScreenControl):
+class CheckButton(ScreenWidget):
     def __init__(self, name, title, bound, action, layout, tooltip=None):
 
         # Widget must be created before calling super
         self.button = QtWidgets.QCheckBox(title)
         super(CheckButton, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
         self.button.stateChanged.connect(self.changed)
         self.button.setChecked(self.current_value())
@@ -278,102 +285,102 @@
     def title(self):
         return ''  # button don't have title label
 
     def value(self):
         return self.button.isChecked()
 
     def get_widget(self):
-        return True, self.button
+        return self.button
 
     def refresh(self):
         self.button.setChecked(self.current_value())
 
 
-class EditText(ScreenControl):
+class EditText(ScreenWidget):
     def __init__(self, name, title, bound, action, layout, tooltip=None):
         # Widget must be created before calling super
         self.edit_text = QtWidgets.QLineEdit()
         self.edit_text.textChanged.connect(self.changed)
         super(EditText, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
 
     def get_widget(self):
-        return True, self.edit_text
+        return self.edit_text
 
     def value(self):
         value = self.edit_text.text()
         return value
 
     def refresh(self):
         self.edit_text.setText(str(self.current_value()))
 
 
-class EditNumber(ScreenControl):
+class EditNumber(ScreenWidget):
     def __init__(self, name, title, bound, action, layout, tooltip=None):
         # Widget must be created before calling super
         self.edit_text = QtWidgets.QLineEdit()
         self.edit_text.setValidator(QtGui.QDoubleValidator())
         self.edit_text.textChanged.connect(self.changed)
         super(EditNumber, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
 
     def get_widget(self):
-        return True, self.edit_text
+        return self.edit_text
 
     def value(self):
         value = float(self.edit_text.text())
         return value
 
     def refresh(self):
         self.edit_text.setText(str(self.current_value()))
 
 
-class EditNumberSpin(ScreenControl):
-    def __init__(self, name, title, bound, action, layout, control_def, tooltip=None, parms_def='parms',
+class EditNumberSpin(ScreenWidget):
+    def __init__(self, name, title, bound, action, layout, widget_def, tooltip=None, parms_def='parms',
                  step_def='step', type_def='type', min_def='minimum', max_def='maximum'):
         # Widget must be created before calling super
-        parms = control_def.get(parms_def, {})
+        parms = widget_def.get(parms_def, {})
         is_integer = parms.get(type_def, 'float') == 'integer'
         self.edit_spin = QtWidgets.QSpinBox(None) if is_integer else QtWidgets.QDoubleSpinBox(None)
         if step_def in parms:
             self.edit_spin.setSingleStep(parms[step_def])
         if min_def in parms:
             self.edit_spin.setMinimum(parms[min_def])
         if max_def in parms:
             self.edit_spin.setMaximum(parms[max_def])
         self.edit_spin.valueChanged.connect(self.changed)
         super(EditNumberSpin, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
 
     def get_widget(self):
-        return True, self.edit_spin
+        return self.edit_spin
 
     def value(self):
         value = float(self.edit_spin.value())
         return value
 
     def refresh(self):
         self.edit_spin.setValue(self.current_value())
 
     def set_min_max(self, min_value, max_value):
         # print('set min:%s max:%s' % (min_value, max_value))
         self.edit_spin.setMinimum(min_value)
         self.edit_spin.setMaximum(max_value)
 
 
-class MenuItem(ScreenControl):
+class MenuItem(ScreenWidget):
     def __init__(self, name, title, bound, action, layout, main_window, tooltip=None):
         # Widget must be created before calling super
         self.menu_item = QtWidgets.QAction(title, main_window)
         if action is not None:
             self.menu_item.triggered.connect(self.changed)
         super(MenuItem, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
 
     def get_widget(self):
-        return False, self.menu_item
+        return self.menu_item
 
 
-class Action(ScreenControl):
+class Action(ScreenWidget):
     """
     Wrapper for a QtAction, useful
     """
     def __init__(self, name, title, provider, main_window, properties, tooltip=None, icon_key='icon'):
         self.name = name
         if icon_key in properties:
             std_icon_name = getattr(QtWidgets.QStyle, properties[icon_key])
@@ -394,46 +401,46 @@
         self.qt_action.setText(self.current_value())
 
     def set_ename(self, new_ename):
         self.ename = new_ename
         self.qt_action.setText(self.ename)
 
 
-class Label(ScreenControl):
+class Label(ScreenWidget):
     """
     Read only text (also known as Label)
     """
     def __init__(self, name, title, bound, action, layout, tooltip=None, align_left=True):
 
         # Widget must be created before calling super
         self.label_title = title
         self.text        = QtWidgets.QLabel(title)
         self.text.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
         if align_left:
             self.text.setAlignment(QtCore.Qt.AlignLeft)
-        bound.set_control_value_if_not_present(name, title)
+        bound.set_value_if_not_present(name, title)
         super(Label, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
 
     def get_widget(self):
-        return True, self.text
+        return self.text
 
     def refresh(self):
         # print('current value:%s' % self.current_value())
         self.text.setText('%s' % self.current_value())
 
 
-class ProgressBar(ScreenControl):
+class ProgressBar(ScreenWidget):
     def __init__(self, name, bound, action, layout, tooltip=None):
 
         # Widget must be created before calling super
         self.progress_bar = QtWidgets.QProgressBar(None)
         super(ProgressBar, self).__init__(name, '', bound, action, layout, tooltip=tooltip)
 
     def get_widget(self):
-        return True, self.progress_bar
+        return self.progress_bar
 
     def get_maximum(self):
         return self.progress_bar.maximum()
 
     def get_value(self):
         return self.progress_bar.value()
 
@@ -450,27 +457,30 @@
     def set_visible(self, value):
         self.progress_bar.setVisible(value)
 
     def reset(self):
         self.progress_bar.reset()
 
 
-class Constant(ScreenControl):
+class Constant(ScreenWidget):
     def __init__(self, name, title, bound, action, layout, tooltip=None):
         # it doesn't show anything, it is used for executing actions at initialization time
         super(Constant, self).__init__(name, title, bound, action, layout, tooltip=tooltip)
         self.cte_value = self.current_value()
         self.exec_action()
 
     def value(self):
         return self.cte_value
 
     def get_widget(self):
-        # Don't add as widget
-        return False, 0
+        """
+        Constant don't have an associated widget
+        :return:
+        """
+        return None
 
 
 class Menu:
     """
     Create a contextual menu to be showed via .popup()
     """
     def __init__(self, parent, title='Menu', actions=()):
```

### Comparing `windeklar-0.2.6/src/WinDeklar/WindowForm.py` & `windeklar-0.3.0/src/WinDeklar/WindowForm.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
 
 class ConfigurableWindow(QtWidgets.QMainWindow):
     """
     Defines a WinForm with many components inside in a declarative manner in a config file
     Notes:
         - a config_file_name is a yaml that has the definition (see view_example.yaml)
-        - a typical windows has some controls in the left and a Figure in the right (like a graph or a map)
+        - a typical windows has some widgets in the left and a Figure in the right (like a graph or a map)
     """
 
     def __init__(self, config_file_name, provider):
         """
         Init
         :param config_file_name: name of the file containing the window definition
         :param provider: handles all the form logic, usually a subclass of HostModel
         """
         super(ConfigurableWindow, self).__init__(parent=None)
 
-        self.controls  = []
+        self.widgets   = []
         self.fig_views = []
         self.provider  = provider
         self.provider.set_main_window(self)
 
         self.win_config = get_win_config(config_file_name)
 
         # status bar logic
@@ -55,90 +55,102 @@
 
         # menu bar
         menu_bar = create_menu_bar(self.win_config, self, self.provider)
         if menu_bar is not None:
             self.setMenuBar(menu_bar)
 
         # toolbar
-        toolbar, toolbar_controls = create_toolbar(self.win_config, self, self.provider)
+        toolbar, toolbar_widgets = create_toolbar(self.win_config, self, self.provider)
         if toolbar is not None:
-            self.controls.extend(toolbar_controls)
+            self.widgets.extend(toolbar_widgets)
             self.addToolBar(toolbar)
 
         # Define the geometry of the main window
         size = self.win_config.get('size', [300, 300, 300, 300])
         QTAux.set_window(self, get_title(self.win_config, self.provider), size)
 
         # Create FRAME
         self.FRAME = QtWidgets.QFrame(self)
         if 'back_color' in self.win_config:
             [c1, c2, c3, c4] = self.win_config['back_color']
             self.FRAME.setStyleSheet("QWidget { background-color: %s }" % QtGui.QColor(c1, c2, c3, c4).name())
         self.LAYOUT   = QtWidgets.QGridLayout()
-        self.fig_views, layout_controls = set_layout(self.LAYOUT, self.win_config.get('layout', []), self,
-                                                     row_col=[0, 0])
-        self.controls.extend(layout_controls)
+        self.fig_views, layout_widgets = set_layout(self.LAYOUT, self.win_config.get('layout', []), self,
+                                                    row_col=[0, 0])
+        self.widgets.extend(layout_widgets)
         self.FRAME.setLayout(self.LAYOUT)
         self.setCentralWidget(self.FRAME)
 
         self.provider.initialize()
         self.refresh()
         self.show()
 
-    def get_control_value(self, name):
+    def get_value(self, name):
+        """
+        Returns the value of a state variable
+        :param name: name of the variable
+        :return:
+        """
         # print('get value for %s' % name)
-        return self.provider.get_control_value(name)
+        return self.provider.get_value(name)
 
-    def control_has_value(self, name):
-        return self.provider.control_has_value(name)
+    def widget_has_value(self, name):
+        return self.provider.widget_has_value(name)
 
-    def set_control_value(self, name, value):
-        self.provider.set_control_value(name, value)
+    def set_widget_value(self, name, value):
+        self.provider.set_value(name, value)
         self.refresh_other_widgets(name)
         self.refresh()
 
-    def set_control_min_max(self, control_name, min_value, max_value):
-        control = self.get_control_by_name(control_name)
-        if control is None:
+    def set_widget_min_max(self, widget_name, min_value, max_value):
+        widget = self.get_widget_by_name(widget_name)
+        if widget is None:
             return
-        control.set_min_max(min_value, max_value)
+        widget.set_min_max(min_value, max_value)
 
-    def set_control_title(self, control_name, new_title):
-        control = self.get_control_by_name(control_name)
-        if control is None:
+    def set_widget_title(self, widget_name, new_title):
+        widget = self.get_widget_by_name(widget_name)
+        if widget is None:
             return
-        control.set_ename(new_title)
+        widget.set_ename(new_title)
+
+    def redraw_figures(self):
+        [figure.draw() for figure in self.fig_views]
 
     def refresh(self):
         # initial values can be set before fig_view was created
-        [fig_view.update_figure() for fig_view in self.fig_views]
+        [figure.update_figure() for figure in self.fig_views]
 
-    def refresh_controls(self):
-        for control in self.controls:
-            control.refresh()
-
-    def refresh_control(self, control_name):
-        control = self.get_control_by_name(control_name)
-        if control is not None:
-            control.refresh()
-
-    def refresh_other_widgets(self, control_name):
-        # if a widget that affect the value of others changed, it is needed to refresh all others'
-        #    ex: in view_color, the encoding combo changes the values of low and high sliders
-        changed = self.get_control_by_name(control_name)
+    def refresh_widgets(self):
+        for widget in self.widgets:
+            widget.refresh()
+
+    def refresh_widget(self, widget_name):
+        widget = self.get_widget_by_name(widget_name)
+        if widget is not None:
+            widget.refresh()
+
+    def refresh_other_widgets(self, widget_name):
+        """
+        If a widget that affect the value of others changed, it is needed to refresh all others'
+            ex: if a combo of countries changes, the combo of cities must be reloaded
+        :param widget_name:
+        :return:
+        """
+        changed = self.get_widget_by_name(widget_name)
         if changed is not None and changed.refresh_others:
             # print('refresh others')
-            for control in self.controls:
-                if control != changed:
-                    control.refresh()
-
-    def get_control_by_name(self, control_name):
-        for control in self.controls:
-            if control.name == control_name:
-                return control
+            for widget in self.widgets:
+                if widget != changed:
+                    widget.refresh()
+
+    def get_widget_by_name(self, widget_name):
+        for widget in self.widgets:
+            if widget.name == widget_name:
+                return widget
         return None
 
     def anim_is_running(self):
         for figure in self.fig_views:
             if figure.anim_is_running:
                 return True
         return False
@@ -154,31 +166,34 @@
             print('No status bar defined')
             return
         self.statusbar.showMessage(msg)
 
 
 class FigureView(FigureCanvas):
     """
-    Display a drawing that responds to a change in control values
+    Display a drawing that responds to a change in widget values
     """
     name_key        = 'name'
     title_key       = 'title'
     subtype_key     = 'subtype'
     animation_key   = 'animation'
     x_axis_key      = 'x_axis'
     y_axis_key      = 'y_axis'
     axes_limits_key = 'axes_limits'
+    text_pos_key    = 'text_position'
 
     def __init__(self, parent, config, size=(1, 1), scaled=True, x_visible=True, y_visible=True):
 
         self.parent   = parent
         self.subtype  = config.get(self.subtype_key, None)
         self.name     = config.get(self.name_key, 'no_name')
         title         = config.get(self.title_key, None)
+        self.text_pos = config.get(self.text_pos_key, None)
 
+        self.box_size    = pb.PointsBox()
         x_axis_def       = config.get(self.x_axis_key, {})
         self.x_axis_name = x_axis_def.get(self.name_key, None)
         y_axis_def       = config.get(self.y_axis_key, {})
         self.y_axis_name = y_axis_def.get(self.name_key, None)
 
         self.size_dim = size
         self.anim     = None
@@ -245,34 +260,69 @@
         if self.anim is not None:
             # in case of animation do not change axes limits, anim itself does it
             return
 
         if self.scaled:
             self.axes.axis('scaled')
 
-        axes_limits = self.parent.provider.axes_limits()
+        axes_limits = self.box_size.size() if not self.box_size.is_empty else None
+
         if axes_limits is not None:
             self.x_lower, self.x_upper, self.y_lower, self.y_upper = axes_limits
         self.axes.set_xbound(lower=self.x_lower, upper=self.x_upper)
         self.axes.set_ybound(lower=self.y_lower, upper=self.y_upper)
         self.axes.get_xaxis().set_visible(self.x_visible)
         self.axes.get_yaxis().set_visible(self.y_visible)
 
         ylabel_name = self.y_axis_name if self.y_axis_name is not None else ' '
         # assigning ' ' is a quick fix to assure y values fit in the figure
         self.axes.set_ylabel(ylabel_name)
         if self.x_axis_name is not None:
             self.axes.set_xlabel(self.x_axis_name)
 
+    def resize_axis(self, points, fixed_points=(), with_reset=True, inc=1.1):
+        """
+        Recalculate the figure size with the given points and resize it
+        :param points: :type list of [x, y]
+        :param fixed_points: list of point to add in addition to points
+        :param with_reset: whether to use the all points or just use the current ones
+        :param inc:
+        :return:
+        """
+        if with_reset:
+            self.box_size.reset()
+        self.box_size.add_points(points)
+        self.box_size.add_points(fixed_points)
+        self.box_size.set_bounds(self.axes, inc)
+
     def update_figure(self):
         self.clear()
         self.parent.provider.update_view(self, self.axes)
         self.parent.provider.apply_zoom()
         self.draw()
 
+    def text_position(self):
+        if self.text_pos is not None:
+            return self.text_pos
+        else:
+            return [0, 0]
+
+    def show_text(self, text_values, position=None):
+        """
+        Show a set of [name, value] in a given position on the graph
+        useful to display summary info like test validity or current speed
+        :param text_values: list of [name, value]
+        :param position: position (x, y) to display the value, if not present the 'text_position' config value is used
+        :return:
+        """
+        position1 = self.text_position() if position is None else position
+        if position1 is None:
+            return
+        show_text_values(self.axes, text_values, position1[0], position1[1])
+
     # Events
     def onclick(self, event):
         self.parent.provider.on_mouse_click(event, self.axes, self)
         self.set_axis()
         self.draw()
 
     def on_mouse_move(self, event):
@@ -381,206 +431,262 @@
         plt.show()
 
 
 class Dialog(QtWidgets.QDialog):
     """
     Functionality for an Input Panel
     """
+
     def __init__(self, dialog_name, provider, default_size=(300, 300, 400, 400)):
         super(Dialog, self).__init__(parent=None)
 
-        self.controls = []
-        self.provider = provider
+        self.widgets   = []
+        self.fig_views = []
+        self.provider  = provider
         self.provider.set_main_window(self)
-        self.fig_view = None
 
         self.win_config = get_win_config(dialog_name)
 
         # Define the geometry of the main window
         size = self.win_config.get('size', default_size)
         QTAux.set_window(self, get_title(self.win_config, self.provider), size)
 
         # Create FRAME
-        self.FRAME = QtWidgets.QFrame(self)
-        self.LAYOUT   = QtWidgets.QGridLayout()
-        self.fig_view, self.controls = set_layout(self.LAYOUT, self.win_config.get('layout', []), self, row_col=[0, 0])
+        self.FRAME  = QtWidgets.QFrame(self)
+        self.LAYOUT = QtWidgets.QGridLayout()
+        self.fig_views, self.widgets = set_layout(self.LAYOUT, self.win_config.get('layout', []), self, row_col=[0, 0])
         self.FRAME.setLayout(self.LAYOUT)
 
         self.provider.initialize()
-        if self.fig_view:
-            self.fig_view.update_figure()
+        self.refresh()
 
     def show(self):
         self.exec_()
 
-    def get_control_value(self, name):
+    def get_value(self, name):
         # print('get value for %s' % name)
-        return self.provider.get_control_value(name)
+        return self.provider.get_value(name)
 
-    def control_has_value(self, name):
-        return self.provider.control_has_value(name)
+    def widget_has_value(self, name):
+        return self.provider.widget_has_value(name)
 
-    def set_control_value(self, name, value):
+    def set_value(self, name, value):
         # print('%s changed to %s' % (name, value))
-        self.provider.set_control_value(name, value)
+        self.provider.set_value(name, value)
         self.refresh_other_widgets(name)
         self.refresh()
 
     def refresh(self):
-        if self.fig_view:
-            # initial values can be set before fig_view was created
-            self.fig_view.update_figure()
-
-    def refresh_controls(self):
-        for control in self.controls:
-            control.refresh()
-
-    def refresh_control(self, control_name):
-        control = self.get_control_by_name(control_name)
-        if control is not None:
-            control.refresh()
+        [fig.update_figure() for fig in self.fig_views]
 
-    def refresh_other_widgets(self, control_name):
+    def refresh_widgets(self):
+        for widget in self.widgets:
+            widget.refresh()
+
+    def refresh_widget(self, widget_name):
+        widget = self.get_widget_by_name(widget_name)
+        if widget is not None:
+            widget.refresh()
+
+    def refresh_other_widgets(self, widget_name):
         # if a widget that affect the value of others changed, it is needed to refresh all others'
         #    ex: in view_color, the encoding combo changes the values of low and high sliders
-        changed = self.get_control_by_name(control_name)
+        changed = self.get_widget_by_name(widget_name)
         if changed is not None and changed.refresh_others:
             # print('refresh others')
-            for control in self.controls:
-                if control != changed:
-                    control.refresh()
-
-    def get_control_by_name(self, control_name):
-        for control in self.controls:
-            if control.name == control_name:
-                return control
+            for widget in self.widgets:
+                if widget != changed:
+                    widget.refresh()
+
+    def get_widget_by_name(self, widget_name):
+        for widget in self.widgets:
+            if widget.name == widget_name:
+                return widget
         return None
 
     def confirmed(self):
-        print('confirmed')
+        # print('confirmed')
         self.close()
 
 
 class HostModel(object):
     """
-    Host for ConfigurableWindow (and ControlAndFigureWindow)
-       provides all the methods need it by ConfigurableWindow (like state management and control's definition)
+    Host for ConfigurableWindow
+       provides all the methods need it by ConfigurableWindow (like state management and widget's definition)
     """
 
     def __init__(self, initial_values=None):
         # keys
         self.zoom_key = 'zoom'
 
-        self.state       = initial_values if initial_values is not None else {}
+        self._state      = initial_values if initial_values is not None else {}
         self.main_window = None
-        self.box_size    = pb.PointsBox()
 
         self.zoom_center = None   # point where to center Zoom
         self.zoom_radius = 10.0   # radius around
+        self.box_size    = pb.PointsBox()  # ToDo: only used in zoom, should be avoided
 
     def set_main_window(self, main_window):
         self.main_window = main_window
 
     def refresh(self):
+        """
+        Refresh the whole WinForm (widgets and figures)
+        :return:
+        """
         if self.main_window is None:
             return
-        self.main_window.refresh_controls()
+        self.main_window.refresh_widgets()
         self.main_window.refresh()
 
-    def refresh_figure(self):
+    def refresh_figures(self):
         """
         Update all the figures in WinForm, useful when some change in the logic change the figure
         ex: when showing a map and a new path between two points in it is calculated
         :return:
         """
         if self.main_window is None:
             return
-        self.main_window.fig_view.draw()
+        self.main_window.redraw_figures()
 
-    def refresh_controls(self):
+    def refresh_widgets(self):
+        """
+        Refresh all widgets
+        :return:
+        """
         if self.main_window is None:
             return
-        self.main_window.refresh_controls()
+        self.main_window.refresh_widgets()
 
-    def refresh_control(self, name):
+    def refresh_widget(self, name):
+        """
+        Refresh just one widget
+        :param name: widget name
+        :return:
+        """
         if self.main_window is None:
             return
-        self.main_window.refresh_control(name)
+        self.main_window.refresh_widget(name)
 
-    def set_control_min_max(self, name, min_value, max_value):
+    def set_widget_min_max(self, name, min_value, max_value):
+        """
+        Set the min and max value of a given widget, useful for Slide when the min,max depends on other values
+        :param name:
+        :param min_value:
+        :param max_value:
+        :return:
+        """
         if self.main_window is None:
             return
-        self.main_window.set_control_min_max(name, min_value, max_value)
+        self.main_window.set_widget_min_max(name, min_value, max_value)
 
-    def set_control_title(self, name, new_title):
+    def set_widget_title(self, name, new_title):
         if self.main_window is None:
             return
-        self.main_window.set_control_title(name, new_title)
+        self.main_window.set_widget_title(name, new_title)
+
+    def set_and_refresh_widget(self, widget_name, value):
+        self._state[widget_name] = value
+        self.refresh_widget(widget_name)
 
-    def set_and_refresh_control(self, control_name, value):
-        self.state[control_name] = value
-        self.refresh_control(control_name)
-
-    def set_control_value(self, name, value):
-        self.state[name] = value
-        self.control_changed(name, value)
+    def set_values(self, values):
+        """
+        Bulk update a set of values
+        :param values: :type dictionary
+        :return:
+        """
+        self._state.update(values)
+
+    def set_value(self, name, value):
+        """
+        Set a new value for a state variable, if the
+        :param name:
+        :param value:
+        :return:
+        """
+        self._state[name] = value
+        self.widget_changed(name, value)
         self.refresh()
 
-    def set_control_value_internal(self, name, value):
+    def set_value_internal(self, name, value):
         """
-        Set a new value for control without firing the control_changed event
+        Set a new value for name without firing the widget_changed event
             Useful when the value is paired with an internal variable and because the slider rounds value some
             precision is lost (see self.orientation_key in view_localization.py for an example)
-        :param name:
+        :param name:    variable name
         :param value:
         :return: nothing
         """
         # print('%s changed to %s (internally)' % (name, value))
-        self.state[name] = value
+        self._state[name] = value
 
-    def set_control_value_if_not_present(self, name, value):
+    def set_value_if_not_present(self, name, value):
         """
-        Set control value only if name is not already in state
-        Useful for Label controls, where the title is the initial value but later can be changed
+        Set variable value only if name is not already in state
+        Useful for Label widgets, where the title is the initial value but later can be changed
         :param name:
         :param value:
         :return:
         """
-        if name not in self.state:
-            self.set_control_value(name, value)
+        if name not in self._state:
+            self.set_value(name, value)
 
-    def control_changed(self, name, value):
+    def widget_changed(self, name, value):
         """
-        Abstract method, used to trigger actions after a control changed
+        Event triggered when any widget changes its value, useful to set the values of other widgets
+        Abstract method
         :param name:
         :param value:
         :return:
         """
         pass
 
-    def get_control_by_name(self, name):
+    def get_widget_by_name(self, name):
         if self.main_window is None:
             return None
-        return self.main_window.get_control_by_name(name)
+        return self.main_window.get_widget_by_name(name)
 
-    def get_control_value(self, name):
-        if name in self.state:
-            return self.state[name]
+    def get_value(self, name, default=None):
+        """
+        Returns the value of a given variable
+            cases:
+                1. if it is already present in the _state it just return the value
+                2. if it is calculated it does the math
+                3. just return the default value
+        :param name:
+        :param default:
+        :return:
+        """
+        if name in self._state:
+            return self._state[name]
         else:
-            return self.calculated_value(name)
+            calc_value = self.calculated_value(name)
+            if calc_value is not None:
+                return calc_value
+            else:
+                return default
 
-    def control_has_value(self, name):
-        return name in self.state
+    def widget_has_value(self, name):
+        return name in self._state
 
-    def controls_def(self):
+    def widgets_def(self):
+        """
+        Abstract method
+        used to programmatically define widgets instead of in the definition file
+        :return:
+        """
         # abstract method
         return []
 
     def initialize(self):
-        # abstract method, use to initialize stuff
+        """
+        Called when the WinForm is loaded, useful for initialization stuff (like loading files)
+        Abstract method
+        :return:
+        """
         pass
 
     def get_file_name(self, title='Open', file_filter='*.*', directory=''):
         """
         Returns a valid file name using the standard dialog
         :param title:        window title
         :param file_filter:  show file that comply with this filter only
@@ -609,35 +715,19 @@
         :return:
         """
         # if main_windows is not set yet just return an empty one in order not to crash,
         # this it not a problem because main_window will be set later
         return self.main_window.progress_bar if self.main_window is not None else GeneralProgressBar()
 
     def title(self):
-        # abstract method
-        return None   # if None then the config title will be used
-
-    def view_size(self):
-        return 10, 10
-
-    def axes_limits(self):
-        # check for empty is necessary for on_click event
-        return self.box_size.size() if not self.box_size.is_empty else None
-
-    def text_position(self):
-        if not self.box_size.is_empty:
-            min_x, _, _, max_y = self.box_size.size()
-            return min_x, max_y
-        return self.main_window.win_config.get('text_position', None) if self.main_window is not None else None
-
-    def show_figure_text(self, ax, text_values):
-        position = self.text_position()
-        if position is None:
-            return
-        show_text_values(ax, text_values, position[0], position[1])
+        """
+        Returns the WinForm title
+        :return: string or None (if None then the config title will be used)
+        """
+        return None
 
     def show_status_bar_msg(self, msg):
         if self.main_window is None:
             print('no main window defined yet')
             return
         self.main_window.show_status_bar_msg(msg)
 
@@ -649,61 +739,45 @@
         :param ax:   axis of the Figure
         :return:
         """
         pass
 
     # Zoom management
     def zoom_active(self):
-        return self.state.get(self.zoom_key, False)
+        return self._state.get(self.zoom_key, False)
 
     def get_zoom_actions(self, event):
         return [['Zoom in', functools.partial(self.set_zoom_in, event)], ['Zoom out', self.set_zoom_out]]
 
     def set_zoom_out(self):
-        self.state[self.zoom_key] = False
+        self._state[self.zoom_key] = False
         self.refresh()
 
     def set_zoom_in(self, event):
-        self.state[self.zoom_key] = True
+        self._state[self.zoom_key] = True
         self.zoom_center = [event.xdata, event.ydata]
         self.refresh()
 
     def toggle_zoom(self):
-        self.state[self.zoom_key] = not self.state[self.zoom_key]
-        if not self.state[self.zoom_key]:
+        self._state[self.zoom_key] = not self._state[self.zoom_key]
+        if not self._state[self.zoom_key]:
             self.refresh()
 
     def set_zoom_center(self, event):
         if self.zoom_active():
             self.zoom_center = [event.xdata, event.ydata]
             self.refresh()
 
     def apply_zoom(self):
         if self.zoom_active() and self.zoom_center is not None:
             self.box_size.reset()
             self.box_size.add_points([[self.zoom_center[0] - self.zoom_radius, self.zoom_center[1] - self.zoom_radius],
                                       [self.zoom_center[0] + self.zoom_radius, self.zoom_center[1] + self.zoom_radius]])
 
-    # figure sizing
-    def resize_figure(self, ax, points, fixed_points=(), with_reset=True, inc=1.1):
-        """
-        Recalculate the figure size with the given points and resize it
-        :param ax:
-        :param points: :type list of [x, y]
-        :param fixed_points: list of point to add in addition to points
-        :param with_reset:
-        :param inc:
-        :return:
-        """
-        if with_reset:
-            self.box_size.reset()
-        self.box_size.add_points(points)
-        self.box_size.add_points(fixed_points)
-        self.box_size.set_bounds(ax, inc)
-
+    # events
     def on_mouse_click(self, event, ax, parent):
         # abstract method
         # print('%s click: button=%d, x=%d, y=%d, xdata=%f, ydata=%f' %
         #      ('double' if event.dblclick else 'single', event.button, event.x, event.y, event.xdata, event.ydata))
         if event.button == QTAux.MouseButton.Right:
             return self.on_right_click(event, ax, parent)
         else:
@@ -725,20 +799,21 @@
         # abstract method
         # print('%s click: button=%d, x=%d, y=%d, xdata=%f, ydata=%f' %
         #      ('double' if event.dblclick else 'single', event.button, event.x, event.y, event.xdata, event.ydata))
         return False
 
     def calculated_value(self, name):
         """
-        Abstract method, used to return a value that is a formula of other values
+        Abstract method, used to return a value that is a formula of other values'
+        ex: a = b + c  so calculated_value of a = state[b] + state[c]
         :param name:
         :return:
         """
         # abstract method
-        return 0.0
+        return None
 
     def save_cycle(self):
         """
         Save the info of a given cycle
         Note: it is directly called from an event in the UI (as defined in a yaml config file)
         :return:
         """
@@ -833,23 +908,23 @@
     def update_properties(self, changed):
         if changed is None:
             return
         self.properties.update(changed)
 
     def update_state(self):
         for k, v in self.properties.items():
-            self.set_control_value(k, v)
-            self.dialog.refresh_control(k)
+            self.set_value(k, v)
+            self.dialog.refresh_widget(k)
 
     def get_changed(self):
         changed = {}
         for k, v in self.properties.items():
-            if k not in self.state or v == self.state[k]:
+            if k not in self._state or v == self._state[k]:
                 continue
-            changed[k] = self.state[k]
+            changed[k] = self._state[k]
         return changed
 
 
 class TestHost(HostModel):
     """
     HostModel specialized for showing a set of tests stored in a file.
         The file name and the test name must be defined in the .yaml config file
@@ -867,38 +942,37 @@
 
     def initialize(self):
         test_file_name = self.main_window.win_config.get('test_file_name', '')
         test_name      = self.main_window.win_config.get('test_name', '')
         test_file      = yaml.get_yaml_file(test_file_name)
         test           = yaml.get_record(test_file['general'], test_name, 'tests', 'test', alternative_key_name='call')
         self.all_cases = test['cases']
-        self.set_control_min_max(self.test_key, 0, len(self.all_cases)-1)
+        self.set_widget_min_max(self.test_key, 0, len(self.all_cases) - 1)
         self.set_current_case()
 
-    def control_changed(self, name, _):
+    def widget_changed(self, name, _):
         if name == self.test_key:
             self.set_current_case()
 
     def set_current_case(self):
         case = self.get_current_case()
         if case is None:
             self.set_no_case()
             return
 
-        self.box_size.reset()  # to avoid resizing window when click
         current_case = case['case']
         self.output  = current_case.get('output', None)
         desc = self.set_case(current_case['input'],  self.output, current_case.get('desc', ''))
         self.show_status_bar_msg(desc)
-        self.refresh_controls()
+        self.refresh_widgets()
 
     def get_current_case(self):
         if not self.all_cases:
             return None
-        return self.all_cases[int(self.state[self.test_key])]
+        return self.all_cases[int(self._state[self.test_key])]
 
     def get_current_description(self, test_description):
         return test_description
 
     def set_case(self, case_input, output, description):
         """Abstract method for setting particular data"""
         return description
@@ -922,68 +996,67 @@
     if title is None:
         title = win_config.get(key, 'Title')
     return title
 
 
 def set_layout(father_layout, layout_config, window, row_col=None):
     fig_views = []
-    controls  = []
+    widgets  = []
     if father_layout is None or not layout_config:
-        return fig_views, controls
+        return fig_views, widgets
     for sub_layout_config1 in layout_config:
         sub_layout_config = sub_layout_config1['item']
-        sub_layout, fig_view_sub, sub_controls = set_layout_items(father_layout, sub_layout_config, window, row_col)
+        sub_layout, fig_view_sub, sub_widgets = set_layout_items(father_layout, sub_layout_config, window, row_col)
         if fig_view_sub is not None:
             fig_views.append(fig_view_sub)
-        controls.extend(sub_controls)
-        fig_views1, controls1 = set_layout(sub_layout, sub_layout_config.get('layout', []), window)
+        widgets.extend(sub_widgets)
+        fig_views1, widgets1 = set_layout(sub_layout, sub_layout_config.get('layout', []), window)
         fig_views.extend(fig_views1)
-        controls.extend(controls1)
-    return fig_views, controls
+        widgets.extend(widgets1)
+    return fig_views, widgets
 
 
 def set_layout_items(father_layout, layout_config, window, row_col=None):
     fig_view    = None
-    controls    = []
+    widgets     = []
     layout_type = layout_config['type']
     subtype     = layout_config.get('subtype', None)
     if layout_type == 'grid':
-        layout, controls = set_grid_layout(father_layout, subtype, layout_config, window, row_col=row_col)
+        layout, widgets = set_grid_layout(father_layout, subtype, layout_config, window, row_col=row_col)
     elif layout_type == 'figure':
         fig_view = set_figure_layout(father_layout, layout_config, window)
         layout   = None
     else:
         print('WARNING: layout type "%s" not implemented' % layout_type)
         layout = None
-    return layout, fig_view, controls
+    return layout, fig_view, widgets
 
 
 def set_grid_layout(father_layout, subtype, layout_config, window, row_col=None):
     if subtype == 'vertical':
         layout = QtWidgets.QVBoxLayout()
     elif subtype == 'horizontal':
         layout = QtWidgets.QHBoxLayout()
     else:
         raise Exception('Subtype %s not implemented for %s' % (subtype, type))
-    controls = add_controls_to_window(layout, layout_config, window)
+    widgets = add_widgets_to_window(layout, layout_config, window)
     if not row_col:
         father_layout.addLayout(layout)
     else:
         father_layout.addLayout(layout, row_col[0], row_col[1])
 
     fixed_width = layout_config.get('width', None)
     if fixed_width is not None:
-        [control.set_fixed_width(fixed_width) for control in controls]
+        [widget.set_fixed_width(fixed_width) for widget in widgets]
 
-    return layout, controls
+    return layout, widgets
 
 
 def set_figure_layout(father_layout, figure_config, window):
-    size     = window.provider.view_size() if window.provider is not None else (1, 0)
-    fig_view = FigureView(window, figure_config, size=size)
+    fig_view = FigureView(window, figure_config)
     father_layout.addWidget(fig_view)
     return fig_view
 
 
 def create_menu_bar(config, main_window, provider, key='menu_bar'):
     if key not in config:
         return None
@@ -1008,46 +1081,46 @@
                 #                        None, self)
                 main_menu.addAction(action)
     return menu_bar
 
 
 def create_toolbar(config, main_window, provider, key='toolbar', icon_key='icon', tooltip_key='tooltip',
                    combo_key='Combo', check_key='Check', type_key='type', label_key='Label', action_key='Action'):
-    controls = []
+    widgets = []
     if key not in config:
-        return None, controls
+        return None, widgets
 
     toolbar        = QtWidgets.QToolBar()
     toolbar_config = config[key]
-    for item1 in toolbar_config:
+    for i, item1 in enumerate(toolbar_config):
         item      = item1['item']
         title     = item.get('title', '')
-        name      = item.get('name', 'NoName')
+        name      = item.get('name', 'Item_%s' % i)
         item_type = item.get(type_key, 'Action')
         tooltip   = item.get(tooltip_key, None)
 
         if item.get('is_separator', False):
             toolbar.addSeparator()
         elif item_type == combo_key:
-            controls.append(QTAux.Combo(name, title, provider, None, toolbar, item))
+            widgets.append(QTAux.Combo(name, title, provider, None, toolbar, item))
         elif item_type == check_key:
-            controls.append(QTAux.CheckButton(name, title, provider, None, toolbar, tooltip))
+            widgets.append(QTAux.CheckButton(name, title, provider, None, toolbar, tooltip))
         elif item_type == label_key:
             QTAux.Label(name, title, provider, None, toolbar, align_left=False)
         elif item_type == action_key:
-            provider.set_control_value(name, title)
+            provider.set_value(name, title)
             action = QTAux.Action(name, title, provider, main_window, item, tooltip=tooltip)
             action.qt_action.triggered.connect(functools.partial(exec_action, provider,
                                                                  function_name=item.get('action', None)))
             toolbar.addAction(action.qt_action)
-            controls.append(action)
+            widgets.append(action)
         else:
             raise Exception('%s is not implemented in Toolbar' % item_type)
 
-    return toolbar, controls
+    return toolbar, widgets
 
 
 def create_status_bar(win_config, main_window, status_key='status_bar'):
     if not win_config.get(status_key, True):  # create a statusbar unless is explicitly forbidden
         return None
     statusbar = QtWidgets.QStatusBar(main_window)
     main_window.setStatusBar(statusbar)
@@ -1108,106 +1181,91 @@
 
     def add_increment(self, increment):
         if self.parent is None:
             return
         self.progress_bar.setValue(self.progress_bar.value()+increment)
 
 
-# Controls definition
-def add_controls_to_window(layout, layout_config, window):
-    controls_config = layout_config.get('controls', [])
-    return def_controls(controls_config, window.provider, layout)
-
-
-def def_controls(controls_definition, provider, layout):
-    controls = []
-    for control in controls_definition:
-        valid, c = def_control(control, provider, layout)
-        if valid:
-            controls.append(c)
-    return controls
-
-
-def def_control(control1, provider, layout, main_key='control'):
-    control = control1[main_key]
-    c_name  = control['name']
-    e_name  = external_name(control)
-    c_type  = control['type']
-    tooltip = control.get('tooltip', None)
-    action  = action_string(control)
-    value   = get_control_initial_value(c_name, control, provider)
+# Widgets definition
+def add_widgets_to_window(layout, layout_config, window):
+    widgets = layout_config.get('widgets', [])
+    return def_widgets(widgets, window.provider, layout)
+
+
+def def_widgets(widgets_definition, provider, layout):
+    widgets = [def_widget(widget, provider, layout) for widget in widgets_definition]
+    return widgets
+
+
+def def_widget(widget1, provider, layout, main_key='widget'):
+    widget  = widget1[main_key]
+    c_name  = widget['name']
+    e_name  = external_name(widget)
+    c_type  = widget['type']
+    tooltip = widget.get('tooltip', None)
+    action  = action_string(widget)
+    value   = get_widget_initial_value(c_name, widget, provider)
     # print('%s initial value: %s' % (c_name, value))
     if value is not None:
-        # value must be set before control creation, so it will appear the first time the control is displayed
-        provider.set_control_value(c_name, value)
+        # value must be set before widget creation, so it will appear the first time the widget is displayed
+        provider.set_value(c_name, value)
 
     if c_type == 'Slider':
-        result = True
-        qt_control = def_slider(c_name, e_name, provider, layout, control['parms'], action, tooltip=tooltip)
+        qt_widget = def_slider(c_name, e_name, provider, layout, widget['parms'], action, tooltip=tooltip)
     elif c_type == 'Combo':
-        result = True
-        qt_control = QTAux.Combo(c_name, e_name, provider, action, layout, control, tooltip=tooltip)
+        qt_widget = QTAux.Combo(c_name, e_name, provider, action, layout, widget, tooltip=tooltip)
     elif c_type == 'EnumCombo':
-        result     = True
-        enum       = eval(control['enum'])
-        qt_control = QTAux.EnumCombo(c_name, e_name, provider, enum, action, layout)
-        # qt_control = def_enum_combo(c_name, e_name, provider, layout, action, control)
+        enum       = eval(widget['enum'])
+        qt_widget = QTAux.EnumCombo(c_name, e_name, provider, enum, action, layout)
+        # qt_widget = def_enum_combo(c_name, e_name, provider, layout, action, widget)
     elif c_type == 'Button':
-        result = True
-        qt_control = def_button(c_name, e_name, provider, layout, action, control, tooltip=tooltip)
+        qt_widget = def_button(c_name, e_name, provider, layout, action, widget, tooltip=tooltip)
     elif c_type == 'Constant':
-        result = False
-        qt_control = def_constant(c_name, e_name, provider, layout, action)
+        qt_widget = def_constant(c_name, e_name, provider, layout, action)
     elif c_type == 'Check':
-        result = True
-        qt_control = QTAux.CheckButton(c_name, e_name, provider, action, layout, tooltip=tooltip)
+        qt_widget = QTAux.CheckButton(c_name, e_name, provider, action, layout, tooltip=tooltip)
     elif c_type in ['Text', 'Label']:
-        result = True
-        qt_control = QTAux.Label(c_name, e_name, provider, action, layout)
+        qt_widget = QTAux.Label(c_name, e_name, provider, action, layout)
     elif c_type == 'EditText':
-        result = True
-        qt_control = QTAux.EditText(c_name, e_name, provider, action, layout, tooltip=tooltip)
+        qt_widget = QTAux.EditText(c_name, e_name, provider, action, layout, tooltip=tooltip)
     elif c_type == 'EditNumber':
-        result = True
-        qt_control = QTAux.EditNumber(c_name, e_name, provider, action, layout)
+        qt_widget = QTAux.EditNumber(c_name, e_name, provider, action, layout)
     elif c_type == 'EditNumberSpin':
-        result = True
-        qt_control = QTAux.EditNumberSpin(c_name, e_name, provider, action, layout, control)
+        qt_widget = QTAux.EditNumberSpin(c_name, e_name, provider, action, layout, widget)
     elif c_type == 'ProgressBar':
-        result = True
-        qt_control = QTAux.ProgressBar(c_name, provider, action, layout)
+        qt_widget = QTAux.ProgressBar(c_name, provider, action, layout)
     else:
-        raise Exception('Control type %s not implemented' % c_type)
+        raise Exception('Widget type "%s" not implemented' % c_type)
 
-    qt_control.refresh_others = control.get('refresh_others', False)
+    qt_widget.refresh_others = widget.get('refresh_others', False)
 
-    return result, qt_control
+    return qt_widget
 
 
-def get_control_initial_value(c_name, control, provider, key_value='value'):
-    if key_value in control:
-        return control[key_value]
-    elif provider.control_has_value(c_name):
-        return provider.get_control_value(c_name)
+def get_widget_initial_value(c_name, widget, provider, key_value='value'):
+    if key_value in widget:
+        return widget[key_value]
+    elif provider.widget_has_value(c_name):
+        return provider.get_value(c_name)
     else:
         return None
 
 
 def def_slider(c_name, e_name, provider, layout, parms, action, tooltip=None):
     [min_e, max_e, scale_e] = parms
     min1   = get_def_value(min_e, provider)
     max1   = get_def_value(max_e, provider)
     scale1 = get_def_value(scale_e, provider)
     return QTAux.Slider(c_name, e_name, provider, min1, max1, action, layout, tooltip=tooltip, scale=scale1)
 
 
-def def_button(c_name, e_name, provider, layout, action, control, tooltip=None, def_width=30, def_length=100):
+def def_button(c_name, e_name, provider, layout, action, widget, tooltip=None, def_width=30, def_length=100):
     if action != '':
-        width  = control.get('width', def_width)
-        length = control.get('length', def_length)
+        width  = widget.get('width', def_width)
+        length = widget.get('length', def_length)
         return QTAux.Button(c_name, e_name, provider, action, layout, tooltip=tooltip, width=width, length=length)
     else:
         raise Exception('Invalid button definition, no action defined')
 
 
 def def_constant(c_name, e_name, provider, layout, action):
     # Only reason to have a constant on window is to exec an action
@@ -1236,16 +1294,16 @@
 
 def get_def_value(v, provider):
     # Note: provider is necessary so eval can use it
     string = QTAux.string_to_eval(v)
     return eval(string) if string is not None else v
 
 
-def action_string(control_def, action_key='action'):
-    return control_def.get(action_key, '')
+def action_string(widget_def, action_key='action'):
+    return widget_def.get(action_key, '')
 
 
 def exec_action(provider, function_name=None):
     # Note: provider is necessary so eval can use it
     if function_name is None:
         return
     full_function_name = 'provider.%s()' % function_name
```

### Comparing `windeklar-0.2.6/src/WinDeklar/graph_aux.py` & `windeklar-0.3.0/src/WinDeklar/graph_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/src/WinDeklar/points_box.py` & `windeklar-0.3.0/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/src/WinDeklar/record.py` & `windeklar-0.3.0/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/src/WinDeklar/signal_aux.py` & `windeklar-0.3.0/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/src/WinDeklar/test_animation.py` & `windeklar-0.3.0/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/src/WinDeklar/test_pyqt.py` & `windeklar-0.3.0/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/src/WinDeklar/view_animation.py` & `windeklar-0.3.0/src/WinDeklar/view_animation.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import WinDeklar.QTAux as QTAux
 import WinDeklar.WindowForm as WinForm
 import WinDeklar.graph_aux as ga
 
 
 class ExampleHost(WinForm.HostModel):
     """
-    Shows a two animated graphs
+    Shows two animated graphs
     """
 
     def __init__(self, function1=np.sin, function2=np.cos, color='Blue', y_bounds=(-1.2, 1.2)):
         # keys (names used in the yaml definition file)
         self.start_stop_key        = 'start_stop'
         self.start_stop_action_key = 'start_stop_action'
         self.graph1_key = 'graph1'
@@ -58,19 +58,19 @@
         """
         Logit to start/stop the graph with only one button (who changes its title depending on the graph is
         running or not_
         :return:
         """
         is_running = self.start_stop_animation()
         if is_running:
-            self.set_control_title(self.start_stop_key, 'Pause Animation')
-            self.set_control_title(self.start_stop_action_key, 'Pause Animation')
+            self.set_widget_title(self.start_stop_key, 'Pause Animation')
+            self.set_widget_title(self.start_stop_action_key, 'Pause Animation')
         else:
-            self.set_control_title(self.start_stop_key, 'Restart Animation')
-            self.set_control_title(self.start_stop_action_key, 'Restart Animation')
+            self.set_widget_title(self.start_stop_key, 'Restart Animation')
+            self.set_widget_title(self.start_stop_action_key, 'Restart Animation')
 
 
 if __name__ == '__main__':
     app = QTAux.def_app()
     provider = ExampleHost()        # class to handle the WinForm logic
     WinForm.run_winform(__file__, provider)
     sys.exit(app.exec_())
```

### Comparing `windeklar-0.2.6/src/WinDeklar/view_animation.yaml` & `windeklar-0.3.0/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/src/WinDeklar/view_example.py` & `windeklar-0.3.0/src/WinDeklar/view_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,50 +33,51 @@
         self.action_name        = 'Action'
         self.last_action_number = 0
         self.directory          = default_directory
         self.file_extension     = file_extension
         self.file_filter        = '*.%s' % self.file_extension
         self.file_name          = None
 
-        initial_values = {}  # used in case some control have an initial value programmatically
+        initial_values = {}  # used in case some control needs to have an initial value programmatically
         super(ExampleHost, self).__init__(initial_values=initial_values)
 
-    def control_changed(self, name, value):
+    def widget_changed(self, name, value):
         """
         Called when a control has changed it values
         :param name:
         :param value:
         :return:
         """
         if name == self.type_key:
             self.show_status_bar_msg('%s graph type chosen' % value)
 
     def update_view(self, figure, ax):
         """
         Update the figure
         Notes:
             - This method is called when any property changes or refresh() is used
-            - All form variables are in dict self.state
+            - All form variables are accessible by get_value
         :param figure:
         :param ax:
         :return:
         """
         if figure.name == self.graph1_key:
-            function_name = self.state.get(self.type_key, 'None')
+            function_name = self.get_value(self.type_key)
             points        = self.get_graph_points(function_name)
-            show_axis     = [True, True] if self.state.get(self.axis_key, True) else [False, False]
+            show_axis     = [True, True] if self.get_value(self.axis_key) else [False, False]
             ga.graph_points(ax, points, x_visible=show_axis[0], y_visible=show_axis[1],
-                            line_width=self.state.get(self.width_key, 1.0))
-            self.resize_figure(ax, points)
+                            line_width=self.get_value(self.width_key, default=1.0))
+            figure.resize_axis(points)
         elif figure.name == self.graph2_key:
-            number_of_points = int(self.state.get(self.points_key, 10))
+            number_of_points = int(self.get_value(self.points_key, default=10))
             p1 = [number_of_points, number_of_points]
             p2 = [0, 0]
             show_arrow(ax, p1, p2)
-            self.resize_figure(ax, [p1, p2])
+            figure.show_text([['points', number_of_points]], position=[1, number_of_points])
+            figure.resize_axis([p1, p2])
 
     def redraw(self):
         """
         Event defined in the yaml file to be called when button redraw is pressed
         :return:
         """
         self.refresh()
@@ -84,15 +85,15 @@
     def initialize(self):
         """
         Code to run when initializing the form
         In this case it is shown how to set visible (or not) a control
         :return:
         """
         # example of how to conditional show a control in the screen
-        control = self.get_control_by_name('just_text')
+        control = self.get_widget_by_name('just_text')
         control.set_visible(False)
 
     # actions
     def event_open_file(self):
         """
         Event defined in the yaml file to be called when File/Open is clicked
         :return:
@@ -116,15 +117,15 @@
             self.event_save_file_as()
         else:
             self.save_file(self.file_name, progress_bar=self.get_progress_bar())
 
     def change_action(self):
         self.last_action_number += 1
         value = '%s %s' % (self.action_name, self.last_action_number)
-        self.set_and_refresh_control(self.action_key, value)
+        self.set_and_refresh_widget(self.action_key, value)
 
     def on_mouse_move(self, event, ax):
         if event.xdata is None or event.ydata is None:
             return
         self.show_status_bar_msg('x:%.2f y:%.2f' % (event.xdata, event.ydata))
 
     # particular code
@@ -132,16 +133,16 @@
         """
         Example on how to use the progress bar
         :param file_name:
         :param progress_bar: use to give feedback about the opening process
         :return:
         """
         file = ya.get_yaml_file(file_name, must_exist=True, verbose=True)
-        self.state.update(file['state'])
-        print(self.state)
+        self.set_values(file['state'])
+        print(self._state)
         self.refresh()
 
         # just an example of how to use the ProgressBar, no actually needed in this case
         progress_bar_example(progress_bar, max_value=100, inc=20, sleep_time=0.2)
 
         msg = '%s opened' % file_name
         self.show_status_bar_msg(msg)
@@ -151,28 +152,28 @@
         Example on how to use the progress bar
         :param file_name:
         :param progress_bar: use to give feedback about the opening process
         :return:
         """
         record = rc.Record(file_name, dir=None, add_time_stamp=False)
         record.write_ln('version: 1')  # just to avoid warnings with editing in pycharm
-        record.write_group('state', self.state, level=0)
+        record.write_group('state', self._state, level=0)
 
         # just an example of how to use the ProgressBar, no actually needed in this case
         progress_bar_example(progress_bar, max_value=100, inc=20, sleep_time=0.2)
 
         msg = '%s saved' % file_name
         self.show_status_bar_msg(msg)
 
     def get_graph_points(self, function_name):
         """
         Returns the points (x,y) to be graphed depending on the graph type and number of points
         :return:
         """
-        number_of_points = int(self.state.get(self.points_key, 10))
+        number_of_points = int(self.get_value(self.points_key, default=10))
         points, msg      = ga.graph_points_for_many_functions(function_name, number_of_points)
         if points is None:
             self.show_status_bar_msg('%s not implemented' % function_name)
             points = []
         return points
```

### Comparing `windeklar-0.2.6/src/WinDeklar/view_example.yaml` & `windeklar-0.3.0/src/WinDeklar/view_example.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -58,60 +58,60 @@
         tooltip: Advance to last step
         # action: button_next_last
     - item:
         name:    action
         title:   Action
         type:    Action
         action:  change_action
-        tooltip: Click to change it
+        tooltip: Click to execute an action
 
   layout:       # defines the layout of the window
       - item:
-          name:    controls_and_figure
+          name:    widgets_and_figure
           type:    grid
           subtype: horizontal          # sub items will be added in the horizontal axis
-          desc:    panel is composed of two sides, the one at the left has controls, at the right a Figure to show a graph
+          desc:    panel is composed of two sides, the one at the left has widgets, at the right a Figure to show a graph
           layout:                      # an item can have layouts inside
             - item:
-                name:    controls
+                name:    widgets
                 type:    grid
                 subtype: vertical      # sub items will be added in the vertical axis
                 width:   300
-                controls:              # an item can have UI controls inside (like combo, slide, etc)
-                  - control:
+                widgets:              # an item can have UI widgets inside (like combo, slide, etc)
+                  - widget:
                       name:    graph_type         # internal name, used in the program file
                       title:   Graph Type         # title to be shown (use '' to not show)
                       type:    Combo              # this is a ComboBox
                       values:  [Sine, Cosine, Random, Other]  # valid values
                       value:   Random                         # initial value
-                      tooltip: Type of graph to show          # message to show when the mouse is over the control
-                  - control:
+                      tooltip: Type of graph to show          # message to show when the mouse is over the widget
+                  - widget:
                       name:    show_axis     # internal name (used in programs), if changed need to change program also
                       title:   Show Axis     # external name, can be changed without problem
-                      type:    Check         # type of control: Check, Slider, Button, Combo
+                      type:    Check         # type of widget: Check, Slider, Button, Combo
                       value:   True          # initial value
                       tooltip: Whether show axis values
-                  - control:
+                  - widget:
                       name:    points
                       title:   Number of points
                       type:    Slider
                       parms:   [2, 100, 1]      # [min_value, max_value, scale]
                       value:   20
-                  - control:
+                  - widget:
                       name:    line_width
                       title:   Line Width
                       type:    EditNumberSpin
                       parms:   {step: 1.0, maximum: 10}
                       value:   1.0
-                  - control:
+                  - widget:
                       name:    just_text
                       title:   ''  # null to avoid present it on the form
                       type:    Text
                       value:   Text
-                  - control:
+                  - widget:
                       name:    redraw
                       title:   Draw again
                       type:    Button
                       action:  redraw   # method to call
 
             - item:
                 name:    figures
@@ -127,10 +127,11 @@
                       x_axis:  {name: 'points'}
                       y_axis:  {name: 'output'}
                       view_size: [100, 10]
                   - item:
                       name:    graph2
                       type:    figure
                       title:   Draw an arc from origin to the number of points
+                      text_position: [2, 10]
                       desc:    a non graph example
                       view_size: [100, 10]
```

### Comparing `windeklar-0.2.6/src/WinDeklar/view_simple_graph.py` & `windeklar-0.3.0/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/src/WinDeklar/yaml_functions.py` & `windeklar-0.3.0/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/LICENSE` & `windeklar-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.6/README.md` & `windeklar-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Description
 A simple, declarative oriented framework to create WinForms in Python.
 
 While it can be used for all kinds of forms, it was created with the purpose of being applied in Robotics, where the need to visualize complex algorithms and, above all, observe the effect of parameter changes is very common.
 
-The forms are defined in a declarative way in an YAML (layouts, controls, toolbar, menus, etc.) and used in a Python program with just a few lines of code.
+The forms are defined in a declarative way in an YAML (layouts, widgets, toolbar, menus, etc.) and used in a Python program with just a few lines of code.
 
 # How to use it
 To create a WinForm it is necessary to create two files:
-* a declaration file (*.yaml) that define the WinForm (menu bar, toolbar, layouts, controls, etc.)
+* a declaration file (*.yaml) that define the WinForm (menu bar, toolbar, layouts, widgets, etc.)
 * a python file (with the same name) that handles all the WinForm logic (events, drawing, etc.)
 
 For a complete form see `view_example.yaml` to understand how the form is defined and `view_example.py` how it is used.
 
 If you run `python view_example.py` the form is: 
 
 <img width="997" alt="winform_example" src="https://github.com/njodal/WIndow_form/assets/28706901/ab02ce1f-9409-454d-8d95-e130fe6d77ed">
```

### Comparing `windeklar-0.2.6/pyproject.toml` & `windeklar-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.2.6"
+version = "0.3.0"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.2.6/PKG-INFO` & `windeklar-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.2.6
+Version: 0.3.0
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,19 +13,19 @@
 Description-Content-Type: text/markdown
 
 # Description
 A simple, declarative oriented framework to create WinForms in Python.
 
 While it can be used for all kinds of forms, it was created with the purpose of being applied in Robotics, where the need to visualize complex algorithms and, above all, observe the effect of parameter changes is very common.
 
-The forms are defined in a declarative way in an YAML (layouts, controls, toolbar, menus, etc.) and used in a Python program with just a few lines of code.
+The forms are defined in a declarative way in an YAML (layouts, widgets, toolbar, menus, etc.) and used in a Python program with just a few lines of code.
 
 # How to use it
 To create a WinForm it is necessary to create two files:
-* a declaration file (*.yaml) that define the WinForm (menu bar, toolbar, layouts, controls, etc.)
+* a declaration file (*.yaml) that define the WinForm (menu bar, toolbar, layouts, widgets, etc.)
 * a python file (with the same name) that handles all the WinForm logic (events, drawing, etc.)
 
 For a complete form see `view_example.yaml` to understand how the form is defined and `view_example.py` how it is used.
 
 If you run `python view_example.py` the form is: 
 
 <img width="997" alt="winform_example" src="https://github.com/njodal/WIndow_form/assets/28706901/ab02ce1f-9409-454d-8d95-e130fe6d77ed">
```

