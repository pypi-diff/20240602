# Comparing `tmp/joyrl-0.6.1.1.tar.gz` & `tmp/joyrl-0.6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.6.1.1.tar", last modified: Sat Jun  1 16:36:22 2024, max compression
+gzip compressed data, was "joyrl-0.6.1.2.tar", last modified: Sun Jun  2 02:52:13 2024, max compression
```

## Comparing `joyrl-0.6.1.1.tar` & `joyrl-0.6.1.2.tar`

### file list

```diff
@@ -1,109 +1,105 @@
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.419801 joyrl-0.6.1.1/
--rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/LICENSE
--rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-01 16:36:22.419715 joyrl-0.6.1.1/PKG-INFO
--rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.1.1/README.md
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.408865 joyrl-0.6.1.1/joyrl/
--rw-r--r--   0 johnjim    (501) staff       (20)      377 2024-06-01 16:36:10.000000 joyrl-0.6.1.1/joyrl/__init__.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.409710 joyrl-0.6.1.1/joyrl/algos/
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.410226 joyrl-0.6.1.1/joyrl/algos/DDPG/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DDPG/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DDPG/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DDPG/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DDPG/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.410707 joyrl-0.6.1.1/joyrl/algos/DQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3519 2024-06-01 16:19:56.000000 joyrl-0.6.1.1/joyrl/algos/DQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.411145 joyrl-0.6.1.1/joyrl/algos/DoubleDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DoubleDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DoubleDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DoubleDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3696 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DoubleDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.411573 joyrl-0.6.1.1/joyrl/algos/DuelingDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DuelingDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1773 2024-06-01 16:33:50.000000 joyrl-0.6.1.1/joyrl/algos/DuelingDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DuelingDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3518 2024-06-01 16:30:55.000000 joyrl-0.6.1.1/joyrl/algos/DuelingDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.412039 joyrl-0.6.1.1/joyrl/algos/NoisyDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/NoisyDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1071 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/NoisyDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/NoisyDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4445 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/NoisyDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.412493 joyrl-0.6.1.1/joyrl/algos/PPO/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/PPO/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-06-01 16:35:55.000000 joyrl-0.6.1.1/joyrl/algos/PPO/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2979 2024-06-01 09:19:48.000000 joyrl-0.6.1.1/joyrl/algos/PPO/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     6921 2024-06-01 10:23:56.000000 joyrl-0.6.1.1/joyrl/algos/PPO/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.412984 joyrl-0.6.1.1/joyrl/algos/QLearning/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/QLearning/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/QLearning/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1.1/joyrl/algos/QLearning/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/QLearning/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.413486 joyrl-0.6.1.1/joyrl/algos/Sarsa/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/Sarsa/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/Sarsa/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1.1/joyrl/algos/Sarsa/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/Sarsa/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.413977 joyrl-0.6.1.1/joyrl/algos/TD3/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/TD3/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/TD3/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/TD3/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/TD3/policy.py
--rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/__init__.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.415367 joyrl-0.6.1.1/joyrl/algos/base/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/base/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)    10114 2024-06-01 16:17:16.000000 joyrl-0.6.1.1/joyrl/algos/base/action_layer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/base/base_layer.py
--rw-r--r--   0 johnjim    (501) staff       (20)    86089 2024-06-01 05:31:25.000000 joyrl-0.6.1.1/joyrl/algos/base/buffer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2755 2024-06-01 05:12:03.000000 joyrl-0.6.1.1/joyrl/algos/base/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/base/experience.py
--rw-r--r--   0 johnjim    (501) staff       (20)    13933 2024-06-01 16:11:14.000000 joyrl-0.6.1.1/joyrl/algos/base/network.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/base/noise.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/base/optm.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7635 2024-06-01 16:21:28.000000 joyrl-0.6.1.1/joyrl/algos/base/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.416553 joyrl-0.6.1.1/joyrl/envs/
--rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/blackjack.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/cliff_walking.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/gridworld.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/gridworld_env.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.416939 joyrl-0.6.1.1/joyrl/envs/gym/
--rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/gym/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/gym/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.1.1/joyrl/envs/gym/wrappers.py
--rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/racetrack.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/register.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/stochastic_mdp.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/windy_gridworld.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.418484 joyrl-0.6.1.1/joyrl/framework/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/framework/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1069 2024-05-30 09:43:52.000000 joyrl-0.6.1.1/joyrl/framework/base.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4442 2024-06-01 08:53:39.000000 joyrl-0.6.1.1/joyrl/framework/collector.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2294 2024-06-01 06:35:14.000000 joyrl-0.6.1.1/joyrl/framework/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5619 2024-06-01 08:53:09.000000 joyrl-0.6.1.1/joyrl/framework/interactor.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2874 2024-06-01 08:53:20.000000 joyrl-0.6.1.1/joyrl/framework/learner.py
--rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.1.1/joyrl/framework/message.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2923 2024-06-01 03:33:53.000000 joyrl-0.6.1.1/joyrl/framework/policy_mgr.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5272 2024-05-30 09:48:58.000000 joyrl-0.6.1.1/joyrl/framework/recorder.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3961 2024-05-31 03:30:30.000000 joyrl-0.6.1.1/joyrl/framework/tester.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/framework/tracker.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7020 2024-06-01 08:53:33.000000 joyrl-0.6.1.1/joyrl/framework/trainer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2524 2024-05-31 14:51:57.000000 joyrl-0.6.1.1/joyrl/framework/utils.py
--rw-r--r--   0 johnjim    (501) staff       (20)     8002 2024-06-01 09:17:47.000000 joyrl-0.6.1.1/joyrl/run.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.418717 joyrl-0.6.1.1/joyrl/scripts/
--rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/scripts/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/scripts/scripts.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.419019 joyrl-0.6.1.1/joyrl/utils/
--rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/utils/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/utils/plot.py
--rw-r--r--   0 johnjim    (501) staff       (20)    37181 2024-05-30 09:48:17.000000 joyrl-0.6.1.1/joyrl/utils/utils.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.419204 joyrl-0.6.1.1/joyrl.egg-info/
--rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/PKG-INFO
--rw-r--r--   0 johnjim    (501) staff       (20)     2455 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/SOURCES.txt
--rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/dependency_links.txt
--rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/entry_points.txt
--rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/requires.txt
--rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/top_level.txt
--rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-01 16:36:22.420134 joyrl-0.6.1.1/setup.cfg
--rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.1.1/setup.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.209836 joyrl-0.6.1.2/
+-rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/LICENSE
+-rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-02 02:52:13.209751 joyrl-0.6.1.2/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.1.2/README.md
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.194928 joyrl-0.6.1.2/joyrl/
+-rw-r--r--   0 johnjim    (501) staff       (20)      357 2024-06-02 02:52:04.000000 joyrl-0.6.1.2/joyrl/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.195824 joyrl-0.6.1.2/joyrl/algos/
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.196608 joyrl-0.6.1.2/joyrl/algos/DDPG/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DDPG/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DDPG/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DDPG/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DDPG/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.197253 joyrl-0.6.1.2/joyrl/algos/DQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-06-02 02:51:34.000000 joyrl-0.6.1.2/joyrl/algos/DQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3627 2024-06-02 02:14:32.000000 joyrl-0.6.1.2/joyrl/algos/DQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.197988 joyrl-0.6.1.2/joyrl/algos/DoubleDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DoubleDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DoubleDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DoubleDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3512 2024-06-02 02:34:38.000000 joyrl-0.6.1.2/joyrl/algos/DoubleDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.198729 joyrl-0.6.1.2/joyrl/algos/DuelingDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DuelingDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1773 2024-06-01 16:33:50.000000 joyrl-0.6.1.2/joyrl/algos/DuelingDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/DuelingDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3626 2024-06-02 02:19:04.000000 joyrl-0.6.1.2/joyrl/algos/DuelingDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.199408 joyrl-0.6.1.2/joyrl/algos/NoisyDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/NoisyDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1071 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/NoisyDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/NoisyDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4445 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/NoisyDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.200123 joyrl-0.6.1.2/joyrl/algos/PPO/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/PPO/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-06-01 16:35:55.000000 joyrl-0.6.1.2/joyrl/algos/PPO/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2979 2024-06-01 09:19:48.000000 joyrl-0.6.1.2/joyrl/algos/PPO/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     6921 2024-06-01 10:23:56.000000 joyrl-0.6.1.2/joyrl/algos/PPO/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.200866 joyrl-0.6.1.2/joyrl/algos/QLearning/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/QLearning/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/QLearning/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1.2/joyrl/algos/QLearning/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/QLearning/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.201438 joyrl-0.6.1.2/joyrl/algos/Sarsa/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/Sarsa/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/Sarsa/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1.2/joyrl/algos/Sarsa/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/Sarsa/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.201941 joyrl-0.6.1.2/joyrl/algos/TD3/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/TD3/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/TD3/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/TD3/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/TD3/policy.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.204080 joyrl-0.6.1.2/joyrl/algos/base/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/base/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    10114 2024-06-01 16:17:16.000000 joyrl-0.6.1.2/joyrl/algos/base/action_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/base/base_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    86101 2024-06-02 02:50:43.000000 joyrl-0.6.1.2/joyrl/algos/base/buffer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2711 2024-06-02 02:50:56.000000 joyrl-0.6.1.2/joyrl/algos/base/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/base/experience.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    13934 2024-06-02 02:51:15.000000 joyrl-0.6.1.2/joyrl/algos/base/network.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/base/noise.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/algos/base/optm.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7793 2024-06-02 02:32:38.000000 joyrl-0.6.1.2/joyrl/algos/base/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.205947 joyrl-0.6.1.2/joyrl/envs/
+-rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/blackjack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/cliff_walking.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/gridworld.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/gridworld_env.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.206458 joyrl-0.6.1.2/joyrl/envs/gym/
+-rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/gym/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/gym/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.1.2/joyrl/envs/gym/wrappers.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/racetrack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/register.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/stochastic_mdp.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/envs/windy_gridworld.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.208520 joyrl-0.6.1.2/joyrl/framework/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/framework/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1073 2024-06-02 02:50:42.000000 joyrl-0.6.1.2/joyrl/framework/base.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4446 2024-06-02 02:50:41.000000 joyrl-0.6.1.2/joyrl/framework/collector.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2295 2024-06-02 02:03:30.000000 joyrl-0.6.1.2/joyrl/framework/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5623 2024-06-02 02:50:40.000000 joyrl-0.6.1.2/joyrl/framework/interactor.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2878 2024-06-02 02:50:39.000000 joyrl-0.6.1.2/joyrl/framework/learner.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.1.2/joyrl/framework/message.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2927 2024-06-02 02:50:38.000000 joyrl-0.6.1.2/joyrl/framework/policy_mgr.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5276 2024-06-02 02:50:37.000000 joyrl-0.6.1.2/joyrl/framework/recorder.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3965 2024-06-02 02:50:36.000000 joyrl-0.6.1.2/joyrl/framework/tester.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/framework/tracker.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7028 2024-06-02 02:50:35.000000 joyrl-0.6.1.2/joyrl/framework/trainer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    39479 2024-06-02 02:50:21.000000 joyrl-0.6.1.2/joyrl/framework/utils.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8007 2024-06-02 02:48:05.000000 joyrl-0.6.1.2/joyrl/run.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.208912 joyrl-0.6.1.2/joyrl/scripts/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/scripts/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.1.2/joyrl/scripts/scripts.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:52:13.209222 joyrl-0.6.1.2/joyrl.egg-info/
+-rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-02 02:52:13.000000 joyrl-0.6.1.2/joyrl.egg-info/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)     2390 2024-06-02 02:52:13.000000 joyrl-0.6.1.2/joyrl.egg-info/SOURCES.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-02 02:52:13.000000 joyrl-0.6.1.2/joyrl.egg-info/dependency_links.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-02 02:52:13.000000 joyrl-0.6.1.2/joyrl.egg-info/entry_points.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-02 02:52:13.000000 joyrl-0.6.1.2/joyrl.egg-info/requires.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-02 02:52:13.000000 joyrl-0.6.1.2/joyrl.egg-info/top_level.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-02 02:52:13.210129 joyrl-0.6.1.2/setup.cfg
+-rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.1.2/setup.py
```

### Comparing `joyrl-0.6.1.1/LICENSE` & `joyrl-0.6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/PKG-INFO` & `joyrl-0.6.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.6.1.1
+Version: 0.6.1.2
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.6.1.1/README.md` & `joyrl-0.6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/DDPG/config.py` & `joyrl-0.6.1.2/joyrl/algos/DDPG/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/DDPG/policy.py` & `joyrl-0.6.1.2/joyrl/algos/DDPG/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/DQN/config.py` & `joyrl-0.6.1.2/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/DQN/policy.py` & `joyrl-0.6.1.2/joyrl/algos/DQN/policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2024-01-25 09:58:33
 LastEditor: JiangJi
-LastEditTime: 2024-06-02 00:19:46
+LastEditTime: 2024-06-02 10:14:18
 Discription: 
 '''
 import torch
 import torch.nn as nn
 import math,random
 import numpy as np
 from joyrl.algos.base.policy import BasePolicy
@@ -57,27 +57,30 @@
         return actions
     
     def learn(self, **kwargs):
         ''' learn policy
         '''
         states, actions, next_states, rewards, dones = kwargs.get('states'), kwargs.get('actions'), kwargs.get('next_states'), kwargs.get('rewards'), kwargs.get('dones')
         # compute current Q values
-        self.loss = 0
+        self.summary_loss = []
+        tot_loss = 0
         actor_outputs = self.model(states)['actor_outputs']
         target_actor_outputs = self.target_model(next_states)['actor_outputs']
         for i in range(len(self.action_size_list)):
             actual_q_value = actor_outputs[i]['q_value'].gather(1, actions[i].long())
             # compute next max q value
             next_q_value_max = target_actor_outputs[i]['q_value'].max(1)[0].unsqueeze(dim=1)
             # compute target Q values
             target_q_value = rewards + (1 - dones) * self.gamma * next_q_value_max
             # compute loss
-            self.loss += nn.MSELoss()(actual_q_value, target_q_value)
+            loss_i = nn.MSELoss()(actual_q_value, target_q_value)
+            tot_loss += loss_i
+            self.summary_loss.append(loss_i.item())
         self.optimizer.zero_grad()
-        self.loss.backward()
+        tot_loss.backward()
         # clip to avoid gradient explosion
         for param in self.model.parameters():
             param.grad.data.clamp_(-1, 1)
         self.optimizer.step()
         # update target net every C steps
         if self.update_step % self.target_update == 0: 
             self.target_model.load_state_dict(self.model.state_dict())
```

### Comparing `joyrl-0.6.1.1/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.6.1.2/joyrl/algos/DoubleDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/DoubleDQN/policy.py` & `joyrl-0.6.1.2/joyrl/algos/NoisyDQN/policy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,106 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
-Date: 2023-12-22 23:02:13
+Date: 2023-04-17 11:23:49
 LastEditor: JiangJi
-LastEditTime: 2024-01-27 12:00:29
+LastEditTime: 2023-12-25 00:18:41
 Discription: 
 '''
 import torch
 import torch.nn as nn
-import math, random
+import torch.optim as optim
+import torch.nn.functional as F
 import numpy as np
+import math
+import random
+
 from joyrl.algos.base.policy import BasePolicy
 from joyrl.algos.base.network import QNetwork
+
 class Policy(BasePolicy):
     def __init__(self,cfg) -> None:
         super(Policy, self).__init__(cfg)
         self.cfg = cfg
-        self.obs_space = cfg.obs_space
-        self.action_space = cfg.action_space
+        self.device = torch.device(cfg.device) 
         self.gamma = cfg.gamma  
         # e-greedy parameters
         self.epsilon_start = cfg.epsilon_start
         self.epsilon_end = cfg.epsilon_end
         self.epsilon_decay = cfg.epsilon_decay
+        self.batch_size = cfg.batch_size
         self.target_update = cfg.target_update
         self.sample_count = 0
         self.update_step = 0
         self.create_graph() # create graph and optimizer
         self.create_summary() # create summary
 
     def create_graph(self):
-        self.policy_net = QNetwork(self.cfg,self.state_size_list).to(self.device)
-        self.target_net = QNetwork(self.cfg,self.state_size_list).to(self.device)
+        self.state_size_list, self.action_size_list = self.get_state_action_size()
+        self.policy_net = QNetwork(self.cfg, self.state_size_list, self.action_size_list).to(self.device)
+        self.target_net = QNetwork(self.cfg, self.state_size_list, self.action_size_list).to(self.device)
         self.target_net.load_state_dict(self.policy_net.state_dict()) # or use this to copy parameters
+        # for noise parameters
+        # if self.cfg.mode == 'train': 
+        #     self.policy_net.train()
+        #     self.target_net.train()
+        # elif self.cfg.mode == 'test':
+        #     self.policy_net.eval()
+        #     self.target_net.eval()
         self.create_optimizer()
 
-    def sample_action(self, state, **kwargs):
+    def sample_action(self, state,  **kwargs):
         ''' sample action
         '''
         # epsilon must decay(linear,exponential and etc.) for balancing exploration and exploitation
         self.sample_count += 1
         self.epsilon = self.epsilon_end + (self.epsilon_start - self.epsilon_end) * \
             math.exp(-1. * self.sample_count / self.epsilon_decay) 
         if random.random() > self.epsilon:
             action = self.predict_action(state)
         else:
-            action = [self.action_space.sample()]
+            action = self.action_space.sample()
         return action
-    
-    @torch.no_grad()
-    def predict_action(self,state,**kwargs):
+    def predict_action(self,state, **kwargs):
         ''' predict action
         '''
-        state = [torch.tensor(np.array(state), device=self.device, dtype=torch.float32).unsqueeze(dim=0)]
-        _ = self.policy_net(state)
-        actions = self.policy_net.action_layers.get_actions()
-        return actions
+        with torch.no_grad():
+            state = torch.tensor(np.array(state), device=self.device, dtype=torch.float32).unsqueeze(dim=0)
+            q_values = self.policy_net(state)
+            action = q_values.max(1)[1].item() # choose action corresponding to the maximum q value
+        return action  
 
     def learn(self, **kwargs):
         ''' train policy
         '''
         states, actions, next_states, rewards, dones = kwargs.get('states'), kwargs.get('actions'), kwargs.get('next_states'), kwargs.get('rewards'), kwargs.get('dones')
-        _ = self.policy_net(states)
-        q_values = self.policy_net.action_layers.get_qvalues()
-        actual_qvalues = q_values.gather(1, actions.long())
-
-        # compute next Q values Q(s_t+1, a)
-        _ = self.policy_net(next_states)
-        next_q_values = self.policy_net.action_layers.get_qvalues()
-
-        # compute next target Q values Q'(s_t+1, a)，which is different from DQN
-        _ = self.target_net(next_states)
-        next_target_qvalues = self.target_net.action_layers.get_qvalues()
-
-        next_target_q_values_action = next_target_qvalues.gather(1, torch.max(next_q_values, 1)[1].unsqueeze(1))
-
-        expected_q_values = rewards + self.gamma * next_target_q_values_action * (1 - dones)  
-        self.loss = nn.MSELoss()(actual_qvalues, expected_q_values)  
-        self.optimizer.zero_grad()  
-        self.loss.backward()  
+        update_step = kwargs.get('update_step')
+        # convert numpy to tensor
+        states = torch.tensor(states, device=self.device, dtype=torch.float32)
+        actions = torch.tensor(actions, device=self.device, dtype=torch.int64).unsqueeze(dim=1)
+        next_states = torch.tensor(next_states, device=self.device, dtype=torch.float32)
+        rewards = torch.tensor(rewards, device=self.device, dtype=torch.float32).unsqueeze(dim=1)
+        dones = torch.tensor(dones, device=self.device, dtype=torch.float32).unsqueeze(dim=1)
+        # compute current Q values
+        q_values = self.policy_net(states).gather(1, actions)
+        # compute next max q value
+        next_q_values = self.target_net(next_states).max(1)[0].unsqueeze(dim=1)
+        # compute target Q values
+        target_q_values = rewards + (1 - dones) * self.gamma * next_q_values
+        # compute loss
+        self.loss = nn.MSELoss()(q_values, target_q_values)
+        self.optimizer.zero_grad()
+        self.loss.backward()
         # clip to avoid gradient explosion
         for param in self.policy_net.parameters():
             param.grad.data.clamp_(-1, 1)
         self.optimizer.step()
         # update target net every C steps
         if self.update_step % self.target_update == 0: 
             self.target_net.load_state_dict(self.policy_net.state_dict())
         self.update_step += 1
-        self.update_summary() # update summary
+        self.policy_net.reset_noise()
+        self.target_net.reset_noise()
+        self.update_summary() # update summary
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `joyrl-0.6.1.1/joyrl/algos/DuelingDQN/config.py` & `joyrl-0.6.1.2/joyrl/algos/DuelingDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/DuelingDQN/policy.py` & `joyrl-0.6.1.2/joyrl/algos/DuelingDQN/policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2022-11-14 23:50:59
 LastEditor: JiangJi
-LastEditTime: 2024-06-02 00:30:01
+LastEditTime: 2024-06-02 10:19:04
 Discription: 
 '''
 import torch
 import torch.nn as nn
 import math,random
 import numpy as np
 from joyrl.algos.base.policy import BasePolicy
@@ -57,27 +57,30 @@
         return actions 
     
     def learn(self, **kwargs):
         ''' learn policy
         '''
         states, actions, next_states, rewards, dones = kwargs.get('states'), kwargs.get('actions'), kwargs.get('next_states'), kwargs.get('rewards'), kwargs.get('dones')
         # compute current Q values
-        self.loss = 0
+        self.summary_loss = []
+        tot_loss = 0
         actor_outputs = self.model(states)['actor_outputs']
         target_actor_outputs = self.target_model(next_states)['actor_outputs']
         for i in range(len(self.action_size_list)):
             actual_q_value = actor_outputs[i]['q_value'].gather(1, actions[i].long())
             # compute next max q value
             next_q_value_max = target_actor_outputs[i]['q_value'].max(1)[0].unsqueeze(dim=1)
             # compute target Q values
             target_q_value = rewards + (1 - dones) * self.gamma * next_q_value_max
             # compute loss
-            self.loss += nn.MSELoss()(actual_q_value, target_q_value)
+            loss_i = nn.MSELoss()(actual_q_value, target_q_value)
+            tot_loss += loss_i
+            self.summary_loss.append(loss_i.item())
         self.optimizer.zero_grad()
-        self.loss.backward()
+        tot_loss.backward()
         # clip to avoid gradient explosion
         for param in self.model.parameters():
             param.grad.data.clamp_(-1, 1)
         self.optimizer.step()
         # update target net every C steps
         if self.update_step % self.target_update == 0: 
             self.target_model.load_state_dict(self.model.state_dict())
```

### Comparing `joyrl-0.6.1.1/joyrl/algos/NoisyDQN/config.py` & `joyrl-0.6.1.2/joyrl/algos/NoisyDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/PPO/config.py` & `joyrl-0.6.1.2/joyrl/algos/PPO/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/PPO/data_handler.py` & `joyrl-0.6.1.2/joyrl/algos/PPO/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/PPO/policy.py` & `joyrl-0.6.1.2/joyrl/algos/PPO/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/QLearning/data_handler.py` & `joyrl-0.6.1.2/joyrl/algos/QLearning/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/QLearning/policy.py` & `joyrl-0.6.1.2/joyrl/algos/QLearning/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/Sarsa/data_handler.py` & `joyrl-0.6.1.2/joyrl/algos/Sarsa/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/Sarsa/policy.py` & `joyrl-0.6.1.2/joyrl/algos/Sarsa/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/TD3/config.py` & `joyrl-0.6.1.2/joyrl/algos/TD3/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/TD3/policy.py` & `joyrl-0.6.1.2/joyrl/algos/TD3/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/base/action_layer.py` & `joyrl-0.6.1.2/joyrl/algos/base/action_layer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/base/base_layer.py` & `joyrl-0.6.1.2/joyrl/algos/base/base_layer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/base/buffer.py` & `joyrl-0.6.1.2/joyrl/algos/base/buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import torch
 import numpy as np
 from enum import Enum
 from collections import deque
 from joyrl.framework.config import MergedConfig
-from joyrl.utils.utils import get_shape_from_obs_space, get_shape_from_act_space
+from joyrl.framework.utils import get_shape_from_obs_space, get_shape_from_act_space
 
 def _cast(x):
     return x.transpose(1, 2, 0, 3).reshape(-1, *x.shape[3:])
 
 class BufferType(Enum):
     ''' buffer type enum
     '''
@@ -274,15 +274,15 @@
         for idx, priority in zip(indices, priorities):
             self.priorities[idx] = priority
     def __len__(self):
         return self.count
 
 
 # MAPPO beginning
-from joyrl.utils.utils import check, get_shape_from_obs_space, get_shape_from_act_space
+from joyrl.framework.utils import check, get_shape_from_obs_space, get_shape_from_act_space
 
 def _flatten(T, N, x):
     return x.reshape(T * N, *x.shape[2:])
 
 def _cast(x):
     return x.transpose(1,0,2).reshape(-1, *x.shape[2:])
 
@@ -665,15 +665,15 @@
             active_masks_batch = _flatten(L, N, active_masks_batch)
             old_action_log_probs_batch = _flatten(L, N, old_action_log_probs_batch)
             adv_targ = _flatten(L, N, adv_targ)
 
             yield share_obs_batch, obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, available_actions_batch
 
 
-from joyrl.utils.utils import get_shape_from_obs_space, get_shape_from_act_space
+from joyrl.framework.utils import get_shape_from_obs_space, get_shape_from_act_space
 
 def _cast(x):
     return x.transpose(1, 2, 0, 3).reshape(-1, *x.shape[3:])
 
 class SharedReplayBuffer(object):
     """
     Buffer to store training data.
```

### Comparing `joyrl-0.6.1.1/joyrl/algos/base/data_handler.py` & `joyrl-0.6.1.2/joyrl/algos/base/data_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-02 15:02:30
 LastEditor: JiangJi
-LastEditTime: 2024-06-01 13:11:59
+LastEditTime: 2024-06-02 10:50:56
 Discription: 
 '''
 import torch
 import numpy as np
 from joyrl.algos.base.buffer import BufferCreator
-from joyrl.algos.base.experience import Exp
 
 class BaseDataHandler:
     ''' Basic data handler
     '''
     def __init__(self,cfg) -> None:
         self.cfg = cfg
         self.buffer = BufferCreator(cfg)()
```

### Comparing `joyrl-0.6.1.1/joyrl/algos/base/network.py` & `joyrl-0.6.1.2/joyrl/algos/base/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-22 23:02:13
 LastEditor: JiangJi
-LastEditTime: 2024-06-02 00:11:14
+LastEditTime: 2024-06-02 10:51:15
 Discription: 
 '''
 import copy
 import torch
 import torch.nn as nn
 from joyrl.algos.base.base_layer import create_layer, LayerConfig
 from joyrl.algos.base.action_layer import ActionLayerType, DiscreteActionLayer, ContinuousActionLayer, DPGActionLayer, DQNActionLayer
 from joyrl.framework.config import MergedConfig
+
 class BranchLayers(nn.Module):
     def __init__(self, branch_layers_cfg : list, input_size_list, **kwargs) -> None:
         super(BranchLayers, self).__init__(**kwargs)
         self.input_size_list = input_size_list
         self.branch_layers = nn.ModuleList([nn.ModuleList() for _ in range(len(self.input_size_list))])
         self.output_size_list = copy.deepcopy(input_size_list)
         self.branch_layers_cfg = branch_layers_cfg
```

### Comparing `joyrl-0.6.1.1/joyrl/algos/base/noise.py` & `joyrl-0.6.1.2/joyrl/algos/base/noise.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/base/optm.py` & `joyrl-0.6.1.2/joyrl/algos/base/optm.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/algos/base/policy.py` & `joyrl-0.6.1.2/joyrl/algos/base/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,39 +108,47 @@
         
     def get_policy_transition(self):
         return self.policy_transition
     
     def create_summary(self):
         ''' create policy summary
         '''
-        self.summary = {
-            'scalar': {
-                'loss': 0.0,
-            },
-        }
+        self.summary = {}
+        self.summary['scalar'] = {}
+        for i in range(len(self.action_size_list)):
+            self.summary['scalar'][f'loss_{i}'] = 0.0
+
     def update_summary(self):
         ''' update policy summary
         '''
-        self.summary['scalar']['loss'] = self.loss.item()
+        for i in range(len(self.action_size_list)):
+            self.summary['scalar'][f'loss_{i}'] = self.summary_loss[i]
+
     def get_summary(self):
         return self.summary['scalar']
+    
     def learn(self, **kwargs):
         ''' learn policy
         '''
         raise NotImplementedError
+    
     def update_data_after_learn(self):
         ''' update data after training
         '''
         self.data_after_train = {}
+        
     def get_data_after_learn(self):
+
         return self.data_after_train
+    
     def save_model(self, fpath):
         ''' save model
         '''
         torch.save(self.model.state_dict(), fpath)
+
     def load_model(self, fpath):
         ''' load model
         '''
         try:
             self.model.load_state_dict(torch.load(fpath, map_location=self.device))
         except:
             print(f"[BasePolicy.load_model] load model from {fpath} failed, please check the model path!")
```

### Comparing `joyrl-0.6.1.1/joyrl/envs/blackjack.py` & `joyrl-0.6.1.2/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/envs/cliff_walking.py` & `joyrl-0.6.1.2/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/envs/gridworld.py` & `joyrl-0.6.1.2/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/envs/gridworld_env.py` & `joyrl-0.6.1.2/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/envs/gym/config.py` & `joyrl-0.6.1.2/joyrl/envs/gym/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/envs/gym/wrappers.py` & `joyrl-0.6.1.2/joyrl/envs/gym/wrappers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/envs/racetrack.py` & `joyrl-0.6.1.2/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/envs/register.py` & `joyrl-0.6.1.2/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/envs/stochastic_mdp.py` & `joyrl-0.6.1.2/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/envs/windy_gridworld.py` & `joyrl-0.6.1.2/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/framework/base.py` & `joyrl-0.6.1.2/joyrl/framework/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-02 17:30:36
 LastEditor: JiangJi
-LastEditTime: 2024-05-30 17:43:52
+LastEditTime: 2024-06-02 10:50:42
 Discription: 
 '''
 import ray
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.message import Msg
-from joyrl.utils.utils import Logger, create_module
+from joyrl.framework.utils import Logger, create_module
 
 
 class Moduler(object):
     def __init__(self, cfg: MergedConfig, **kwargs) -> None:
         self.cfg = cfg
         self.name = kwargs.get('name', 'Moduler')
         self.logger = Logger(self.cfg.log_dir, log_name = self.name)
```

### Comparing `joyrl-0.6.1.1/joyrl/framework/collector.py` & `joyrl-0.6.1.2/joyrl/framework/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-22 23:02:13
 LastEditor: JiangJi
-LastEditTime: 2024-06-01 16:52:10
+LastEditTime: 2024-06-02 10:50:41
 Discription: 
 '''
 import ray
 import time
 import multiprocessing as mp
 from queue import Queue, Empty, Full
 import threading
 from joyrl.framework.message import Msg, MsgType
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.base import Moduler
-from joyrl.utils.utils import exec_method
+from joyrl.framework.utils import exec_method
 from joyrl.framework.utils import DeQueue
 
 class Collector(Moduler):
     ''' Collector for collecting training data
     '''
     def __init__(self, cfg: MergedConfig, **kwargs) -> None:
         super().__init__(cfg, **kwargs)
```

### Comparing `joyrl-0.6.1.1/joyrl/framework/config.py` & `joyrl-0.6.1.2/joyrl/framework/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-02 15:30:09
 LastEditor: JiangJi
-LastEditTime: 2024-06-01 14:35:10
+LastEditTime: 2024-06-02 10:03:30
 Discription: 
 '''
 class DefaultConfig:
     ''' Default parameters for running
     '''
     def __init__(self) -> None:
         pass
@@ -51,9 +51,9 @@
         self.online_eval_episode = 10 # online eval episodes
         self.model_save_fre = 500 # model save frequency per update step
         # load model settings
         self.load_checkpoint = False # if load checkpoint
         self.load_path = "Train_single_CartPole-v1_DQN_20230515-211721" # path to load model
         self.load_model_step = 'best' # load model at which step
         # stats recorder settings
-        self.interact_summary_fre = 1 # record interact stats per episode
+        self.interact_summary_fre = 10 # record interact stats per episode
         self.policy_summary_fre = 100 # record update stats per update step
```

### Comparing `joyrl-0.6.1.1/joyrl/framework/interactor.py` & `joyrl-0.6.1.2/joyrl/framework/interactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2024-02-25 15:46:04
 LastEditor: JiangJi
-LastEditTime: 2024-06-01 16:53:05
+LastEditTime: 2024-06-02 10:50:40
 Discription: 
 '''
 import gymnasium as gym
 import ray
 import time
 import copy
 from joyrl.algos.base.experience import Exp
 from joyrl.framework.message import Msg, MsgType
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.base import Moduler
 from joyrl.framework.recorder import Recorder
-from joyrl.utils.utils import exec_method, create_module
+from joyrl.framework.utils import exec_method, create_module
 
 class Interactor(Moduler):
     def __init__(self, cfg: MergedConfig, **kwargs) -> None:
         super().__init__(cfg, **kwargs)
         self.id = kwargs.get('id', 0)
         self.env = kwargs.get('env', None)
         self.policy = copy.deepcopy(kwargs['policy'])
```

### Comparing `joyrl-0.6.1.1/joyrl/framework/learner.py` & `joyrl-0.6.1.2/joyrl/framework/learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-02 15:02:30
 LastEditor: JiangJi
-LastEditTime: 2024-06-01 16:53:20
+LastEditTime: 2024-06-02 10:50:39
 Discription: 
 '''
 import ray
 import copy
 import time
 from typing import Tuple
 import numpy as np
 from joyrl.framework.message import Msg, MsgType
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.base import Moduler
 from joyrl.framework.recorder import Recorder
-from joyrl.utils.utils import exec_method, create_module
+from joyrl.framework.utils import exec_method, create_module
 
 class Learner(Moduler):
     ''' learner
     '''
     def __init__(self, cfg : MergedConfig, **kwargs) -> None:
         super().__init__(cfg, **kwargs)
         self.id = kwargs.get('id', 0)
```

### Comparing `joyrl-0.6.1.1/joyrl/framework/message.py` & `joyrl-0.6.1.2/joyrl/framework/message.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/framework/policy_mgr.py` & `joyrl-0.6.1.2/joyrl/framework/policy_mgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-22 23:02:13
 LastEditor: JiangJi
-LastEditTime: 2024-06-01 11:33:53
+LastEditTime: 2024-06-02 10:50:38
 Discription: 
 '''
 import time
 import copy
 import threading
 import torch
 from typing import Dict, List
 from queue import Queue
 from ray.util.queue import Queue as RayQueue
 from joyrl.framework.message import Msg, MsgType
 from joyrl.algos.base.policy import BasePolicy
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.base import Moduler
-from joyrl.utils.utils import exec_method
+from joyrl.framework.utils import exec_method
 
 class PolicyMgr(Moduler):
     ''' model manager
     '''
     def __init__(self, cfg: MergedConfig, *args, **kwargs) -> None:
         super().__init__(cfg, *args, **kwargs)
         self.policy = copy.deepcopy(kwargs['policy'])
```

### Comparing `joyrl-0.6.1.1/joyrl/framework/recorder.py` & `joyrl-0.6.1.2/joyrl/framework/recorder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-04-28 16:18:44
 LastEditor: JiangJi
-LastEditTime: 2024-05-30 17:48:58
+LastEditTime: 2024-06-02 10:50:37
 Discription: 
 '''
 import ray 
 from ray.util.queue import Queue as RayQueue
 from pathlib import Path
 import pickle
 import time
@@ -17,15 +17,15 @@
 
 import pandas as pd
 from queue import Queue
 from torch.utils.tensorboard import SummaryWriter  
 from joyrl.framework.message import Msg, MsgType
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.base import Moduler
-from joyrl.utils.utils import exec_method
+from joyrl.framework.utils import exec_method
 
 class Recorder(Moduler):
     ''' Recorder for recording training information
     '''
     def __init__(self, cfg: MergedConfig, **kwargs) -> None:
         super().__init__(cfg, **kwargs)
         self.type = kwargs.get('type', 'recorder')
```

### Comparing `joyrl-0.6.1.1/joyrl/framework/tester.py` & `joyrl-0.6.1.2/joyrl/framework/tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-02 15:02:30
 LastEditor: JiangJi
-LastEditTime: 2024-05-31 11:29:45
+LastEditTime: 2024-06-02 10:50:36
 Discription: 
 '''
 import time
 import copy
 import os
 import threading
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.base import Moduler
 from joyrl.framework.message import Msg, MsgType
-from joyrl.utils.utils import exec_method
+from joyrl.framework.utils import exec_method
     
 class OnlineTester(Moduler):
     ''' Online tester
     '''
     def __init__(self, cfg : MergedConfig, *args, **kwargs) -> None:
         super().__init__(cfg, *args, **kwargs)
         self.env = copy.deepcopy(kwargs['env'])
```

### Comparing `joyrl-0.6.1.1/joyrl/framework/tracker.py` & `joyrl-0.6.1.2/joyrl/framework/tracker.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/framework/trainer.py` & `joyrl-0.6.1.2/joyrl/framework/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-02 15:02:30
 LastEditor: JiangJi
-LastEditTime: 2024-06-01 16:53:24
+LastEditTime: 2024-06-02 10:50:35
 Discription: 
 '''
 import copy
 import time
 import ray
 from ray.util.queue import Queue as RayQueue
 from joyrl.framework.message import Msg, MsgType
@@ -18,16 +18,16 @@
 from joyrl.framework.collector import Collector
 from joyrl.framework.tracker import Tracker
 from joyrl.framework.interactor import Interactor
 from joyrl.framework.learner import Learner
 from joyrl.framework.tester import OnlineTester
 from joyrl.framework.policy_mgr import PolicyMgr
 from joyrl.framework.recorder import Recorder
-from joyrl.utils.utils import exec_method, create_module
-from joyrl.utils.utils import Logger
+from joyrl.framework.utils import exec_method, create_module
+from joyrl.framework.utils import Logger
 from joyrl.framework.utils import SharedData
 
 class Trainer(Moduler):
     ''' Collector for collecting training data
     '''
     def __init__(self, cfg: MergedConfig,**kwargs) -> None:
         super().__init__(cfg, **kwargs)
```

### Comparing `joyrl-0.6.1.1/joyrl/run.py` & `joyrl-0.6.1.2/joyrl/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-22 13:16:59
 LastEditor: JiangJi
-LastEditTime: 2024-06-01 17:17:47
+LastEditTime: 2024-06-02 10:47:58
 Discription: 
 '''
 import os,copy
 import ray
 import argparse,datetime,importlib,yaml
 import gymnasium as gym
 from pathlib import Path
 from joyrl.framework.config import GeneralConfig, MergedConfig, DefaultConfig
 from joyrl.framework.trainer import Trainer
-from joyrl.utils.utils import merge_class_attrs, all_seed, create_module,exec_method
+from joyrl.framework.utils import merge_class_attrs, all_seed, create_module, exec_method
 
 class Launcher(object):
     def __init__(self, **kwargs):
         self.custom_general_cfg = kwargs.get('general_cfg', None)
         self.custom_algo_cfg = kwargs.get('algo_cfg', None)
         self.custom_env_cfg = kwargs.get('env_cfg', None)
         self.custom_env = kwargs.get('env', None)
```

### Comparing `joyrl-0.6.1.1/joyrl/scripts/scripts.py` & `joyrl-0.6.1.2/joyrl/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/joyrl/utils/utils.py` & `joyrl-0.6.1.2/joyrl/framework/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
-Author: John
+Author: JiangJi
 Email: johnjim0816@gmail.com
-Date: 2021-03-12 16:02:24
-LastEditor: John
-LastEditTime: 2024-05-30 17:48:11
+Date: 2024-05-26 23:54:07
+LastEditor: JiangJi
+LastEditTime: 2024-06-02 10:49:38
 Discription: 
-Environment: 
 '''
 import os
 import math
 import copy
 import numpy as np
 import torch
 import torch.nn as nn
@@ -23,16 +22,85 @@
 from matplotlib import animation
 import seaborn as sns
 import yaml
 import pandas as pd
 from functools import wraps
 from time import time
 import logging
+import ray
+from threading import Lock
+from queue import Queue, Empty
 from matplotlib.font_manager import FontProperties  # 导入字体模块
 
+@ray.remote
+class SharedData:
+    ''' 
+    '''
+    def __init__(self, initial_value: float | int | dict) -> None:
+        self.value = initial_value
+        self.lock = Lock()
+
+    def get_value(self):
+        with self.lock:
+            return self.value
+
+    def set_value(self, new_value):
+        with self.lock:
+            self.value = new_value
+class DeQueue(Queue):
+    ''' Creating a thread-safe dequeue
+    '''
+    def pop(self, block=True, timeout=None):
+        '''Remove and return an item from the queue.
+        If optional args 'block' is true and 'timeout' is None (the default),
+        block if necessary until an item is available. If 'timeout' is
+        a non-negative number, it blocks at most 'timeout' seconds and raises
+        the Empty exception if no item was available within that time.
+        Otherwise ('block' is false), return an item if one is immediately
+        available, else raise the Empty exception ('timeout' is ignored
+        in that case).
+        '''
+        with self.not_empty:
+            if not block:
+                if not self._qsize():
+                    raise Empty
+            elif timeout is None:
+                while not self._qsize():
+                    self.not_empty.wait()
+            elif timeout < 0:
+                raise ValueError("'timeout' must be a non-negative number")
+            else:
+                endtime = time() + timeout
+                while not self._qsize():
+                    remaining = endtime - time()
+                    if remaining <= 0.0:
+                        raise Empty
+                    self.not_empty.wait(remaining)
+            item = self._pop()
+            self.not_full.notify()
+            return item
+    
+    def pop_nowait(self):
+        '''Remove and return an item from the queue without blocking.
+        Only get an item if one is immediately available. Otherwise
+        raise the Empty exception.
+        '''
+        return self.pop(block=False)
+    
+    # Get an item from the queue right
+    def _pop(self):
+        return self.queue.pop()
+    
+    def append(self, item):
+        ''' Put an item into the queue.
+        '''
+        with self.mutex:
+            self.queue.append(item)
+            self.unfinished_tasks += 1
+
 def chinese_font():
     ''' 设置中文字体，注意需要根据自己电脑情况更改字体路径，否则还是默认的字体
     '''
     try:
         font = FontProperties(
         fname='/System/Library/Fonts/STHeiti Light.ttc', size=15) # fname系统字体路径，此处是mac的
     except:
@@ -48,15 +116,15 @@
               cfg.algo_name), fontproperties=chinese_font())
     plt.xlabel(u'回合数', fontproperties=chinese_font())
     plt.plot(rewards)
     plt.plot(ma_rewards)
     plt.legend((u'奖励', u'滑动平均奖励',), loc="best", prop=chinese_font())
     if cfg.save:
         plt.savefig(cfg.result_path+f"{tag}_rewards_curve_cn")
-    # plt.show()
+
 def save_frames_as_gif(frames, fpath=None):
     ''' 保存gif动图
     '''
     Path(fpath).mkdir(parents=True, exist_ok=True)
     #Mess with this to change frame size
     plt.figure(figsize=(frames[0].shape[1] / 72.0, frames[0].shape[0] / 72.0), dpi=72)
 
@@ -116,14 +184,15 @@
     '''
     Path(fpath).mkdir(parents=True, exist_ok=True)
     df = pd.DataFrame(res_dic)
     df.to_csv(f"{fpath}/res.csv",index=None)
 def merge_class_attrs(ob1, ob2):
     ob1.__dict__.update(ob2.__dict__)
     return ob1
+
 def get_logger(fpath):
     Path(fpath).mkdir(parents=True, exist_ok=True)
     # logger = logging.getLogger(name='r')  # set root logger if not set name
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.INFO)
     formatter = logging.Formatter(
         '%(asctime)s - %(name)s - %(levelname)s: - %(message)s',
@@ -139,15 +208,15 @@
     # add Handler
     logger.addHandler(ch)
     logger.addHandler(fh)
     return logger
 
 def load_cfgs(cfgs, fpath):
     with open(fpath) as f:
-        load_cfg = yaml.load(f,Loader=yaml.FullLoader)
+        load_cfg = yaml.load(f, Loader=yaml.FullLoader)
         for cfg_type in cfgs:
             for k, v in load_cfg[cfg_type].items():
                 setattr(cfgs[cfg_type], k, v)
 
 def timing(func_name=True):
     def decorator(func):
         @wraps(func)
```

### Comparing `joyrl-0.6.1.1/joyrl.egg-info/PKG-INFO` & `joyrl-0.6.1.2/joyrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.6.1.1
+Version: 0.6.1.2
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.6.1.1/joyrl.egg-info/SOURCES.txt` & `joyrl-0.6.1.2/joyrl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,11 +79,8 @@
 joyrl/framework/policy_mgr.py
 joyrl/framework/recorder.py
 joyrl/framework/tester.py
 joyrl/framework/tracker.py
 joyrl/framework/trainer.py
 joyrl/framework/utils.py
 joyrl/scripts/__init__.py
-joyrl/scripts/scripts.py
-joyrl/utils/__init__.py
-joyrl/utils/plot.py
-joyrl/utils/utils.py
+joyrl/scripts/scripts.py
```

### Comparing `joyrl-0.6.1.1/setup.cfg` & `joyrl-0.6.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.1/setup.py` & `joyrl-0.6.1.2/setup.py`

 * *Files identical despite different names*

