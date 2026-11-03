---
title: Managing Multiple Robots
date: 2026-05-04
categories: [Multiple Robots, Simulation, Getting Started]
tags: [multiple robots, simulation, setup]     # TAG names should always be lowercase
description: Managing Multiple Robots with ROS2
# toc: false
---

# Managing Multiple Robots 

In the last section we ran a full experiment, including data analysis.  This one will be a bit shorter and will focus on allowing you to control multiple robots as opposed to a single robot.  

We're also going back to the beginning where we launch our simulator from one terminal and our ROS nodes from other terminals.  If you want this to run headless then you'll need to extend our `run_headless.sh` script to kick off multiple ROS instances.

No data analysis here, just pure chaos.

## Running multiple robots

We'll need to tweak our ROS package to allow for multiple robots.

```bash
ros2 launch irobot_create_gz_bringup create3_gz.launch.py
```

In your second terminal, kick off your robot:

```bash
ros2 run create3_demo_talker_py undock_and_talk
```

Now, the crazy bit, in your **third** terminal, kick off **another** robot:

```bash
ros2 run create3_demo_talker_py undock_and_talk
```

## Homework Extensions

