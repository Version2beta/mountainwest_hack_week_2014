# Introduction to Docker

John Turnbull, Docker VP of Services, @kartar, james@docker.io

Docker: a framework that's built on top of container virtualizations.

Container virtualization: Virtualization without the hypervisor part. A thin layer on top of the operating system that makes calls to the host operating system.

* Very performant
* Very lightweight
* Based on lxc

Docker's analog is shipping containers

* Isolated, layered, standard and content agnostic
* Easy, lightweight way to model reality
* Devs care about app, ops care about the container
* Golden images () without the overhead

Why not VMs / VPSs?

* speed
* portability
* size
* density
* performance
* cost

Technology stack

* Runs on most Linux distros
* cgroups and namespacing
* Device mapper or AUFS or vfs or pluggable
* libcontainer or lxc or pluggable

Dockerfile

Docker index for images

DOCKER 1.0 NEXT MONTH!!

