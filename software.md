---
layout: page
title: Software Setup
permalink: /software/
modified: 2013-05-31
category: articles
comments: true
share: true
---

**NOTE:** This is a work in progress

<hr />

The OLCF has created a set of simple to use scripts to guide you through setting up your own TinyTitan.

### Requirements

- Raspberry Pis running the Raspbian distribution
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

