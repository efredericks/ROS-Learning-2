---
title: Deploying to Physical Robots
date: 2026-05-05
categories: [Multiple Robots, Simulation, Getting Started]
tags: [multiple robots, simulation, setup]     # TAG names should always be lowercase
description: Managing Multiple Robots with ROS2
# toc: false
---

# Physical Robot Deployment

*Note: if you do not have access to a physical robot you can skim over this section*

In this section we will go over how to take the programs developed for ROS simulations and make them run on a physical robot.  The main requirement is that the physical robot is setup to handle ROS in the same way that your simulated robots handle them.

For this we'll be setting up and deploying our basic setup to both the iRobot Create 3 and bitcraze Crazyflie 2.1.

## Setup

This will get our robots ready to handle our basic and logging setups.  Note that we will be streaming logging data over a ROS topic to avoid filling up local storage.

### iRobot Create 3

Fortunately, the Create 3 is already setup to receive ROS messages.  Refer to their documentation for putting the robot into ROS mode: <TBD>.

### bitcraze CrazyFlie 2.1

If you recall from the `CrazySwarm` setup, the firmware used for the simulator is **not intended** for use with the physical robot.  You'll need to build a new firmware, though the software we've developed so far should work fine.

TBD

## Application Deployment

Now we'll deploy our applications to the physical robots.  We'll need to make a slight tweak to our logging to ensure that the topic is broadcast over the network.

### iRobot Create 3

### bitcraze Crazyflie 2.1


## Homework Extensions


