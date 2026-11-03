---
title: Run-Time Requirements Analysis
date: 2026-05-09
categories: [Requirements Analysis, Software Engineering]
tags: [requirements, software engineering]     # TAG names should always be lowercase
description: Run-time requirements analysis
# toc: false
---

# Run-time requirements analysis with the Create 3

In this section we will perform requirements analysis at run time for the Create 3.  To do this we'll need to (1) define requirements, (2) define utility functions to *measure* our requirements, and (3) log/analyze our data.

We'll use a single Create 3 and our mission will be to reach a waypoint and send out a success message once that happens.  We also want our robot to go back home to charge if its battery gets too low.

## Requirements definition

Now, we'll define our software requirements based on our key objectives above.  We'll use the `SHALL` syntax as our requirements language.

> We are using requirements here, however there is nothing stopping you from using a goal model or suite of test cases instead.  Utility functions can measure those as well!

We'll want to make sure that our requirements are measurable as well - if they aren't then they're not really helpful for any form of validation.

> R1: The robot shall navigate to its waypoint within a configurable number of seconds.

> R2: Upon reaching the waypoint the robot shall broadcast a `success` message.



## Utility functions

## Analysis

## Homework Extensions

