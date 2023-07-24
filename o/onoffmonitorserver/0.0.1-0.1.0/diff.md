# Comparing `tmp/onoffmonitorserver-0.0.1-py3-none-any.whl.zip` & `tmp/onoffmonitorserver-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,18 @@
-Zip file size: 6431 bytes, number of entries: 17
+Zip file size: 6595 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 17:32 onoffmonitorserver/__init__.py
--rw-r--r--  2.0 unx      107 b- defN 23-Jul-06 17:32 onoffmonitorserver/admin.py
+-rw-r--r--  2.0 unx      137 b- defN 23-Jul-22 16:30 onoffmonitorserver/admin.py
 -rw-r--r--  2.0 unx      204 b- defN 23-Jul-06 17:32 onoffmonitorserver/apps.py
 -rw-r--r--  2.0 unx      365 b- defN 23-Jul-06 17:32 onoffmonitorserver/filters.py
--rw-r--r--  2.0 unx      862 b- defN 23-Jul-06 17:32 onoffmonitorserver/models.py
+-rw-r--r--  2.0 unx     1561 b- defN 23-Jul-22 16:30 onoffmonitorserver/models.py
 -rw-r--r--  2.0 unx      333 b- defN 23-Jul-06 17:32 onoffmonitorserver/permissions.py
--rw-r--r--  2.0 unx      659 b- defN 23-Jul-06 17:32 onoffmonitorserver/serializers.py
+-rw-r--r--  2.0 unx     1106 b- defN 23-Jul-22 16:30 onoffmonitorserver/serializers.py
 -rw-r--r--  2.0 unx       60 b- defN 23-Jul-06 17:32 onoffmonitorserver/tests.py
--rw-r--r--  2.0 unx      233 b- defN 23-Jul-06 17:32 onoffmonitorserver/urls.py
--rw-r--r--  2.0 unx     1019 b- defN 23-Jul-06 17:32 onoffmonitorserver/views.py
--rw-r--r--  2.0 unx     1514 b- defN 23-Jul-06 17:32 onoffmonitorserver/migrations/0001_initial.py
--rw-r--r--  2.0 unx      326 b- defN 23-Jul-06 17:32 onoffmonitorserver/migrations/0002_remove_status_user.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jul-22 16:30 onoffmonitorserver/urls.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Jul-22 16:41 onoffmonitorserver/views.py
+-rw-r--r--  2.0 unx     2205 b- defN 23-Jul-22 16:30 onoffmonitorserver/migrations/0001_initial.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 17:32 onoffmonitorserver/migrations/__init__.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Jul-07 12:04 onoffmonitorserver-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 12:04 onoffmonitorserver-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-07 12:04 onoffmonitorserver-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1495 b- defN 23-Jul-07 12:04 onoffmonitorserver-0.0.1.dist-info/RECORD
-17 files, 8348 bytes uncompressed, 3917 bytes compressed:  53.1%
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-24 16:11 onoffmonitorserver-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 16:11 onoffmonitorserver-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-24 16:11 onoffmonitorserver-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-24 16:11 onoffmonitorserver-0.1.0.dist-info/RECORD
+16 files, 10990 bytes uncompressed, 4269 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -27,26 +27,23 @@
 
 Filename: onoffmonitorserver/views.py
 Comment: 
 
 Filename: onoffmonitorserver/migrations/0001_initial.py
 Comment: 
 
-Filename: onoffmonitorserver/migrations/0002_remove_status_user.py
-Comment: 
-
 Filename: onoffmonitorserver/migrations/__init__.py
 Comment: 
 
-Filename: onoffmonitorserver-0.0.1.dist-info/METADATA
+Filename: onoffmonitorserver-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: onoffmonitorserver-0.0.1.dist-info/WHEEL
+Filename: onoffmonitorserver-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: onoffmonitorserver-0.0.1.dist-info/top_level.txt
+Filename: onoffmonitorserver-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: onoffmonitorserver-0.0.1.dist-info/RECORD
+Filename: onoffmonitorserver-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## onoffmonitorserver/admin.py

```diff
@@ -1,4 +1,8 @@
 from django.contrib import admin
 from . import models
 
-admin.site.register((models.Device, models.Status))
+admin.site.register((
+    models.Monitor,
+    models.Device,
+    models.Status
+))
```

## onoffmonitorserver/models.py

```diff
@@ -2,21 +2,39 @@
 Model classes to represent database tables
 """
 from django.conf import settings
 from django.db import models
 from django.utils import timezone
 
 
+class Monitor(models.Model):
+    """
+    Model for storing data about a monitor (such as "garage")
+    """
+    user = models.ForeignKey(settings.AUTH_USER_MODEL,
+                             on_delete=models.CASCADE)
+    name = models.CharField(max_length=100)
+
+    def __str__(self):
+        return f'{self.name} ({self.user})'
+
+
 class Device(models.Model):
     """
     Model for storing data about a device (such as "boiler")
     """
     user = models.ForeignKey(settings.AUTH_USER_MODEL,
                              on_delete=models.CASCADE)
     name = models.CharField(max_length=100)
+    monitor = models.ForeignKey(Monitor, on_delete=models.CASCADE)
+    gpio_pin = models.PositiveSmallIntegerField(
+        verbose_name='GPIO pin on monitor')
+
+    def __str__(self):
+        return f'{self.name} ({self.user})'
 
 
 class Status(models.Model):
     """
     Model for storing the status of a device (on or off) at a given time
     """
     STATUS_CHOICES = (
@@ -24,9 +42,13 @@
         (1, 'On'),
     )
     device = models.ForeignKey(Device, on_delete=models.CASCADE)
     status = models.PositiveSmallIntegerField(
         choices=STATUS_CHOICES, default=0)
     time = models.DateTimeField(default=timezone.now)
 
+    def __str__(self):
+        return f'{self.device} {self.STATUS_CHOICES[int(self.status)][1]}'
+
     class Meta:
+        """Metadata form Status Model"""
         verbose_name_plural = 'Statuses'
```

## onoffmonitorserver/serializers.py

```diff
@@ -1,21 +1,37 @@
 from rest_framework.serializers import ModelSerializer, ValidationError, CurrentUserDefault, HiddenField
 
 from . import models
 
 
-class DeviceSerializer(ModelSerializer):
+class MonitorSerializer(ModelSerializer):
     user = HiddenField(default=CurrentUserDefault())
+
     class Meta:
         model = models.Device
         fields = ['id', 'name', 'user']
 
 
+class DeviceSerializer(ModelSerializer):
+    user = HiddenField(default=CurrentUserDefault())
+
+    def validate(self, attrs):
+        print(attrs)
+        if attrs['monitor'].user != attrs['user']:
+            raise ValidationError('Device owner must be the current user')
+        return super().validate(attrs)
+
+    class Meta:
+        model = models.Device
+        fields = ['id', 'name', 'user', 'monitor', 'gpio_pin']
+
+
 class StatusSerializer(ModelSerializer):
+    user = CurrentUserDefault()
     def validate(self, attrs):
-        if attrs['device'].user != CurrentUserDefault()(self):
+        if attrs['device'].user != self.user(self):
             raise ValidationError('Device owner must be the current user')
         return super().validate(attrs)
 
     class Meta:
         model = models.Status
         fields = ['id', 'device', 'status', 'time']
```

## onoffmonitorserver/urls.py

```diff
@@ -1,9 +1,10 @@
 from rest_framework.routers import DefaultRouter
 
-from .views import DeviceViewSet, StatusViewSet
+from .views import MonitorViewSet, DeviceViewSet, StatusViewSet
 
 router = DefaultRouter()
+router.register('monitor', MonitorViewSet)
 router.register('device', DeviceViewSet)
 router.register('status', StatusViewSet)
 
 urlpatterns = router.urls
```

## onoffmonitorserver/views.py

```diff
@@ -1,26 +1,60 @@
 # pylint:disable=no-member
 from knox.auth import TokenAuthentication
+from rest_framework import status
 from rest_framework.authentication import SessionAuthentication
+from rest_framework.decorators import action
 from rest_framework.permissions import IsAuthenticated
+from rest_framework.response import Response
 from rest_framework.viewsets import ModelViewSet
 
 from . import models
 from .filters import DeviceOwnerFilter, StatusOwnerFilter
 from .permissions import IsDeviceOwner, IsStatusOwner
-from .serializers import DeviceSerializer, StatusSerializer
+from .serializers import MonitorSerializer, DeviceSerializer, StatusSerializer
+
+
+class MonitorViewSet(ModelViewSet):
+    """
+    ViewSet for managing Monitor objects
+    """
+    queryset = models.Monitor.objects.all()
+    serializer_class = MonitorSerializer
+    permission_classes = [IsAuthenticated, IsDeviceOwner]
+    authentication_classes = [SessionAuthentication, TokenAuthentication]
+    filter_backends = [DeviceOwnerFilter]
+
+    @action(methods=['GET'], detail=True, url_path='conf')
+    def device_list(self, request, pk: int):
+        return Response(models.Device.objects.filter(monitor_id=pk).values('id', 'gpio_pin'))
 
 
 class DeviceViewSet(ModelViewSet):
+    """
+    ViewSet for managing Device objects
+    """
     queryset = models.Device.objects.all()
     serializer_class = DeviceSerializer
     permission_classes = [IsAuthenticated, IsDeviceOwner]
     authentication_classes = [SessionAuthentication, TokenAuthentication]
     filter_backends = [DeviceOwnerFilter]
 
 
 class StatusViewSet(ModelViewSet):
+    """
+    ViewSet for managing Status objects
+    """
     queryset = models.Status.objects.all()
     serializer_class = StatusSerializer
     permission_classes = [IsAuthenticated, IsStatusOwner]
     authentication_classes = [SessionAuthentication, TokenAuthentication]
     filter_backends = [StatusOwnerFilter]
+
+    @action(methods=['POST'], detail=False, url_path='n')
+    def create_no_return(self, request):
+        """
+        Create a Status object but don't return the created data
+        """
+        response = super().create(request)
+        response.data = None
+        response.status_code = status.HTTP_204_NO_CONTENT
+        return response
```

## onoffmonitorserver/migrations/0001_initial.py

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2.3 on 2023-07-05 18:58
+# Generated by Django 4.2.3 on 2023-07-14 13:57
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
 
 
@@ -16,24 +16,41 @@
 
     operations = [
         migrations.CreateModel(
             name='Device',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('name', models.CharField(max_length=100)),
-                ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
+                ('gpio_pin', models.PositiveSmallIntegerField(verbose_name='GPIO pin on monitor')),
             ],
         ),
         migrations.CreateModel(
             name='Status',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('status', models.PositiveSmallIntegerField(choices=[(0, 'Off'), (1, 'On')], default=0)),
                 ('time', models.DateTimeField(default=django.utils.timezone.now)),
                 ('device', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='onoffmonitorserver.device')),
-                ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
             ],
             options={
                 'verbose_name_plural': 'Statuses',
             },
         ),
+        migrations.CreateModel(
+            name='Monitor',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=100)),
+                ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
+            ],
+        ),
+        migrations.AddField(
+            model_name='device',
+            name='monitor',
+            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='onoffmonitorserver.monitor'),
+        ),
+        migrations.AddField(
+            model_name='device',
+            name='user',
+            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL),
+        ),
     ]
```

## Comparing `onoffmonitorserver-0.0.1.dist-info/METADATA` & `onoffmonitorserver-0.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: onoffmonitorserver
-Version: 0.0.1
+Version: 0.1.0
 Summary: Django app for monitoring the on/off status of devices
 Author: Joe Greaves
 Project-URL: Homepage, https://github.com/Grvs44/onoffmonitorserver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: <4,>=3.9
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: django (>=4.2.3)
 Requires-Dist: djangorestframework (>=3.14.0)
 Requires-Dist: django-rest-knox (>=4.2.0)
 
 # On/Off Monitor Server
 ## Installation
```

## Comparing `onoffmonitorserver-0.0.1.dist-info/RECORD` & `onoffmonitorserver-0.1.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 onoffmonitorserver/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-onoffmonitorserver/admin.py,sha256=LM2R81_1OgxE8vDn95oMe5QMzevmHaoh9lVFWsWNHJg,107
+onoffmonitorserver/admin.py,sha256=zIKRnR95dyCRkXPMlExPPPX4s3Zk_oClWKxyfxAR1Es,137
 onoffmonitorserver/apps.py,sha256=kPufj7Z9UAxHGq2v6ir3QxPm-vf1R1tKG6o4-CJA_X4,204
 onoffmonitorserver/filters.py,sha256=d1OFS5Mtip2nLS7lvdwtJPrG-ZmfORQjQ8HEl6C4VIo,365
-onoffmonitorserver/models.py,sha256=6sinzCRE2A3myQl6Ph4y8jtsj2qeCEnXPMHy-KWAum0,862
+onoffmonitorserver/models.py,sha256=BWfI-OGECsQR2-s7CvS50nPlrulqOlRXjqgBai73TMA,1561
 onoffmonitorserver/permissions.py,sha256=y-dURrhXm4hJorZ8QBsg51ak-cZ1EaDg-KicePa-R24,333
-onoffmonitorserver/serializers.py,sha256=rCmFH1Mjw2m-FglMP9shdn0eEdh4eT-LzqTCkRsfysI,659
+onoffmonitorserver/serializers.py,sha256=dKP_toieY1Y935DsMmQ-UsA7tBBVhb_qpb_myE6ggvE,1106
 onoffmonitorserver/tests.py,sha256=mrbGGRNg5jwbTJtWWa7zSKdDyeB4vmgZCRc2nk6VY-g,60
-onoffmonitorserver/urls.py,sha256=WdzMWymOLasqLwCybE5NzLRZR_Q7floL46XihfNdHJw,233
-onoffmonitorserver/views.py,sha256=XEF3M2OI3YzX8tezkst4Yf_t7fDQJoc54oqJ0y4TUE4,1019
-onoffmonitorserver/migrations/0001_initial.py,sha256=89DcC29JeyBQydWJ1MxMq1fmpMJfQkSOug1jGU6scL4,1514
-onoffmonitorserver/migrations/0002_remove_status_user.py,sha256=OajvfmOtF4Z_29Bi7tLXejx-HZjFi52jEtm3uISmQ0Y,326
+onoffmonitorserver/urls.py,sha256=aO7I65KuJTpYyBnWMy7OZEbr4JDfyrpgTnEc5TdAu90,292
+onoffmonitorserver/views.py,sha256=sIZj0mSAR0xN1VItsv-vgcgPWfiqEGXyXFegH4f3xhQ,2170
+onoffmonitorserver/migrations/0001_initial.py,sha256=vSqXj4PR2ARTDmmJuJUofWdLH481q30NtR2EFoZCDJs,2205
 onoffmonitorserver/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-onoffmonitorserver-0.0.1.dist-info/METADATA,sha256=lbOOgT_lalGAhxkKYko8MKn277wsoB8OypgKQKlwFfw,1060
-onoffmonitorserver-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-onoffmonitorserver-0.0.1.dist-info/top_level.txt,sha256=To5bX54jTRb2wvSPY4AX9oenfUC4REFMMcWmUuBJdZ4,19
-onoffmonitorserver-0.0.1.dist-info/RECORD,,
+onoffmonitorserver-0.1.0.dist-info/METADATA,sha256=OBSf08LFYYSjaGj8fz3aqztZkWs4p7X_WdCS33re5KY,1061
+onoffmonitorserver-0.1.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+onoffmonitorserver-0.1.0.dist-info/top_level.txt,sha256=To5bX54jTRb2wvSPY4AX9oenfUC4REFMMcWmUuBJdZ4,19
+onoffmonitorserver-0.1.0.dist-info/RECORD,,
```

