---
title: Software Proposal
---

## Introduction

Our teams software design represents a smart plant system that combines multiple sensors and actuators to help maintain ideal growing conditions. Each section is a subsystem, which includes a soil moisture sensor, light sensor, water pump, and grow light, that works together to monitor and adjust the environment automatically. The system operates on the Microchip Curiosity Nano, where each board continuously reads data, processes it, and communicates to each other to coordinate actions.

The diagram below shows how each subsystem initializes, collects data, takes action based on sensor readings and loops continuously to keep the system stable.

## Team Activity Diagram

![SoftwareDiagram](newsoft.png)

Team Activity Diagram | [PDF Download](softio.pdf) | [Draw.io Download](https://drive.google.com/file/d/14Mvt6AI8rmQZjSnXgR-JArQeQUlvBvEq/view?usp=drive_link)

## Decision Making Process

Our team designed the software structure by dividing the system into 4 modular subsystems: a soil moisture sensor, a water pump, brightness sensor, and a grow light. We designed it in this way to ensure clarity between individual responsibilities of group members and to show visually what those responsibilities are. We designed it using 4 parallel activity loops in order to represent the embedded environment where individual tasks are split up into smaller circuits. The inclusion of an initialization step in each subsystem ensures proper and repeatable startup behavior. Each subsystem should work together to create a modular system which will monitor, water, and provide light to a plant in real time. 