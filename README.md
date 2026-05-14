# **Learning Git**
    
## Table of contents
  1. [Why I create this?](#1-why-i-create-this)
  2. [Control Version system](#2-control-version-system)<br>
    2.1. [Local Version Control System](#21-local-version-control-system)<br>
    2.2. [Centralized Version Control System](#22-centralized-version-control-system)<br>
    2.3. [Distributed Version Control System](#23-distributed-version-control-system)<br>

## 1. Why I create this?
I'm learning git from scratch so made this repo to practice as I go.
You'll find notes, terms, and concepts that I'm learning from the book Pro Git and its HTML version at [Learn Git](https://git-scm.com/learn)

## 2. Control Version system
First of all, let's talk about version control, is a system that records changes to a file over time. Doesn't matter if you screw things up because you can roll it back or if you lose a file with this you can easily recover it.

### 2.1. Local Version Control System
A simple local VCS without RCS is just copying files into another folder with a timestamp in the name. This is super simple but super risky because you can forget where you are or overwrite the wrong file. To solve this problem, programmers built local VCSs a simple database on your computer that tracks all your file changes. A popular one was RCS, which saves the differences between file versions so it can rebuild any version at any point in time.

![local version control system](/images/LVC.png)

### 2.2. Centrilized Version Control System

![centralized version control system](/images/02_)

### Distributed Version Control System

![distributed version control system](/images/03_distributed_version_control.png)
