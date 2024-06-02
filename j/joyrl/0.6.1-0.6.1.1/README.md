# Comparing `tmp/joyrl-0.6.1.tar.gz` & `tmp/joyrl-0.6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.6.1.tar", last modified: Sat Jun  1 16:28:17 2024, max compression
+gzip compressed data, was "joyrl-0.6.1.1.tar", last modified: Sat Jun  1 16:36:22 2024, max compression
```

## Comparing `joyrl-0.6.1.tar` & `joyrl-0.6.1.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.637101 joyrl-0.6.1/
--rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.1/LICENSE
--rw-r--r--   0 johnjim    (501) staff       (20)    11637 2024-06-01 16:28:17.637005 joyrl-0.6.1/PKG-INFO
--rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.1/README.md
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.621262 joyrl-0.6.1/joyrl/
--rw-r--r--   0 johnjim    (501) staff       (20)      375 2024-06-01 16:28:07.000000 joyrl-0.6.1/joyrl/__init__.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.622270 joyrl-0.6.1/joyrl/algos/
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.623082 joyrl-0.6.1/joyrl/algos/DDPG/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DDPG/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DDPG/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DDPG/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DDPG/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.623720 joyrl-0.6.1/joyrl/algos/DQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3519 2024-06-01 16:19:56.000000 joyrl-0.6.1/joyrl/algos/DQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.624266 joyrl-0.6.1/joyrl/algos/DoubleDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DoubleDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DoubleDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DoubleDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3696 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DoubleDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.624906 joyrl-0.6.1/joyrl/algos/DuelingDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DuelingDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      907 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DuelingDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DuelingDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3948 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DuelingDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.625500 joyrl-0.6.1/joyrl/algos/NoisyDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/NoisyDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1071 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/NoisyDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/NoisyDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4445 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/NoisyDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.626554 joyrl-0.6.1/joyrl/algos/PPO/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/PPO/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-05-09 17:05:41.000000 joyrl-0.6.1/joyrl/algos/PPO/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2979 2024-06-01 09:19:48.000000 joyrl-0.6.1/joyrl/algos/PPO/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     6921 2024-06-01 10:23:56.000000 joyrl-0.6.1/joyrl/algos/PPO/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.627293 joyrl-0.6.1/joyrl/algos/QLearning/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/QLearning/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/QLearning/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1/joyrl/algos/QLearning/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/QLearning/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.627889 joyrl-0.6.1/joyrl/algos/Sarsa/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/Sarsa/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/Sarsa/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1/joyrl/algos/Sarsa/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/Sarsa/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.628365 joyrl-0.6.1/joyrl/algos/TD3/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/TD3/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/TD3/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/TD3/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/TD3/policy.py
--rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/__init__.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.630721 joyrl-0.6.1/joyrl/algos/base/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/base/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)    10114 2024-06-01 16:17:16.000000 joyrl-0.6.1/joyrl/algos/base/action_layer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/base/base_layer.py
--rw-r--r--   0 johnjim    (501) staff       (20)    86089 2024-06-01 05:31:25.000000 joyrl-0.6.1/joyrl/algos/base/buffer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2755 2024-06-01 05:12:03.000000 joyrl-0.6.1/joyrl/algos/base/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/base/experience.py
--rw-r--r--   0 johnjim    (501) staff       (20)    13933 2024-06-01 16:11:14.000000 joyrl-0.6.1/joyrl/algos/base/network.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/base/noise.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/base/optm.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7635 2024-06-01 16:21:28.000000 joyrl-0.6.1/joyrl/algos/base/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.632256 joyrl-0.6.1/joyrl/envs/
--rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/blackjack.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/cliff_walking.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/gridworld.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/gridworld_env.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.632703 joyrl-0.6.1/joyrl/envs/gym/
--rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/gym/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/gym/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.1/joyrl/envs/gym/wrappers.py
--rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/racetrack.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/register.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/stochastic_mdp.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/windy_gridworld.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.635296 joyrl-0.6.1/joyrl/framework/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/framework/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1069 2024-05-30 09:43:52.000000 joyrl-0.6.1/joyrl/framework/base.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4442 2024-06-01 08:53:39.000000 joyrl-0.6.1/joyrl/framework/collector.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2294 2024-06-01 06:35:14.000000 joyrl-0.6.1/joyrl/framework/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5619 2024-06-01 08:53:09.000000 joyrl-0.6.1/joyrl/framework/interactor.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2874 2024-06-01 08:53:20.000000 joyrl-0.6.1/joyrl/framework/learner.py
--rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.1/joyrl/framework/message.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2923 2024-06-01 03:33:53.000000 joyrl-0.6.1/joyrl/framework/policy_mgr.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5272 2024-05-30 09:48:58.000000 joyrl-0.6.1/joyrl/framework/recorder.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3961 2024-05-31 03:30:30.000000 joyrl-0.6.1/joyrl/framework/tester.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/framework/tracker.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7020 2024-06-01 08:53:33.000000 joyrl-0.6.1/joyrl/framework/trainer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2524 2024-05-31 14:51:57.000000 joyrl-0.6.1/joyrl/framework/utils.py
--rw-r--r--   0 johnjim    (501) staff       (20)     8002 2024-06-01 09:17:47.000000 joyrl-0.6.1/joyrl/run.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.635790 joyrl-0.6.1/joyrl/scripts/
--rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/scripts/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/scripts/scripts.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.636298 joyrl-0.6.1/joyrl/utils/
--rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/utils/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/utils/plot.py
--rw-r--r--   0 johnjim    (501) staff       (20)    37181 2024-05-30 09:48:17.000000 joyrl-0.6.1/joyrl/utils/utils.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.636509 joyrl-0.6.1/joyrl.egg-info/
--rw-r--r--   0 johnjim    (501) staff       (20)    11637 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/PKG-INFO
--rw-r--r--   0 johnjim    (501) staff       (20)     2455 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/SOURCES.txt
--rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/dependency_links.txt
--rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/entry_points.txt
--rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/requires.txt
--rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/top_level.txt
--rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-01 16:28:17.637437 joyrl-0.6.1/setup.cfg
--rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.1/setup.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.419801 joyrl-0.6.1.1/
+-rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/LICENSE
+-rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-01 16:36:22.419715 joyrl-0.6.1.1/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.1.1/README.md
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.408865 joyrl-0.6.1.1/joyrl/
+-rw-r--r--   0 johnjim    (501) staff       (20)      377 2024-06-01 16:36:10.000000 joyrl-0.6.1.1/joyrl/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.409710 joyrl-0.6.1.1/joyrl/algos/
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.410226 joyrl-0.6.1.1/joyrl/algos/DDPG/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DDPG/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DDPG/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DDPG/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DDPG/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.410707 joyrl-0.6.1.1/joyrl/algos/DQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3519 2024-06-01 16:19:56.000000 joyrl-0.6.1.1/joyrl/algos/DQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.411145 joyrl-0.6.1.1/joyrl/algos/DoubleDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DoubleDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DoubleDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DoubleDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3696 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DoubleDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.411573 joyrl-0.6.1.1/joyrl/algos/DuelingDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DuelingDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1773 2024-06-01 16:33:50.000000 joyrl-0.6.1.1/joyrl/algos/DuelingDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/DuelingDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3518 2024-06-01 16:30:55.000000 joyrl-0.6.1.1/joyrl/algos/DuelingDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.412039 joyrl-0.6.1.1/joyrl/algos/NoisyDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/NoisyDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1071 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/NoisyDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/NoisyDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4445 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/NoisyDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.412493 joyrl-0.6.1.1/joyrl/algos/PPO/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/PPO/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-06-01 16:35:55.000000 joyrl-0.6.1.1/joyrl/algos/PPO/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2979 2024-06-01 09:19:48.000000 joyrl-0.6.1.1/joyrl/algos/PPO/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     6921 2024-06-01 10:23:56.000000 joyrl-0.6.1.1/joyrl/algos/PPO/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.412984 joyrl-0.6.1.1/joyrl/algos/QLearning/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/QLearning/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/QLearning/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1.1/joyrl/algos/QLearning/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/QLearning/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.413486 joyrl-0.6.1.1/joyrl/algos/Sarsa/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/Sarsa/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/Sarsa/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1.1/joyrl/algos/Sarsa/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/Sarsa/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.413977 joyrl-0.6.1.1/joyrl/algos/TD3/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/TD3/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/TD3/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/TD3/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/TD3/policy.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.415367 joyrl-0.6.1.1/joyrl/algos/base/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/base/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    10114 2024-06-01 16:17:16.000000 joyrl-0.6.1.1/joyrl/algos/base/action_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/base/base_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    86089 2024-06-01 05:31:25.000000 joyrl-0.6.1.1/joyrl/algos/base/buffer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2755 2024-06-01 05:12:03.000000 joyrl-0.6.1.1/joyrl/algos/base/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/base/experience.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    13933 2024-06-01 16:11:14.000000 joyrl-0.6.1.1/joyrl/algos/base/network.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/base/noise.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/algos/base/optm.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7635 2024-06-01 16:21:28.000000 joyrl-0.6.1.1/joyrl/algos/base/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.416553 joyrl-0.6.1.1/joyrl/envs/
+-rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/blackjack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/cliff_walking.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/gridworld.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/gridworld_env.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.416939 joyrl-0.6.1.1/joyrl/envs/gym/
+-rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/gym/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/gym/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.1.1/joyrl/envs/gym/wrappers.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/racetrack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/register.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/stochastic_mdp.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/envs/windy_gridworld.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.418484 joyrl-0.6.1.1/joyrl/framework/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/framework/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1069 2024-05-30 09:43:52.000000 joyrl-0.6.1.1/joyrl/framework/base.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4442 2024-06-01 08:53:39.000000 joyrl-0.6.1.1/joyrl/framework/collector.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2294 2024-06-01 06:35:14.000000 joyrl-0.6.1.1/joyrl/framework/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5619 2024-06-01 08:53:09.000000 joyrl-0.6.1.1/joyrl/framework/interactor.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2874 2024-06-01 08:53:20.000000 joyrl-0.6.1.1/joyrl/framework/learner.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.1.1/joyrl/framework/message.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2923 2024-06-01 03:33:53.000000 joyrl-0.6.1.1/joyrl/framework/policy_mgr.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5272 2024-05-30 09:48:58.000000 joyrl-0.6.1.1/joyrl/framework/recorder.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3961 2024-05-31 03:30:30.000000 joyrl-0.6.1.1/joyrl/framework/tester.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/framework/tracker.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7020 2024-06-01 08:53:33.000000 joyrl-0.6.1.1/joyrl/framework/trainer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2524 2024-05-31 14:51:57.000000 joyrl-0.6.1.1/joyrl/framework/utils.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8002 2024-06-01 09:17:47.000000 joyrl-0.6.1.1/joyrl/run.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.418717 joyrl-0.6.1.1/joyrl/scripts/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/scripts/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/scripts/scripts.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.419019 joyrl-0.6.1.1/joyrl/utils/
+-rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/utils/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.1/joyrl/utils/plot.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    37181 2024-05-30 09:48:17.000000 joyrl-0.6.1.1/joyrl/utils/utils.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:36:22.419204 joyrl-0.6.1.1/joyrl.egg-info/
+-rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)     2455 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/SOURCES.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/dependency_links.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/entry_points.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/requires.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-01 16:36:22.000000 joyrl-0.6.1.1/joyrl.egg-info/top_level.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-01 16:36:22.420134 joyrl-0.6.1.1/setup.cfg
+-rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.1.1/setup.py
```

### Comparing `joyrl-0.6.1/LICENSE` & `joyrl-0.6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/PKG-INFO` & `joyrl-0.6.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.6.1
+Version: 0.6.1.1
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.6.1/README.md` & `joyrl-0.6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/DDPG/config.py` & `joyrl-0.6.1.1/joyrl/algos/DDPG/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/DDPG/policy.py` & `joyrl-0.6.1.1/joyrl/algos/DDPG/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/DQN/config.py` & `joyrl-0.6.1.1/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/DQN/policy.py` & `joyrl-0.6.1.1/joyrl/algos/DQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.6.1.1/joyrl/algos/DoubleDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/DoubleDQN/policy.py` & `joyrl-0.6.1.1/joyrl/algos/DoubleDQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/DuelingDQN/config.py` & `joyrl-0.6.1.1/joyrl/algos/NoisyDQN/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,28 @@
+#!/usr/bin/env python
+# coding=utf-8
+'''
+Author: JiangJi
+Email: johnjim0816@gmail.com
+Date: 2023-02-21 20:32:11
+LastEditor: JiangJi
+LastEditTime: 2023-05-18 13:38:56
+Discription: 
+'''
 class AlgoConfig(object):
+    ''' algorithm parameters
+    '''
     def __init__(self) -> None:
-        # set epsilon_start=epsilon_end can obtain fixed epsilon=epsilon_end
-        self.dueling = True # use dueling network
+        # set epsilon_start=epsilon_end to get fixed epsilon, i.e. epsilon=epsilon_end
         self.epsilon_start = 0.95  # epsilon start value
         self.epsilon_end = 0.01  # epsilon end value
-        self.epsilon_decay = 500  # epsilon decay rate
-        self.gamma = 0.99  # discount factor
+        self.epsilon_decay = 500  # epsilon decay
+        self.gamma = 0.95  # reward discount factor
         self.lr = 0.0001  # learning rate
-        self.buffer_type = 'REPLAY_QUE' # replay buffer type
         self.max_buffer_size = 100000  # replay buffer size
         self.batch_size = 64  # batch size
         self.target_update = 4  # target network update frequency
         # value network layers config
         self.value_layers = [
-            {'layer_type': 'Linear', 'layer_size': [256], 'activation': 'ReLU'},
-            {'layer_type': 'Linear', 'layer_size': [256], 'activation': 'ReLU'},
+            {'layer_type': 'noisy_linear', 'layer_size': [64], 'activation': 'ReLU','std_init': 0.4},
+            {'layer_type': 'noisy_linear', 'layer_size': [64], 'activation': 'ReLU','std_init': 0.4},
         ]
```

### Comparing `joyrl-0.6.1/joyrl/algos/DuelingDQN/policy.py` & `joyrl-0.6.1.1/joyrl/algos/NoisyDQN/policy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,85 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
-Date: 2022-11-14 23:50:59
+Date: 2023-04-17 11:23:49
 LastEditor: JiangJi
-LastEditTime: 2023-12-24 20:35:14
+LastEditTime: 2023-12-25 00:18:41
 Discription: 
 '''
 import torch
 import torch.nn as nn
-import math,random
+import torch.optim as optim
+import torch.nn.functional as F
 import numpy as np
+import math
+import random
+
 from joyrl.algos.base.policy import BasePolicy
 from joyrl.algos.base.network import QNetwork
-        
+
 class Policy(BasePolicy):
     def __init__(self,cfg) -> None:
         super(Policy, self).__init__(cfg)
         self.cfg = cfg
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
-        self.to(self.device)
 
     def create_graph(self):
         self.state_size_list, self.action_size_list = self.get_state_action_size()
         self.policy_net = QNetwork(self.cfg, self.state_size_list, self.action_size_list).to(self.device)
         self.target_net = QNetwork(self.cfg, self.state_size_list, self.action_size_list).to(self.device)
         self.target_net.load_state_dict(self.policy_net.state_dict()) # or use this to copy parameters
+        # for noise parameters
+        # if self.cfg.mode == 'train': 
+        #     self.policy_net.train()
+        #     self.target_net.train()
+        # elif self.cfg.mode == 'test':
+        #     self.policy_net.eval()
+        #     self.target_net.eval()
         self.create_optimizer()
 
     def sample_action(self, state,  **kwargs):
         ''' sample action
         '''
         # epsilon must decay(linear,exponential and etc.) for balancing exploration and exploitation
         self.sample_count += 1
         self.epsilon = self.epsilon_end + (self.epsilon_start - self.epsilon_end) * \
             math.exp(-1. * self.sample_count / self.epsilon_decay) 
         if random.random() > self.epsilon:
             action = self.predict_action(state)
         else:
             action = self.action_space.sample()
         return action
-    
     def predict_action(self,state, **kwargs):
         ''' predict action
         '''
         with torch.no_grad():
             state = torch.tensor(np.array(state), device=self.device, dtype=torch.float32).unsqueeze(dim=0)
             q_values = self.policy_net(state)
             action = q_values.max(1)[1].item() # choose action corresponding to the maximum q value
         return action  
-    
+
     def learn(self, **kwargs):
         ''' train policy
         '''
         states, actions, next_states, rewards, dones = kwargs.get('states'), kwargs.get('actions'), kwargs.get('next_states'), kwargs.get('rewards'), kwargs.get('dones')
+        update_step = kwargs.get('update_step')
         # convert numpy to tensor
         states = torch.tensor(states, device=self.device, dtype=torch.float32)
         actions = torch.tensor(actions, device=self.device, dtype=torch.int64).unsqueeze(dim=1)
         next_states = torch.tensor(next_states, device=self.device, dtype=torch.float32)
         rewards = torch.tensor(rewards, device=self.device, dtype=torch.float32).unsqueeze(dim=1)
         dones = torch.tensor(dones, device=self.device, dtype=torch.float32).unsqueeze(dim=1)
         # compute current Q values
@@ -84,9 +96,11 @@
         for param in self.policy_net.parameters():
             param.grad.data.clamp_(-1, 1)
         self.optimizer.step()
         # update target net every C steps
         if self.update_step % self.target_update == 0: 
             self.target_net.load_state_dict(self.policy_net.state_dict())
         self.update_step += 1
+        self.policy_net.reset_noise()
+        self.target_net.reset_noise()
         self.update_summary() # update summary
- 
+
```

### Comparing `joyrl-0.6.1/joyrl/algos/PPO/config.py` & `joyrl-0.6.1.1/joyrl/algos/PPO/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/PPO/data_handler.py` & `joyrl-0.6.1.1/joyrl/algos/PPO/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/PPO/policy.py` & `joyrl-0.6.1.1/joyrl/algos/PPO/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/QLearning/data_handler.py` & `joyrl-0.6.1.1/joyrl/algos/QLearning/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/QLearning/policy.py` & `joyrl-0.6.1.1/joyrl/algos/QLearning/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/Sarsa/data_handler.py` & `joyrl-0.6.1.1/joyrl/algos/Sarsa/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/Sarsa/policy.py` & `joyrl-0.6.1.1/joyrl/algos/Sarsa/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/TD3/config.py` & `joyrl-0.6.1.1/joyrl/algos/TD3/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/TD3/policy.py` & `joyrl-0.6.1.1/joyrl/algos/TD3/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/base/action_layer.py` & `joyrl-0.6.1.1/joyrl/algos/base/action_layer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/base/base_layer.py` & `joyrl-0.6.1.1/joyrl/algos/base/base_layer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/base/buffer.py` & `joyrl-0.6.1.1/joyrl/algos/base/buffer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/base/data_handler.py` & `joyrl-0.6.1.1/joyrl/algos/base/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/base/network.py` & `joyrl-0.6.1.1/joyrl/algos/base/network.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/base/noise.py` & `joyrl-0.6.1.1/joyrl/algos/base/noise.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/base/optm.py` & `joyrl-0.6.1.1/joyrl/algos/base/optm.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/algos/base/policy.py` & `joyrl-0.6.1.1/joyrl/algos/base/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/envs/blackjack.py` & `joyrl-0.6.1.1/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/envs/cliff_walking.py` & `joyrl-0.6.1.1/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/envs/gridworld.py` & `joyrl-0.6.1.1/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/envs/gridworld_env.py` & `joyrl-0.6.1.1/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/envs/gym/config.py` & `joyrl-0.6.1.1/joyrl/envs/gym/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/envs/gym/wrappers.py` & `joyrl-0.6.1.1/joyrl/envs/gym/wrappers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/envs/racetrack.py` & `joyrl-0.6.1.1/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/envs/register.py` & `joyrl-0.6.1.1/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/envs/stochastic_mdp.py` & `joyrl-0.6.1.1/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/envs/windy_gridworld.py` & `joyrl-0.6.1.1/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/base.py` & `joyrl-0.6.1.1/joyrl/framework/base.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/collector.py` & `joyrl-0.6.1.1/joyrl/framework/collector.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/config.py` & `joyrl-0.6.1.1/joyrl/framework/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/interactor.py` & `joyrl-0.6.1.1/joyrl/framework/interactor.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/learner.py` & `joyrl-0.6.1.1/joyrl/framework/learner.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/message.py` & `joyrl-0.6.1.1/joyrl/framework/message.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/policy_mgr.py` & `joyrl-0.6.1.1/joyrl/framework/policy_mgr.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/recorder.py` & `joyrl-0.6.1.1/joyrl/framework/recorder.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/tester.py` & `joyrl-0.6.1.1/joyrl/framework/tester.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/tracker.py` & `joyrl-0.6.1.1/joyrl/framework/tracker.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/trainer.py` & `joyrl-0.6.1.1/joyrl/framework/trainer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/framework/utils.py` & `joyrl-0.6.1.1/joyrl/framework/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/run.py` & `joyrl-0.6.1.1/joyrl/run.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/scripts/scripts.py` & `joyrl-0.6.1.1/joyrl/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl/utils/utils.py` & `joyrl-0.6.1.1/joyrl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/joyrl.egg-info/PKG-INFO` & `joyrl-0.6.1.1/joyrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.6.1
+Version: 0.6.1.1
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.6.1/joyrl.egg-info/SOURCES.txt` & `joyrl-0.6.1.1/joyrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/setup.cfg` & `joyrl-0.6.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1/setup.py` & `joyrl-0.6.1.1/setup.py`

 * *Files identical despite different names*

