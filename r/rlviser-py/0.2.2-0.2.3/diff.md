# Comparing `tmp/rlviser_py-0.2.2.tar.gz` & `tmp/rlviser_py-0.2.3.tar.gz`

## Comparing `rlviser_py-0.2.2.tar` & `rlviser_py-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,12 @@
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 rlviser_py-0.2.2/Cargo.toml
--rw-r--r--   0     1001      123     2774 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/.gitignore
--rw-r--r--   0     1001      123     1070 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/LICENSE
--rw-r--r--   0     1001      123      490 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/README.md
--rw-r--r--   0     1001      123      390 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/pyproject.toml
--rw-r--r--   0     1001      123      255 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/rlviser_py.pyi
--rw-r--r--   0     1001      123       74 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/rustfmt.toml
--rw-r--r--   0     1001      123    32938 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/src/bytes.rs
--rw-r--r--   0     1001      123      995 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/src/gym.rs
--rw-r--r--   0     1001      123     4269 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/src/lib.rs
--rw-r--r--   0     1001      123     1443 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/src/socket.rs
--rw-r--r--   0     1001      123     7635 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/Cargo.lock
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 rlviser_py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 rlviser_py-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      123     1070 2023-07-24 02:13:22.000000 rlviser_py-0.2.3/LICENSE
+-rw-r--r--   0     1001      123      490 2023-07-24 02:13:22.000000 rlviser_py-0.2.3/README.md
+-rw-r--r--   0     1001      123      390 2023-07-24 02:13:22.000000 rlviser_py-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      123      583 2023-07-24 02:13:22.000000 rlviser_py-0.2.3/rlviser_py.pyi
+-rw-r--r--   0     1001      123    34852 2023-07-24 02:13:22.000000 rlviser_py-0.2.3/src/bytes.rs
+-rw-r--r--   0     1001      123      995 2023-07-24 02:13:22.000000 rlviser_py-0.2.3/src/gym.rs
+-rw-r--r--   0     1001      123     5390 2023-07-24 02:13:22.000000 rlviser_py-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      123     2561 2023-07-24 02:13:22.000000 rlviser_py-0.2.3/src/rocketsim.rs
+-rw-r--r--   0     1001      123     1443 2023-07-24 02:13:22.000000 rlviser_py-0.2.3/src/socket.rs
+-rw-r--r--   0     1001      123     7637 2023-07-24 02:13:22.000000 rlviser_py-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 rlviser_py-0.2.3/PKG-INFO
```

### Comparing `rlviser_py-0.2.2/LICENSE` & `rlviser_py-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.2.2/src/bytes.rs` & `rlviser_py-0.2.3/src/bytes.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,97 @@
-use glam::{Mat3A as RotMat, Quat, Vec3A as Vec3};
+use core::panic;
 
-#[derive(Clone, Copy, Default, Debug)]
+use glam::{Mat3A, Quat, Vec3A};
+use pyo3::FromPyObject;
+
+#[derive(Clone, Copy, Debug, Default, FromPyObject)]
+pub struct Vec3 {
+    pub x: f32,
+    pub y: f32,
+    pub z: f32,
+}
+
+impl Vec3 {
+    pub const ZERO: Self = Self::new(0., 0., 0.);
+    pub const X: Self = Self::new(1., 0., 0.);
+    pub const Y: Self = Self::new(0., 1., 0.);
+    pub const Z: Self = Self::new(0., 0., 1.);
+
+    pub const fn new(x: f32, y: f32, z: f32) -> Self {
+        Self { x, y, z }
+    }
+
+    pub const fn from_array(array: [f32; 3]) -> Self {
+        Self::new(array[0], array[1], array[2])
+    }
+}
+
+impl From<[f32; 3]> for Vec3 {
+    #[inline]
+    fn from(value: [f32; 3]) -> Self {
+        Self::from_array(value)
+    }
+}
+
+impl From<Vec3A> for Vec3 {
+    #[inline]
+    fn from(value: Vec3A) -> Self {
+        Self::new(value.x, value.y, value.z)
+    }
+}
+
+#[derive(Clone, Copy, Debug, FromPyObject)]
+pub struct RotMat {
+    pub forward: Vec3,
+    pub right: Vec3,
+    pub up: Vec3,
+}
+
+impl Default for RotMat {
+    #[inline]
+    fn default() -> Self {
+        Self::IDENTITY
+    }
+}
+
+impl RotMat {
+    pub const IDENTITY: Self = Self::new(Vec3::X, Vec3::Y, Vec3::Z);
+
+    #[inline]
+    pub const fn new(x_axis: Vec3, y_axis: Vec3, z_axis: Vec3) -> Self {
+        Self {
+            forward: x_axis,
+            right: y_axis,
+            up: z_axis,
+        }
+    }
+}
+
+impl From<Mat3A> for RotMat {
+    #[inline]
+    fn from(value: Mat3A) -> Self {
+        Self {
+            forward: value.x_axis.into(),
+            right: value.y_axis.into(),
+            up: value.z_axis.into(),
+        }
+    }
+}
+
+#[derive(Clone, Copy, Default, Debug, FromPyObject)]
 pub struct BallHitInfo {
     pub is_valid: bool,
     pub relative_pos_on_ball: Vec3,
     pub ball_pos: Vec3,
     pub extra_hit_vel: Vec3,
     pub tick_count_when_hit: u64,
     pub tick_count_when_extra_impulse_applied: u64,
 }
 
-#[derive(Clone, Copy, Debug)]
+#[derive(Clone, Copy, Debug, FromPyObject)]
 pub struct BallState {
     pub pos: Vec3,
     pub vel: Vec3,
     pub ang_vel: Vec3,
 }
 
 impl Default for BallState {
@@ -32,70 +109,82 @@
 #[derive(Clone, Copy, Default, Debug)]
 pub enum Team {
     #[default]
     Blue,
     Orange,
 }
 
-#[derive(Clone, Copy, Default, Debug)]
+impl Team {
+    #[inline]
+    pub fn from_u8(value: u8) -> Self {
+        match value {
+            0 => Self::Blue,
+            1 => Self::Orange,
+            _ => panic!("Invalid team value: {}", value),
+        }
+    }
+}
+
+#[derive(Clone, Copy, Default, Debug, FromPyObject)]
 pub struct WheelPairConfig {
     pub wheel_radius: f32,
     pub suspension_rest_length: f32,
     pub connection_point_offset: Vec3,
 }
 
-#[derive(Clone, Copy, Default, Debug)]
+#[derive(Clone, Copy, Default, Debug, FromPyObject)]
 pub struct CarConfig {
     pub hitbox_size: Vec3,
     pub hitbox_pos_offset: Vec3,
     pub front_wheels: WheelPairConfig,
     pub back_wheels: WheelPairConfig,
     pub dodge_deadzone: f32,
 }
 
-#[derive(Clone, Copy, Debug, Default)]
+#[derive(Clone, Copy, Debug, Default, FromPyObject)]
 pub struct CarControls {
     pub throttle: f32,
     pub steer: f32,
     pub pitch: f32,
     pub yaw: f32,
     pub roll: f32,
     pub boost: bool,
     pub jump: bool,
     pub handbrake: bool,
 }
 
-#[derive(Clone, Copy, Debug, Default)]
+#[derive(Clone, Copy, Debug, Default, FromPyObject)]
 pub struct CarState {
     pub pos: Vec3,
     pub rot_mat: RotMat,
     pub vel: Vec3,
     pub ang_vel: Vec3,
     pub is_on_ground: bool,
     pub has_jumped: bool,
     pub has_double_jumped: bool,
     pub has_flipped: bool,
     pub last_rel_dodge_torque: Vec3,
     pub jump_time: f32,
     pub flip_time: f32,
+
     pub is_flipping: bool,
     pub is_jumping: bool,
     pub air_time_since_jump: f32,
     pub boost: f32,
     pub time_spent_boosting: f32,
     pub is_supersonic: bool,
     pub supersonic_time: f32,
     pub handbrake_val: f32,
     pub is_auto_flipping: bool,
     pub auto_flip_timer: f32,
     pub auto_flip_torque_scale: f32,
-    pub has_contact: bool,
+    pub has_world_contact: bool,
     pub contact_normal: Vec3,
-    pub other_car_id: u32,
-    pub cooldown_timer: f32,
+    pub car_contact_id: u32,
+    pub car_contact_cooldown_timer: f32,
     pub is_demoed: bool,
     pub demo_respawn_timer: f32,
     pub ball_hit_info: BallHitInfo,
     pub last_controls: CarControls,
 }
 
 #[derive(Clone, Copy, Default, Debug)]
@@ -148,17 +237,17 @@
         bytes
     }
 }
 
 impl ToBytesExact<{ Self::NUM_BYTES }> for RotMat {
     fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
         let mut bytes = [0; Self::NUM_BYTES];
-        bytes[..Vec3::NUM_BYTES].copy_from_slice(&self.x_axis.to_bytes());
-        bytes[Vec3::NUM_BYTES..Vec3::NUM_BYTES * 2].copy_from_slice(&self.y_axis.to_bytes());
-        bytes[Vec3::NUM_BYTES * 2..].copy_from_slice(&self.z_axis.to_bytes());
+        bytes[..Vec3::NUM_BYTES].copy_from_slice(&self.forward.to_bytes());
+        bytes[Vec3::NUM_BYTES..Vec3::NUM_BYTES * 2].copy_from_slice(&self.right.to_bytes());
+        bytes[Vec3::NUM_BYTES * 2..].copy_from_slice(&self.up.to_bytes());
         bytes
     }
 }
 
 impl ToBytesExact<{ Self::NUM_BYTES }> for BallState {
     fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
         let mut bytes = [0; Self::NUM_BYTES];
@@ -301,27 +390,27 @@
         // auto_flip_torque_scale: f32,
         bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 8
             ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9]
             .copy_from_slice(&self.auto_flip_torque_scale.to_le_bytes());
         // has_contact: bool,
         bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9
             ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9]
-            .copy_from_slice(&(self.has_contact as u8).to_le_bytes());
+            .copy_from_slice(&(self.has_world_contact as u8).to_le_bytes());
         // contact_normal: Vec3,
         bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9
             ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9]
             .copy_from_slice(&self.contact_normal.to_bytes());
         // other_car_id: u32,
         bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9
             ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9 + u32::NUM_BYTES]
-            .copy_from_slice(&self.other_car_id.to_le_bytes());
+            .copy_from_slice(&self.car_contact_id.to_le_bytes());
         // cooldown_timer: f32,
         bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9 + u32::NUM_BYTES
             ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 10 + u32::NUM_BYTES]
-            .copy_from_slice(&self.cooldown_timer.to_le_bytes());
+            .copy_from_slice(&self.car_contact_cooldown_timer.to_le_bytes());
         // is_demoed: bool,
         bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 10 + u32::NUM_BYTES
             ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 10 + u32::NUM_BYTES]
             .copy_from_slice(&(self.is_demoed as u8).to_le_bytes());
         // demo_respawn_timer: f32,
         bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 10 + u32::NUM_BYTES
             ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 11 + u32::NUM_BYTES]
@@ -442,17 +531,17 @@
 
 impl FromBytesExact for RotMat {
     const NUM_BYTES: usize = Vec3::NUM_BYTES * 3;
 
     #[inline]
     fn from_bytes(bytes: &[u8]) -> Self {
         RotMat {
-            x_axis: Vec3::from_bytes(&bytes[..Vec3::NUM_BYTES]),
-            y_axis: Vec3::from_bytes(&bytes[Vec3::NUM_BYTES..Vec3::NUM_BYTES * 2]),
-            z_axis: Vec3::from_bytes(&bytes[Vec3::NUM_BYTES * 2..]),
+            forward: Vec3::from_bytes(&bytes[..Vec3::NUM_BYTES]),
+            right: Vec3::from_bytes(&bytes[Vec3::NUM_BYTES..Vec3::NUM_BYTES * 2]),
+            up: Vec3::from_bytes(&bytes[Vec3::NUM_BYTES * 2..]),
         }
     }
 }
 
 impl FromBytesExact for BallState {
     const NUM_BYTES: usize = Vec3::NUM_BYTES * 3;
 
@@ -601,24 +690,24 @@
                 &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 6
                     ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 8],
             ),
             auto_flip_torque_scale: f32::from_bytes(
                 &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 7
                     ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9],
             ),
-            has_contact: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9] != 0,
+            has_world_contact: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9] != 0,
             contact_normal: Vec3::from_bytes(
                 &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 8
                     ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9],
             ),
-            other_car_id: u32::from_bytes(
+            car_contact_id: u32::from_bytes(
                 &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 8
                     ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9 + u32::NUM_BYTES],
             ),
-            cooldown_timer: f32::from_bytes(
+            car_contact_cooldown_timer: f32::from_bytes(
                 &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 8 + u32::NUM_BYTES
                     ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 10 + u32::NUM_BYTES],
             ),
             is_demoed: bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 10 + u32::NUM_BYTES] != 0,
             demo_respawn_timer: f32::from_bytes(
                 &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 9 + u32::NUM_BYTES
                     ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 11 + u32::NUM_BYTES],
```

### Comparing `rlviser_py-0.2.2/src/gym.rs` & `rlviser_py-0.2.3/src/gym.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.2.2/src/lib.rs` & `rlviser_py-0.2.3/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 mod bytes;
 mod gym;
+mod rocketsim;
 mod socket;
 
 use crate::{
     bytes::{BoostPad, BoostPadState},
     gym::GymState,
 };
-use bytes::{BallState, CarConfig, CarInfo, CarState, GameState, Team, WheelPairConfig};
-use glam::{Mat3A, Quat, Vec3A};
+use bytes::{BallState, CarConfig, CarInfo, CarState, GameState, Team, Vec3, WheelPairConfig};
+use glam::{Mat3A, Quat};
 use gym::BOOST_PADS_LENGTH;
 use pyo3::prelude::*;
 use std::sync::{
     atomic::{AtomicU64, Ordering},
     RwLock,
 };
 
@@ -30,47 +31,48 @@
 
 pynamedmodule! {
     doc: "rlviser_py is a module for interacting with RLViser from Python",
     name: rlviser_py,
     funcs: [
         set_boost_pad_locations,
         render_rlgym,
+        render,
         quit
     ],
     classes: []
 }
 
 const TICK_RATE: f32 = 1. / 120.;
 
 static TICK_COUNT: AtomicU64 = AtomicU64::new(0);
-static BOOST_PAD_LOCATIONS: RwLock<[Vec3A; BOOST_PADS_LENGTH]> = RwLock::new([Vec3A::ZERO; BOOST_PADS_LENGTH]);
+static BOOST_PAD_LOCATIONS: RwLock<[Vec3; BOOST_PADS_LENGTH]> = RwLock::new([Vec3::ZERO; BOOST_PADS_LENGTH]);
 
 /// Set the boost pad locations to send to RLViser in each packet
 #[pyfunction]
 fn set_boost_pad_locations(locations: [[f32; 3]; BOOST_PADS_LENGTH]) {
     BOOST_PAD_LOCATIONS
         .write()
         .unwrap()
         .iter_mut()
-        .zip(locations.into_iter())
-        .for_each(|(rloc, pyloc)| *rloc = Vec3A::from_array(pyloc));
+        .zip(locations)
+        .for_each(|(rloc, pyloc)| *rloc = Vec3::from_array(pyloc));
 }
 
 pub const OCTANE: CarConfig = CarConfig {
-    hitbox_size: Vec3A::new(120.507, 86.6994, 38.6591),
-    hitbox_pos_offset: Vec3A::new(13.87566, 0., 20.755),
+    hitbox_size: Vec3::new(120.507, 86.6994, 38.6591),
+    hitbox_pos_offset: Vec3::new(13.87566, 0., 20.755),
     front_wheels: WheelPairConfig {
         wheel_radius: 12.5,
         suspension_rest_length: 38.755,
-        connection_point_offset: Vec3A::new(51.25, 25.9, 20.755),
+        connection_point_offset: Vec3::new(51.25, 25.9, 20.755),
     },
     back_wheels: WheelPairConfig {
         wheel_radius: 15.,
         suspension_rest_length: 37.055,
-        connection_point_offset: Vec3A::new(-33.75, 29.5, 20.755),
+        connection_point_offset: Vec3::new(-33.75, 29.5, 20.755),
     },
     dodge_deadzone: 0.5,
 };
 
 #[inline]
 fn array_to_quat(array: [f32; 4]) -> Quat {
     Quat::from_xyzw(-array[1], -array[2], array[3], array[0])
@@ -89,15 +91,15 @@
             ang_vel: gym_state.ball.angular_velocity.into(),
         },
         ball_rot: array_to_quat(gym_state.ball.quaternion),
         pads: BOOST_PAD_LOCATIONS
             .read()
             .unwrap()
             .into_iter()
-            .zip(gym_state.boost_pads.into_iter())
+            .zip(gym_state.boost_pads)
             .map(|(position, is_active)| BoostPad {
                 position,
                 is_big: position.z == 73.,
                 state: BoostPadState {
                     is_active: is_active > 0.5,
                     ..Default::default()
                 },
@@ -110,27 +112,68 @@
             .map(|(id, player)| CarInfo {
                 id: id as u32 + 1,
                 team: if player.team_num < 0.5 { Team::Blue } else { Team::Orange },
                 state: CarState {
                     pos: player.car_data.position.into(),
                     vel: player.car_data.linear_velocity.into(),
                     ang_vel: player.car_data.angular_velocity.into(),
-                    rot_mat: Mat3A::from_quat(array_to_quat(player.car_data.quaternion)),
+                    rot_mat: Mat3A::from_quat(array_to_quat(player.car_data.quaternion)).into(),
                     is_on_ground: player.on_ground != 0,
                     is_demoed: player.is_demoed != 0,
                     has_flipped: player.has_flip == 0,
                     has_jumped: player.has_jump == 0,
                     ..Default::default()
                 },
                 config: OCTANE,
             })
             .collect(),
     };
 
     socket::send_game_state(&game_state).unwrap();
 }
 
+#[pyfunction]
+fn render(
+    tick_count: u64,
+    tick_rate: f32,
+    boost_pad_states: [bool; BOOST_PADS_LENGTH],
+    ball: BallState,
+    cars: Vec<(u32, u8, CarConfig, rocketsim::CarState)>,
+) {
+    let game_state = GameState {
+        tick_count,
+        tick_rate,
+        ball,
+        // no way of getting rotation right now
+        ball_rot: Quat::IDENTITY,
+        pads: BOOST_PAD_LOCATIONS
+            .read()
+            .unwrap()
+            .into_iter()
+            .zip(boost_pad_states)
+            .map(|(position, is_active)| BoostPad {
+                position,
+                is_big: position.z == 73.,
+                state: BoostPadState {
+                    is_active,
+                    ..Default::default()
+                },
+            })
+            .collect(),
+        cars: cars
+            .into_iter()
+            .map(|(id, team, config, state)| CarInfo {
+                id,
+                team: Team::from_u8(team),
+                config,
+                state: state.into(),
+            })
+            .collect(),
+    };
+    socket::send_game_state(&game_state).unwrap();
+}
+
 /// Send the quit signal to RLViser
 #[pyfunction]
 fn quit() {
     socket::quit().unwrap();
 }
```

### Comparing `rlviser_py-0.2.2/src/socket.rs` & `rlviser_py-0.2.3/src/socket.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.2.2/Cargo.lock` & `rlviser_py-0.2.3/Cargo.lock`

 * *Files 12% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "glam"
-version = "0.24.0"
+version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad83ab008a4fa3b31dfa713dd41b5a9bdea1e94e4cf1e2fc274ffbd49b0271d3"
+checksum = "42218cb640844e3872cc3c153dc975229e080a6c4733b34709ef445610550226"
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
@@ -84,86 +84,86 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
@@ -171,67 +171,67 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rlviser-py"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "glam",
  "once_cell",
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
```

### Comparing `rlviser_py-0.2.2/PKG-INFO` & `rlviser_py-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlviser-py
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python implementation that manages a UDP connection to RLViser
 Keywords: rlviser,rocket-league,udp,python,rlbot
 License: MIT
```

