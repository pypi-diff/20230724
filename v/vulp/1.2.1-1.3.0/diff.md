# Comparing `tmp/vulp-1.2.1.tar.gz` & `tmp/vulp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulp-1.2.1.tar", last modified: Fri Jul  7 10:18:31 2023, max compression
+gzip compressed data, was "vulp-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vulp-1.2.1.tar` & `vulp-1.3.0.tar`

### file list

```diff
@@ -1,41 +1,38 @@
--rw-r--r--   0        0        0    10970 2023-07-07 10:18:31.435026 vulp-1.2.1/README.md
--rw-r--r--   0        0        0     1406 2023-07-07 10:18:31.431026 vulp-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      685 2023-07-07 10:18:31.431026 vulp-1.2.1/vulp/__init__.py
--rw-r--r--   0        0        0     3628 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/AgentInterface.cpp
--rw-r--r--   0        0        0     2957 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/AgentInterface.h
--rw-r--r--   0        0        0     1991 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/BUILD
--rw-r--r--   0        0        0      862 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/Request.h
--rw-r--r--   0        0        0     9017 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/Spine.cpp
--rw-r--r--   0        0        0     6184 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/Spine.h
--rw-r--r--   0        0        0     5110 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/StateMachine.cpp
--rw-r--r--   0        0        0     3944 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/StateMachine.h
--rw-r--r--   0        0        0      872 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/position_commands.h
--rw-r--r--   0        0        0     1011 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/request.py
--rw-r--r--   0        0        0      783 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/spine_error.py
--rw-r--r--   0        0        0     6305 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/spine_interface.py
--rw-r--r--   0        0        0     1638 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/tests/AgentInterfaceTest.cpp
--rw-r--r--   0        0        0      718 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/tests/BUILD
--rw-r--r--   0        0        0    10158 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/tests/SpineTest.cpp
--rw-r--r--   0        0        0     3799 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/tests/StateMachineTest.cpp
--rw-r--r--   0        0        0     6602 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/tests/spine_interface_test.py
--rw-r--r--   0        0        0     1420 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/BUILD
--rw-r--r--   0        0        0     1716 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/Spinlock.h
--rw-r--r--   0        0        0     2604 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/SynchronousClock.cpp
--rw-r--r--   0        0        0     2987 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/SynchronousClock.h
--rw-r--r--   0        0        0     1193 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/handle_interrupts.cpp
--rw-r--r--   0        0        0     1121 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/handle_interrupts.h
--rw-r--r--   0        0        0     2025 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/low_pass_filter.h
--rw-r--r--   0        0        0     1003 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/math.h
--rw-r--r--   0        0        0     1302 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/random_string.h
--rw-r--r--   0        0        0     2106 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/realtime.h
--rw-r--r--   0        0        0     1416 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/serialize.py
--rw-r--r--   0        0        0      351 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/BUILD
--rw-r--r--   0        0        0     1502 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/SpinlockTest.cpp
--rw-r--r--   0        0        0     1356 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/SynchronousClockTest.cpp
--rw-r--r--   0        0        0     1234 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/low_pass_filter_test.cpp
--rw-r--r--   0        0        0      859 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/math_test.cpp
--rw-r--r--   0        0        0     1215 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/random_string_test.cpp
--rw-r--r--   0        0        0      920 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/realtime_test.cpp
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 vulp-1.2.1/setup.py
--rw-r--r--   0        0        0    12228 1970-01-01 00:00:00.000000 vulp-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11282 2023-07-24 07:51:53.863614 vulp-1.3.0/README.md
+-rw-r--r--   0        0        0     1406 2023-07-24 07:51:53.863614 vulp-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      685 2023-07-24 07:51:53.863614 vulp-1.3.0/vulp/__init__.py
+-rw-r--r--   0        0        0     3628 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/AgentInterface.cpp
+-rw-r--r--   0        0        0     2957 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/AgentInterface.h
+-rw-r--r--   0        0        0     1992 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/BUILD
+-rw-r--r--   0        0        0      862 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/Request.h
+-rw-r--r--   0        0        0     8981 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/Spine.cpp
+-rw-r--r--   0        0        0     6184 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/Spine.h
+-rw-r--r--   0        0        0     5110 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/StateMachine.cpp
+-rw-r--r--   0        0        0     3944 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/StateMachine.h
+-rw-r--r--   0        0        0      872 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/position_commands.h
+-rw-r--r--   0        0        0     1011 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/request.py
+-rw-r--r--   0        0        0      783 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/spine_error.py
+-rw-r--r--   0        0        0     6305 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/spine_interface.py
+-rw-r--r--   0        0        0     1713 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/tests/AgentInterfaceTest.cpp
+-rw-r--r--   0        0        0      718 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/tests/BUILD
+-rw-r--r--   0        0        0     9987 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/tests/SpineTest.cpp
+-rw-r--r--   0        0        0     3628 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/tests/StateMachineTest.cpp
+-rw-r--r--   0        0        0     6718 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/spine/tests/spine_interface_test.py
+-rw-r--r--   0        0        0     1299 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/BUILD
+-rw-r--r--   0        0        0     2604 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/SynchronousClock.cpp
+-rw-r--r--   0        0        0     2987 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/SynchronousClock.h
+-rw-r--r--   0        0        0     1193 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/handle_interrupts.cpp
+-rw-r--r--   0        0        0     1121 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/handle_interrupts.h
+-rw-r--r--   0        0        0     2025 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/low_pass_filter.h
+-rw-r--r--   0        0        0     1003 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/math.h
+-rw-r--r--   0        0        0     1302 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/random_string.h
+-rw-r--r--   0        0        0     2368 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/realtime.h
+-rw-r--r--   0        0        0     1416 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/serialize.py
+-rw-r--r--   0        0        0      524 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/tests/BUILD
+-rw-r--r--   0        0        0     1356 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/tests/SynchronousClockTest.cpp
+-rw-r--r--   0        0        0     1234 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/tests/low_pass_filter_test.cpp
+-rw-r--r--   0        0        0      859 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/tests/math_test.cpp
+-rw-r--r--   0        0        0     1215 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/tests/random_string_test.cpp
+-rw-r--r--   0        0        0      920 2023-07-24 07:51:53.859614 vulp-1.3.0/vulp/utils/tests/realtime_test.cpp
+-rw-r--r--   0        0        0    12540 1970-01-01 00:00:00.000000 vulp-1.3.0/PKG-INFO
```

### Comparing `vulp-1.2.1/README.md` & `vulp-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# Vulp — Real-time motion control for Python
+# Vulp – Robot/simulation switch
 
 ![C++ version](https://img.shields.io/badge/C++-17/20-blue.svg?style=flat)
 [![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/vulp/bazel.yml?branch=main)](https://github.com/tasts-robots/vulp/actions/workflows/bazel.yml)
 [![Documentation](https://img.shields.io/badge/docs-online-brightgreen?style=flat)](https://tasts-robots.org/doc/vulp/)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/vulp/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/vulp?branch=main)
 [![PyPI version](https://img.shields.io/pypi/v/vulp)](https://pypi.org/project/vulp/)
 [![Example project](https://img.shields.io/badge/example-upkie-green)](https://github.com/tasts-robots/upkie)
-[![Chat](https://img.shields.io/badge/matrix-joint%20chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
+[![Chat](https://img.shields.io/badge/matrix-chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
-Vulp provides an action-observation loop to control robots from Python, like this:
+Vulp provides an action-observation loop to control robots from standalone "agent" processes, like this:
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/tasts-robots/vulp/main/doc/figures/action-observation-loop-full.svg" alt="Action-observation loop with Vulp" class="center"/>
 </p>
 
-Vulp works on Linux (desktop and Raspberry Pi) with [moteus](https://github.com/mjbots/moteus/) actuators and [Bullet](https://github.com/bulletphysics/bullet3) for simulation.
+Vulp is designed for robots built with the mjbots stack ([moteus](https://github.com/mjbots/moteus/) servo controllers and [pi3hat](https://github.com/mjbots/pi3hat/) communication board). It provides a robot/simulation switch to train or test agents in [Bullet](https://github.com/bulletphysics/bullet3) before running them on the real thing.
+
+Vulp supports Linux and macOS for development, and Raspberry Pi OS for robot deployment.
 
 ### Try it out!
 
-No installation required on Linux:
+Assuming you already have a C++ compiler and Python interpreter, you can try a robot simulation without installing any software on your system:
 
 <img src="https://user-images.githubusercontent.com/1189580/170496331-e1293dd3-b50c-40ee-9c2e-f75f3096ebd8.png" height="100" align="right" />
 
 ```console
 $ git clone https://github.com/tasts-robots/upkie.git
 $ cd upkie
-$ ./start_test_balancer.sh
+$ ./start_wheel_balancer.sh
 ```
 
-Connect a USB controller to move the robot around. 🎮
-
 Check out the [``upkie``](https://github.com/tasts-robots/upkie) repository for an example where Vulp is used with Upkie wheeled biped, including simulation environments, real-robot spines, state observers and locomotion agents.
 
 ## Details
 
 More accurately, Vulp is a tiny inter-process communication (IPC) protocol shipped with reference libraries (currently in Python and C++, other languages welcome). It is suitable for tasks that require [real-time](https://en.wiktionary.org/wiki/real-time#English) but *not* high-frequency performance. The main use case for this is balancing, as there is [theoretical and empirical evidence](https://arxiv.org/abs/1907.01805) suggesting that bipeds and quadrupeds can balance themselves as leisurely as 5–15 Hz, although balance control is frequently implemented at 200–1000 Hz. And if you are wondering whether Python is suitable for real-time applications, we were too! Until we [tried it out](#performance).
 
 In Vulp, a fast program, called a _spine_, talks to a slow program, called an _agent_, in a standard action-observation loop. Spine and agent run in separate processes and exchange ``action`` and ``observation`` dictionaries through shared memory. For instance, ``action`` can be a set of joint commands and ``observation`` a set of joint observations. Vulp provides a pipeline API to grow more complex spines with additional controllers (for higher-level actions) and observers (for richer observations). For example, a spine can run an inverse kinematics solver, or output its own ground contact estimation.
```

### Comparing `vulp-1.2.1/pyproject.toml` & `vulp-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "msgpack >=1.0.2",
-    "posix_ipc >=1.0.5",
+    "posix_ipc >=1.1.1",
 ]
 keywords = ["motion control", "real time", "robotics"]
 
 [project.urls]
 Documentation = "https://tasts-robots.org/doc/vulp/"
 Source = "https://github.com/tasts-robots/vulp"
 Tracker = "https://github.com/tasts-robots/vulp/issues"
```

### Comparing `vulp-1.2.1/vulp/__init__.py` & `vulp-1.3.0/vulp/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Real-time motion control for Python."""
 
-__version__ = "1.2.1"
+__version__ = "1.3.0"
```

### Comparing `vulp-1.2.1/vulp/spine/AgentInterface.cpp` & `vulp-1.3.0/vulp/spine/AgentInterface.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/AgentInterface.h` & `vulp-1.3.0/vulp/spine/AgentInterface.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/BUILD` & `vulp-1.3.0/vulp/spine/BUILD`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     hdrs = [
         "Spine.h",
     ],
     srcs = [
         "Spine.cpp",
     ],
     linkopts = select({
-        "//:linux": ["-lrt"],
+        "@//:linux": ["-lrt"],
         "@//conditions:default": [],
     }),
     deps = [
         "//actuation:imu_data",
         "//actuation:interface",
         "//observation:observe_imu",
         "//observation:observe_servos",
```

### Comparing `vulp-1.2.1/vulp/spine/Request.h` & `vulp-1.3.0/vulp/spine/Request.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/Spine.cpp` & `vulp-1.3.0/vulp/spine/Spine.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -50,16 +50,20 @@
       agent_interface_(params.shm_name, params.shm_size),
       observer_pipeline_(observers),
       logger_(params.log_path),
       caught_interrupt_(vulp::utils::handle_interrupts()),
       state_machine_(agent_interface_),
       state_cycle_beginning_(State::kOver),
       state_cycle_end_(State::kOver) {
-  // Thread name as it appears in the `cmd` column of `ps`
+// Thread name as it appears in the `cmd` column of `ps`
+#ifdef __APPLE__
+  pthread_setname_np("spine_thread");
+#else
   pthread_setname_np(pthread_self(), "spine_thread");
+#endif
 
   // Real-time configuration
   // NB: it is too late to lock memory here, this should be done by the caller
   if (params.cpu >= 0) {
     utils::configure_cpu(params.cpu);
     utils::configure_scheduler(10);
   }
@@ -189,26 +193,26 @@
         state_machine_.state() == State::kShutdown) {
       actuation_.write_stop_commands();
     } else if (state_machine_.state() == State::kAct) {
       Dictionary& action = dict_("action");
       actuation_.write_position_commands(action);
       // TODO(scaron): don't re-send actuation
       // See https://github.com/tasts-robots/vulp/issues/2
-      // spdlog::info("[Spine::cycle_actuation] ok");
+      // spdlog::info("[Spine] ok");
     } else {
-      // spdlog::warn("[Spine::cycle_actuation] re-sending previous commands");
+      // spdlog::warn("[Spine] re-sending previous commands");
     }
   } catch (const std::exception& e) {
-    spdlog::error("[Spine::cycle_actuation] Caught an exception: {}", e.what());
-    spdlog::error("[Spine::cycle_actuation] Sending stop commands...");
+    spdlog::error("[Spine] Caught an exception: {}", e.what());
+    spdlog::error("[Spine] Sending stop commands...");
     state_machine_.process_event(Event::kInterrupt);
     actuation_.write_stop_commands();
   } catch (...) {
-    spdlog::error("[Spine::cycle_actuation] Caught an unknown exception!");
-    spdlog::error("[Spine::cycle_actuation] Sending stop commands...");
+    spdlog::error("[Spine] Caught an unknown exception!");
+    spdlog::error("[Spine] Sending stop commands...");
     state_machine_.process_event(Event::kInterrupt);
     actuation_.write_stop_commands();
   }
 
   // Whatever exceptions were thrown around, we caught them and at this
   // point every actuation command is either a stop or a position one.
```

### Comparing `vulp-1.2.1/vulp/spine/Spine.h` & `vulp-1.3.0/vulp/spine/Spine.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/StateMachine.cpp` & `vulp-1.3.0/vulp/spine/StateMachine.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/StateMachine.h` & `vulp-1.3.0/vulp/spine/StateMachine.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/__init__.py` & `vulp-1.3.0/vulp/spine/__init__.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/request.py` & `vulp-1.3.0/vulp/spine/request.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/spine_error.py` & `vulp-1.3.0/vulp/spine/spine_error.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/spine_interface.py` & `vulp-1.3.0/vulp/spine/spine_interface.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/tests/AgentInterfaceTest.cpp` & `vulp-1.3.0/vulp/spine/tests/AgentInterfaceTest.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -22,24 +22,26 @@
 #include <map>
 #include <memory>
 #include <string>
 #include <vector>
 
 #include "gtest/gtest.h"
 #include "vulp/spine/AgentInterface.h"
+#include "vulp/utils/random_string.h"
 
 namespace vulp::spine {
 
 class AgentInterfaceTest : public ::testing::Test {
  protected:
   void SetUp() override {
-    agent_interface_ = std::make_unique<AgentInterface>("tester", 1024);
+    agent_interface_ =
+        std::make_unique<AgentInterface>("/" + utils::random_string(), 1024);
   }
 
-  void TearDown() {}
+  void TearDown() override {}
 
   std::unique_ptr<AgentInterface> agent_interface_;
 };
 
 TEST_F(AgentInterfaceTest, GetSetRequest) {
   agent_interface_->set_request(Request::kObservation);
   ASSERT_EQ(agent_interface_->request(), Request::kObservation);
```

### Comparing `vulp-1.2.1/vulp/spine/tests/BUILD` & `vulp-1.3.0/vulp/spine/tests/BUILD`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/spine/tests/SpineTest.cpp` & `vulp-1.3.0/vulp/spine/tests/SpineTest.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -85,44 +85,39 @@
 
 }  // namespace testing
 
 class SpineTest : public ::testing::Test {
  protected:
   //! Initialize spine for a new test
   void SetUp() override {
-    const auto* test_info =
-        ::testing::UnitTest::GetInstance()->current_test_info();
-
     params_.cpu = -1;         // no realtime scheduling
     params_.frequency = 400;  // Hz
-    params_.shm_name = std::string("/") + test_info->test_case_name() + "_" +
-                       test_info->name() + "_" + utils::random_string();
+    params_.shm_name = std::string("/") + utils::random_string();
     params_.shm_size = 1024;
 
     actuation::ServoLayout layout;
     layout.add_servo(1, 1, "bar");
     layout.add_servo(2, 1, "foo");
 
     const double dt = 1.0 / params_.frequency;
     actuation_interface_ = std::make_unique<MockInterface>(layout, dt);
 
     schwifty_observer_ = std::make_unique<SchwiftyObserver>();
     observation_.append_observer(schwifty_observer_);
     spine_ = std::make_unique<testing::Spine>(params_, *actuation_interface_,
                                               observation_);
-
     int file_descriptor =
         ::shm_open(params_.shm_name.c_str(), O_RDWR | O_CREAT, 0666);
     ASSERT_GE(file_descriptor, 0);
     mmap_ = ::mmap(nullptr, params_.shm_size, PROT_READ | PROT_WRITE,
                    MAP_SHARED, file_descriptor, 0);
     ASSERT_GE(::close(file_descriptor), 0);
   }
 
-  void TearDown() {
+  void TearDown() override {
     ASSERT_GE(::munmap(mmap_, params_.shm_size), 0);
 
     // Check that the destructor unlinks shared memory
     spine_.reset();
     ASSERT_LT(::shm_unlink(params_.shm_name.c_str()), 0);
     ASSERT_EQ(errno, ENOENT);
   }
```

### Comparing `vulp-1.2.1/vulp/spine/tests/StateMachineTest.cpp` & `vulp-1.3.0/vulp/spine/tests/StateMachineTest.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -27,20 +27,16 @@
 using spine::AgentInterface;
 using spine::StateMachine;
 
 class StateMachineTest : public ::testing::Test {
  protected:
   //! Prepare state machine for a new test
   void SetUp() override {
-    const auto* test_info =
-        ::testing::UnitTest::GetInstance()->current_test_info();
     const size_t shm_size = 1 * (1 << 20);
-    const std::string shm_name =
-        std::string("/") + test_info->test_case_name() + "_" +
-        test_info->name() + "_" + utils::random_string();
+    const std::string shm_name = std::string("/") + utils::random_string();
     agent_interface_ = std::make_unique<AgentInterface>(shm_name, shm_size);
     state_machine_ = std::make_unique<StateMachine>(*agent_interface_);
   }
 
   //! Get current request
   Request request() { return agent_interface_->request(); }
```

### Comparing `vulp-1.2.1/vulp/spine/tests/spine_interface_test.py` & `vulp-1.3.0/vulp/spine/tests/spine_interface_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,24 @@
         """
         Initialize a new fixture instance.
 
         Args:
             shm_name: Name of shared memory file.
             size: Size of shared memory file in bytes.
         """
-        shared_memory = posix_ipc.SharedMemory(
+        self.shared_memory = posix_ipc.SharedMemory(
             shm_name, posix_ipc.O_CREAT, size=size, read_only=False
         )
         _mmap = mmap.mmap(
-            shared_memory.fd,
-            shared_memory.size,
+            self.shared_memory.fd,
+            self.shared_memory.size,
             flags=mmap.MAP_SHARED,
             prot=mmap.PROT_READ | mmap.PROT_WRITE,
         )
-        shared_memory.close_fd()
+        self.shared_memory.close_fd()
         self._mmap = _mmap
         self._packer = msgpack.Packer(default=serialize, use_bin_type=True)
         self._unpacker = msgpack.Unpacker(raw=False)
 
         self.last_action = {}
         self.last_config = {}
         self.shm_name = shm_name
@@ -89,14 +89,18 @@
             self.assertEqual(self.read_request(), Request.kNone)
 
         self.assertTrue(hasattr(SpineInterface, "_wait_for_spine"))
         SpineInterface._wait_for_spine = wait_monkeypatch
         self.spine = SpineInterface(shm_name=shm_name)
         self.write_request(Request.kNone)  # same as Spine constructor
 
+    def tearDown(self) -> None:
+        self._mmap.close()
+        self.shared_memory.unlink()
+
     def read_request(self) -> int:
         """
         Get shared memory request.
         """
         self._mmap.seek(0)
         return int.from_bytes(self._mmap.read(4), byteorder=sys.byteorder)
```

### Comparing `vulp-1.2.1/vulp/utils/BUILD` & `vulp-1.3.0/vulp/utils/BUILD`

 * *Files 13% similar despite different names*

```diff
@@ -39,20 +39,14 @@
 cc_library(
     name = "realtime",
     hdrs = ["realtime.h"],
     include_prefix = "vulp/utils",
 )
 
 cc_library(
-    name = "spinlock",
-    hdrs = ["Spinlock.h"],
-    include_prefix = "vulp/utils",
-)
-
-cc_library(
     name = "synchronous_clock",
     hdrs = ["SynchronousClock.h"],
     srcs = ["SynchronousClock.cpp"],
     deps = [
         ":math",
         "@spdlog",
     ],
@@ -63,15 +57,14 @@
     name = "utils",
     deps = [
         ":handle_interrupts",
         ":low_pass_filter",
         ":math",
         ":random_string",
         ":realtime",
-        ":spinlock",
         ":synchronous_clock",
     ],
 )
 
 py_library(
     name = "serialize",
     srcs = [
```

### Comparing `vulp-1.2.1/vulp/utils/SynchronousClock.cpp` & `vulp-1.3.0/vulp/utils/SynchronousClock.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/SynchronousClock.h` & `vulp-1.3.0/vulp/utils/SynchronousClock.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/handle_interrupts.cpp` & `vulp-1.3.0/vulp/utils/handle_interrupts.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/handle_interrupts.h` & `vulp-1.3.0/vulp/utils/handle_interrupts.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/low_pass_filter.h` & `vulp-1.3.0/vulp/utils/low_pass_filter.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/math.h` & `vulp-1.3.0/vulp/utils/math.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/random_string.h` & `vulp-1.3.0/vulp/utils/random_string.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/realtime.h` & `vulp-1.3.0/vulp/utils/realtime.h`

 * *Files 16% similar despite different names*

```diff
@@ -17,48 +17,60 @@
 #pragma once
 
 #include <sched.h>
 #include <sys/mman.h>
 
 #include <stdexcept>
 
+#ifdef __APPLE__
+#include <spdlog/spdlog.h>
+#endif
+
 namespace vulp::utils {
 
 /*! Set the current thread to run on a given CPU core.
  *
  * \param cpu CPU core for this thread (on the Pi, CPUID in {0, 1, 2, 3}).
  *
  * \throw std::runtime_error If the operation failed.
  */
 inline void configure_cpu(int cpu) {
+#ifndef __APPLE__
   constexpr int kPid = 0;  // this thread
   cpu_set_t cpuset = {};
   CPU_ZERO(&cpuset);
   CPU_SET(cpu, &cpuset);
   if (::sched_setaffinity(kPid, sizeof(cpu_set_t), &cpuset) < 0) {
     throw std::runtime_error("Error setting CPU affinity");
   }
+#else
+  spdlog::warn("[configure_cpu] This function does nothing on macOS");
+#endif
 }
 
 /*! Configure the scheduler policy to round-robin for this thread.
  *
  * \param priority Priority of this thread for the scheduler, ranging from 1
  *     (low) to 99 (high). See `man sched`. For the brain, this priority should
  *     be lower than that of the spine.
  *
  * \throw std::runtime_error If the operation failed.
  */
 inline void configure_scheduler(int priority) {
+#ifndef __APPLE__
   constexpr int kPid = 0;  // this thread
   struct sched_param params = {};
   params.sched_priority = priority;
   if (::sched_setscheduler(kPid, SCHED_RR, &params) < 0) {
     throw std::runtime_error(
         "Error setting realtime scheduler, try running as root (use sudo)");
   }
+#else
+  spdlog::warn("[configure_scheduler] This function does nothing on macOS");
+#endif
 }
 
 /*! Lock all memory to RAM so that the kernel doesn't page it to swap.
  *
  * The Linux man pages have a great NOTES section on this. Worth a read!
  */
 inline bool lock_memory() {
```

### Comparing `vulp-1.2.1/vulp/utils/serialize.py` & `vulp-1.3.0/vulp/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/tests/SynchronousClockTest.cpp` & `vulp-1.3.0/vulp/utils/tests/SynchronousClockTest.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/tests/low_pass_filter_test.cpp` & `vulp-1.3.0/vulp/utils/tests/low_pass_filter_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/tests/math_test.cpp` & `vulp-1.3.0/vulp/utils/tests/math_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/tests/random_string_test.cpp` & `vulp-1.3.0/vulp/utils/tests/random_string_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/vulp/utils/tests/realtime_test.cpp` & `vulp-1.3.0/vulp/utils/tests/realtime_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.1/PKG-INFO` & `vulp-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulp
-Version: 1.2.1
+Version: 1.3.0
 Summary: Real-time motion control for Python.
 Keywords: motion control,real time,robotics
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -16,52 +16,52 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: msgpack >=1.0.2
-Requires-Dist: posix_ipc >=1.0.5
+Requires-Dist: posix_ipc >=1.1.1
 Project-URL: Changelog, https://github.com/tasts-robots/vulp/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://tasts-robots.org/doc/vulp/
 Project-URL: Source, https://github.com/tasts-robots/vulp
 Project-URL: Tracker, https://github.com/tasts-robots/vulp/issues
 
-# Vulp — Real-time motion control for Python
+# Vulp – Robot/simulation switch
 
 ![C++ version](https://img.shields.io/badge/C++-17/20-blue.svg?style=flat)
 [![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/vulp/bazel.yml?branch=main)](https://github.com/tasts-robots/vulp/actions/workflows/bazel.yml)
 [![Documentation](https://img.shields.io/badge/docs-online-brightgreen?style=flat)](https://tasts-robots.org/doc/vulp/)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/vulp/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/vulp?branch=main)
 [![PyPI version](https://img.shields.io/pypi/v/vulp)](https://pypi.org/project/vulp/)
 [![Example project](https://img.shields.io/badge/example-upkie-green)](https://github.com/tasts-robots/upkie)
-[![Chat](https://img.shields.io/badge/matrix-joint%20chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
+[![Chat](https://img.shields.io/badge/matrix-chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
-Vulp provides an action-observation loop to control robots from Python, like this:
+Vulp provides an action-observation loop to control robots from standalone "agent" processes, like this:
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/tasts-robots/vulp/main/doc/figures/action-observation-loop-full.svg" alt="Action-observation loop with Vulp" class="center"/>
 </p>
 
-Vulp works on Linux (desktop and Raspberry Pi) with [moteus](https://github.com/mjbots/moteus/) actuators and [Bullet](https://github.com/bulletphysics/bullet3) for simulation.
+Vulp is designed for robots built with the mjbots stack ([moteus](https://github.com/mjbots/moteus/) servo controllers and [pi3hat](https://github.com/mjbots/pi3hat/) communication board). It provides a robot/simulation switch to train or test agents in [Bullet](https://github.com/bulletphysics/bullet3) before running them on the real thing.
+
+Vulp supports Linux and macOS for development, and Raspberry Pi OS for robot deployment.
 
 ### Try it out!
 
-No installation required on Linux:
+Assuming you already have a C++ compiler and Python interpreter, you can try a robot simulation without installing any software on your system:
 
 <img src="https://user-images.githubusercontent.com/1189580/170496331-e1293dd3-b50c-40ee-9c2e-f75f3096ebd8.png" height="100" align="right" />
 
 ```console
 $ git clone https://github.com/tasts-robots/upkie.git
 $ cd upkie
-$ ./start_test_balancer.sh
+$ ./start_wheel_balancer.sh
 ```
 
-Connect a USB controller to move the robot around. 🎮
-
 Check out the [``upkie``](https://github.com/tasts-robots/upkie) repository for an example where Vulp is used with Upkie wheeled biped, including simulation environments, real-robot spines, state observers and locomotion agents.
 
 ## Details
 
 More accurately, Vulp is a tiny inter-process communication (IPC) protocol shipped with reference libraries (currently in Python and C++, other languages welcome). It is suitable for tasks that require [real-time](https://en.wiktionary.org/wiki/real-time#English) but *not* high-frequency performance. The main use case for this is balancing, as there is [theoretical and empirical evidence](https://arxiv.org/abs/1907.01805) suggesting that bipeds and quadrupeds can balance themselves as leisurely as 5–15 Hz, although balance control is frequently implemented at 200–1000 Hz. And if you are wondering whether Python is suitable for real-time applications, we were too! Until we [tried it out](#performance).
 
 In Vulp, a fast program, called a _spine_, talks to a slow program, called an _agent_, in a standard action-observation loop. Spine and agent run in separate processes and exchange ``action`` and ``observation`` dictionaries through shared memory. For instance, ``action`` can be a set of joint commands and ``observation`` a set of joint observations. Vulp provides a pipeline API to grow more complex spines with additional controllers (for higher-level actions) and observers (for richer observations). For example, a spine can run an inverse kinematics solver, or output its own ground contact estimation.
```

