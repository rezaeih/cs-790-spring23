# P4 Tutorial

## Introduction

Welcome to the P4 Tutorial!

I've prepared two exercises to help you get started with P4
programming:

1. Introduction and Language Basics (mandatory)
* [Basic Forwarding](./basic)


2. Monitoring and Debugging (mandatory)
* [Explicit Congestion Notification](./ecn)


3. Dynamic Behavior (extra credit)
* [Load Balancing](./load_balance)

## Obtaining required software

To complete the exercises, you will need to either build a
virtual machine using the explanation below, or install all the  dependencies such as p4c, bmv2, and mininet by hand. Refer to README file in previous directory for links.

To build the virtual machine:
- Install [Vagrant](https://vagrantup.com) and [VirtualBox](https://virtualbox.org)
- `cd vm`
- `vagrant up`
- Log in with username `p4` and password `p4` and issue the command `sudo shutdown -r now`
- When the machine reboots, you should have a graphical desktop machine with the required
software pre-installed.
- `cd vm` (inside the running vm)
- `chmod 777 ./root-bootstrap.sh; sudo chown 777 ./root-bootstrap.sh`
- `sudo ./root-bootstrap.sh`
- `chmod 777 ./user-bootstrap.sh; sudo chown 777 ./user-bootstrap.sh`
- `pip install pathlib`
- `sudo ./user-bootstrap.sh`
- 

To install dependencies by hand, please reference the [vm](../vm) installation scripts.
They contain the dependencies, versions, and installation procedure.
You can run them directly on an Ubuntu 16.04 machine:
- `sudo ./root-bootstrap.sh`
- `sudo ./user-bootstrap.sh`
