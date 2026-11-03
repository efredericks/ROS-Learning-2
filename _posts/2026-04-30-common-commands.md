---
title: Common Commands
date: 2026-04-30
categories: [Getting Started, Commands]
tags: [setup, lookup, commands]     # TAG names should always be lowercase
description: List of common commands used for this research project
# toc: false
---

# Common commands

This section is intentionally at the top to keep track of all the "common commands" you'll need to run for every simulation.  It is not intended to be a fully-comprehensive cheatsheet, but moreso a list of things to remember.

## Environment / Startup commands

|||
|------|------|
| `distrobox enter <x>` | Enter a particular operating system using distrobox, e.g., `distrobox enter humble` |
| `distrobox install <x>` | Install a specific operating system using distrobox, e.g., `distrobox create --image ubuntu:22.04 --name humble --nvidia` |
| `distrobox exit` | Exit out of distrobox |
| `distrobox list` (or `distrobox ls`) | List out installed environments for distrobox |
| `distrobox stop <x>` | Stop the container from consuming resources, e.g., `distrobox stop humble` |
| `source install/local_setup.bash` | Loads the local resources for the current project into the shell (assuming you're in the root of the workspace, e.g., `~/distrobox/jazzy/create3_ws`) | 

## Build Commands

|||
|------|------|
| `rosdep install --from-path src -yi` | Install dependencies for ROS project |
| `colcon build --symlink-install` | Build workspace after changes (don't forget to `source` the `local_setup.bash` file again!) |

## Interaction commands

Run simulation

## Filesystem commands

Navigate
Get info from log






<!-- 
> This is a neutral information block.
{: .prompt-info }

> This is a helpful tip or recommendation.
{: .prompt-tip }

> This is a warning to alert users about potential issues.
{: .prompt-warning }

> This is a critical alert for dangerous actions.
{: .prompt-danger } 
-->