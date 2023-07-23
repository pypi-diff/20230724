# Comparing `tmp/pih-1.46231.tar.gz` & `tmp/pih-1.47001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.46231.tar", last modified: Thu Jul 13 05:06:15 2023, max compression
+gzip compressed data, was "pih-1.47001.tar", last modified: Sun Jul 23 22:34:30 2023, max compression
```

## Comparing `pih-1.46231.tar` & `pih-1.47001.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 05:06:15.683650 pih-1.46231/
--rw-rw-rw-   0        0        0      261 2023-07-13 05:06:15.667995 pih-1.46231/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 05:06:15.324249 pih-1.46231/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.46231/pih/__init__.py
--rw-rw-rw-   0        0        0    19907 2023-07-13 01:30:06.000000 pih-1.46231/pih/collection.py
--rw-rw-rw-   0        0        0    56312 2023-07-13 04:47:44.000000 pih-1.46231/pih/console_api.py
--rw-rw-rw-   0        0        0   106507 2023-07-13 03:02:11.000000 pih-1.46231/pih/const.py
--rw-rw-rw-   0        0        0   303620 2023-07-13 05:05:09.000000 pih-1.46231/pih/pih.py
--rw-rw-rw-   0        0        0    24689 2023-07-09 01:49:27.000000 pih-1.46231/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.46231/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.46231/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.46231/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6368 2023-07-11 03:24:37.000000 pih-1.46231/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.46231/pih/service_example.py
--rw-rw-rw-   0        0        0    37523 2023-07-12 23:19:16.000000 pih-1.46231/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.46231/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-13 05:06:15.621121 pih-1.46231/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-13 05:06:13.000000 pih-1.46231/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-13 05:06:14.000000 pih-1.46231/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 05:06:13.000000 pih-1.46231/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-13 05:06:13.000000 pih-1.46231/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-13 05:06:13.000000 pih-1.46231/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-07-13 05:05:53.000000 pih-1.46231/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-13 05:06:15.683650 pih-1.46231/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-23 22:34:31.026589 pih-1.47001/
+-rw-rw-rw-   0        0        0      261 2023-07-23 22:34:31.042215 pih-1.47001/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-23 22:34:30.760968 pih-1.47001/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47001/pih/__init__.py
+-rw-rw-rw-   0        0        0    20299 2023-07-23 12:16:34.000000 pih-1.47001/pih/collection.py
+-rw-rw-rw-   0        0        0    59317 2023-07-23 13:04:31.000000 pih-1.47001/pih/console_api.py
+-rw-rw-rw-   0        0        0   108878 2023-07-23 12:45:02.000000 pih-1.47001/pih/const.py
+-rw-rw-rw-   0        0        0   307138 2023-07-23 22:34:04.000000 pih-1.47001/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-17 14:57:37.000000 pih-1.47001/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47001/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47001/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47001/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6403 2023-07-20 06:09:44.000000 pih-1.47001/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47001/pih/service_example.py
+-rw-rw-rw-   0        0        0    37894 2023-07-20 06:21:53.000000 pih-1.47001/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47001/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:34:30.995344 pih-1.47001/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-23 22:34:28.000000 pih-1.47001/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-23 22:34:29.000000 pih-1.47001/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-23 22:34:28.000000 pih-1.47001/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-23 22:34:28.000000 pih-1.47001/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-23 22:34:28.000000 pih-1.47001/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-07-14 01:37:00.000000 pih-1.47001/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 22:34:31.042215 pih-1.47001/setup.cfg
```

### Comparing `pih-1.46231/pih/collection.py` & `pih-1.47001/pih/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from datetime import datetime
+from datetime import datetime, timedelta
 from enum import Enum
 from typing import Any, Generic, Tuple, TypeVar, List
 from collections import namedtuple
 
 Rect = namedtuple("Rect", ["left", "top", "width", "height"])
 
 
@@ -187,44 +187,50 @@
     inaccessibility_check_values: Tuple[int] = (2, 20, 15)
 
 @dataclass
 class SiteResourceDescription(ResourceDescription):
     check_certificate_status: bool = False
     check_free_space_status: bool = False
     driver_name: str | None = None
+    internal: bool = False
    
 
 @dataclass
 class ResourceStatus(ResourceDescription):
     accessable: bool | None = None
     inaccessibility_counter: int = 0
 
 @dataclass
 class WSResourceStatus(ResourceStatus):
-    
     pass
 
 @dataclass
+class ServerResourceStatus(ResourceStatus):
+    pass
+
+
+@dataclass
 class SiteResourceStatus(ResourceStatus, SiteResourceDescription):
     certificate_status: str | None = None
     free_space_status: str | None = None
 
 @dataclass
-class MarkBase:
+class MarkPerson:
     FullName: str | None = None
     TabNumber: str | None = None
 
 
 @dataclass
-class MarkSimple(MarkBase):
+class MarkPersonDivision(MarkPerson):
     DivisionName: str | None = None
+    DivisionID: int | None = None
 
 
 @dataclass
-class TemporaryMark(MarkBase):
+class TemporaryMark(MarkPerson):
     OwnerTabNumber: str | None = None
 
 
 @dataclass
 class PolibasePersonBase:
     pin: int | None = None
     FullName: str | None = None
@@ -346,32 +352,32 @@
     grade: int | None = None
     message: str | None = None
     informationWay: int | None = None
     feedbackCallStatus: int | None = None
 
 
 @dataclass
-class Mark(MarkSimple):
+class Mark(MarkPersonDivision):
     pID: int | None = None
     mID: int | None = None
     GroupName: str | None = None
     GroupID: int | None = None
     Comment: str | None = None
     telephoneNumber: str | None = None
     type: int | None = None
 
 
 @dataclass
-class MarkDivision:
+class PersonDivision:
     id: int | None = None
     name: str | None = None
 
 
 @dataclass
-class TimeTrackingEntity(MarkSimple):
+class TimeTrackingEntity(MarkPersonDivision):
     TimeVal: str | None = None
     Mode: int | None = None
 
 
 @dataclass
 class TimeTrackingResultByDate:
     date: str | None = None
@@ -515,15 +521,15 @@
     title: str | None = None
     text: str | None = None
     id: str | None = None
     images: list[str] | None = None
 
 @dataclass
 class InventoryReportItem:
-    name: str | None = None
+    name: str | int | None = None
     inventory_number: str | None = None
     row: str | None = None
     quantity: int | None = None
     name_column: int | None = None
     inventory_number_column: int | None = None
     quantity_column: int | None = None
 
@@ -543,14 +549,18 @@
     free_space: int | None = None
     size: int | None = None
 
 @dataclass
 class TimeSeriesStatistics:
     count: int = 0
     values: list[datetime] | None = None
+    distance: list[timedelta] | None = None
+    min: int | None = None
+    max: int | None = None
+    avg: int | None = None
 
 @dataclass
 class PrinterReport(PrinterStatus):
     name: str | None = None
     model: str | None = None
     serial: int | None = None
     adminDescription: str | None = None
@@ -711,14 +721,18 @@
     auto_init: bool = True
 
 
 @dataclass
 class IntStorageValue(StorageValue):
     default_value: int = 0
 
+@dataclass
+class IntStorageValueWithMin(IntStorageValue):
+    min_value: int = 0
+
 
 @dataclass
 class FloatStorageValue(StorageValue):
     default_value: float
 
 @dataclass
 class BoolStorageValue(StorageValue):
```

### Comparing `pih-1.46231/pih/console_api.py` & `pih-1.47001/pih/console_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 from datetime import datetime
 import os
 import re
 
 pih_exists = importlib.util.find_spec("pih.pih") is not None
 if not pih_exists:
     sys.path.append("//pih/facade")
-from pih.const import CONST, MarkType, PASSWORD, USER_PROPERTIES, FIELD_COLLECTION, PasswordSettings, CheckableSections, HOSTS, AD, PATHS, FILE
+from pih.const import (MarkType, PASSWORD, PasswordSettings, 
+                       CheckableSections, FILE)
 from pih import PIH, A, NotFound, ActionValue, ActionStack, Input, Output, Session, while_not_do
 from pih.collection import (Mark, User, FullName, 
-                            MarkDivision, UserBase, LoginPasswordPair, 
+                            PersonDivision, UserBase, LoginPasswordPair, 
                             MarkGroup, Result, FieldItemList,
                             WorkstationDescription, ResourceStatus, SiteResourceStatus,
                             CTIndicationsValue, Workstation, RobocopyJobStatus, 
-                            ChillerIndicationsValueContainer, PrinterReport, DiskStatistics)
+                            ChillerIndicationsValueContainer, PrinterReport, DiskStatistics,
+                            IntStorageValue)
+from pih.tools import j
 from pih import A
 
 class ConsoleAppsApi:
 
     LINE: str = "........................................................"
 
     def __init__(self, pih: PIH = None):
@@ -42,15 +45,15 @@
         self.description: str = None
         self.use_template_user: bool
         self.need_to_create_mark: bool = None
 
     def create_qr_code_for_mobile_helper_command(self, command: str | None = None, title: str | None = None, show_result: bool = True) -> str | None:
         command = command or self.input.input("Введите название команды")
         title = title or self.input.input("Введите заголовок")
-        result = A.A_QR.for_mobile_helper_command(command, title, os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, A.PTH.replace_prohibited_symbols_from_path_with_symbol(A.PTH.add_extension(command, FILE.EXTENSION.PNG))), 56)
+        result = A.A_QR.for_mobile_helper_command(command, title, os.path.join(A.PTH.MOBILE_HELPER.QR_CODE_FOLDER, A.PTH.replace_prohibited_symbols_from_path_with_symbol(A.PTH.add_extension(command, FILE.EXTENSION.PNG))), 56)
         qr_code_image_path: str = A.PTH_QR.mobile_helper_command(command)
         if show_result:
             if result:
                 self.output.good(
                     f"Файл qr кода {self.bold(title)} создан.\nПуть к файлу:\n{self.bold(qr_code_image_path)}\n")
             else:
                 self.output.error("qr код не был создан")
@@ -82,130 +85,167 @@
             else:
                 self.output.write_line("Информация о дисках:\n")
                 for disk_statistics in disk_statistics_list:
                     self.output.write_line(f" {A.CT_V.BULLET} {self.bold(disk_statistics.name)}: {A.D_F.size(disk_statistics.free_space)} из {A.D_F.size(disk_statistics.size)}")
         else:
             self.output.error("Хост не доступен или не найден")
 
+    @property
+    def is_mobile(self) -> bool:
+        return self.session.name == "mobile"
+
     def resources_and_indications_check(self, checkable_section_list: list[CheckableSections], ask_for_update_before: bool = False, force_update: bool = False, all: bool = False) -> None:
-        if CheckableSections.RESOURCES in checkable_section_list or CheckableSections.WS in checkable_section_list:
-            def label_function(resource: ResourceStatus, index: int) -> str:
-                result: list[str] = [] 
-                accessable: bool = resource.accessable
-                status: str = A.D_F.yes_no(accessable, True)
-                result.append(" ".join((status, self.bold(self.output.blue_str(
-                    resource.name)))))
-                if isinstance(resource, SiteResourceStatus):
-                    if resource.check_free_space_status:
-                        free_space_result_list: str = resource.free_space_status.split(" ")
-                        result.append(f"      Cвободное место: {free_space_result_list[0]} ({free_space_result_list[1]})")
-                    if resource.check_certificate_status:
-                        result.append(f"      Сертификат доступен до: {resource.certificate_status}")
-                return A.CT.NEW_LINE.join(result)
-            force_update = force_update or (ask_for_update_before and self.input.yes_no(
-                "Обновить перед получением"))
-            if force_update:
+        with self.output.make_indent(1):
+            if CheckableSections.RESOURCES in checkable_section_list or (
+                CheckableSections.WS in checkable_section_list\
+                or CheckableSections.SERVERS in checkable_section_list):
+                def label_function(resource: ResourceStatus, index: int) -> str:
+                    result: list[str] = [] 
+                    accessable: bool = resource.accessable
+                    status: str = A.D_F.yes_no(accessable, True)
+                    result.append(" ".join((status, self.bold(self.output.blue_str(
+                        resource.name)))))
+                    if isinstance(resource, SiteResourceStatus):
+                        if resource.check_free_space_status:
+                            free_space_result_list: str = resource.free_space_status.split(" ")
+                            result.append(f"      Cвободное место: {free_space_result_list[0]} ({free_space_result_list[1]})")
+                        if resource.check_certificate_status:
+                            result.append(f"      Сертификат доступен до: {resource.certificate_status}")
+                    return A.CT.NEW_LINE.join(result)
+                force_update = force_update or (ask_for_update_before and self.input.yes_no(
+                    "Обновить перед получением"))
+                if force_update:
+                    self.output.write_line(
+                        self.italic(f"{self.get_formatted_given_name()}, ожидайте получение результата..."))
+                for checkable_section in [CheckableSections.RESOURCES, CheckableSections.WS, CheckableSections.SERVERS]:
+                    if checkable_section in checkable_section_list:
+                        if self.is_mobile:
+                            self.output.new_line()
+                        if all:
+                            self.output.write_line(" ".join((A.CT_V.BULLET, self.bold(A.D.check(checkable_section == CheckableSections.RESOURCES, "Основные ресурсы", A.D.check(checkable_section == CheckableSections.WS, "Наблюдаемые компьютеры", "Серверы"))))))
+                        with self.output.make_indent(2, True):
+                            self.output.write_result(A.R_R.get_status_list([checkable_section], force_update, all if len(checkable_section_list) == 1 and CheckableSections.WS in checkable_section_list else False), False, label_function=label_function, separated_result_item=self.is_mobile)
+            if CheckableSections.INDICATIONS in checkable_section_list:
+                #self.output.separated_line()
+                #self.output.write_line(f"Показания доступны по адрессу:\n{self.bold('http://indications')}, если заходить с рабочего компьютера\nили\n{self.bold('http://192.168.100.138')}, если заходить с мобильного телефона, подключенного к корпоративной wifi сети")
+                if self.is_mobile:
+                    self.output.new_line()
+                self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в помещении КТ"))
+                with self.output.make_indent(2, True):
+                    self.output.write_result(A.R_I.last_ct_value_containers(True))
+                self.output.separated_line()
+                self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в техническом помещении МРТ"))
+                chiller_indications_value_container_result: Result[list[ChillerIndicationsValueContainer]] = A.R_I.last_chiller_value_containers(True)
+                chiller_indications_value_container: ChillerIndicationsValueContainer = A.R.get_first_item(chiller_indications_value_container_result)
+                path: str = A.PTH_I.CHILLER_DATA_IMAGE_LAST
+                modification_timstamp: float = os.path.getmtime(path)
+                file_creating_datetime: datetime | None = datetime.fromtimestamp(modification_timstamp if modification_timstamp > 0 else os.path.getctime(path))
+                with self.output.make_indent(2, True):
+                    self.output.write_result(chiller_indications_value_container_result, title="Показания чиллера\n" if A.D_C.INDICATIONS.chiller_value_actual(chiller_indications_value_container) else f"{self.bold('Внимание!')}: Показания чиллера неактуальны\n", separated_result_item=False)
+                    self.output.write_image(f"Изображение дисплея чиллера\nВремя снятия: {A.D_F.datetime(file_creating_datetime)}", A.D_CO.file_to_base64(A.PTH_I.CHILLER_DATA_IMAGE_LAST_RESULT))
+            if CheckableSections.MATERIALIZED_RESOURCES in checkable_section_list:
+                if self.is_mobile:
+                    self.output.new_line()
+                self.output.separated_line()
                 self.output.write_line(
-                    self.italic(f"{self.get_formatted_given_name()}, ожидайте получение результата..."))
-            for checkable_section in [CheckableSections.RESOURCES, CheckableSections.WS]:
-                if checkable_section in checkable_section_list:
+                    self.bold(f"{A.CT_V.BULLET} Материальные ресурсы:"))
+                with self.output.make_indent(2, True):
+                    for resource_type in A.CT_MR.TYPES:
+                        self.output.write_line(f"{A.CT_V.BULLET} {self.bold(A.D.get(resource_type).description)}")
+                        with self.output.make_indent(2, True):
+                            self.output.write_line(j(("\nКоличество: ", str(A.D_MR.get_count(resource_type)))))
+                            self.output.write_line(A.D_F.statistics(resource_type))
+            if CheckableSections.VALENTA in checkable_section_list:
+                scanned_file_path_list: list[str] = A.PTH.get_file_list_by_directory_info(
+                    A.PTH.WS_816_SCAN.VALUE)
+                count: int = len(scanned_file_path_list)
+                if self.is_mobile:
                     self.output.new_line()
-                    if all:
-                        self.output.write_line(self.bold(A.CT_V.BULLET + (" Основные ресурсы" if checkable_section == CheckableSections.RESOURCES else " Наблюдаемые компьютеры")))
-                    with self.output.make_indent(2):
-                        self.output.write_result(A.R_R.get_status_list([checkable_section], force_update, all if len(checkable_section_list) == 1 and CheckableSections.WS in checkable_section_list else False), False, label_function=label_function, separated_result_item=True)
-        if CheckableSections.INDICATIONS in checkable_section_list:
-            #self.output.separated_line()
-            #self.output.write_line(f"Показания доступны по адрессу:\n{self.bold('http://indications')}, если заходить с рабочего компьютера\nили\n{self.bold('http://192.168.100.138')}, если заходить с мобильного телефона, подключенного к корпоративной wifi сети")
-            self.output.new_line()
-            self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в помещении КТ"))
-            with self.output.make_indent(2):
-                self.output.write_result(A.R_I.last_ct_value_containers(True))
-            self.output.separated_line()
-            self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в техническом помещении МРТ"))
-            chiller_indications_value_container_result: Result[list[ChillerIndicationsValueContainer]] = A.R_I.last_chiller_value_containers(True)
-            chiller_indications_value_container: ChillerIndicationsValueContainer = A.R.get_first_element(chiller_indications_value_container_result)
-            path: str = A.PTH_I.CHILLER_DATA_IMAGE_LAST
-            modification_timstamp: float = os.path.getmtime(path)
-            modification_datetime: datetime | None = datetime.fromtimestamp(modification_timstamp if modification_timstamp > 0 else os.path.getctime(path))
-            with self.output.make_indent(2):
-                self.output.write_result(chiller_indications_value_container_result, title="Показания чиллера\n" if A.D_C.INDICATIONS.chiller_value_actual(chiller_indications_value_container) else f"{self.bold('Внимание!')}: Показания чиллера неактуальны\n", separated_result_item=False)
-                self.output.write_image(f"Изображение дисплея чиллера\nВремя снятия: {A.D_F.datetime(modification_datetime)}", A.D_CO.file_to_base64(A.PTH_I.CHILLER_DATA_IMAGE_LAST_RESULT))
-        if CheckableSections.VALENTA in checkable_section_list:
-            count: int = len(A.PTH.get_file_list_by_directory_info(A.PTH.WS_816_SCAN.VALUE))
-            self.output.new_line()
-            self.output.write_line(
-                self.bold(f"{A.CT_V.BULLET} Новые исследования в Валенте: " + ("Нет" if count == 0 else f"Да ({count})")))
-        if CheckableSections.SERVERS in checkable_section_list:
-            self.output.new_line()
-            self.output.write_line(self.bold(f"{A.CT_V.BULLET} Доступность серверов"))
-            with self.output.make_indent(2):
-                A.R.every(A.R_SRVS.all_description(), lambda server: self.output.write_line(" " .join((A.D_F.yes_no(A.C_R.accessibility_by_ping(server.name, count=1), True), self.bold(server.name)))))
-        if CheckableSections.PRINTERS in checkable_section_list:
-            self.output.new_line()
-            self.output.separated_line()
-            self.output.write_line(
-                self.bold(f"{A.CT_V.BULLET} Отчет по принтерам"))
-            printer_report_list: list[PrinterReport] = A.R_PR.report(send_to_log=False).data
-            for printer_report in printer_report_list:
                 self.output.separated_line()
-                with self.output.make_indent(2):
-                    self.output.write_line(A.D_F.printer_report(printer_report, self.bold))     
-        if not all:
-            if CheckableSections.BACKUPS in checkable_section_list:
-                robocopy_job_status_list: Result[list[RobocopyJobStatus]] = A.R_B.robocopy_job_status_list()
-                sort_by_status: bool = self.input.yes_no("Сортировать по статусу", no_label=f"{self.bold(f'Сортировать по дате выполнения - {A.CT_V.NUMBER_SYMBOLS[0]}')}")
-                A.R.sort(robocopy_job_status_list, (lambda item: item.last_status or max(A.CT_RBK.STATUS_CODE.keys())) if sort_by_status else lambda item: datetime.fromtimestamp(0) if A.D_C.empty(item.last_created) else A.D.datetime_from_string(item.last_created), sort_by_status)
-                def job_status_item_label_function(job_status: RobocopyJobStatus, index: int) -> str:
-                    name: str = job_status.name
-                    source: str = job_status.source
-                    destination: str = job_status.destination 
-                    status: int | None = None
-                    date: str | None = None
-                    if job_status.active:
-                        date = "выполняется"
+                self.output.write_line(
+                    self.bold(f"{A.CT_V.BULLET} Новые исследования в Валенте: " + ("Нет" if count == 0 else f"Да ({count})")))    
+                if count > 0:
+                    if self.input.yes_no("Показать отсканированные изображения"):
+                        for scanned_file_path in scanned_file_path_list:
+                            self.output.write_image(j(("Дата создания файла: ", A.D_F.datetime(datetime.fromtimestamp(os.path.getctime(scanned_file_path))))),
+                                A.D_CO.file_to_base64(scanned_file_path))
+                    if self.input.yes_no("Синхронизировать Валенту"):
+                        A.A_ACT.was_done(A.CT_ACT.VALENTA_SYNCHRONIZATION, self.session.user)
+            if CheckableSections.PRINTERS in checkable_section_list:
+                def printer_report(printer_report: PrinterReport) -> str:
+                    report_list: list[str] = []
+                    admin_description_list: list[str] = ("" or printer_report.adminDescription).split(",")
+                    name: str = printer_report.ip.split('.')[0]
+                    report_list.append(f"{self.bold('Модель')}: {printer_report.model}\n{self.bold('Название')}: {name}\n{self.bold('Описание')}: {printer_report.description}")
+                    if printer_report.name != -401 and "infoless" not in admin_description_list:   
+                        for item in (("Тонер", printer_report.get_toner), None if "drumless" in admin_description_list else ("Драм-юнит", printer_report.get_drum)):
+                            if A.D.is_not_none(item):
+                                report_list.append(f" {A.CT_V.BULLET} {self.bold(item[0])}")
+                                report_list += [f"   {self.bold(color.upper())}: %d%%" % item[1](color) for color in (["k"] if "bw" in admin_description_list else ["c", "m", "y", "k"])]
                     else:
-                        if job_status.last_created is not None:
-                            date = f"{A.D_F.datetime(job_status.last_created)}"
-                        status = job_status.last_status
-                    variants: list[str] = ["--" if status is None else self.bold(str(status)), "--" if A.D_C.empty(date) else self.bold(date)]
-                    return "".join([f" {A.CT_V.BULLET} ", variants[not sort_by_status], ": ", variants[sort_by_status], "".join([ "\n   ", name, ": ", source, A.CT_V.ARROW, destination])])
-                variants: list[str] = [self.bold("Статус"), self.bold("Дата выполнения")]
-                self.output.write_result(
-                    robocopy_job_status_list, False, label_function=job_status_item_label_function, separated_result_item=False, title="".join([f" {A.CT_V.BULLET} ", variants[not sort_by_status], ": ", variants[sort_by_status], "\n", "   Название Robocopy-задания", f"\n{ConsoleAppsApi.LINE}"]))
+                        report_list.append(f"Принтер {A.D.if_check(printer_report.accessable, '', 'не ')}доступен")
+                    return "\n".join(report_list)
+                if self.is_mobile:
+                    self.output.new_line()
+                self.output.separated_line()
+                self.output.write_line(
+                    self.bold(f"{A.CT_V.BULLET} Отчет по принтерам"))
+                printer_report_list: list[PrinterReport] = A.R_PR.report().data
+                for printer_report_item in printer_report_list:
+                    self.output.separated_line()
+                    with self.output.make_indent(2, True):
+                        self.output.write_line(printer_report(printer_report_item))
+            if not all:
+                if CheckableSections.BACKUPS in checkable_section_list:
+                    robocopy_job_status_list: Result[list[RobocopyJobStatus]] = A.R_B.robocopy_job_status_list()
+                    sort_by_status: bool = self.input.yes_no("Сортировать по статусу", no_label=f"{self.bold(f'Сортировать по дате выполнения - {A.CT_V.NUMBER_SYMBOLS[0]}')}")
+                    A.R.sort(robocopy_job_status_list, (lambda item: item.last_status or max(A.CT_RBK.STATUS_CODE.keys())) if sort_by_status else lambda item: datetime.fromtimestamp(0) if A.D_C.empty(item.last_created) else A.D.datetime_from_string(item.last_created), sort_by_status)
+                    def job_status_item_label_function(job_status: RobocopyJobStatus, index: int) -> str:
+                        name: str = job_status.name
+                        source: str = job_status.source
+                        destination: str = job_status.destination 
+                        status: int | None = None
+                        date: str | None = None
+                        if job_status.active:
+                            date = "выполняется"
+                        else:
+                            if job_status.last_created is not None:
+                                date = f"{A.D_F.datetime(job_status.last_created)}"
+                            status = job_status.last_status
+                        variants: list[str] = ["--" if status is None else self.bold(str(status)), "--" if A.D_C.empty(date) else self.bold(date)]
+                        return "".join([f" {A.CT_V.BULLET} ", variants[not sort_by_status], ": ", variants[sort_by_status], "".join([ "\n   ", name, ": ", source, A.CT_V.ARROW, destination])])
+                    variants: list[str] = [self.bold("Статус"), self.bold("Дата выполнения")]
+                    self.output.write_result(
+                        robocopy_job_status_list, False, label_function=job_status_item_label_function, separated_result_item=False, title="".join([f" {A.CT_V.BULLET} ", variants[not sort_by_status], ": ", variants[sort_by_status], "\n", "   Название Robocopy-задания", f"\n{ConsoleAppsApi.LINE}"]))
 
-    def polibase_restart(self, forced: bool = False) -> None:
-        if self.input.yes_no("Перезапустить"):
+    def polibase_restart(self) -> None:
+        if self.input.yes_no("Перезапустить сервер Polibase"):
             check_word: str = A.CT_P.NAME
             test: bool = not (check_word == self.input.input(
                 f"Введите контрольное слово: {self.bold(check_word)}"))
-            if not test and A.C_R.polibase_accessibility(True) and not forced:
-                self.output.error(
-                    "Перезапуск Polibase: перезапуск невозможен - сервер доступен")
-            else:
-                notify: bool = test or self.input.yes_no("Уведомить пользователей", True)
-                title: str = f"Перезапуск Polibase{' test' if test else ''}"
-                polibase_host: str = HOSTS.POLIBASE_TEST.NAME if test else HOSTS.POLIBASE.NAME
-                self.output.write_line(A.L.it(
-                    f"{title}: Начат процесс закрытия программы Polibase на компьютерах."))
-                A.A_P.client_program_close_for_all(notify, None, test)
-                self.output.new_line()
-                self.output.write_line(A.L.it(
-                    f"{title}: Начат процесс перезагрузки сервера Polibase."))
-                A.A_P.restart(test)
-                while_not_do(lambda: not A.C_R.accessibility_by_ping(
-                    polibase_host), sleep_time=5)
-                self.output.new_line()
-                self.output.write_line(A.L.it(
-                     f"{title}: Начат процесс загрузки сервера Polibase."))
-                while_not_do(lambda: A.C_R.accessibility_by_ping(polibase_host), sleep_time=5)
-                self.output.new_line()
-                A.E.wait_server_start(polibase_host)
-                self.output.write_line(A.L.it(f"{title}: Завершен процесс загрузки сервера Polibase."))
-                A.ME_P.notify_about_polibase_restarted(test)
+            notify: bool = test or self.input.yes_no("Уведомить пользователей", True)
+            title: str = f"Перезапуск Polibase{' test' if test else ''}"
+            polibase_host: str = A.CT_H.POLIBASE_TEST.NAME if test else A.CT_H.POLIBASE.NAME
+            self.output.write_line(A.L.it(
+                f"{title}: Начат процесс закрытия программы Polibase на компьютерах."))
+            A.A_P.client_program_close_for_all(notify, None, test)
+            self.output.new_line()
+            self.output.write_line(A.L.it(
+                f"{title}: Начат процесс перезагрузки сервера Polibase."))
+            A.A_P.restart(test)
+            while_not_do(lambda: not A.C_R.accessibility_by_ping(
+                polibase_host), sleep_time=5)
+            self.output.new_line()
+            self.output.write_line(A.L.it(
+                    f"{title}: Начат процесс загрузки сервера Polibase."))
+            while_not_do(lambda: A.C_R.accessibility_by_ping(polibase_host), sleep_time=5)
+            self.output.new_line()
+            A.E.wait_server_start(polibase_host)
+            self.output.write_line(A.L.it(f"{title}: Завершен процесс загрузки сервера Polibase."))
+            A.ME_P.notify_about_polibase_restarted(test)
 
     def polibase_client_program_close(self, search_value: str | None = None, for_all: bool = False) -> None:
         if for_all:
             check_word: str = A.CT_P.NAME
             test: bool = not (check_word == (search_value or self.input.input(
             f"Введите контрольное слово - {self.bold(check_word)}")))
             A.A_P.client_program_close_for_all(True, self.input.input("Введите сообщение для пользователей Polibase"), test) 
@@ -216,25 +256,25 @@
                     if A.A_P.client_program_close_for_workstation(workstation):
                         self.output.good(f"Программа Polibase закрыта на компьютере {workstation.name}")
                 A.R.every(workstation_list, every_action)
             except NotFound as error:
                 self.output.error(error.get_details())
                 search_value = None
 
-    def process_kill(self, host_name: str, process_name: str) -> None:
+    def process_kill(self, host_name: str | None, process_name: str | None) -> None:
         try:
             workstation_list: Result[list[Workstation]] = A.R_WS.by_any(host_name or self.input.input("Введите запрос для поиска компьютера"))
             def every_action(workstation: Workstation, process_name: str) -> None:
                 process_value: int | str = process_name
                 try:
                     process_value = int(process_value)
                 except ValueError:
                     pass
                 if A.A_WS.kill_process(process_value, workstation.name):
-                    self.output.good(A.D.if_check(isinstance(process_value, str), f"Процесс с именем \"{process_value}\"", f"Программа с идентификационным номером {process_value}") + f"закрыта на компьютере {workstation.name}")
+                    self.output.good(A.D.if_check(isinstance(process_value, str), f"Процесс с именем \"{process_value}\"", f"Программа с идентификационным номером {process_value}") + f" закрыта на компьютере {workstation.name}")
                 else:
                     self.output.error("Процесс не найден")
             A.R.every(workstation_list, lambda workstation: every_action(workstation, process_name or self.input.input("Введите название процесса или его PID")))
         except NotFound as error:
             self.output.error(error.get_details())
             host_name = None
 
@@ -244,42 +284,42 @@
         return self.pih.output
 
     @property
     def input(self) -> Input:
         return self.pih.input
 
     def send_whatsapp_message(self, telephone_number: str, message: str) -> bool:
-        return A.ME_WH_W.send(telephone_number, message, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.IT)
+        return A.ME_WH_W.send(telephone_number, message, A.CT_ME_WH_W.PROFILE.IT)
 
     def mark_find(self, value: str | None = None) -> None:
         self.output.mark.by_any(value or self.input.mark.any())
 
     def arg(self, index: int = 0, default_value: Any = None) -> Any:
         return self.session.arg(index, default_value)
 
     def register_ct_indications(self) -> None:
         text: str = f"число, которое может содержать дробную часть разделенную {self.bold('точкой')} или {self.bold('запятой')}"
         number_format_notification_text: str = f"- {self.italic(text)}"
         def float_check_function(value: str | None, show_error: bool = True) -> str | None:
             result: float | None = None
             if value is not None:
-                result = A.D_E.float(value)
+                result = A.D_Ex.float(value)
             if show_error and result is None:
                 self.output.error(
                     f"Введите {self.bold('число')} {number_format_notification_text}")
             return None if result is None else str(result)
         temperature: float = float_check_function(self.arg(), False) or self.input.input(
             f"Введите значение {self.bold('температуры')} {number_format_notification_text}", check_function=float_check_function)
         humidity: float = float_check_function(self.arg(1), False) or self.input.input(
             f"Введите значение {self.bold('влажности')} {number_format_notification_text}", check_function=float_check_function)
         indications_value: CTIndicationsValue = CTIndicationsValue(temperature, humidity)
         if A.A_I_CT.register(indications_value):
-            with self.output.send_to_group(CONST.MESSAGE.WHATSAPP.GROUP.CT_INDICATIONS):
+            with self.output.send_to_group(A.CT_ME_WH.GROUP.CT_INDICATIONS):
                 self.output.write_result(
-                    Result(FIELD_COLLECTION.INDICATIONS.CT_VALUE, indications_value), title=f"{self.get_formatted_given_name()}, отправил следующие показания в помещение КТ:")
+                    Result(A.CT_FC.INDICATIONS.CT_VALUE, indications_value), title=f"{self.get_formatted_given_name()}, отправил следующие показания в помещение КТ:")
             self.output.good("Спасибо, показания отправлены")
 
     def find_free_mark(self, value: str = None) -> None:
         self.output.mark.result(A.R_M.by_any(
             value or self.input.mark.any()), "Список свободных карт доступа:")
 
     def find_user(self, value: str = None) -> None:
@@ -290,15 +330,15 @@
             self.output.error(error.get_details())
         else:
             self.output.user.result(result, "Пользователи:")
 
     def create_password(self) -> str:
         password: str = None
         password_settings: PasswordSettings = PASSWORD.get(self.input.indexed_field_list(
-            "Выберите тип пароля", FIELD_COLLECTION.POLICY.PASSWORD_TYPE))
+            "Выберите тип пароля", A.CT_FC.POLICY.PASSWORD_TYPE))
         while True:
             password = self.input.user.generate_password(
                 True, password_settings)
             self.output.value("Пароль", password)
             if self.input.yes_no("Использовать", True):
                 break
         if self.input.yes_no("Отправить в ИТ отдел"):
@@ -383,23 +423,23 @@
     def bold(self, value: str) -> str:
         return self.output.bold(value)
 
     def italic(self, value: str) -> str:
         return self.output.italic(value)
 
     def run_command(self, command_list: list[str] = None) -> None:
-        default_host: str = CONST.HOST.DC2.NAME
+        default_host: str = A.CT_H.DC2.NAME
         host: str = None
         def get_command_list() -> list[str]:
             command_list: tuple[list[str], list[str]] = A.D.dequotes(
                 self.pih.input.input("Введите команду"))
             return list(filter(lambda item: not A.D_C.empty(item), command_list[0] + command_list[1]))
         command_list = command_list or get_command_list()
         use_psexec: bool = A.D_C.empty([value for value in list(map(
-            lambda item: item.lower(), command_list)) if value in CONST.PSTOOLS.COMMAND_LIST])
+            lambda item: item.lower(), command_list)) if value in A.CT.PSTOOLS.COMMAND_LIST])
         result: CompletedProcess = None
         if use_psexec:
             if A.D_C.empty(host):
                 if self.input.yes_no(f"Использовать хост {self.bold(default_host)}, для выполнения команды", no_label=f"{self.bold('Или введите название хоста')}"):
                     host = default_host
                 else:
                     host = self.input.answer
@@ -459,15 +499,15 @@
             group_name: str = free_mark.GroupName
             self.tab_number = free_mark.TabNumber
             self.output.value("Группа карты доступа", group_name)
             return self.output.get_action_value("Номер карты пропуска", self.tab_number)
 
         def get_division() -> ActionValue:
             self.output.header("Выбор подразделения")
-            person_division: MarkDivision = self.input.mark.person_division()
+            person_division: PersonDivision = self.input.mark.person_division()
             self.division_id = person_division.id
             return self.output.get_action_value("Подразделение, к которому прикреплена персона", person_division.name)
 
         ActionStack("Данные пользователя",
                     get_full_name,
                     get_division,
                     get_telephone_number,
@@ -486,15 +526,15 @@
             else:
                 self.output.error("Карта доступа не создана!")
 
     def send_workstation_message_to_all(self) -> None:
         message: str = self.input.message(
             f"{self.get_formatted_given_name()}, введите сообщение для всех пользователей")
         A.ME_WS.to_all_workstations(
-            message, None, [CONST.HOST.WS255], self.session)
+            message, None, [A.CT_H.WS255], self.session)
 
     @property
     def user(self) -> User:
         return self.session.user
 
     @property
     def user_description(self) -> str:
@@ -569,15 +609,15 @@
         if self.input.yes_no(f"Создать временную карту для {full_name} с табельным номеров {tab_number}", True):
             if A.A_M.make_as_temporary(temporary_mark, owner_mark):
                 self.output.good("Временная карта создана")
                 telephone_number: str = owner_mark.telephoneNumber
                 A.Eit_notify_about_create_temporary_mark(
                     full_name, tab_number)
                 if not A.C.telephone_number(telephone_number):
-                    user: User = A.R.get_first_element(A.R_U.by_any(
+                    user: User = A.R.get_first_item(A.R_U.by_any(
                         owner_mark))
                     if user is not None:
                         telephone_number = user.telephoneNumber
                 if A.C.telephone_number(telephone_number):
                     if self.input.yes_no("Уведомить персону", True):
                         self.send_whatsapp_message(
                             telephone_number, f"Сообщение от ИТ отдела: День добрый, {self.get_formatted_given_name(full_name)}, Вам выдана временная карта доступа с номером {tab_number}")
@@ -627,39 +667,39 @@
             else:
                 self.output.notify(
                     f"{user.name}, похоже не пользователь, у которого должен быть номер телефона")
 
     def start_user_property_setter(self, property_name: str, search_value: str = None, choose_user: bool = False) -> None:
         try:
             user_list: list[User] = None
-            fields: FieldItemList = FIELD_COLLECTION.AD.USER
+            fields: FieldItemList = A.CT_FC.AD.USER
             active: bool | None = True if (
-                property_name == USER_PROPERTIES.PASSWORD or property_name == USER_PROPERTIES.TELEPHONE_NUMBER) else None
+                property_name == A.CT_UP.PASSWORD or property_name == A.CT_UP.TELEPHONE_NUMBER) else None
             if choose_user:
                 user_list = self.input.user.by_any(search_value, active)
             else:
                 result: Result[list[User]] = A.R_U.by_any(
                     self.input.user.title_any(), active)
                 user_list = result.data
-            if property_name == USER_PROPERTIES.USER_STATUS:
-                for status in [AD.ACTIVE_USERS_CONTAINER_DN, AD.INACTIVE_USERS_CONTAINER_DN]:
+            if property_name == A.CT_UP.USER_STATUS:
+                for status in [A.CT_AD.ACTIVE_USERS_CONTAINER_DN, A.CT_AD.INACTIVE_USERS_CONTAINER_DN]:
                     work_user_list: list[User] = self.pih.DATA.FILTER.users_by_dn(
-                        user_list, AD.INACTIVE_USERS_CONTAINER_DN if status == AD.ACTIVE_USERS_CONTAINER_DN else AD.ACTIVE_USERS_CONTAINER_DN)
+                        user_list, A.CT_AD.INACTIVE_USERS_CONTAINER_DN if status == A.CT_AD.ACTIVE_USERS_CONTAINER_DN else A.CT_AD.ACTIVE_USERS_CONTAINER_DN)
                     for index, user in enumerate(work_user_list):
                         try:
                             self.output.user.result(Result(fields, [user]))
-                            if self.input.yes_no(f"{'Активировать' if status == AD.ACTIVE_USERS_CONTAINER_DN else 'Деактивировать' } пользователя"):
-                                if status == AD.ACTIVE_USERS_CONTAINER_DN:
+                            if self.input.yes_no(f"{'Активировать' if status == A.CT_AD.ACTIVE_USERS_CONTAINER_DN else 'Деактивировать' } пользователя"):
+                                if status == A.CT_AD.ACTIVE_USERS_CONTAINER_DN:
                                     if self.input.yes_no("Использовать шаблон для пользователя", True):
                                         user_container = self.input.user.template()
                                     else:
                                         user_container = self.input.user.container()
                                 else:
                                     user_container = UserBase(
-                                        distinguishedName=AD.INACTIVE_USERS_CONTAINER_DN)
+                                        distinguishedName=A.CT_AD.INACTIVE_USERS_CONTAINER_DN)
                                 if self.pih.ACTION.USER.set_status(user, status, user_container):
                                     self.output.good("Успешно")
                                 else:
                                     self.output.error("Ошибка")
                             else:
                                 self.output.new_line()
                                 self.output.error("Отмена")
@@ -669,32 +709,32 @@
                                 self.output.error("Отмена")
                             else:
                                 self.output.error("Отмена - следующий")
                             self.output.new_line()
             else:
                 for index, user in enumerate(user_list):
                     try:
-                        if property_name == USER_PROPERTIES.TELEPHONE_NUMBER:
+                        if property_name == A.CT_UP.TELEPHONE_NUMBER:
                             self.output.user.result(
                                 Result(fields, [user]), None)
                             telephone = self.input.telephone_number()
                             if self.pih.CHECK.telephone_number(telephone) and self.input.yes_no("Установить", True):
                                 if self.pih.ACTION.USER.set_telephone_number(user, telephone):
                                     self.output.good("Успешно")
                                 else:
                                     self.output.error("Ошибка")
                             else:
                                 self.output.error("Отмена")
-                        elif property_name == USER_PROPERTIES.PASSWORD:
+                        elif property_name == A.CT_UP.PASSWORD:
                             self.output.user.result(
                                 Result(fields, [user]), "Пользователи:")
                             password: str = None
                             while True:
                                 password = self.input.user.generate_password(True, PASSWORD.get(
-                                    self.input.indexed_field_list("Выберите тип пароля", FIELD_COLLECTION.POLICY.PASSWORD_TYPE)))
+                                    self.input.indexed_field_list("Выберите тип пароля", A.CT_FC.POLICY.PASSWORD_TYPE)))
                                 self.output.value("Пароль", password)
                                 if self.input.yes_no("Использовать", True):
                                     break
                             if self.input.yes_no("Установить", True):
                                 if self.pih.ACTION.USER.set_password(user, password):
                                     self.output.good("Успешно")
                                 else:
@@ -809,15 +849,15 @@
                         f"Найдена карта доступа для персоны {full_name_string} с номером {mark.TabNumber}. Использовать", True):
                     self.need_to_create_mark = False
                     return None
             self.need_to_create_mark = self.input.yes_no(
                 f"Создать карту доступа для персоны '{full_name_string}'", True)
             if self.need_to_create_mark:
                 self.output.header("Выбор подразделения")
-                person_division: MarkDivision = self.input.mark.person_division()
+                person_division: PersonDivision = self.input.mark.person_division()
                 self.division_id = person_division.id
                 return self.output.get_action_value("Подразделение персоны, которой принадлежит карта доступа", person_division.name)
             return None
 
         def get_tab_number() -> ActionValue:
             if self.need_to_create_mark:
                 self.output.header("Создание карты доступа")
```

### Comparing `pih-1.46231/pih/const.py` & `pih-1.47001/pih/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-﻿from enum import *
+﻿from enum import Enum, auto
 import os
 
-from pih.collection import FieldItem, FieldItemList, EventDescription, ParamItem, PasswordSettings, StorageValue, ResourceDescription, SiteResourceDescription, PolibaseDocumentDescription, MedicalDirectionDescription, ActionDescription, IntStorageValue, BoolStorageValue, TimeStorageValue, DateListStorageValue, FloatStorageValue
+from pih.collection import (FieldItem, FieldItemList, EventDescription, 
+                            ParamItem, PasswordSettings, StorageValue, 
+                            ResourceDescription, SiteResourceDescription, PolibaseDocumentDescription, 
+                            MedicalDirectionDescription, ActionDescription, IntStorageValue, 
+                            BoolStorageValue, TimeStorageValue, DateListStorageValue, 
+                            FloatStorageValue)
 from pih.rpc_collection import ServiceDescription, ServiceInformationBase
 from pih.rpc_const import ServiceCommands
 
 class DATA:
 
     #deprecated
     class EXTRACTOR:
@@ -120,14 +125,15 @@
 
     class USER:
         MARKETER: str = "marketer"
         CALL_CENTRE_ADMINISTRATOR: str = "callCentreAdmin"
         REGISTRATION_AND_CALL: str = "reg_and_call"
         CONTROL_SERVICE: str = "cctv"
         INDICATIONS_ALL: str = "indications_all"
+        ADMINISTRATOR: str = "Administrator"
 
     class JobPisitions(Enum):
         HR: int = auto()
         IT: int = auto()
         CALL_CENTRE: int = auto()
         REGISTRATOR: int = auto()
         RD: int = auto()
@@ -292,30 +298,34 @@
     HEAT_BEAT_PERIOD: int = 60
 
     NEW_LINE: str = "\n"
 
     class TEST:
 
         WORKSTATION_MAME: str = HOSTS.DEVELOPER.NAME
-        USER: str = "nak"
+        USER: str | None = "nak"
+        #"nak"
         PIN: int = 100310
         NAME: str = "test"
 
     GROUP_PREFIX: str = "group:"
 
     SITE_PROTOCOL: str = "https://"
     UNTRUST_SITE_PROTOCOL: str = "http://" 
     
     SITE_NAME: str = "pacifichosp"
     SITE_URL: str = f"{SITE_NAME}.com"
     EMAIL_SERVER_URL: str = f"mail.{SITE_URL}"
     RECEPTION_EMAIL_LOGIN: str = f"reception.{SITE_NAME}"
 
-    WIKI_ADDRESS: str = f"{UNTRUST_SITE_PROTOCOL}wiki"
-    API_SITE_ADDRESS: str = f"api.{SITE_URL}"
+    WIKI_SITE_NAME: str = f"wiki"
+    WIKI_SITE_ADDRESS: str = f"{UNTRUST_SITE_PROTOCOL}{WIKI_SITE_NAME}"
+    OMS_SITE_NAME: str = "oms"
+    OMS_SITE_ADDRESS: str = f"{UNTRUST_SITE_PROTOCOL}{OMS_SITE_NAME}"
+    API_SITE_URL: str = f"api.{SITE_URL}"
     BITRIX_SITE_URL: str = "bitrix.cmrt.ru"
 
     INTERNATIONAL_TELEPHONE_NUMBER_PREFIX: str = "7"
     TELEPHONE_NUMBER_PREFIX: str = f"+{INTERNATIONAL_TELEPHONE_NUMBER_PREFIX}"
     INTERNAL_TELEPHONE_NUMBER_PREFIX: str = "тел."
 
     DATETIME_SPLITTER: str = "T"
@@ -393,15 +403,15 @@
                 URL_SEND_BUTTONS_MESSAGE: str = f"{URL_MESSAGE}/buttons/send?{PROFILE_SUFFIX}"
                 URL_GET_MESSAGES: str = f"{URL_MESSAGE}s/get?{PROFILE_SUFFIX}"
                 URL_GET_STATUS: str = f"{URL_API_SYNC}/get/status?{PROFILE_SUFFIX}"
                 CONTACT_SUFFIX: str = "@c.us"
 
                 class PROFILE(Enum):
                     IT: str = "e6706eaf-ae17"
-                    CALL_CENTRE: str = "56ad2cb1-a5ac"
+                    CALL_CENTRE: str = "81b820f8-cd6e"
                     MARKETER: str = "c31db01c-b6d6"
                     DEFAULT: str = CALL_CENTRE
                     
                 AUTHORIZATION: str = "6b356d3f53124af3078707163fdaebca3580dc38"
             
     class PYTHON:
 
@@ -642,14 +652,17 @@
 
             @staticmethod
             def sorted() -> list:
                 return sorted(CONST.POLIBASE.DOCUMENT_DESCRIPTIONS, key=lambda item: item.value.title_height, reverse=True)
     
     class VISUAL:
 
+        YES: str = "✅"
+        NO: str = "❌"
+
         NUMBER_SYMBOLS: list[str] = [
            "0️⃣",
            "1️⃣",
            "2️⃣",
            "3️⃣", 
            "4️⃣",
            "5️⃣",
@@ -669,15 +682,15 @@
 class MATERIALIZED_RESOURCES:
 
     NAME: str = "MATERIALIZED_RESOURCES"
     ALIAS: str = "MR"
 
     class TYPES(Enum):
     
-        CHILLER_FILTER_COUNT: IntStorageValue = IntStorageValue("CHF", description="Количество фильтров для чиллера")
+        CHILLER_FILTER_COUNT: IntStorageValue = IntStorageValue("CHF", description="Фильтры для чиллера")
 
 
 class RESOURCES:
 
     class DESCRIPTIONS:
     
         INTERNET: ResourceDescription = ResourceDescription(
@@ -692,17 +705,21 @@
         POLIBASE: ResourceDescription = ResourceDescription("polibase", "Polibase", inaccessibility_check_values=(2, 10000, 15))
 
         SITE_LIST: list[SiteResourceDescription] = [
             SiteResourceDescription(
                         CONST.SITE_URL, f"Сайт компании: {CONST.SITE_URL}", check_certificate_status=True, check_free_space_status=False),
             SiteResourceDescription(CONST.EMAIL_SERVER_URL,
                         f"Сайт корпоративной почты: {CONST.EMAIL_SERVER_URL}", check_certificate_status=True, check_free_space_status=True, driver_name="/dev/mapper/centos_tenant26--02-var"),
-            SiteResourceDescription(CONST.API_SITE_ADDRESS,
-                                    f"Api сайта {CONST.SITE_URL}: {CONST.API_SITE_ADDRESS}", check_certificate_status=True, check_free_space_status=False),
-            SiteResourceDescription(CONST.BITRIX_SITE_URL, f"Сайт Битрикс ЦМРТ24: {CONST.BITRIX_SITE_URL}")
+            SiteResourceDescription(CONST.API_SITE_URL,
+                                    f"Api сайта {CONST.SITE_URL}: {CONST.API_SITE_URL}", check_certificate_status=True, check_free_space_status=False),
+            SiteResourceDescription(CONST.BITRIX_SITE_URL, f"Сайт Битрикс ЦМРТ24: {CONST.BITRIX_SITE_URL}"),
+            SiteResourceDescription(
+                CONST.OMS_SITE_ADDRESS, f"Сайт омс: {CONST.OMS_SITE_ADDRESS}", internal = True),
+            SiteResourceDescription(
+                CONST.WIKI_SITE_ADDRESS, f"Сайт wiki: {CONST.WIKI_SITE_ADDRESS}",  internal=True)
         ]
     
     class INACCESSABLE_REASONS(Enum):
 
         CERTIFICATE_ERROR: str = "Ошибка проверки сертификата"
         SERVICE_UNAVAILABLE: str = "Ошибка 503: Сервис недоступен"
 
@@ -719,14 +736,15 @@
     RESOURCES: int = auto()
     WS: int = auto()
     PRINTERS: int = auto()
     INDICATIONS: int = auto()
     BACKUPS: int = auto()
     VALENTA: int = auto()
     SERVERS: int = auto()
+    MATERIALIZED_RESOURCES: int = auto()
 
     @staticmethod
     def all() :
         return [item for item in CheckableSections]
     
 class DocumentTypes(Enum):
     
@@ -962,14 +980,15 @@
     PIN: str = "pin"
     PID: str = "pid"
     VISIT_ID: str = "visitID"
     MESSAGE_ID: str = "messageID"
     VALUE: str = "value"
     FILE: str = "file"
     DIVISION_NAME: str = "DivisionName"
+    DIVISION_ID: str = "DivisionID"
     BARCODE: str = "barcode"
     PROPERTIES: str = "properties"
     PARAMETERS: str = "parameters"
     MESSAGE: str = "message"
     STATUS: str = "status"
     FEEDBACK_CALL_STATUS: str = "feedbackCallStatus"
     REGISTRATION_DATE: str = "registrationDate"
@@ -979,14 +998,15 @@
     DOCTOR_FULL_NAME: str = "doctorFullName"
     SERVICE_GROUP_ID: str = "serviceGroupID"
     PORT_NAME: str = "portName"
     TEMPERATURE: str = "temperature"
     HUMIDITY: str = "humidity"
     INDICATORS: str = "indicators"
     DATA: str = "data"
+    COUNT: str = "count"
 
     SEARCH_ATTRIBUTE_LOGIN: str = USER_PROPERTIES.LOGIN
     SEARCH_ATTRIBUTE_NAME: str = USER_PROPERTIES.NAME
 
     TELEPHONE_NUMBER: str = USER_PROPERTIES.TELEPHONE_NUMBER
     EMAIL: str = f"e{USER_PROPERTIES.EMAIL}"
     DN: str = USER_PROPERTIES.DN
@@ -1354,19 +1374,20 @@
 
 class LogMessageFlags(Enum):
     NORMAL: int = 1
     ERROR: int = 2
     NOTIFICATION: str = 4
     DEBUG: str = 8
     SAVE: int = 16
-    TASK: int = 17
     SILENCE: str = 32
     RESULT: int = 64
     WHATSAPP: int = 128
     ALERT: int = 256
+    TASK: int = 512
+    SAVE_ONCE: int = 1024
     DEFAULT: str = NORMAL
 
 POLIBASE_BASE: ServiceDescription = ServiceDescription(
         host=CONST.HOST.POLIBASE.NAME,
         pyton_executor_path=r"C:\Users\adm\AppData\Local\Programs\Python\Python310\python.exe",
         run_from_system_account=True
         )
@@ -1520,31 +1541,32 @@
                                                         ],
                                                 modules=["pyad", "pywin32", "wmi"]
                                             )
     WS: ServiceDescription = ServiceDescription(
                                                 name="WS",
                                                 description="Workstation service",
                                                 host=CONST.HOST.BACKUP_WORKER.NAME,
-                                                commands=[
-                                                    ServiceCommands.reboot,
-                                                    ServiceCommands.shutdown,
-                                                    ServiceCommands.send_message_to_user_or_workstation,
-                                                    ServiceCommands.kill_process
-                                                ])
+                                                commands=   
+                                                        [
+                                                            ServiceCommands.reboot,
+                                                            ServiceCommands.shutdown,
+                                                            ServiceCommands.send_message_to_user_or_workstation,
+                                                            ServiceCommands.kill_process
+                                                        ]
+                                                )
 
     PRINTER: ServiceDescription = ServiceDescription(
                                                     name="Printer",
                                                     description="Printer service", 
                                                     host=CONST.HOST.DC2.NAME, 
                                                     commands=
                                                             [
-                                                                ServiceCommands.printers_report,
-                                                                #ServiceCommands.printers_status
+                                                                ServiceCommands.printers_report
                                                             ]
-                                                           )
+                                                    )
     
     DOCS: ServiceDescription = ServiceDescription(
                                                             name="Docs",
                                                             description="Documents service",
                                                             host=CONST.HOST.DC2.NAME,
                                                             commands=[
                                                                 ServiceCommands.get_inventory_report,
@@ -1556,33 +1578,34 @@
                                                                 ServiceCommands.check_inventory_report,
                                                                 ServiceCommands.save_inventory_report_item,
                                                                 ServiceCommands.close_inventory_report,
                                                                 ServiceCommands.create_note,
                                                                 ServiceCommands.get_note,
                                                             ],
                                                             modules=["xlsxwriter", "xlrd", "xlutils", "openpyxl",
-                                                                    "python-barcode", "Pillow", "transliterate", "qrcode", "docx-mailmerge", "gkeepapi"]
+                                                                    "python-barcode", "Pillow", "qrcode", "docx-mailmerge", "gkeepapi"]
                                                         )
 
     MARK: ServiceDescription = ServiceDescription(
                                                 name="Orion",
                                                 description="Orion service",
                                                 host=CONST.HOST.DC2.NAME,
                                                 commands=
                                                         [
-                                                            ServiceCommands.get_free_marks,
-                                                            ServiceCommands.get_temporary_marks,
-                                                            ServiceCommands.get_person_divisions,
+                                                            ServiceCommands.get_free_mark_list,
+                                                            ServiceCommands.get_temporary_mark_list,
+                                                            ServiceCommands.get_mark_person_division_list,
                                                             ServiceCommands.get_time_tracking,
-                                                            ServiceCommands.get_all_persons,
+                                                            ServiceCommands.get_mark_list,
                                                             ServiceCommands.get_mark_by_tab_number,
                                                             ServiceCommands.get_mark_by_person_name,
-                                                            ServiceCommands.get_free_marks_group_statistics,
-                                                            ServiceCommands.get_free_marks_by_group_id,
+                                                            ServiceCommands.get_free_mark_group_statistics_list,
+                                                            ServiceCommands.get_free_mark_list_by_group_id,
                                                             ServiceCommands.get_owner_mark_for_temporary_mark,
+                                                            ServiceCommands.get_mark_list_by_division_id,
                                                             ServiceCommands.set_full_name_by_tab_number, 
                                                             ServiceCommands.set_telephone_by_tab_number,
                                                             ServiceCommands.check_mark_free,
                                                             ServiceCommands.create_mark,
                                                             ServiceCommands.make_mark_as_free_by_tab_number,
                                                             ServiceCommands.make_mark_as_temporary,
                                                             ServiceCommands.remove_mark_by_tab_number,
@@ -1613,15 +1636,15 @@
                                                                 ServiceCommands.set_polibase_person_email,
                                                                 ServiceCommands.set_barcode_for_polibase_person,
                                                                 ServiceCommands.check_polibase_person_card_registry_folder_name,
                                                                 ServiceCommands.set_polibase_person_telephone_number,
                                                                 ServiceCommands.get_polibase_person_operator_by_pin,
                                                                 ServiceCommands.get_polibase_person_by_email
                                                             ], 
-                                                    modules=["cx-Oracle", "fastapi", "uvicorn", "transliterate"])
+                                                    modules=["cx-Oracle", "fastapi", "uvicorn"])
 
     POLIBASE_DATABASE: ServiceDescription = ServiceDescription(
         name="PolibaseDB",
         description="Polibase database api",
         host=POLIBASE_BASE.host, 
         pyton_executor_path=POLIBASE_BASE.pyton_executor_path,
         run_from_system_account=POLIBASE_BASE.run_from_system_account,
@@ -1984,14 +2007,16 @@
     PERSON_PIN: ParamItem = ParamItem(FIELD_NAME_COLLECTION.PERSON_PIN, "")
     PERSON_NAME: ParamItem = ParamItem(FIELD_NAME_COLLECTION.PERSON_NAME, "")
     REGISTRATOR_PERSON_NAME: ParamItem = ParamItem(FIELD_NAME_COLLECTION.REGISTRATOR_PERSON_NAME, "")
     REGISTRATOR_PERSON_PIN: ParamItem = ParamItem(
         FIELD_NAME_COLLECTION.REGISTRATOR_PERSON_PIN, "")
     CARD_REGISTRY_FOLDER: ParamItem = ParamItem(FIELD_NAME_COLLECTION.CARD_REGISTRY_FOLDER, "")
     DESTINATION: ParamItem = ParamItem(FIELD_NAME_COLLECTION.DESTINATION, "")
+    COUNT: ParamItem = ParamItem(FIELD_NAME_COLLECTION.COUNT, "Количество")
+
 
 class Events(Enum):
 
     DEBUG: EventDescription = EventDescription(
         "It is a debug event", LogMessageChannels.POLIBASE, LogMessageFlags.DEBUG.value)
         
     PRINTER_REPORT: EventDescription = EventDescription("Принтер {printer_name} ({location}):\n {printer_report}", LogMessageChannels.PRINTER, LogMessageFlags.NORMAL, (ParamItem(
@@ -2040,18 +2065,18 @@
     BACKUP_ROBOCOPY_JOB_WAS_STARTED: EventDescription = EventDescription(
         "Robocopy: Начато выполнение задания: {name}. PID процесса: {pid}", LogMessageChannels.BACKUP, (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE), (PARAM_ITEMS.NAME, PARAM_ITEMS.PID))
 
     BACKUP_ROBOCOPY_JOB_WAS_COMPLETED: EventDescription = EventDescription(
         "Robocopy: Завершено выполнение задания: {name}. Статус: {status_string}", LogMessageChannels.BACKUP, (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE), (PARAM_ITEMS.NAME, ParamItem("status_string", ""), PARAM_ITEMS.STATUS))
     #
     POLIBASE_CREATION_DB_DUMP_START: EventDescription = EventDescription(
-        "Базы данных Polibase: Начато создание дампа", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL)
+        "Базы данных Polibase: Начато создание дампа", LogMessageChannels.BACKUP, (LogMessageFlags.NORMAL, LogMessageFlags.SAVE))
     
     POLIBASE_CREATION_DB_DUMP_COMPLETE: EventDescription = EventDescription(
-        "Базы данных Polibase: Завершено создание дампа", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL)
+        "Базы данных Polibase: Завершено создание дампа", LogMessageChannels.BACKUP, (LogMessageFlags.NORMAL, LogMessageFlags.SAVE))
     
     POLIBASE_CREATION_ARCHIVED_DB_DUMP_START: EventDescription = EventDescription(
         "Базы данных Polibase: Начато архивирование дампа", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL)
 
     POLIBASE_CREATION_ARCHIVED_DB_DUMP_COMPLETE: EventDescription = EventDescription(
         "Базы данных Polibase: Завершено архивирование дампа", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL)
     
@@ -2080,23 +2105,29 @@
 
     IT_NOTIFY_ABOUT_MARK_RETURN: EventDescription = EventDescription("Добрый день, отдел Информационных технологий.\nКарта доступа для персоны: {name} возвращена!\nНомер карты: {tab_number}", LogMessageChannels.IT, LogMessageFlags.NOTIFICATION.value, (PARAM_ITEMS.NAME, ParamItem("tab_number", "")))
 
     IT_TASK_AFTER_CREATE_NEW_USER: EventDescription = EventDescription("Добрый день, {it_user_name}.\nНеобходимо создать почту для пользователя: {name}\nАдресс электронной почты: {mail}\nПароль: {password}", LogMessageChannels.IT, LogMessageFlags.TASK.value, (ParamItem(
         "it_user_name", ""), PARAM_ITEMS.NAME, ParamItem("mail", ""), ParamItem("password", "")))
 
     WATCHABLE_WORKSTATION_IS_NOT_ACCESSABLE: EventDescription = EventDescription(
-        "Компьютер {workstation_name} вне сети", LogMessageChannels.RESOURCES, LogMessageFlags.ERROR, [ParamItem("workstation_name", "")])
+        "Компьютер {} вне сети", LogMessageChannels.RESOURCES, LogMessageFlags.ERROR, [PARAM_ITEMS.NAME])
     
     WATCHABLE_WORKSTATION_IS_ACCESSABLE: EventDescription = EventDescription(
-        "Компьютер {workstation_name} в сети", LogMessageChannels.RESOURCES, LogMessageFlags.NORMAL, [ParamItem("workstation_name", "")])
+        "Компьютер {} в сети", LogMessageChannels.RESOURCES, LogMessageFlags.NORMAL, [PARAM_ITEMS.NAME])
     
+    SERVER_IS_NOT_ACCESSABLE: EventDescription = EventDescription(
+        "Сервер {} вне сети", LogMessageChannels.RESOURCES, (LogMessageFlags.ERROR, LogMessageFlags.SAVE_ONCE),  [PARAM_ITEMS.NAME])
+
+    SERVER_IS_ACCESSABLE: EventDescription = EventDescription(
+        "Сервер {} в сети", LogMessageChannels.RESOURCES, (LogMessageFlags.NORMAL, LogMessageFlags.SAVE_ONCE), [PARAM_ITEMS.NAME])
+
     #MRI
      
     MRI_CHILLER_FILTER_WAS_CHANGED: EventDescription = EventDescription(
-        "Фильтр водяного охлаждения был заменён", LogMessageChannels.RESOURCES, (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE))
+        "Фильтр водяного охлаждения МРТ был заменён. Количество оставшихся фильтров: {}", LogMessageChannels.RESOURCES, (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE), [PARAM_ITEMS.COUNT])
     
     MRI_CHILLER_TEMPERATURE_ALERT_WAS_FIRED: EventDescription = EventDescription(
         "Превышена температура чиллера", LogMessageChannels.RESOURCES, (LogMessageFlags.ERROR, LogMessageFlags.SAVE))
     
     MRI_CHILLER_WAS_TURNED_OFF: EventDescription = EventDescription(
         "чиллера", LogMessageChannels.RESOURCES, (LogMessageFlags.ERROR, LogMessageFlags.SAVE), (ParamItem(FIELD_NAME_COLLECTION.DATE, ""), ))
 
@@ -2145,17 +2176,26 @@
 
 
 class Actions(Enum):
 
     CHILLER_FILTER_CHANGING: ActionDescription = ActionDescription(
         "CHILLER_FILTER_CHANGING", ("filter", ), "Замена фильтра очистки воды", "Заменить фильтр очистки воды")
     
+    SWITCH_TO_EXTERNAL_WATER_SOURCE: ActionDescription = ActionDescription(
+        "SWITCH_TO_EXTERNAL_WATER_SOURCE", ("external_ws", ), "Переход на внешнее (городское) водоснабжение", "Перейти на внешнее (городское) водоснабжение")
+    
+    SWITCH_TO_INTERNAL_WATER_SOURCE: ActionDescription = ActionDescription(
+        "SWITCH_TO_INTERNAL_WATER_SOURCE", ("internal_ws", ), "Переход на внутреннее водоснабжение", "Перейти на внутреннее водоснабжение")
+    
     VALENTA_SYNCHRONIZATION: ActionDescription = ActionDescription(
         "VALENTA_SYNCHRONIZATION", ("valenta", "валента"), "Синхронизация Валенты", "Совершить синхронизацию для Валенты", False, True)
 
+    TIME_TRACKING_REPORT: ActionDescription = ActionDescription(
+        "TIME_TRACKING_REPORT", ("tt", "урв"), "Отчеты по учёту рабочего времени", "Создать", False, True)
+
 
 class EMAIL:
 
     NAS: str = "@".join(("nas", CONST.SITE_URL))
     IT: str = "@".join(("it", CONST.SITE_URL))
     EXTERNAL_MAIL_SERVICE: str = "mail.pacifichosp@mail.ru"
     MAILER_DAEMON: str = "mailer-daemon@corp.mail.ru"
```

### Comparing `pih-1.46231/pih/pih.py` & `pih-1.47001/pih/pih.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 import base64
 import uuid
 import time
 from enum import Enum
 from string import Formatter
 import urllib.parse
 
+from transliterate import translit
+
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
 
 from pih.collection import  *
 from pih.tools import *
 from pih.const import *
@@ -457,15 +459,15 @@
 
 
 class MarkInputAbstract:
 
     def free(self, group: MarkGroup = None) -> Mark:
         raise NotImplemented()
 
-    def person_division(self) -> MarkDivision:
+    def person_division(self) -> PersonDivision:
         raise NotImplemented()
 
     def by_name(self) -> Mark:
         raise NotImplemented()
 
     def by_any(self, value: str | None = None) -> Mark:
         raise NotImplemented()
@@ -486,15 +488,15 @@
         self.output: OutputBase
         self.mark: MarkInputBase
         self.user: UserInputBase
 
 
 class OutputBase(OutputAbstract, OutputExtendedAbstract):
 
-    def __init__(self, user_output: UserOutputBase = None, mark_output: MarkOutputBase = None):
+    def __init__(self, user_output: UserOutputBase | None = None, mark_output: MarkOutputBase | None = None):
         self.text_before: str = ""
         self.text_after: str = ""
         self.indent_symbol: str = " "
         self.indent_value: int = 0
         self.user: UserOutputBase = user_output
         self.user.parent = self
         self.mark: MarkOutputBase = mark_output
@@ -543,20 +545,21 @@
         raise NotImplemented()
 
     def add_allowed_group(self, value: AD.Groups) -> None:
         raise NotImplemented()
 
 class SessionBase(SessionAbstract):
 
-    def __init__(self, input: InputBase = None, output: OutputBase = None):
+    def __init__(self, input: InputBase | None = None, output: OutputBase | None = None, name: str | None = None):
         self.allowed_groups: list[AD.Groups] = []
         self.login: str | None = None
         self.user: User = None
         self.input: InputBase = input
         self.output: OutputBase = output
+        self.name: str | None = name
 
     def add_allowed_group(self, value: AD.Groups) -> None:
         self.allowed_groups.append(value)
 
 
 class Session(SessionBase):
 
@@ -678,15 +681,15 @@
 
     @contextmanager
     def make_indent(self, value: int, additional: bool = False) -> bool:
         try:
             self.set_indent([0, self.indent][additional] + value)
             yield True
         finally:
-            self.set_indent([0, self.indent - value][additional])
+            self.set_indent([self.indent, self.indent - value][additional])
 
     def set_indent(self, value: int) -> None:
         self.indent_value = value
         self.text_before = self.indent_symbol * value
 
     def bold(self, value: str) -> str:
         return f"\033[1m{value}\033[0m"
@@ -1308,17 +1311,17 @@
                     return self.parent.item_by_index(
                         "Выберите карту доступа введя индекс", data)
                 else:
                     self.parent.output.error(
                         f"Нет свободных карт для группы доступа '{group.GroupName}'!")
                     return self.free()
 
-    def person_division(self) -> MarkDivision:
-        division_list: list[MarkDivision] = PIH.RESULT.MARK.person_divisions().data
-        division_list.insert(0, MarkDivision(0, "Без подразделения"))
+    def person_division(self) -> PersonDivision:
+        division_list: list[PersonDivision] = PIH.RESULT.MARK.person_divisions().data
+        division_list.insert(0, PersonDivision(0, "Без подразделения"))
         return self.parent.item_by_index("Выберите подразделение для персоны, которой принадлежит карта доступа", division_list, lambda item, _: item.name )
 
     def by_name(self) -> Mark:
         self.parent.output.head2("Введите имя персоны")
         result: Result[list[Mark]] = None
         while result is None:
             try:
@@ -1542,15 +1545,14 @@
     pass
 
 
 class NamePolicy:
 
     @staticmethod
     def get_first_letter(name: str) -> str:
-        from transliterate import translit
         letter = name[0]
         if letter.lower() == "ю":
             return "yu"
         return translit(letter, "ru", reversed=True).lower()
 
     @staticmethod
     def convert_to_login(full_name: FullName) -> FullName:
@@ -1606,15 +1608,15 @@
             recipient = recipient if isinstance(recipient, str) else EnumTool.get(recipient)
             session: MobileSession = MobileSession(recipient, EnumTool.get(Flags.SILENCE))
             recipient_as_whatsapp_group: bool = recipient.endswith(A.CT_ME_WH.GROUP_SUFFIX)
             if use_login and not recipient_as_whatsapp_group:
                 session.say_hello()
             output: MobileOutput = MobileOutput(session)
             if not recipient_as_whatsapp_group:
-                output.user.get_formatted_given_name = lambda _: format_given_name(session, output)
+                output.user.get_formatted_given_name = lambda: format_given_name(session, output)
             return output
 
         @staticmethod
         def waiting_for_input_from(recipient: str, handler: Callable[[str, Callable[[None], None]], None] | None = None) -> str | None:
             def internal_handler(message: str, close_handler: Callable[[None], None]) -> None:
                 PIH.MIO.ANSWER[recipient].append(message)
                 if DataTool.is_empty(handler):
@@ -1625,15 +1627,15 @@
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
         @staticmethod
         def local() -> str:
-            return "1.46231"
+            return "1.47001"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -2057,14 +2059,18 @@
                              (command_name, parameters))
                 except Error as error:
                     PIH.output.error("Log send error")
             PIH.LOG.executor.submit(internal_send_command,
                                     value.name, PIH.EVENT.BUILDER.create_parameters_map(value, parameters))   
 
         @staticmethod
+        def mri_filter_was_changed() -> None:
+            PIH.EVENT.send(Events.MRI_CHILLER_FILTER_WAS_CHANGED, (PIH.DATA.MATERIALIZED_RESOURCES.get_count(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER_COUNT),))
+
+        @staticmethod
         def computer_was_started(name: str) -> None:
             PIH.EVENT.send(
                 Events.COMPUTER_WAS_STARTED, (name,))
 
         @staticmethod
         def server_was_started(name: str) -> None:
             PIH.EVENT.send(
@@ -2072,15 +2078,15 @@
 
         @staticmethod
         def get_parameter(event: Events, parameters: dict[str, Any], parameter_name: str | None = None) -> Any | dict[str, Any]:
             parameters_map: dict[str, Any] = PIH.EVENT.BUILDER.create_parameters_map(event, parameters)
             return DataTool.check_not_none(parameter_name, lambda: parameters_map[parameter_name], parameters_map)
 
         class BUILDER:
-    
+
             @staticmethod
             def create_parameters_map(event: Events, parameters: tuple[Any] | None = None, check_for_parameters_count: bool = True) -> dict:
                 event_description: EventDescription = EnumTool.get(event)
                 parameter_pattern_list: list = DataTool.as_list(
                     event_description.params)
                 parameters = parameters or ()
                 if check_for_parameters_count and len(parameter_pattern_list) > len(parameters):
@@ -2106,15 +2112,15 @@
                 def get_information() -> tuple[Any]:
                     workstation_name: str = "<не определён>"
                     workstation_description: str = "<не определён>"
                     if actual:
                         try:
                             user: User = A.R_U.by_polibase_pin(
                                 registrator_person.pin).data
-                            workstation: Workstation = A.R.get_first_element(
+                            workstation: Workstation = A.R.get_first_item(
                                 A.R_WS.by_login(user.samAccountName)) or A.R_WS.by_name(A.CT.TEST.WORKSTATION_MAME).data
                             if A.D.is_not_none(workstation):
                                 workstation_name = workstation.name
                                 workstation_description = workstation.description
                         except NotFound:
                                 pass
                     return (person.FullName, person.pin, person.email, registrator_person.FullName, workstation_name, workstation_description)
@@ -2138,35 +2144,35 @@
                                                     information.host, information.port, information.pid,  information))
 
             @staticmethod
             def action_was_done(action: Actions | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(Events.ACTION_WAS_DONE, action, lambda: (None, EnumTool.get(action).name,))
 
             @staticmethod
-            def chiller_temperature_alert_was_fired() -> Events | tuple[Events, tuple[Any]]:
+            def chiller_temperature_alert_was_fired() -> Events:
                 return PIH.EVENT.BUILDER.create_event(Events.MRI_CHILLER_TEMPERATURE_ALERT_WAS_FIRED)
 
             @staticmethod
-            def polibase_person_set_card_registry_folder(name: str | None = None, person: PolibasePerson | None = None) -> Events | tuple[Events, tuple[Any]]:
+            def polibase_person_set_card_registry_folder(name: str | None = None, person_or_pin: PolibasePerson | int | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(
-                        Events.CARD_REGISTRY_FOLDER_WAS_SET_FOR_POLIBASE_PERSON, (name, person), lambda: (DataTool.if_not_empty(person, lambda person: person.pin), name))
+                        Events.CARD_REGISTRY_FOLDER_WAS_SET_FOR_POLIBASE_PERSON, (name, person_or_pin), lambda: (DataTool.if_not_empty(person_or_pin, lambda person: PIH.RESULT.POLIBASE._person_pin(person)), name))
             
             @staticmethod
             def card_registry_folder_start_card_sorting(name: str | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(
                         Events.CARD_REGISTRY_FOLDER_START_CARD_SORTING, name, lambda: (name, ))
 
             @staticmethod
             def card_registry_folder_complete_card_sorting(name: str | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(
                         Events.CARD_REGISTRY_FOLDER_COMPLETE_CARD_SORTING, name, lambda: (PIH.DATA.FORMAT.polibase_person_card_registry_folder(name), ))
 
             staticmethod
-            def chiller_was_turned_off() -> Events | tuple[Events, tuple[Any]]:
-                return PIH.EVENT.BUILDER.create_event(Events.MRI_CHILLER_TEMPERATURE_ALERT_WAS_TURNED_OFF)
+            def chiller_was_turned_off() -> Events:
+                return PIH.EVENT.BUILDER.create_event(Events.MRI_CHILLER_WAS_TURNED_OFF)
 
             @staticmethod
             def service_was_stopped(information: ServiceInformationBase | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(Events.SERVICE_WAS_STOPPED, information, lambda: (information.name, information) )
             
             @staticmethod
             def polibase_persons_barcodes_old_format_were_detected(person_pin_list: list[int] | None = None) -> Events | tuple[Events, tuple[Any]]:
@@ -2273,15 +2279,15 @@
         def service_was_not_started(information: ServiceInformation, error: str) -> None:
             PIH.EVENT.send(Events.SERVICE_WAS_NOT_STARTED, (information.name,
                                                             information.host, information.port, error, information))
 
         @staticmethod
         def hr_notify_about_new_employee(login: User) -> None:
             user: User = PIH.RESULT.USER.by_login(login).data
-            hr_user: User = ResultTool.get_first_element(
+            hr_user: User = ResultTool.get_first_item(
                 PIH.RESULT.USER.by_job_position(AD.JobPisitions.HR))
             PIH.EVENT.send(Events.HR_NOTIFY_ABOUT_NEW_EMPLOYEE, (FullNameTool.to_given_name(hr_user.name),
                                                                         user.name, user.mail))
 
         @staticmethod
         def it_notify_about_user_creation(login: str, password: str) -> None:
             it_user_list: list[User] = PIH.RESULT.USER.by_job_position(
@@ -2481,15 +2487,15 @@
             if blocked:
                 return action()
             else:
                 Thread(target=action).start()
                 return None
 
         @staticmethod
-        def call_command(value: ServiceCommands, parameters: Any | None = None, timeout: int | None = None, blocked: bool = True, long_operation_duration: int | None = None) -> str | None:
+        def call_command(value: ServiceCommands, parameters: dict[str, Any] | None = None, timeout: int | None = None, blocked: bool = True, long_operation_duration: int | None = None) -> str | None:
            return PIH.SERVICE.call(None, value, parameters, timeout, blocked, long_operation_duration)
 
         @staticmethod
         def get_support_host_list(role_or_information: ServiceRoles | ServiceInformationBase) -> list[str]:
             return list(filter(lambda item: item.name.startswith(f"{PIH.SERVICE.SUPPORT_NAME_PREFIX}{ServiceRoles.description(role_or_information).name}"), PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP))
 
         class ADMIN:
@@ -2631,18 +2637,18 @@
                 def internal_start_handler(service: IService) -> None:
                     if starts_handler is not None:
                         if starts_handler.__code__.co_argcount == 1:
                             starts_handler(service)
                         else:
                             starts_handler()
                 service: IService = RPC.create_service()
-                from inspect import signature
+                from inspect import signature, Signature
                 def internal_call_handler(command_name: str, parameter_list: ParameterList, context) -> Any | None:
                     if not DataTool.is_empty(call_handler):
-                        sig = signature(call_handler)
+                        sig: Signature = signature(call_handler)
                         arg_count: int = len(sig.parameters) - ("self" in sig.parameters)
                         if arg_count == 3:
                             if DataTool.is_in(sig.parameters, "context"):
                                 return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list, context) 
                             if DataTool.is_in(sig.parameters, "subscribtion_result"):
                                 return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list, PIH.DATA.EXTRACT.subscribtion_result(parameter_list))    
                         return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list) 
@@ -2820,14 +2826,17 @@
             @staticmethod
             def mobile_helper_command(name: str) -> str:
                 name = PIH.DATA.FORMAT.mobile_helper_command(name)
                 return os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(name, FILE.EXTENSION.PNG)))
 
     class DATA(DataTool, StringTool, ListTool, DateTimeTool, EnumTool, FullNameTool):
 
+        def translit(value, language_code=None, reversed=False, strict=False):
+            return translit(value, language_code, reversed, strict)
+
         def find_variable(name: str | None) -> list[StorageValue]:
             return PIH.DATA.MATERIALIZED_RESOURCES.find(name) + PIH.SETTINGS.find(name)
         
         class VARIABLE:
 
             NAME: str = "variable"
 
@@ -2982,14 +2991,27 @@
                     return PIH.DATA.FORMAT.telephone_number(value.split(CONST.MESSAGE.WHATSAPP.WAPPI.CONTACT_SUFFIX)[0])
                 if isinstance(value, dict):
                     return PIH.DATA.FORMAT.telephone_number(value["user"])
                 
             class EVENT:
 
                 @staticmethod
+                def parameter(event_ds: EventDS | None, param_item: ParamItem) -> Any | None:
+                    if DataTool.is_none(event_ds):
+                        return None
+                    event: Events = EnumTool.get(Events, event_ds.name)
+                    event_description: EventDescription = EnumTool.get(event)
+                    param_index: int = event_description.params.index(param_item)
+                    if param_index == -1 or param_index >= len(event_ds.parameters):
+                        return None
+                    for index, name in enumerate(event_ds.parameters):
+                        if index == param_index:
+                            return event_ds.parameters[name]
+
+                @staticmethod
                 def whatsapp_message(parameter_list: ParameterList) -> WhatsAppMessage | None:
                     allow: bool = PIH.DATA.EXTRACT.subscribtion_result(parameter_list).result
                     message: WhatsAppMessage | None = None
                     if allow:
                         event, parameters = PIH.DATA.EXTRACT.EVENT.with_parameters(parameter_list)
                         if event == Events.WHATSAPP_MESSAGE_RECEIVED:
                             message = DataTool.fill_data_from_source(WhatsAppMessage(), parameters[0])
@@ -3024,15 +3046,23 @@
                                     out_parameters.append(None)
                             else:
                                 out_parameters.append(in_parameters[event_parameters_description.name])
                     return event, out_parameters
                 
             @staticmethod
             def subscribtion_result(parameter_list: ParameterList) -> SubscribtionResult | None:
-                return None if DataTool.is_empty(parameter_list.list) or not PIH.DATA.CHECK.has_subscribtion_result(parameter_list) else DataTool.fill_data_from_source(SubscribtionResult(), parameter_list.list[-1])
+                def extractor() -> SubscriberInformation:
+                    result: SubscribtionResult = DataTool.fill_data_from_source(SubscribtionResult(), parameter_list.list[-1])
+                    if isinstance(result.result, str):
+                        try:
+                            result.result = DataTool.rpc_unrepresent(result.result)
+                        except Exception as error:
+                            pass
+                    return result                                               
+                return None if DataTool.is_empty(parameter_list.list) or not PIH.DATA.CHECK.has_subscribtion_result(parameter_list) else extractor()
             
             @staticmethod
             def parameter_list(parameter_list: ParameterList) -> ParameterList:
                 return ParameterList(parameter_list.get()) if PIH.DATA.CHECK.has_subscribtion_result(parameter_list) else parameter_list
 
             @staticmethod
             def email(value: str) -> str | None:
@@ -3157,19 +3187,34 @@
             @staticmethod 
             def bytes_to_string(value: bytes) -> str:
                 return value.decode("utf-8")
             
         class STATISTICS:
 
             @staticmethod
-            def for_chiller_filter() -> TimeSeriesStatistics:
-                events_result: Result[list[EventDS]] = PIH.RESULT.EVENTS.get(*PIH.EVENT.BUILDER.action_was_done(A.CT_A.CHILLER_FILTER_CHANGING))
+            def by_name(value: str) -> TimeSeriesStatistics | None:
+                def is_equal(value: MATERIALIZED_RESOURCES.TYPES, name: str) -> bool:
+                    return EnumTool.get(value).key_name == name or value.name == name
+                if is_equal(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER_COUNT, value):
+                    return PIH.DATA.STATISTICS.for_chiller_filter()
+                return None
+
+            @staticmethod
+            def for_chiller_filter() -> TimeSeriesStatistics | None:
+                events_result: Result[list[EventDS]] = PIH.RESULT.EVENTS.get(*PIH.EVENT.BUILDER.action_was_done(A.CT_ACT.CHILLER_FILTER_CHANGING))
                 if ResultTool.is_empty(events_result):
                     return None
-                return TimeSeriesStatistics(len(events_result), ResultTool.map(events_result, lambda event: event.timestamp).data)
+                datetime_list: list[datetime] = ResultTool.map(events_result, lambda event: event.timestamp).data
+                distance: list[timedelta] = []
+                for index, _ in enumerate(datetime_list):
+                    if index == len(datetime_list) - 1:
+                        break
+                    value: timedelta = datetime_list[index + 1] - datetime_list[index]
+                    distance.append(int(value.total_seconds()))
+                return TimeSeriesStatistics(len(events_result), datetime_list, distance, min(distance), max(distance), int(sum(distance) / len(distance)))
             
         class CHECK:
 
             @staticmethod
             def polibase_person_has_new_barcode_format(polibase_person: PolibasePerson) -> bool:
                 return not (DataTool.is_empty(polibase_person.barcode) or polibase_person.barcode.find(CONST.POLIBASE.BARCODE.NEW_PREFIX) == -1)
 
@@ -3207,43 +3252,42 @@
                 @staticmethod
                 def chiller_value_valid(value: ChillerIndicationsValue) -> bool:
                     return not DataTool.is_empty(value.temperature)
 
         class FORMAT:
 
             @staticmethod
+            def statistics(type: MATERIALIZED_RESOURCES.TYPES) -> str | None:
+                statistics: TimeSeriesStatistics | None = PIH.DATA.STATISTICS.by_name(type.name)
+                if DataTool.is_none(statistics):
+                    return None
+                count: int = PIH.DATA.MATERIALIZED_RESOURCES.get_count(type)
+                def to_days(value: int) -> int:
+                    return int(value / 60 / 60 / 24)
+                return j(
+                    (
+                        "Осталось по времени (дней):",
+                        f" {CONST.VISUAL.BULLET} Максимально: {count * to_days(statistics.max)}",
+                        f" {CONST.VISUAL.BULLET} Минимально: {count * to_days(statistics.min)}",
+                        f" {CONST.VISUAL.BULLET} В среднем: {count * to_days(statistics.avg)}",
+                    ),
+                    "\n"
+                )
+
+
+            @staticmethod
             def yes_no(value: bool, symbolic: bool = False) -> str:
-                c = DataTool.if_check
-                return c(value, c(symbolic, "✅", "Да"), c(symbolic, "❌", "Нет"))
+                c: Callable[[bool, Callable[[None], Any | None] | Any, Callable[[None], Any | None] | Any], Any] = DataTool.check
+                return c(value, c(symbolic, CONST.VISUAL.YES, "Да"), c(symbolic, CONST.VISUAL.NO, "Нет"))
 
             @staticmethod
             def size(value: int) -> str:
                 return str(int(value / 1024 / 1024 / 1024 )) + " Гб"
 
             @staticmethod
-            def printer_report(printer_report: PrinterReport, title_label_function: Callable[[str], str] = lambda value: value) -> str:
-                report_list: list[str] = []
-                if printer_report.name != -401:
-                    name: str = printer_report.ip.split('.')[0]
-                    report_list.append(f"{title_label_function('Модель')}: {printer_report.model}\n{title_label_function('Название')}: {name}\n{title_label_function('Описание')}: {printer_report.description}")
-                    admin_description_list: list[str] = ("" or printer_report.adminDescription).split(",")
-                    if "infoless" not in admin_description_list:
-                        for item in (("Тонер", printer_report.get_toner), None if "drumless" in admin_description_list else ("Драм-юнит", printer_report.get_drum)  ):
-                            if DataTool.is_not_none(item):
-                                report_list.append(f"\n {A.CT_V.BULLET} {title_label_function(item[0])}")
-                                action: Callable[[str], str] = item[1]
-                                report_list += [f"   {title_label_function(color.upper())}: %d%%" % action(color) for color in (["k"] if "bw" in admin_description_list else ["c", "m", "y", "k"])]
-                else:
-                    if not printer_report.accessable:
-                        report_list.append("Принтер недоступен")
-                    else:
-                        report_list.append("Принтер доступен")
-                return "\n".join(report_list)
-
-            @staticmethod
             def format(value: str) -> str:
                 fields: list[str] = [name for _, name, _, _ in Formatter().parse(value) if name]
                 #my_fields: list[str] = DataTool.to_list(DATA.FORMATTER)
                 formatter: dict[str, str] = {}
                 for field_item in fields:
                     #if field_item in my_fields:
                     formatter[field_item] = PIH.DATA.FORMAT.by_formatter_name(field_item, None)
@@ -3266,15 +3310,15 @@
                     result = value.name
                 else:
                     result = str(value)
                 if escaped_string:
                     if isinstance(value, (str, datetime, Enum)):
                         result = f"'{result}'"
                     if isinstance(value, dict):
-                        result = f"'{DataTool.represent(value, False)}'"
+                        result = f"'{DataTool.rpc_represent(value, False)}'"
                 return DataTool.check_not_none(mapper, lambda: mapper(result), result)
                 
             @staticmethod
             def host(value: str, reverse: bool = False) -> str:
                 host_start: str = r"\\"
                 if reverse:
                     if value.startswith(host_start):
@@ -3361,15 +3405,15 @@
                 return PIH.DATA.FORMAT.telephone_number(value, CONST.INTERNATIONAL_TELEPHONE_NUMBER_PREFIX)
 
             @staticmethod
             def email(value: str, add_default_domain: bool = False, remove_restricted_symbols: bool = False) -> str:
                 if add_default_domain and value.find("@") == -1:
                     return PIH.DATA.FORMAT.email("@".join((value, CONST.SITE_URL)))
                 if remove_restricted_symbols:
-                    for char in "\"(),:;<>[\\]":
+                    for char in "\"(),:;<>[\\] ":
                         value = value.replace(char, "")
                 return value#.lower()
 
             @staticmethod
             def name(value: str, remove_non_alpha: bool = False, name_part_minimal_length: int | None = None) -> str:
                 name_part_list: list[str] = list(
                     filter(lambda item: len(item) > (0 if name_part_minimal_length is None else name_part_minimal_length - 1), value.split(" ")))
@@ -3505,22 +3549,22 @@
             def person_by_pin(value: int, test: bool | None = None) -> PolibasePerson:
                 return PIH.RESULT.POLIBASE.person_by_pin(value, test).data
 
             @staticmethod
             def duplicate_persons_by_person(person: PolibasePerson, check_for_birth: bool = True) -> list[PolibasePerson]:
                 def check_function(check_person: PolibasePerson) -> bool:
                     return check_person.pin != person.pin and (not check_for_birth or check_person.Birth == person.Birth)
-                return ResultTool.get_first_element(ResultTool.filter(PIH.RESULT.POLIBASE.persons_by_full_name(person.FullName), lambda item: check_function(item)))
+                return ResultTool.get_first_item(ResultTool.filter(PIH.RESULT.POLIBASE.persons_by_full_name(person.FullName), lambda item: check_function(item)))
             
             @staticmethod
             def unique_by_telephone(value: str) -> PolibasePerson:
                 value = PIH.DATA.FORMAT.telephone_number(value)
                 def check_function(check_person: PolibasePerson) -> bool:
                     return PIH.DATA.FORMAT.telephone_number(check_person.telephoneNumber) == value
-                return ResultTool.get_first_element(ResultTool.filter(PIH.RESULT.POLIBASE.person_by_telephone_number(value), lambda item: check_function(item)))
+                return ResultTool.get_first_item(ResultTool.filter(PIH.RESULT.POLIBASE.person_by_telephone_number(value), lambda item: check_function(item)))
 
             @staticmethod
             def duplicate_persons_by_person_pin(value: int, check_birth: bool = True) -> list[PolibasePerson]:
                 try:
                     return PIH.DATA.POLIBASE.duplicate_persons_by_person(PIH.RESULT.POLIBASE.person_by_pin(value).data, check_birth)
                 except NotFound as error:
                     return None
@@ -3551,23 +3595,23 @@
             return os.getppid()
 
     class RESULT(ResultTool):
 
         class EVENTS:
 
            @staticmethod
-           def get(value: Events, parameters: dict | None = None) -> Result[list[EventDS]]:
+           def get(value: Events, parameters: tuple[Any] | None = None) -> Result[list[EventDS]]:
                 def extractor(data: Any) -> EventDS:
                     result: EventDS = DataTool.fill_data_from_source(EventDS(), data)
                     #from json string to python object
                     result.parameters = DataTool.rpc_unrepresent(result.parameters)
                     if isinstance(result.timestamp, str):
                         result.timestamp = DateTimeTool.datetime_from_string(result.timestamp)
                     return result
-                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_event, EventDS(value.name, PIH.EVENT.BUILDER.create_parameters_map(value, parameters or {}, check_for_parameters_count = False))), extractor)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_event, EventDS(value.name, PIH.EVENT.BUILDER.create_parameters_map(value, parameters, check_for_parameters_count = False))), extractor)
 
         class NOTES:
     
             @staticmethod
             def by_name(name: str) -> Result[Note]:
                 id: str = DataTool.rpc_unrepresent(PIH.SERVICE.call_command(
                     ServiceCommands.get_gkeep_item_id, (name, )))
@@ -3755,15 +3799,15 @@
                 except NotFound:
                     detail: str = f"Компьютер с параметром поиска {value} не найден"
                     raise NotFound(detail)
 
             @staticmethod
             def by_name(value: str) -> Result[Workstation]:
                 value = PIH.DATA.FORMAT.string(value).lower()
-                result: Result[Workstation] = ResultTool.with_first_element(ResultTool.filter(
+                result: Result[Workstation] = ResultTool.with_first_item(ResultTool.filter(
                     PIH.RESULT.WORKSTATION.all(), lambda item: item.name.lower() == value))
                 if ResultTool.is_empty(result):
                     raise NotFound(f"Компьютер с именем {value} не найден")
                 return result
 
             @staticmethod
             def all() -> Result[list[Workstation]]:
@@ -3891,78 +3935,80 @@
                 def filter_by_server_name(printer_list: list[PrinterADInformation]) -> list[PrinterADInformation]:
                     return list(filter(lambda item: item.serverName == CONST.HOST.PRINTER_SERVER.NAME, printer_list))
                 result: Result[list[PrinterADInformation]] = DataTool.to_result(
                     PIH.SERVICE.call_command(ServiceCommands.get_printers), PrinterADInformation)
                 return Result(result.fields, filter_by_server_name(result.data))
 
             @staticmethod
-            def report(send_to_log: bool = True) -> Result[list[PrinterReport]]:
-                return DataTool.to_result(
-                    PIH.SERVICE.call_command(ServiceCommands.printers_report, send_to_log), PrinterReport)
-
-            """ @staticmethod
-            def status(redirect_to_log: bool = True) -> Result[list[PrinterStatus]]:
+            def report() -> Result[list[PrinterReport]]:
                 return DataTool.to_result(
-                    PIH.SERVICE.call_command(ServiceCommands.printers_status, redirect_to_log), PrinterStatus) """
+                    PIH.SERVICE.call_command(ServiceCommands.printers_report), PrinterReport)
 
         class MARK:
 
             @staticmethod
             def by_tab_number(value: str) -> Result[Mark]:
                 result: Result[Mark] = DataTool.to_result(
                     PIH.SERVICE.call_command(ServiceCommands.get_mark_by_tab_number, value), Mark)
                 if ResultTool.is_empty(result):
                     details: str = f"Карта доступа с номером '{value}' не найдена"
                     raise NotFound(details)
                 return result
 
             @staticmethod
-            def person_divisions() -> Result[list[Mark]]:
-                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_person_divisions), MarkDivision)
+            def by_division(division_or_id: PersonDivision | int) -> Result[list[Mark]]:
+                division_id: int = DataTool.check(isinstance(
+                    division_or_id, PersonDivision), lambda: division_or_id.id, division_or_id)
+                return DataTool.to_result(
+                    PIH.SERVICE.call_command(ServiceCommands.get_mark_list_by_division_id, division_id), Mark)
+
+            @staticmethod
+            def person_divisions() -> Result[list[PersonDivision]]:
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_mark_person_division_list), PersonDivision)
 
             @staticmethod
             def by_name(value: str, first_item: bool = False) -> Result[list[Mark]]:
                 return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_mark_by_person_name, value), Mark, first_item)
 
             @staticmethod
             def by_full_name(value: FullName, first_item: bool = False) -> Result[list[Mark]]:
                 return PIH.RESULT.MARK.by_name(FullNameTool.fullname_from_string(value), first_item)
 
             @staticmethod
             def temporary_list() -> Result[list[TemporaryMark]]:
-                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_temporary_marks), TemporaryMark)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_temporary_mark_list), TemporaryMark)
 
             @staticmethod
             def by_any(value: str) -> Result[list[Mark]]:
                 if PIH.CHECK.MARK.tab_number(value):
                     return ResultTool.as_list(PIH.RESULT.MARK.by_tab_number(value))
                 elif PIH.CHECK.name(value, True):
                     return PIH.RESULT.MARK.by_name(value)
                 return Result()
 
             @staticmethod
             def free_list(show_with_guest_marks: bool = False) -> Result[list[Mark]]:
                 result: Result[list[Mark]] = DataTool.to_result(
-                    PIH.SERVICE.call_command(ServiceCommands.get_free_marks), Mark)
+                    PIH.SERVICE.call_command(ServiceCommands.get_free_mark_list), Mark)
 
                 def filter_function(item: Mark) -> bool:
                     return EnumTool.get(MarkType, item.type) != MarkType.GUEST
                 return result if show_with_guest_marks else ResultTool.filter(result, filter_function)
 
             @staticmethod
             def free_marks_by_group_id(value: int) -> Result[list[Mark]]:
-                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_free_marks_by_group_id, value), Mark)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_free_mark_list_by_group_id, value), Mark)
 
             @staticmethod
             def free_marks_group_statistics(show_guest_marks: bool | None = None) -> Result[list[MarkGroupStatistics]]:
-                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_free_marks_group_statistics, show_guest_marks), MarkGroupStatistics)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_free_mark_group_statistics_list, show_guest_marks), MarkGroupStatistics)
 
             @staticmethod
             def all() -> Result[list[Mark]]:
-                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_all_persons), Mark)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_mark_list), Mark)
 
             @staticmethod
             def temporary_mark_owner(mark: Mark) -> Result[Mark]:
                 return DataTool.check(mark is not None and EnumTool.get(MarkType, mark.type) == MarkType.TEMPORARY, lambda: DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_owner_mark_for_temporary_mark, mark.TabNumber), Mark), None)
 
             @staticmethod
             def temporary_mark_owner_by_tab_number(value: str) -> Result[Mark]:
@@ -3978,15 +4024,15 @@
 
                 @staticmethod
                 def by(value: PolibasePersonVisitNotification) -> Result[list[PolibasePersonVisitNotification]]:
                     return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.search_polibase_person_visit_notifications, value), PolibasePersonVisitNotification)
 
                 @staticmethod
                 def by_message_id(value: int) -> Result[PolibasePersonVisitNotification]:
-                    return ResultTool.with_first_element(PIH.RESULT.POLIBASE.NOTIFICATION.by(PolibasePersonVisitNotification(messageID=value)))
+                    return ResultTool.with_first_item(PIH.RESULT.POLIBASE.NOTIFICATION.by(PolibasePersonVisitNotification(messageID=value)))
 
                 class CONFIRMATION:
                     
                     @staticmethod
                     def by(recipient: str, sender: str) -> Result[PolibasePersonNotificationConfirmation]:
                         return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.search_polibase_person_notification_confirmation, PolibasePersonNotificationConfirmation(recipient, sender)), PolibasePersonNotificationConfirmation)
 
@@ -4158,15 +4204,15 @@
                     return PIH.RESULT.USER.by_login(workstation.samAccountName)
                 else:
                     raise PIH.ERROR.USER.get_not_found_error(
                         "внутренним номером телефона", True, str(value))
 
             @staticmethod
             def by_polibase_pin(value: int) -> Result[User]:
-                return ResultTool.with_first_element(PIH.RESULT.USER.by_name(PIH.RESULT.POLIBASE.person_by_pin(value).data.FullName))
+                return ResultTool.with_first_item(PIH.RESULT.USER.by_name(PIH.RESULT.POLIBASE.person_by_pin(value).data.FullName))
 
             @staticmethod
             def by_workstation_name(name: str) -> Result[User]:
                 name = name.lower()
                 user_workstation: Workstation = DataTool.to_result(PIH.SERVICE.call_command(
                     ServiceCommands.get_user_by_workstation, name), Workstation, True).data
                 if DataTool.is_empty(user_workstation):
@@ -4274,14 +4320,21 @@
 
         class EVENTS:
 
             @staticmethod
             def has(value: Events | None, parameters: tuple[Any] | None) -> bool:
                 return not ResultTool.is_empty(PIH.RESULT.EVENTS.get(value, parameters))
 
+            @staticmethod
+            def timeouted(event: Events, parameters: dict | None, timeout: int) -> bool:
+                event_ds: EventDS | None = A.R.get_first_item(
+                    A.R.sort(A.R_E.get(event, parameters), lambda item: item.timestamp, reserve=True))
+                return DataTool.is_none(event_ds) or (
+                    DateTimeTool.now() - event_ds.timestamp).seconds > timeout
+
         class SETTINGS:
     
             @staticmethod
             def by_time(current: datetime, settings: SETTINGS) -> bool:
                 return DateTimeTool.is_equal_by_time(current, PIH.SETTINGS.to_datetime(settings))
 
         class INDICATION:
@@ -5052,16 +5105,35 @@
             @staticmethod
             def send(message: DelayedMessage, high_priority: bool = True) -> bool:
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.send_delayed_message, (PIH.ACTION.MESSAGE.DELAYED.prepeare_message(message), high_priority)))
 
     class CARD_REGISTRY:
 
         @staticmethod
-        def set_folder_for_person(folder_name: str, person: PolibasePerson) -> bool:
-            return PIH.ACTION.POLIBASE.set_card_registry_folder(folder_name, person)
+        def set_folder_for_person(folder_name: str | None, person_or_pin: PolibasePerson | int, already_set: bool = False) -> bool:
+            result: bool = already_set or PIH.ACTION.POLIBASE.set_card_registry_folder(folder_name, person_or_pin)
+            event_builder = PIH.EVENT.BUILDER.polibase_person_set_card_registry_folder
+            if result:
+                if DataTool.is_empty(folder_name):
+                    A.A_E.remove(*event_builder(None, person_or_pin))
+                    result = True
+                else:
+                    event_ds: EventDS | None = ResultTool.get_first_item(PIH.RESULT.EVENTS.get(
+                        *event_builder(None, person_or_pin)))
+                    allow_to_add: bool = False
+                    if DataTool.is_not_none(event_ds):
+                        card_registry_folder: str = event_ds.parameters[FIELD_NAME_COLLECTION.CARD_REGISTRY_FOLDER]
+                        allow_to_add = card_registry_folder != folder_name
+                        if allow_to_add:
+                            PIH.ACTION.EVENTS.remove(
+                                *event_builder(card_registry_folder, person_or_pin))
+                    else:
+                        PIH.EVENT.send(
+                            *event_builder(folder_name, person_or_pin))
+            return result
 
         @staticmethod
         def start_card_sorting_for(folder_name: str) -> None:
             event_builder_function: Callable[[None], Events | tuple[Events, tuple[Any]]] = PIH.EVENT.BUILDER.card_registry_folder_start_card_sorting
             PIH.ACTION.EVENTS.remove(
                 *event_builder_function(folder_name))
             PIH.ACTION.EVENTS.remove(
@@ -5088,15 +5160,16 @@
             if folder_is_sorted:
                 ResultTool.sort(polibase_person_list_result, PIH.DATA.POLIBASE.sort_person_list_by_pin)
             else:
                 polibase_person_list_map: dict[int, PolibasePerson] = {person.pin : person for person in polibase_person_list_result.data}
                 polibase_person_list: list[PolibasePerson] = []
                 polibase_person_pin_list: list[int] = PIH.CARD_REGISTRY.persons_pin_by_folder(folder_name)
                 for pin in polibase_person_pin_list:
-                    polibase_person_list.append(polibase_person_list_map[pin])
+                    if DataTool.is_in(polibase_person_list_map, pin):
+                        polibase_person_list.append(polibase_person_list_map[pin])
                 polibase_person_list_result.data = polibase_person_list
             return polibase_person_list_result
 
         @staticmethod
         def persons_pin_by_folder(folder_name: str) -> list[int]:
             def map_function(value: EventDS | PolibasePerson) -> int:
                 if isinstance(value, PolibasePerson):
@@ -5116,43 +5189,49 @@
             @staticmethod
             def listen(value: str) -> bool:
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.listen_for_new_files, (value, )))   
 
         class ACTIONS:
 
             @staticmethod
-            def done(action: Actions | str, user_login: str) -> bool | None:
-                user: User = A.R_U.by_login(user_login, True, True).data
+            def was_done(action: Actions | str, user_login_or_user: str | User | None = None) -> bool | None:
+                user: User | None = None
+                if isinstance(user_login_or_user, User):
+                    user = user_login_or_user
+                if A.D_C.empty(user_login_or_user) or isinstance(user_login_or_user, str):
+                    user = A.R_U.by_login(user_login_or_user or AD.USER.ADMINISTRATOR, True, True).data
                 _action: Actions | None = PIH.DATA.ACTIONS.get(action)
                 if DataTool.is_none(_action):
                     return None
-                PIH.EVENT.send(Events.ACTION_WAS_DONE, (_action.value.description, _action.name, user.name, user_login))
+                PIH.EVENT.send(Events.ACTION_WAS_DONE, (EnumTool.get(_action).description, _action.name, user.name, user.samAccountName))
                 return True
 
             @staticmethod
             def have_to_be_done(action: Actions | str) -> bool | None:
                 _action: Actions | None = PIH.DATA.ACTIONS.get(action)
                 if DataTool.is_none(_action):
                     return None
-                PIH.EVENT.send(Events.ACTION_HAVE_TO_BE_DONE, (_action.name, _action.value.description))
+                PIH.EVENT.send(Events.ACTION_HAVE_TO_BE_DONE, (_action.name, EnumTool.get(_action).description))
                 return True
 
         class EVENTS:
     
             @staticmethod
-            def register(value: Events, parameters: dict | None = None) -> bool:
+            def register(value: Events, parameters: dict[str, Any] | None = None, remove_before: bool = False) -> bool:
+                if remove_before:
+                    PIH.ACTION.EVENTS.remove(value, parameters)
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.register_event, (EventDS(value.name, parameters, DateTimeTool.now()), )))
 
             @staticmethod
-            def update(value: Events, parameter_for_search: tuple[Any], parameters: tuple[Any]) -> bool:
-                return PIH.ACTION.EVENTS.remove(value, parameter_for_search) and PIH.ACTION.EVENTS.register(value, PIH.EVENT.BUILDER.create_parameters_map(value, parameters))
+            def update(value: Events, parameter_for_search: tuple[Any], parameters_for_set: tuple[Any]) -> bool:
+                return PIH.ACTION.EVENTS.remove(value, parameter_for_search) and PIH.ACTION.EVENTS.register(value, PIH.EVENT.BUILDER.create_parameters_map(value, parameters_for_set))
 
             @staticmethod
-            def remove(value: Events, parameters: tuple[Any]) -> bool:
-                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.remove_event, EventDS(value.name, PIH.EVENT.BUILDER.create_parameters_map(value, parameters, check_for_parameters_count=False))))
+            def remove(value: Events, parameters: tuple[Any] | dict[str, Any]) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.remove_event, EventDS(value.name, DataTool.check(isinstance(parameters, dict), parameters, lambda: PIH.EVENT.BUILDER.create_parameters_map(value, parameters, check_for_parameters_count=False)))))
 
         class NOTES:
         
             @staticmethod
             def create(name: str, note: Note) -> bool:
                 id: str | None = DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_note, (note, )))
                 if DataTool.is_empty(id):
@@ -5390,32 +5469,16 @@
                     return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.update_polibase_person_information_quest, (value, search_critery)))
 
             @staticmethod
             def create_barcode_for_person(person_or_pin: PolibasePerson | int, test: bool | None = None) -> bool:
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_barcode_for_polibase_person, (PIH.RESULT.POLIBASE._person_pin(person_or_pin), test)))
 
             @staticmethod
-            def set_card_registry_folder(value: str, person: PolibasePerson, test: bool | None = None) -> bool:
-                result: bool = DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_polibase_person_card_folder_name, (value, person.pin, test)))
-                if result:
-                    event_ds: EventDS | None = ResultTool.get_first_element(PIH.RESULT.EVENTS.get(
-                        *PIH.EVENT.BUILDER.polibase_person_set_card_registry_folder(None, person)))
-                    allow_to_add: bool = False
-                    if DataTool.is_not_none(event_ds):
-                        card_registry_folder: str = event_ds.parameters[FIELD_NAME_COLLECTION.CARD_REGISTRY_FOLDER]
-                        allow_to_add = card_registry_folder != value
-                        if allow_to_add:
-                            PIH.ACTION.EVENTS.remove(
-                                *PIH.EVENT.BUILDER.polibase_person_set_card_registry_folder(card_registry_folder, person))
-                    else:
-                        allow_to_add = True
-                    if allow_to_add:
-                        PIH.EVENT.send(
-                            *PIH.EVENT.BUILDER.polibase_person_set_card_registry_folder(value, person))
-                return result
+            def set_card_registry_folder(value: str | None, person_or_pin: PolibasePerson | int, test: bool | None = None) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_polibase_person_card_folder_name, (value, PIH.RESULT.POLIBASE._person_pin(person_or_pin), test)))
 
             @staticmethod
             def set_email(value: str, person: PolibasePerson, test: bool | None = None) -> bool:
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_polibase_person_email, (value, person.pin, test)))
             
             @staticmethod
             def set_telephone_number(index: int, value: str, person: PolibasePerson, test: bool | None = None) -> bool:
@@ -5584,16 +5647,16 @@
 
     R = root.RESULT
     D = root.DATA
     D_V = D.VARIABLE
     D_TN = D.TELEPHONE_NUMBER
     D_MR = D.MATERIALIZED_RESOURCES
     D_FL = D.FILTER
-    D_E = D.EXTRACT
-    D_E_E = D_E.EVENT
+    D_Ex = D.EXTRACT
+    D_Ex_E = D_Ex.EVENT
     D_M = D.MARK
     D_C = D.CHECK
     D_STAT = D.STATISTICS
     A = root.ACTION
     A_D = A.DOCUMENTS
     A_QR = A.QR_CODE
     A_I = A.INDICATION
@@ -5734,15 +5797,15 @@
     CT_ME = CT.MESSAGE
     CT_ME_WH = CT_ME.WHATSAPP
     CT_ME_WH_W = CT_ME_WH.WAPPI
     CT_L_ME_F = LogMessageFlags
     CT_L_ME_CH = LogMessageChannels
     CT_V = CT.VISUAL
     CT_E = Events
-    CT_A = Actions
+    CT_ACT = Actions
     CT_MD = MEDICAL_DOCUMENT
     CT_MD_DT = CT_MD.DIRECTION_TYPES
     CT_DS = CT.DATA_STORAGE
     CT_FNC = FIELD_NAME_COLLECTION
     CT_FCA = FIELD_COLLECTION_ALIAS
     CT_UP = USER_PROPERTIES
     CT_AD = AD
```

### Comparing `pih-1.46231/pih/rpc.py` & `pih-1.47001/pih/rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                         self.service.create_subscribtions(parameter_list.next(ServiceInformationBase()))
                         return True
                     if sc == SC.update_service_information:
                         A.SRV_A.update_service_information(parameter_list.next_as_list(
                             ServiceInformation), parameter_list.next())
                         return True
                     if sc == SC.heart_beat:
-                        date_string: str = A.D_E.parameter_list(parameter_list).get()
+                        date_string: str = A.D_Ex.parameter_list(parameter_list).get()
                         date: datetime = datetime.strptime(date_string, CONST.ISO_DATETIME_FORMAT)
                         parameter_list.set(0, date)
                         RPC.SESSION.life_time = date - RPC.SESSION.start_time
                 return None if A.D_C.empty(self.call_handler) else self.call_subscribers_after(sc, parameter_list, self.call_handler(
                     command_name, self.call_subscribers_before(sc, parameter_list), context))
             except Exception as error:
                 A.ER.global_except_hook(type(error), error, error.__traceback__)
@@ -378,15 +378,15 @@
             self.server.stop(0)
     
     class CommandClient():
 
         def __init__(self, host: str, port: int):
             self.stub = pb2_grpc.UnaryStub(grpc.insecure_channel(f"{host}:{port}"))
 
-        def call_command(self, name: str, parameters: str = None, timeout: int = None):
+        def call_command(self, name: str, parameters: str | None = None, timeout: int = None):
             return self.stub.rpcCallCommand(pb2.rpcCommand(name=name, parameters=parameters), timeout=timeout)
 
     @staticmethod
     def ping(role_or_information: ServiceRoles | ServiceInformationBase) -> ServiceInformation:
         if DEBUG:
             from pih import A
         else:
```

### Comparing `pih-1.46231/pih/rpcCommandCall_pb2.py` & `pih-1.47001/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.46231/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47001/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.46231/pih/rpc_collection.py` & `pih-1.47001/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.46231/pih/rpc_const.py` & `pih-1.47001/pih/rpc_const.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,26 +70,26 @@
     remove_user: int = auto()
     get_all_workstation_description: int = auto()
     get_all_workstations: int = auto()
     get_workstation_list_by_user_login: int = auto()
     get_user_by_workstation: int = auto()
     #Printer
     printers_report: int = auto()
-    #printers_status: int = auto()
     #Orion
-    get_free_marks: int = auto()
-    get_temporary_marks: int = auto()
-    get_person_divisions: int = auto()
+    get_free_mark_list: int = auto()
+    get_temporary_mark_list: int = auto()
+    get_mark_person_division_list: int = auto()
     get_time_tracking: int = auto()
-    get_all_persons: int = auto()
+    get_mark_list: int = auto()
     get_owner_mark_for_temporary_mark: int = auto()
     get_mark_by_tab_number: int = auto()
     get_mark_by_person_name: int = auto()
-    get_free_marks_group_statistics: int = auto()
-    get_free_marks_by_group_id: int = auto()
+    get_free_mark_group_statistics_list: int = auto()
+    get_free_mark_list_by_group_id: int = auto()
+    get_mark_list_by_division_id: int = auto()
     set_full_name_by_tab_number: int = auto()
     set_telephone_by_tab_number: int = auto()
     check_mark_free: int = auto()
     create_mark: int = auto()
     remove_mark_by_tab_number: int = auto()
     make_mark_as_free_by_tab_number: int = auto()
     make_mark_as_temporary: int = auto()
```

### Comparing `pih-1.46231/pih/service_example.py` & `pih-1.47001/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.46231/pih/tools.py` & `pih-1.47001/pih/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,30 @@
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
 from pih.const import PASSWORD_GENERATION_ORDER, FIELD_COLLECTION_ALIAS, CONST
 from pih.collection import R, T, FieldItem, FieldItemList, FullName, Result, User, PolibasePerson
 
+def i(value: str) -> str:
+    if not DataTool.is_empty(value) and value.find("_") == -1:
+        return f"_{value}_"
+    return value or ""
+
+def b(value: str) -> str:
+    if not DataTool.is_empty(value) and value.find("*") == -1:
+        return f"*{value}*"
+    return value or ""
+
+def nl(value: str, count: int = 1) -> str:
+    return value + "\n"*count
+
+def j(value: tuple | list[str], splitter: str = "") -> str:
+    return splitter.join(value)
+
 class EnumTool:
 
     @staticmethod
     def get(cls: Enum | Any, key: str | None = None, default_value: Any | None = None, return_value: bool = True) -> Any | None:
         if return_value and DataTool.is_empty(key):
             if isinstance(cls, Enum):
                 return cls.value
@@ -70,20 +86,16 @@
         if data is None:
             return default_value
         if len(data) <= index:
             return default_value
         return data[index]
 
     @staticmethod
-    def represent(data: dict, ensure_ascii: bool = True) -> str:
-        return json.dumps(data, cls=PIHEncoder, ensure_ascii=ensure_ascii)
-
-    @staticmethod
-    def rpc_represent(data: dict) -> str | None:
-        return json.dumps(data, cls=PIHEncoder) if data is not None else None
+    def rpc_represent(data: dict | None, ensure_ascii: bool = True) -> str | None:
+        return json.dumps(data, cls=PIHEncoder, ensure_ascii=ensure_ascii) if data is not None else None
 
     @staticmethod
     def rpc_unrepresent(value: str | None) -> dict | None:
         return None if DataTool.is_empty(value) else json.loads(value) 
 
     @staticmethod
     def to_result(result_string: str, class_type_holder: Any | Callable[[Any], Any] | None = None, first_data_item: bool = False) -> Result:
@@ -186,19 +198,19 @@
         return DataTool.if_check(not DataTool.is_empty(value), lambda: value[0], default_value) if isinstance(value, (list, tuple)) else value or default_value
 
     @staticmethod
     def if_check(check_value: bool, true_value: Callable[[None], Any | None] | Any, false_value: Callable[[None], Any | None] | Any | None = None) -> Any | None:
         return (true_value() if callable(true_value) else true_value) if check_value else (false_value() if not DataTool.is_none(false_value) and callable(false_value) else false_value)
 
     @staticmethod
-    def if_is_in(value: Any, arg_name: str, default_value:  Any | Callable[[None], Any | None] | None = None) -> Any | None:
+    def if_is_in(value: Any, arg_name: Any, default_value:  Any | Callable[[None], Any | None] | None = None) -> Any | None:
         return DataTool.if_check(DataTool.is_in(value, arg_name), lambda: value[arg_name], default_value)
     
     @staticmethod
-    def is_in(value: Any, arg_name: str) -> bool:
+    def is_in(value: Any, arg_name: Any) -> bool:
         return arg_name in value
 
     @staticmethod
     def check(value: bool, true_value: Callable[[None], Any | None] | Any, false_value: Callable[[None], Any | None] | Any = None) -> Any | None:
         return (true_value() if callable(true_value) else true_value) if value else (false_value() if callable(false_value) else false_value)
 
     @staticmethod
@@ -476,20 +488,20 @@
         return result
 
     @staticmethod
     def is_empty(result: Result | None) -> bool:
         return DataTool.is_none(result) or DataTool.is_empty(result.data)
 
     @staticmethod
-    def get_first_element(result: Result[list[T] | T], default_value: Any | None = None) -> T | Any | None:
+    def get_first_item(result: Result[list[T] | T], default_value: Any | None = None) -> T | Any | None:
         return DataTool.get_first_item(result.data, default_value)
 
     @staticmethod
-    def with_first_element(result: Result[T], default_value: Any = None) -> Result[T]:
-        result.data = ResultTool.get_first_element(result, default_value)
+    def with_first_item(result: Result[list[T] | T], default_value: Any | None = None) -> Result[T]:
+        result.data = ResultTool.get_first_item(result, default_value)
         return result
 
     @staticmethod
     def to_string(result: Result[T], use_index: bool = True, item_separator: str = "\n", value_separator: str | None = None, show_caption: bool = True) -> str:
         result_string_list: list[str] = []
         data: list = DataTool.as_list(result.data)
         item_result_string_list: list[str] = None
```

### Comparing `pih-1.46231/pih/widgets.py` & `pih-1.47001/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.46231/pih_setup.py` & `pih-1.47001/pih_setup.py`

 * *Files identical despite different names*

