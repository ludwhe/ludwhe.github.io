---
layout: post
title:  "Virtualization on Linux: Introduction"

categories: [linux, virtualization]
---

Creating and running virtual machines is becoming a more and more common tasks
in today's computing workflows. Thanks to the ever-widening availability of
computer hardware and its constant optimization, it is becoming easier than
ever for anyone interested enough to create fast, useful virtual machines.

Maybe you run Linux but want to be able to play games (which don't already work
on [Proton](https://github.com/ValveSoftware/Proton) or plain
[WineHQ](https://www.winehq.org/)). Maybe you want to isolate processes on your
computer for security purposes. Maybe you just find it interesting to try out ;
in any scenario, here is the first in a series of posts aimed at helping you
understand your possibilities and concepts that can help you get started.

## Some virtualization vocabulary

Before we start diving into what virtualization **is**, we have to define
some common and useful vocabulary:

- **Host**: a **host** is a system which, well, *hosts* a virtual machine. In the case of this series, the host will be Linux.
- **Guest**: a **guest** is a system which is “virtualized” by the host. It runs inside the virtual machine.
- **Hypervisor**: the **hypervisor** (or monitor) is the software which allows us to create, start, stop and otherwise manage virtual machines. There exist different types of hypervisors:
  - **Type-1** or **bare-metal** hypervisors run directly on your computer hardware (think an OS which is made to virtualize other OSs). Examples are [Xen](https://xenproject.org/) and [VMWare ESXi](https://www.vmware.com/products/esxi-and-esx.html).
  - **Type-2** hypervisors are programs which run on conventional operating systems. Examples are [Oracle VirtualBox](https://www.virtualbox.org/), [VMWare Workstation Player](https://www.vmware.com/products/workstation-player/workstation-player.html) and [Workstation Pro](https://www.vmware.com/products/workstation-pro.html).

## Types of virtualization

There are several ways of running a virtualized operating system on your
computer, and especially on Linux. The most common and well-known way to
do so is called **hardware virtualization**.

### Hardware virtualization

Full virtualization / Para-virtualization

### Operating-system-level virtualization (containers)

chroot

control groups (cgroups) and docker

## Common virtual machine operations

start/stop/snapshot/restore/migrate
