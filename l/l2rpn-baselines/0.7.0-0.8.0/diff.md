# Comparing `tmp/l2rpn_baselines-0.7.0.tar.gz` & `tmp/l2rpn_baselines-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2rpn_baselines-0.7.0.tar", last modified: Thu Jul 13 12:25:09 2023, max compression
+gzip compressed data, was "l2rpn_baselines-0.8.0.tar", last modified: Mon Jul 24 14:43:06 2023, max compression
```

## Comparing `l2rpn_baselines-0.7.0.tar` & `l2rpn_baselines-0.8.0.tar`

### file list

```diff
@@ -1,178 +1,181 @@
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.050962 l2rpn_baselines-0.7.0/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       67 2020-07-05 18:33:35.000000 l2rpn_baselines-0.7.0/MANIFEST.in
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2963 2023-07-13 12:25:09.050962 l2rpn_baselines-0.7.0/PKG-INFO
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1496 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/README.md
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.878962 l2rpn_baselines-0.7.0/l2rpn_baselines/
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.906962 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7899 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/Action_reduced_list.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    24276 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/ActorCritic_Agent.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    24393 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/AsynchronousActorCritic.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2711 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/Runner.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      927 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7650 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      710 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/run_grid2viz.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7085 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/train.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1446 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/user_environment_make.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.910962 l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      253 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    20167 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/baseline.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4642 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2520 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.914962 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      785 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1051 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQSimple.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3000 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQ_NN.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2039 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQ_NNParam.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7048 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/evaluate.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    13151 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.918962 l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      168 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1182 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/doNothing.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3825 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/eval_donothing.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      192 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/main.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.930962 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      387 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15296 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2014 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQNConfig.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6671 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN_NN.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5376 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/evaluate.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3853 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/inspect_action_space.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7010 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/prioritized_replay_buffer.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5411 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/segment_tree.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5234 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.938962 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      398 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15146 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1984 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQNConfig.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7463 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN_NN.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5386 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3277 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/experienceBuffer.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5411 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.942962 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      338 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1339 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     9326 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet_NN.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7262 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3682 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/leapNet_NNParam.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    17875 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.950962 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      325 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1163 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQSimple.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3259 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQ_NN.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1814 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQ_NNParam.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7444 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/evaluate.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    13127 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.950962 l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      259 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6474 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    23719 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/expertAgent.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.958962 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4716 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/DDQN_NN.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    26004 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/Geirina.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      962 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4164 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4166 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/generate_action_space.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4359 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/prioritized_memory.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2741 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.970962 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11803 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/Kaist.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      140 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3976 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/check_your_submission.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8092 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/converter.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3707 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3905 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/models.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3948 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/sublayer.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.978962 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       34 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11849 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/agent.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8009 2023-07-13 12:12:49.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/converter.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3970 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/models.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3954 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/sublayer.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      763 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/submission.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.982962 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/utils/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      441 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/utils/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      418 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/utils/zip_dir.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3302 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/utils/zip_for_codalab.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.990962 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      358 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7327 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1262 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15449 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NN.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8656 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NNParam.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6074 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/study.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    17952 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.994962 l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      706 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      549 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2907 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/make_agent.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    53226 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/optimCVXPY.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.998962 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      699 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4179 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/env_rllib.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8761 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11078 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/rllibagent.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10417 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.006962 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1072 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10730 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    13122 2022-11-29 14:09:24.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/train.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    12448 2022-07-11 09:20:27.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/utils.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.010962 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3995 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/OPF_saveload_investigation.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    17638 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/PandapowerOPFAgent.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      956 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/__init__.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3696 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4264 2023-07-13 12:12:50.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/pp_functions.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.018962 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      293 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6946 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1284 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    13601 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld_NN.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3033 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld_NNParam.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    14025 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.026962 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      321 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/__init__.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5145 2022-11-29 14:09:20.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3277 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/experienceBuffer.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15513 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1570 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN_Config.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10790 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN_NN.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5440 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/slice_util.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5644 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.030962 l2rpn_baselines-0.7.0/l2rpn_baselines/Template/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1005 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Template/__init__.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3957 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Template/evaluate.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6151 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Template/template.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     2603 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/Template/train.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.030962 l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2010 2023-06-19 09:23:59.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/TopoOracleAgent.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      259 2023-06-19 09:23:59.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8267 2023-06-19 09:23:59.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/evaluate.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     9436 2023-06-19 09:23:59.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/train.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      913 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/__init__.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:09.050962 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1576 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10366 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/baseDeepQ.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2225 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/cli_eval.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1990 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/cli_train.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    51498 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/deepQAgent.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8560 2023-01-24 08:55:34.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/gymAgent.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    16162 2023-02-03 14:21:58.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/gymenv_custom.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2253 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/make_multi_env.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11336 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/nnParam.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2416 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/replayBuffer.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1782 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/save_log_gif.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      789 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/str2bool.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2459 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/train_generic.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    16056 2022-07-04 14:17:45.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/trainingParam.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      631 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/waring_msgs.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4138 2022-01-20 14:34:19.000000 l2rpn_baselines-0.7.0/l2rpn_baselines/utils/zip_for_codalab.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-13 12:25:08.894962 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2963 2023-07-13 12:25:08.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/PKG-INFO
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6275 2023-07-13 12:25:08.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/SOURCES.txt
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        1 2023-07-13 12:25:08.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/dependency_links.txt
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        1 2022-02-03 09:33:41.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/not-zip-safe
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      401 2023-07-13 12:25:08.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/requires.txt
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       16 2023-07-13 12:25:08.000000 l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/top_level.txt
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       38 2023-07-13 12:25:09.050962 l2rpn_baselines-0.7.0/setup.cfg
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2685 2023-07-13 12:01:30.000000 l2rpn_baselines-0.7.0/setup.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.371964 l2rpn_baselines-0.8.0/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      609 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/AUTHORS.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    16725 2020-07-05 18:33:35.000000 l2rpn_baselines-0.8.0/LICENSE
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    16725 2020-07-05 18:33:35.000000 l2rpn_baselines-0.8.0/LICENSE.md
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       67 2020-07-05 18:33:35.000000 l2rpn_baselines-0.8.0/MANIFEST.in
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2565 2023-07-24 14:43:06.371964 l2rpn_baselines-0.8.0/PKG-INFO
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1496 2023-07-13 12:01:30.000000 l2rpn_baselines-0.8.0/README.md
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.219962 l2rpn_baselines-0.8.0/l2rpn_baselines/
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.239962 l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7899 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/Action_reduced_list.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    24276 2023-07-24 14:34:03.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/ActorCritic_Agent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    24393 2023-07-24 14:34:03.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/AsynchronousActorCritic.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2711 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/Runner.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      927 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7650 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      710 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/run_grid2viz.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7085 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/train.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1446 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/user_environment_make.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.247962 l2rpn_baselines-0.8.0/l2rpn_baselines/CurriculumAgent/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      253 2023-07-13 12:01:30.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/CurriculumAgent/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    20167 2023-07-13 12:01:30.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/CurriculumAgent/baseline.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4642 2023-07-13 12:01:30.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/CurriculumAgent/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2520 2023-07-13 12:01:30.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/CurriculumAgent/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.251962 l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      785 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1051 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/deepQSimple.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3000 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/deepQ_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2039 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/deepQ_NNParam.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7048 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/evaluate.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    13151 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.255962 l2rpn_baselines-0.8.0/l2rpn_baselines/DoNothing/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      168 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoNothing/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1182 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoNothing/doNothing.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3825 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoNothing/eval_donothing.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      192 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoNothing/main.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.267963 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      387 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15296 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2014 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQNConfig.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6805 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN_NN.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5376 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/evaluate.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3853 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/inspect_action_space.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7010 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/prioritized_replay_buffer.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5411 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/segment_tree.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5234 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.275963 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      398 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15146 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1984 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQNConfig.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7474 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN_NN.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5386 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3277 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/experienceBuffer.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5411 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.279963 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      338 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1339 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     9462 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7262 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3682 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/leapNet_NNParam.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    17875 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.287963 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      325 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1163 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/duelQSimple.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3259 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/duelQ_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1814 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/duelQ_NNParam.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7444 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/evaluate.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    13127 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.287963 l2rpn_baselines-0.8.0/l2rpn_baselines/ExpertAgent/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      259 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/ExpertAgent/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6474 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/ExpertAgent/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    23719 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/ExpertAgent/expertAgent.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.291963 l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4716 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/DDQN_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    26004 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/Geirina.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      962 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4164 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4166 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/generate_action_space.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4359 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/prioritized_memory.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2741 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.299963 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11803 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/Kaist.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      140 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3976 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/check_your_submission.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8092 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/converter.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3707 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3905 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/models.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3948 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/sublayer.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.303963 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       34 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11849 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/agent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8009 2023-07-13 12:12:49.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/converter.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3970 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/models.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3954 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/sublayer.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      763 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/submission.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.307963 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/utils/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      441 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/utils/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      418 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/utils/zip_dir.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3302 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/utils/zip_for_codalab.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.315963 l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      358 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7327 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1262 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15585 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8656 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NNParam.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6074 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/study.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    17952 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.315963 l2rpn_baselines-0.8.0/l2rpn_baselines/OptimCVXPY/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      706 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/OptimCVXPY/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      549 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/OptimCVXPY/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2907 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/OptimCVXPY/make_agent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    53226 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/OptimCVXPY/optimCVXPY.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.323963 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      774 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5526 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/env_rllib.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8761 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11059 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/rllibagent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10380 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.323963 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_SB3/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1072 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_SB3/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10730 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_SB3/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    13122 2022-11-29 14:09:24.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_SB3/train.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    12448 2022-07-11 09:20:27.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_SB3/utils.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.327963 l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3995 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/OPF_saveload_investigation.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    17638 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/PandapowerOPFAgent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      956 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/__init__.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3696 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4264 2023-07-13 12:12:50.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/pp_functions.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.331963 l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      293 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6946 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1284 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/sacOld.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    13601 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/sacOld_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3033 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/sacOld_NNParam.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    14025 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.343964 l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      321 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/__init__.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5145 2022-11-29 14:09:20.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3277 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/experienceBuffer.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    15513 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/sliceRDQN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1570 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/sliceRDQN_Config.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10801 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/sliceRDQN_NN.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5440 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/slice_util.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5644 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.347964 l2rpn_baselines-0.8.0/l2rpn_baselines/Template/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1005 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Template/__init__.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     3957 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Template/evaluate.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6151 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Template/template.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     2603 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/Template/train.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.351964 l2rpn_baselines-0.8.0/l2rpn_baselines/TopoOracleAgent/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2010 2023-06-19 09:23:59.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/TopoOracleAgent/TopoOracleAgent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      259 2023-06-19 09:23:59.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/TopoOracleAgent/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8267 2023-06-19 09:23:59.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/TopoOracleAgent/evaluate.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     9436 2023-06-19 09:23:59.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/TopoOracleAgent/train.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      913 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/__init__.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.367964 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1576 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10366 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/baseDeepQ.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2225 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/cli_eval.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1990 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/cli_train.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    51671 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/deepQAgent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8622 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/gymAgent.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    16636 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/gymenv_custom.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2253 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/make_multi_env.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11336 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/nnParam.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2416 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/replayBuffer.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1782 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/save_log_gif.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      789 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/str2bool.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2459 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/train_generic.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    16056 2022-07-04 14:17:45.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/trainingParam.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      631 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/waring_msgs.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4138 2022-01-20 14:34:19.000000 l2rpn_baselines-0.8.0/l2rpn_baselines/utils/zip_for_codalab.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2023-07-24 14:43:06.227962 l2rpn_baselines-0.8.0/l2rpn_baselines.egg-info/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2565 2023-07-24 14:43:06.000000 l2rpn_baselines-0.8.0/l2rpn_baselines.egg-info/PKG-INFO
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6306 2023-07-24 14:43:06.000000 l2rpn_baselines-0.8.0/l2rpn_baselines.egg-info/SOURCES.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        1 2023-07-24 14:43:06.000000 l2rpn_baselines-0.8.0/l2rpn_baselines.egg-info/dependency_links.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        1 2022-02-03 09:33:41.000000 l2rpn_baselines-0.8.0/l2rpn_baselines.egg-info/not-zip-safe
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      391 2023-07-24 14:43:06.000000 l2rpn_baselines-0.8.0/l2rpn_baselines.egg-info/requires.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       16 2023-07-24 14:43:06.000000 l2rpn_baselines-0.8.0/l2rpn_baselines.egg-info/top_level.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       38 2023-07-24 14:43:06.371964 l2rpn_baselines-0.8.0/setup.cfg
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2692 2023-07-24 14:42:58.000000 l2rpn_baselines-0.8.0/setup.py
```

### Comparing `l2rpn_baselines-0.7.0/PKG-INFO` & `l2rpn_baselines-0.8.0/l2rpn_baselines.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,84 @@
 Metadata-Version: 2.1
-Name: l2rpn_baselines
-Version: 0.7.0
+Name: l2rpn-baselines
+Version: 0.8.0
 Summary: L2RPN Baselines a repository to host baselines for l2rpn competitions.
 Home-page: https://github.com/rte-france/L2RPN_Baselines
 Author: Benjamin DONNOT
 Author-email: benjamin.donnot@rte-france.com
 License: MPL
-Description: # L2RPN_Baselines
-        Repository hosting reference baselines for the [L2RPN challenge](https://l2rpn.chalearn.org/)
-        
-        # Install 
-        
-        ## Requirements
-        `python3 >= 3.6`
-        
-        ## Instal from PyPI
-        ```sh
-        pip3 install l2rpn_baselines
-        ```
-        ## Install from source
-        ```sh
-        git clone https://github.com/rte-france/l2rpn-baselines.git
-        cd l2rpn-baselines
-        pip3 install -U .
-        cd ..
-        rm -rf l2rpn-baselines
-        ```
-        
-        # Contribute
-        
-        We welcome contributions: see the [contribute guide](/CONTRIBUTE.md) for details.
-        
-        # Get started with a baseline
-        
-        Say you want to know how you compared with the "PPO_SB3" baseline implementation in this repository (for the
-        sake of this example).
-        
-        ## Train it (optional)
-        As no weights are provided for this baselines by default (yet), you will first need to train such a baseline:
-        
-        ```python
-        import grid2op
-        from l2rpn_baselines.PPO_SB3 import train
-        env = grid2op.make("l2rpn_case14_sandbox")
-        res = train(env, save_path="THE/PATH/TO/SAVE/IT", iterations=100)
-        ```
-        
-        You can have more information about extra argument of the "train" function in the 
-        [CONTRIBUTE](/CONTRIBUTE.md) file.
-        
-        ## Evaluate it
-        Once trained, you can reload it and evaluate its performance with the provided "evaluate" function:
-        
-        ```python
-        import grid2op
-        from l2rpn_baselines.PPO_SB3 import evaluate
-        env = grid2op.make("l2rpn_case14_sandbox")
-        res = evaluate(env, load_path="THE/PATH/TO/LOAD/IT", nb_episode=10)
-        ```
-        
-        You can have more information about extra argument of the "evaluate" function in the 
-        [CONTRIBUTE](/CONTRIBUTE.md) file.
-        
 Keywords: ML powergrid optmization RL power-systems
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
-Provides-Extra: CurriculumAgent
-Provides-Extra: PPO_RLLIB
-Provides-Extra: PPO_SB3
 Provides-Extra: docs
 Provides-Extra: optional
+Provides-Extra: PPO_RLLIB
+Provides-Extra: PPO_SB3
+Provides-Extra: CurriculumAgent
+License-File: LICENSE
+License-File: LICENSE.md
+License-File: AUTHORS.txt
+
+# L2RPN_Baselines
+Repository hosting reference baselines for the [L2RPN challenge](https://l2rpn.chalearn.org/)
+
+# Install 
+
+## Requirements
+`python3 >= 3.6`
+
+## Instal from PyPI
+```sh
+pip3 install l2rpn_baselines
+```
+## Install from source
+```sh
+git clone https://github.com/rte-france/l2rpn-baselines.git
+cd l2rpn-baselines
+pip3 install -U .
+cd ..
+rm -rf l2rpn-baselines
+```
+
+# Contribute
+
+We welcome contributions: see the [contribute guide](/CONTRIBUTE.md) for details.
+
+# Get started with a baseline
+
+Say you want to know how you compared with the "PPO_SB3" baseline implementation in this repository (for the
+sake of this example).
+
+## Train it (optional)
+As no weights are provided for this baselines by default (yet), you will first need to train such a baseline:
+
+```python
+import grid2op
+from l2rpn_baselines.PPO_SB3 import train
+env = grid2op.make("l2rpn_case14_sandbox")
+res = train(env, save_path="THE/PATH/TO/SAVE/IT", iterations=100)
+```
+
+You can have more information about extra argument of the "train" function in the 
+[CONTRIBUTE](/CONTRIBUTE.md) file.
+
+## Evaluate it
+Once trained, you can reload it and evaluate its performance with the provided "evaluate" function:
+
+```python
+import grid2op
+from l2rpn_baselines.PPO_SB3 import evaluate
+env = grid2op.make("l2rpn_case14_sandbox")
+res = evaluate(env, load_path="THE/PATH/TO/LOAD/IT", nb_episode=10)
+```
+
+You can have more information about extra argument of the "evaluate" function in the 
+[CONTRIBUTE](/CONTRIBUTE.md) file.
```

### Comparing `l2rpn_baselines-0.7.0/README.md` & `l2rpn_baselines-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/Action_reduced_list.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/Action_reduced_list.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/ActorCritic_Agent.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/ActorCritic_Agent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/AsynchronousActorCritic.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/AsynchronousActorCritic.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/Runner.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/Runner.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/__init__.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/run_grid2viz.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/run_grid2viz.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/AsynchronousActorCritic/user_environment_make.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/AsynchronousActorCritic/user_environment_make.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/baseline.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/CurriculumAgent/baseline.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/CurriculumAgent/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/CurriculumAgent/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/CurriculumAgent/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/__init__.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQSimple.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/deepQSimple.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQ_NN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/deepQ_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/deepQ_NNParam.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/deepQ_NNParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DeepQSimple/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DeepQSimple/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/doNothing.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoNothing/doNothing.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoNothing/eval_donothing.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoNothing/eval_donothing.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQNConfig.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQNConfig.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN_NN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/doubleDuelingDQN_NN.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,18 @@
         grads = tape.gradient(loss, self.model.trainable_variables)
 
         # Apply gradients
         grad_pairs = zip(grads, self.model.trainable_variables)
         self.optimizer.apply_gradients(grad_pairs)
 
         # Store LR
-        self.train_lr = self.optimizer._decayed_lr('float32').numpy()
+        if hasattr(self.optimizer, "_decayed_lr"):
+            self.train_lr = self.optimizer._decayed_lr('float32').numpy()
+        else:
+            self.train_lr = self.optimizer.learning_rate.numpy()
         # Return loss scalar
         return loss.numpy()
 
     def _batch_loss(self, y_true, y_pred):
         sq_error = tf.math.square(y_true - y_pred, name="sq_error")
 
         # We store it because that's the priorities vector
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/inspect_action_space.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/inspect_action_space.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/prioritized_replay_buffer.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/prioritized_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/segment_tree.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/segment_tree.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingDQN/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingDQN/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQNConfig.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQNConfig.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN_NN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/doubleDuelingRDQN_NN.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                                outputs=model_outputs,
                                name=self.__class__.__name__)
         losses = [
             self._mse_loss,
             self._no_loss,
             self._no_loss
         ]
-        self.optimizer = tfko.Adam(lr=self.lr, clipnorm=1.0)
+        self.optimizer = tfko.Adam(learning_rate=self.lr, clipnorm=1.0)
         self.model.compile(loss=losses, optimizer=self.optimizer)
 
     def _no_loss(self, y_true, y_pred):
         return 0.0
 
     def _mse_loss(self, Qnext, Q):
         loss = tf.math.reduce_mean(tf.math.square(Qnext - Q), name="loss_mse")
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/experienceBuffer.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/experienceBuffer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DoubleDuelingRDQN/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DoubleDuelingRDQN/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet_NN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/duelQLeapNet_NN.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,18 @@
             grads, _ = tf.clip_by_global_norm(grads, self._max_global_norm_grad)
         if self._max_value_grad is not None:
             grads = [tf.clip_by_value(grad, -self._max_value_grad, self._max_value_grad) for grad in grads]
 
         # Apply gradients
         optimizer_model.apply_gradients(zip(grads, model.trainable_variables))
         # Store LR
-        self.train_lr = optimizer_model._decayed_lr('float32').numpy()
+        if hasattr(optimizer_model, "_decayed_lr"):
+            self.train_lr = optimizer_model._decayed_lr('float32').numpy()
+        else:
+            self.train_lr = optimizer_model.learning_rate.numpy()
         # Return loss scalar
         return loss_npy
 
     def _clipped_batch_loss(self, y_true, y_pred):
         sq_error = tf.math.square(y_true - y_pred, name="sq_error")
         batch_sq_error = tf.math.reduce_sum(sq_error, axis=1, name="batch_sq_error")
         if self._max_loss is not None:
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/leapNet_NNParam.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/leapNet_NNParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQLeapNet/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQLeapNet/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQSimple.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/duelQSimple.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQ_NN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/duelQ_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/duelQ_NNParam.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/duelQ_NNParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/DuelQSimple/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/DuelQSimple/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/ExpertAgent/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/ExpertAgent/expertAgent.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/ExpertAgent/expertAgent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/DDQN_NN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/DDQN_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/Geirina.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/Geirina.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/__init__.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/generate_action_space.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/generate_action_space.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/prioritized_memory.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/prioritized_memory.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Geirina/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Geirina/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/Kaist.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/Kaist.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/check_your_submission.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/check_your_submission.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/converter.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/converter.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/models.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/models.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/sublayer.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/sublayer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/agent.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/agent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/converter.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/converter.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/models.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/models.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/sublayer.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/sublayer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/submission/submission.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/submission/submission.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Kaist/utils/zip_for_codalab.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Kaist/utils/zip_for_codalab.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NN.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,15 +301,18 @@
         if self._max_value_grad is not None:
             grads = [tf.clip_by_value(grad, -self._max_value_grad, self._max_value_grad)
                      for grad in grads]
 
         # Apply gradients
         optimizer_model.apply_gradients(zip(grads, self._qnet_variables))
         # Store LR
-        self.train_lr = optimizer_model._decayed_lr('float32').numpy()
+        if hasattr(optimizer_model, "_decayed_lr"):
+            self.train_lr = optimizer_model._decayed_lr('float32').numpy()
+        else:
+            self.train_lr = optimizer_model.learning_rate.numpy()
 
         # Return loss scalar
         return loss_npy
 
     def _clipped_batch_loss(self, y_true, y_pred):
         sq_error = tf.math.square(y_true - y_pred, name="sq_error")
         batch_sq_error = tf.math.reduce_sum(sq_error, axis=1, name="batch_sq_error")
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NNParam.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/leapNetEncoded_NNParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/study.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/study.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/LeapNetEncoded/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/LeapNetEncoded/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/__init__.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/OptimCVXPY/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/OptimCVXPY/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/make_agent.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/OptimCVXPY/make_agent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/OptimCVXPY/optimCVXPY.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/OptimCVXPY/optimCVXPY.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/__init__.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,13 +5,15 @@
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of L2RPN Baselines, L2RPN Baselines a repository to host baselines for l2rpn competitions.
 
 __all__ = [
     "evaluate",
     "train",
-    "PPO_RLLIB"
+    "PPO_RLLIB",
+    "Env_RLLIB"
 ]
 
 from l2rpn_baselines.PPO_RLLIB.rllibagent import RLLIBAgent as PPO_RLLIB
 from l2rpn_baselines.PPO_RLLIB.evaluate import evaluate
 from l2rpn_baselines.PPO_RLLIB.train import train
+from l2rpn_baselines.PPO_RLLIB.env_rllib import Env_RLLIB
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/env_rllib.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/env_rllib.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,20 +2,33 @@
 # See AUTHORS.txt
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of L2RPN Baselines, L2RPN Baselines a repository to host baselines for l2rpn competitions.
 
-import gym
+
 import grid2op
-from grid2op.gym_compat import BoxGymActSpace, BoxGymObsSpace, GymEnv
+from grid2op.gym_compat import (BoxGymActSpace,
+                                BoxGymObsSpace,
+                                GymEnv
+                                )
+from grid2op.gym_compat.utils import ALL_ATTR_CONT
+from grid2op.gym_compat.box_gym_obsspace import ALL_ATTR_OBS
 from l2rpn_baselines.PPO_SB3 import remove_non_usable_attr
 
 
+if GymEnv._gymnasium:
+    import gymnasium as gym
+    from gymnasium.spaces import Box
+else:
+    import gym
+    from gym.spaces import Box
+
+
 class Env_RLLIB(gym.Env):
     """
     This class represents the Environment usable
     from rllib, mapping a grid2op environment.
     
     It is primarily made to serve as example of what is possible to achieve.
     You might probably want to customize this environment to your specific
@@ -23,15 +36,23 @@
 
     This agents uses the rllib framework to code for 
     a neural network.
     
     .. warning::
         A grid2op environment is created  when this agent is made. We found
         out rllib worked better this way.
+    
+    .. alert::
+        This class inherits either from `gymnasium.Env` or 
+        `gym.Env` depending on grid2op underlying `GymEnv` base class.
+        
+        Please consult grid2op docs for more information.
         
+        By default it should be a gymnasium environment !
+    
     To be built, it requires the `env_config` parameters. This parameter is a 
     dictionnary with keys:
     
     - "env_name": the name of the environment you want to make
     - "obs_attr_to_keep": the attributes of the observation you want to use
       in the gym observation space (gym observation space is converted
       to a Box)
@@ -57,45 +78,60 @@
         if "obs_attr_to_keep" in env_config:
             obs_attr_to_keep = env_config["obs_attr_to_keep"]
             del  env_config["obs_attr_to_keep"]
         act_attr_to_keep = None
         if "act_attr_to_keep" in env_config:  
             act_attr_to_keep = env_config["act_attr_to_keep"]
             del  env_config["act_attr_to_keep"]
+            
         if "backend_class" in env_config:
             backend_kwargs = {}
             if "backend_kwargs" in env_config:
                 backend_kwargs = env_config["backend_kwargs"]
                 del env_config["backend_kwargs"]
             backend = env_config["backend_class"](**backend_kwargs)
             del  env_config["backend_class"]
+        else:
+            try:
+                from lightsim2grid import LightSimBackend
+                backend = LightSimBackend()
+            except ImportError as exc_:
+                from grid2op.Backend import PandaPowerBackend
+                backend = PandaPowerBackend()
+                
             
         # 1. create the grid2op environment
         self.env_glop = grid2op.make(nm_env, backend=backend, **env_config)
         # clean the attribute
         act_attr_to_keep = remove_non_usable_attr(self.env_glop, act_attr_to_keep)
         
         # 2. create the gym environment
         self.env_gym = GymEnv(self.env_glop)
 
-        # 3. customize action space
-        if obs_attr_to_keep is not None:
-            self.env_gym.observation_space.close()
-            self.env_gym.observation_space =  BoxGymObsSpace(self.env_glop.observation_space,
-                                                             attr_to_keep=obs_attr_to_keep)
-        
-        if act_attr_to_keep is not None:    
-            self.env_gym.action_space.close()
-            self.env_gym.action_space = BoxGymActSpace(self.env_glop.action_space,
-                                                       attr_to_keep=act_attr_to_keep)
+        # 3. customize action space and observation space
+        if obs_attr_to_keep is None:
+            obs_attr_to_keep = ALL_ATTR_OBS
+        
+        self.env_gym.observation_space.close()
+        self.env_gym.observation_space = BoxGymObsSpace(self.env_glop.observation_space,
+                                                        attr_to_keep=obs_attr_to_keep)
+        
+        if act_attr_to_keep is None:    
+            act_attr_to_keep = ALL_ATTR_CONT
+        self.env_gym.action_space.close()
+        self.env_gym.action_space = BoxGymActSpace(self.env_glop.action_space,
+                                                    attr_to_keep=act_attr_to_keep)
 
         # 4. specific to rllib
-        self.action_space = self.env_gym.action_space
-        self.observation_space = self.env_gym.observation_space
-
-    def reset(self):
-        obs = self.env_gym.reset()
-        return obs
-
+        self.action_space = Box(low=self.env_gym.action_space.low,
+                                high=self.env_gym.action_space.high,
+                                shape=self.env_gym.action_space.shape)
+        self.observation_space = Box(low=self.env_gym.observation_space.low,
+                                     high=self.env_gym.observation_space.high,
+                                     shape=self.env_gym.observation_space.shape)
+
+    def reset(self, *, seed=None, options=None):
+        tmp = self.env_gym.reset(seed=seed, options=options)
+        return tmp
+    
     def step(self, action):
-        obs, reward, done, info = self.env_gym.step(action)
-        return obs, reward, done, info
+        return self.env_gym.step(action)
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/rllibagent.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/rllibagent.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,61 +2,62 @@
 # See AUTHORS.txt
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of L2RPN Baselines, L2RPN Baselines a repository to host baselines for l2rpn competitions.
 
-import copy
 import os
 import re
-from typing import List, Optional
 
 from l2rpn_baselines.utils import GymAgent
 from l2rpn_baselines.PPO_RLLIB.env_rllib import Env_RLLIB
 
 try:
-    from ray.rllib.agents.ppo import PPOTrainer
+    try:
+        from ray.rllib.algorithms.ppo import PPO
+    except ImportError:
+        from ray.rllib.agents.ppo import PPOTrainer as PPO
     _CAN_USE_RLLIB = True
 except ImportError:
     _CAN_USE_RLLIB = False
     
-    class PPOTrainer(object):
+    class PPO(object):
         """
         Do not use, this class is a template when rllib is not installed.
         
-        It represents `from ray.rllib.agents.ppo import PPOTrainer`
+        It represents `from ray.rllib.algorithms.ppo import PPO`
         """
         
 
 class RLLIBAgent(GymAgent):
     """This class represents the Agent (directly usable with grid2op framework)
 
-    This agents uses the stable baseline `nn_type` (by default PPOTrainer) as
+    This agents uses the stable baseline `nn_type` (by default PPO) as
     the neural network to take decisions on the grid.
     
     To be built, it requires:
     
     - `g2op_action_space`: a grid2op action space (used for initializing the grid2op agent)
     - `gym_act_space`: a gym observation space (used for the neural networks)
     - `gym_obs_space`: a gym action space (used for the neural networks)
     - `nn_config`: the parameters used to build the rllib "trainer" (the thing
       tagged "nn_config" in rllib)
     
     It can also accept different types of parameters:
     
-    - `nn_type`: the type of "neural network" from rllib (by default PPOTrainer)
+    - `nn_type`: the type of "neural network" from rllib (by default PPO)
     - `nn_path`: the path where the neural network can be loaded from
     
     For this class `nn_config` is mandatory. The trainer is built with:
     
     .. code-block:: python
     
         from l2rpn_baselines.PPO_RLLIB import Env_RLLIB
-        PPOTrainer(env=Env_RLLIB, config=nn_config)
+        PPO(env=Env_RLLIB, config=nn_config)
     
     Examples
     ---------
     The best way to have such an agent is either to train it:
     
     .. code-block:: python
     
@@ -106,15 +107,15 @@
                       # function eg:
                       # "param": ...
                       # "reward_class": ...
                       # "other_reward": ...
                       # "difficulty": ...
                       }
 
-        # now define the configuration for the PPOTrainer
+        # now define the configuration for the PPO
         env_config_ppo = {
             # config to pass to env class
             "env_config": env_config,
             #neural network config
             "lr": 1e-4, # learning_rate
             "model": {
                 "fcnet_hiddens": [100, 100, 100],  # neural net architecture
@@ -142,15 +143,15 @@
                                    
     """
     def __init__(self,
                  g2op_action_space,
                  gym_act_space,
                  gym_obs_space,
                  nn_config,
-                 nn_type=PPOTrainer,
+                 nn_type=PPO,
                  nn_path=None,
                  ):
         if not _CAN_USE_RLLIB:
             raise ImportError("Cannot import ray[rllib]. Impossible to use this class.")
         
         self._nn_type = nn_type
         if nn_config is None:
@@ -190,15 +191,15 @@
         """
         Load the NN model.
         
         In the case of a PPO agent, this is equivalent to perform the:
         
         .. code-block:: python
             
-            PPOTrainer.restore(nn_path)
+            PPO.restore(nn_path)
             
         """
         self.build()
         chkts = sorted(os.listdir(self._nn_path))
         last_chkts = [re.match("checkpoint_[0-9]+$", el) is not None
                      for el in chkts]
         last_chkts = [el for el, ok_ in zip(chkts, last_chkts) if ok_]
@@ -214,18 +215,18 @@
     def build(self):
         """Create the underlying NN model from scratch.
         
         In the case of a PPO agent, this is equivalent to perform the:
         
         .. code-block:: python
             
-            PPOTrainer(env= Env_RLLIB, config=nn_config)
+            PPO(env= Env_RLLIB, config=nn_config)
             
         """
-        self.nn_model = PPOTrainer(**self._nn_kwargs)
+        self.nn_model = PPO(**self._nn_kwargs)
 
 if __name__ == "__main__":
     import grid2op
     from grid2op.gym_compat import BoxGymObsSpace, BoxGymActSpace
     from lightsim2grid import LightSimBackend
     
     env_name = "l2rpn_case14_sandbox"  # or any other name
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_RLLIB/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_RLLIB/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
                                      save_used_attribute,
                                      remove_non_usable_attr
                                     )
 from l2rpn_baselines.PPO_RLLIB.rllibagent import RLLIBAgent
 
 try:
     import ray
-    from ray.rllib.agents import ppo
     from ray.tune.logger import pretty_print
     _CAN_USE_RLLIB = True
 except ImportError as exc_:
     _CAN_USE_RLLIB = False
 
 
 def train(env,
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/__init__.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_SB3/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_SB3/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_SB3/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PPO_SB3/utils.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PPO_SB3/utils.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/OPF_saveload_investigation.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/OPF_saveload_investigation.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/PandapowerOPFAgent.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/PandapowerOPFAgent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/__init__.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/PandapowerOPFAgent/pp_functions.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/PandapowerOPFAgent/pp_functions.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/sacOld.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld_NN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/sacOld_NN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/sacOld_NNParam.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/sacOld_NNParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SACOld/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SACOld/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/experienceBuffer.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/experienceBuffer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/sliceRDQN.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN_Config.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/sliceRDQN_Config.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/sliceRDQN_NN.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/sliceRDQN_NN.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
                                outputs=model_outputs,
                                name=self.__class__.__name__)
         losses = [
             self._clipped_mse_loss,
             self._no_loss,
             self._no_loss
         ]
-        self.optimizer = tfko.Adam(lr=self.lr, clipnorm=1.0)
+        self.optimizer = tfko.Adam(learning_rate=self.lr, clipnorm=1.0)
         self.model.compile(loss=losses, optimizer=self.optimizer)
 
     def _no_loss(self, y_true, y_pred):
         return 0.0
 
     def _clipped_mse_loss(self, Qnext, Q):
         loss = tf.math.reduce_mean(tf.math.square(Qnext - Q), name="loss_mse")
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/slice_util.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/slice_util.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/SliceRDQN/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/SliceRDQN/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Template/__init__.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Template/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Template/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Template/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Template/template.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Template/template.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/Template/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/Template/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/TopoOracleAgent.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/TopoOracleAgent/TopoOracleAgent.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/evaluate.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/TopoOracleAgent/evaluate.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/TopoOracleAgent/train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/TopoOracleAgent/train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/__init__.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # See AUTHORS.txt
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of L2RPN Baselines, L2RPN Baselines a repository to host baselines for l2rpn competitions.
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 all_baselines_li = [
     "Template",
     "DoNothing",
     "ExpertAgent",
     "PPO_RLLIB",
     "PPO_SB3",
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/__init__.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/baseDeepQ.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/baseDeepQ.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/cli_eval.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/cli_eval.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/cli_train.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/cli_train.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/deepQAgent.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/deepQAgent.py`

 * *Files 1% similar despite different names*

```diff
@@ -677,15 +677,18 @@
             s_batch, a_batch, r_batch, d_batch, s2_batch = self.replay_buffer.sample(self._training_param.minibatch_size)
             tf_writer = None
             if self.__graph_saved is False:
                 tf_writer = self._tf_writer
             loss = self.deep_q.train(s_batch, a_batch, r_batch, d_batch, s2_batch,
                                      tf_writer)
             # save learning rate for later
-            self._train_lr = self.deep_q._optimizer_model._decayed_lr('float32').numpy()
+            if hasattr(self.deep_q._optimizer_model, "_decayed_lr"):
+                self.train_lr = self.deep_q._optimizer_model._decayed_lr('float32').numpy()
+            else:
+                self.train_lr = self.deep_q._optimizer_model.learning_rate.numpy()
             self.__graph_saved = True
             if not np.all(np.isfinite(loss)):
                 # if the loss is not finite i stop the learning
                 return False
             self.deep_q.target_train()
             self._losses[training_step:] = np.sum(loss)
         return True
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/gymAgent.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/gymAgent.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,16 @@
     def clean_heuristic_actions(self, observation: BaseObservation, reward: float, done: bool) -> None:
         """This function allows to cure the heuristic actions. 
         
         It is called at each step, just after the heuristic actions are computed (but before they are selected).
         
         It can be used, for example, to reorder the `self._action_list` for example.
 
+        It is not used during training.
+        
         Args:
             observation (BaseObservation): The current observation
             reward (float): the current reward
             done (bool): the current flag "done"
         """
         pass
     
@@ -195,10 +197,10 @@
         if grid2op_act is None:
             gym_obs = self._gym_obs_space.to_gym(observation)
             gym_act = self.get_act(gym_obs, reward, done)
             grid2op_act = self._gym_act_space.from_gym(gym_act)
             
             # fix the action if needed (for example by limiting curtailment and storage)
             if self._has_heuristic:
-                grid2op_act = self.gymenv.fix_action(grid2op_act)
+                grid2op_act = self.gymenv.fix_action(grid2op_act, observation)
             
         return grid2op_act
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/gymenv_custom.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/gymenv_custom.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     #. the observation (corresponding to the last step above) is then converted to a gym action (thanks to the observation_space)
        which is forwarded to the agent.
     
     The agent then only "sees" what is not processed by the heuristic. It is trained only on the relevant "state".
 
     """
     POSSIBLE_REWARD_CUMUL = ["init", "last", "sum", "max"]
-    def __init__(self, env_init, *args, reward_cumul="init", **kwargs):
+    def __init__(self, env_init, *args, reward_cumul="last", **kwargs):
         super().__init__(env_init, *args, **kwargs)
         self._reward_cumul = reward_cumul
         
         if not self._reward_cumul in type(self).POSSIBLE_REWARD_CUMUL:
             raise RuntimeError("Wrong argument for the reward_cumul parameters. "
                                f"You provided \"{self._reward_cumul}\" (possible "
                                f"values are {type(self).POSSIBLE_REWARD_CUMUL}).")
@@ -178,15 +178,15 @@
                     
                 if tmp_done:
                     break
             if done:
                 break
         return g2op_obs, res_reward, done, info
     
-    def fix_action(self, grid2op_action):
+    def fix_action(self, grid2op_action, g2op_obs):
         """This function can be used to "fix" / "modify" / "cut" / "change"
         a grid2op action just before it will be applied to the underlying "env.step(...)"
         
         This can be used, for example to "limit the curtailment or storage" of the
         action in case this one is too strong and would lead to a game over.
 
         By default it does nothing.
@@ -230,48 +230,59 @@
             Whether the episode is over or not
             
         info: Dict
             Other type of informations
             
         """
         g2op_act_tmp = self.action_space.from_gym(gym_action)
-        g2op_act = self.fix_action(g2op_act_tmp)
+        g2op_act = self.fix_action(g2op_act_tmp, self._previous_act)
         g2op_obs, reward, done, info = self.init_env.step(g2op_act)
         if not done:
             g2op_obs, reward, done, info = self.apply_heuristics_actions(g2op_obs, reward, done, info)
+        self._previous_act = g2op_obs
         gym_obs = self.observation_space.to_gym(g2op_obs)
-        return gym_obs, float(reward), done, info
+        if hasattr(type(self), "_gymnasium") and type(self)._gymnasium:
+            truncated = False
+            return gym_obs, float(reward), done, truncated, info
+        else:
+            return gym_obs, float(reward), done, info
         
-    def reset(self, seed=None, return_info=False, options=None):
+    def reset(self, *, seed=None, return_info=False, options=None):
         """This function implements the "reset" function. It is called at the end of every episode and
         marks the beginning of a new one.
         
         Again, before the agents sees any observations from the environment, they are processed by the 
         "heuristics" / "expert rules".
         
         .. note::
             The first observation seen by the agent is not necessarily the first observation of the grid2op environment.
 
         Returns
         -------
         gym_obs:
             The first open ai gym observation received by the agent
         """
+        if hasattr(type(self), "_gymnasium") and type(self)._gymnasium:
+            return_info = True
+            
         done = True
         info = {}  # no extra information provided !
         while done:
-            super().reset(seed, return_info, options)  # reset the scenario
+            super()._aux_reset(seed, return_info, options)  # reset the scenario
             g2op_obs = self.init_env.get_obs()  # retrieve the observation
             reward = self.init_env.reward_range[0]  # the reward at first step is always minimal
             
             # perform the "heuristics" steps
             g2op_obs, reward, done, info = self.apply_heuristics_actions(g2op_obs, reward, False, info)
             
             # convert back the observation to gym
-            gym_obs = self.observation_space.to_gym(g2op_obs)
+            if not done:
+                self._previous_act = g2op_obs
+                gym_obs = self.observation_space.to_gym(g2op_obs)
+                break
             
         if return_info:
             return gym_obs, info
         else:
             return gym_obs
     
 class GymEnvWithReco(GymEnvWithHeuristics):
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/make_multi_env.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/make_multi_env.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/nnParam.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/nnParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/replayBuffer.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/replayBuffer.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/save_log_gif.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/save_log_gif.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/str2bool.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/str2bool.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/train_generic.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/train_generic.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/trainingParam.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/trainingParam.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/waring_msgs.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/waring_msgs.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines/utils/zip_for_codalab.py` & `l2rpn_baselines-0.8.0/l2rpn_baselines/utils/zip_for_codalab.py`

 * *Files identical despite different names*

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/PKG-INFO` & `l2rpn_baselines-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,84 @@
 Metadata-Version: 2.1
-Name: l2rpn-baselines
-Version: 0.7.0
+Name: l2rpn_baselines
+Version: 0.8.0
 Summary: L2RPN Baselines a repository to host baselines for l2rpn competitions.
 Home-page: https://github.com/rte-france/L2RPN_Baselines
 Author: Benjamin DONNOT
 Author-email: benjamin.donnot@rte-france.com
 License: MPL
-Description: # L2RPN_Baselines
-        Repository hosting reference baselines for the [L2RPN challenge](https://l2rpn.chalearn.org/)
-        
-        # Install 
-        
-        ## Requirements
-        `python3 >= 3.6`
-        
-        ## Instal from PyPI
-        ```sh
-        pip3 install l2rpn_baselines
-        ```
-        ## Install from source
-        ```sh
-        git clone https://github.com/rte-france/l2rpn-baselines.git
-        cd l2rpn-baselines
-        pip3 install -U .
-        cd ..
-        rm -rf l2rpn-baselines
-        ```
-        
-        # Contribute
-        
-        We welcome contributions: see the [contribute guide](/CONTRIBUTE.md) for details.
-        
-        # Get started with a baseline
-        
-        Say you want to know how you compared with the "PPO_SB3" baseline implementation in this repository (for the
-        sake of this example).
-        
-        ## Train it (optional)
-        As no weights are provided for this baselines by default (yet), you will first need to train such a baseline:
-        
-        ```python
-        import grid2op
-        from l2rpn_baselines.PPO_SB3 import train
-        env = grid2op.make("l2rpn_case14_sandbox")
-        res = train(env, save_path="THE/PATH/TO/SAVE/IT", iterations=100)
-        ```
-        
-        You can have more information about extra argument of the "train" function in the 
-        [CONTRIBUTE](/CONTRIBUTE.md) file.
-        
-        ## Evaluate it
-        Once trained, you can reload it and evaluate its performance with the provided "evaluate" function:
-        
-        ```python
-        import grid2op
-        from l2rpn_baselines.PPO_SB3 import evaluate
-        env = grid2op.make("l2rpn_case14_sandbox")
-        res = evaluate(env, load_path="THE/PATH/TO/LOAD/IT", nb_episode=10)
-        ```
-        
-        You can have more information about extra argument of the "evaluate" function in the 
-        [CONTRIBUTE](/CONTRIBUTE.md) file.
-        
 Keywords: ML powergrid optmization RL power-systems
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
-Provides-Extra: CurriculumAgent
-Provides-Extra: PPO_RLLIB
-Provides-Extra: PPO_SB3
 Provides-Extra: docs
 Provides-Extra: optional
+Provides-Extra: PPO_RLLIB
+Provides-Extra: PPO_SB3
+Provides-Extra: CurriculumAgent
+License-File: LICENSE
+License-File: LICENSE.md
+License-File: AUTHORS.txt
+
+# L2RPN_Baselines
+Repository hosting reference baselines for the [L2RPN challenge](https://l2rpn.chalearn.org/)
+
+# Install 
+
+## Requirements
+`python3 >= 3.6`
+
+## Instal from PyPI
+```sh
+pip3 install l2rpn_baselines
+```
+## Install from source
+```sh
+git clone https://github.com/rte-france/l2rpn-baselines.git
+cd l2rpn-baselines
+pip3 install -U .
+cd ..
+rm -rf l2rpn-baselines
+```
+
+# Contribute
+
+We welcome contributions: see the [contribute guide](/CONTRIBUTE.md) for details.
+
+# Get started with a baseline
+
+Say you want to know how you compared with the "PPO_SB3" baseline implementation in this repository (for the
+sake of this example).
+
+## Train it (optional)
+As no weights are provided for this baselines by default (yet), you will first need to train such a baseline:
+
+```python
+import grid2op
+from l2rpn_baselines.PPO_SB3 import train
+env = grid2op.make("l2rpn_case14_sandbox")
+res = train(env, save_path="THE/PATH/TO/SAVE/IT", iterations=100)
+```
+
+You can have more information about extra argument of the "train" function in the 
+[CONTRIBUTE](/CONTRIBUTE.md) file.
+
+## Evaluate it
+Once trained, you can reload it and evaluate its performance with the provided "evaluate" function:
+
+```python
+import grid2op
+from l2rpn_baselines.PPO_SB3 import evaluate
+env = grid2op.make("l2rpn_case14_sandbox")
+res = evaluate(env, load_path="THE/PATH/TO/LOAD/IT", nb_episode=10)
+```
+
+You can have more information about extra argument of the "evaluate" function in the 
+[CONTRIBUTE](/CONTRIBUTE.md) file.
```

### Comparing `l2rpn_baselines-0.7.0/l2rpn_baselines.egg-info/SOURCES.txt` & `l2rpn_baselines-0.8.0/l2rpn_baselines.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+AUTHORS.txt
+LICENSE
+LICENSE.md
 MANIFEST.in
 README.md
 setup.py
 l2rpn_baselines/__init__.py
 l2rpn_baselines.egg-info/PKG-INFO
 l2rpn_baselines.egg-info/SOURCES.txt
 l2rpn_baselines.egg-info/dependency_links.txt
```

### Comparing `l2rpn_baselines-0.7.0/setup.py` & `l2rpn_baselines-0.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,44 +4,45 @@
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of L2RPN Baselines, L2RPN Baselines a repository to host baselines for l2rpn competitions.
 
 import setuptools
 from setuptools import setup
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 
 pkgs = {
     "required": [
         "grid2op",
         "statsmodels>=0.11.1",
         "scipy>=1.4.1",
         "numpy",
-        "gym>=0.17.2"
+        "gymnasium",
+        "lightsim2grid"
     ],
     "extras": {
         "docs": [
             "numpydoc>=0.9.2",
             "sphinx>=2.4.4",
             "sphinx-rtd-theme>=0.4.3",
             "sphinxcontrib-trio>=1.1.0",
             "autodocsumm>=0.2.7",
-            "cvxpy"
         ],
         "optional": ["grid2op[optional]>=1.6.5",
                      "tensorflow>=2.2.0",
                      "Keras>=2.3.1",
                      "torch>=1.4.0",
                      "scikit-learn>=0.22.2",
+                     "cvxpy"
                      ],
         "PPO_RLLIB": ["ray[rllib]",
                       "jsonpickle",
-                      "lightsim2grid"],
-        "PPO_SB3": ["stable_baselines3", "lightsim2grid"],
+                      "torch"],
+        "PPO_SB3": ["stable_baselines3"],
         "CurriculumAgent":["curriculumagent"]
     }
 }
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

