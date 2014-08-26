---
layout: page
title: Software Setup
permalink: /software/
modified: 2013-05-31
category: articles
comments: true
share: true
---

<hr />

## TinyTitan setup

The OLCF has created a set of simple to use scripts to guide you through setting up your own TinyTitan. Once TinyTitan has been setup you will be ready to run the demo software

### Requirements

- At least two Raspberry Pis running the Raspbian distribution
- A network router or switch to connect the Pis to
- An active internet connection

### Step One
Step one will update each Raspberry Pi and configure the name and network settings. To start connect each Pi that will be part of the TinyTitan cluster to an active internet connect. Download the initial setup script and run it in a terminal as such:

```
$ curl -kfsSLO https://raw.github.com/TinyTitan/TinySetup/master/pi_setup.sh
$ bash pi_setup.sh
```

When prompted for the node number start at 1 and incriment to the total number of Raspberry Pi nodes.

### Step Two
With step one completed on all nodes connect each node to the router or switch. On the Pi that was given a node number of 1 login and download/run the second script

```
$ git clone https://github.com/TinyTitan/TinySetup.git
$ cd TinySetup
$ bash pi_post_setup.sh
```

### Step Three
Your TinyTitan unit should now be ready to go. Checkout the TinySPH and PiBrot examples available through the TinyTitan repo.

## TinySPH
TinySPH is a parallel 2D Smoothed Particle Hydrodynamics(SPH) code, designed to run in real time on the Oak Ridge Leadership Computing Facility's "Tiny Titan" Raspberry Pi cluster. This application was designed to demonstrate distributed computing concepts and while it works best in a distributed environment it is possible to run on a shared memory system such as a single multicore processor. Although the code is designed for Tiny Titan it should, perhaps with some small build tweaks, compile and run on various flavors of Linux and OS X. The code makes use of MPI for distributed computing and requires at least two mpi processes(1 render, 1 compute).

![alt text](https://raw.githubusercontent.com/AdamSimpson/SPH/master/images/SPH_Screenshot.png "SPH Screenshot")

For full details please see the TinySPH github page: https://github.com/TinyTitan/SPH

# PiBrot
PiBrot is a parallel Mandelbrot set race. The screen is divided in half vertically with one MPI task drawing the left side image and an identical image being drawn on the right side with N-2 MPI tasks, where N is the total number of MPI tasks.

The completed image on the right as the left attempts to catch up
![alt text](https://raw.githubusercontent.com/AdamSimpson/PiBrot/master/images/final_screenshot.png "Final Screenshot")

For full details please see the PiBrot github page: https://github.com/TinyTitan/PiBrot
