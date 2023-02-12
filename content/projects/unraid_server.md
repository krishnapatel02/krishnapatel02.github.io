---
author:
    name: "Krishna Patel"
date: 2022-07-05
title: Unraid Server
weight: 10
---

## Introduction: 
This server will be used for multiple applications through virtualization. Unraid is a linux distro that allows the partitioning of resources to virtual machines/ The VMs will be used to run multiple servers/docker containers: one for a game server, one for media serving over the local network, and the last for miscellaneous development use.

## Hardware:
#### CPU: Intel Core i7 4960X 6 Core Processor
#### RAM: 32GB DDR3 8GB x 4
#### SSD: 256GB 
#### Hard Drives: 1TB 3.5" (3)
#### GPU: NVIDIA GTX 970
#### Motherboard: ASUS X79 Deluxe

This hardware is mostly old and will be repurposed. The hard drives were all bought from a local electronics recycling store for $10 each. The processor has enough cores for multiple VMs and there is sufficient memory to allow each VM to have at least 6GB of RAM. The hard drives will be in a xfs array with one drive used for parity data. This means I will be able to lose one drive before facing data loss, however this means I will be left with only 2TB of storage. The SSD will be used as a cache for the hard drives because Unraid boots off of a flash drive. The GPU can be passed through to one of the docker containers for GPU encoding or workload acceleration. Unraid also has a web server so configurations can be changed when the machine is run in a headless state. 