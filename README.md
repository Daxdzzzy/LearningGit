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

![local version control system](/images/01_local_version_control.png)

### 2.2. Centrilized Version Control System
This system improves upon and solves the problems that RCS has, like not just one client being allowed to work on the file. This system handles multiple clients on one single server. The client checks out files and saves versioned changes. All clients can see what others have changed or are working on because when some client saves and commits that file, the database stores that information and another client can see it. The management of this is good because the manager of the server has fine-grained control over all clients, like who can do what. When the server goes down, everything stops, or if something is corrupted on that server, all history is lost. When the client checks out from whatever server, they only get a single snapshot of that history.

![centralized version control system](/images/02_centralized_version_control.png)

### Distributed Version Control System
This one is the best of the three because it fixes all the problems, the server stores everything, projects, whatever and every client clones the whole server onto their own machine. So you’re not just getting the latest version, you’re cloning the full history, which gives you a complete backup. It also lets people work simultaneosly. Like this example to make it clearer, we’ve got two servers with different jobs. The first, Pumpkin, is our main project server where we keep all the important source files. The second, Squash, is just an auxiliary server for our experimental team. So I’ll be working locally on my laptop. After I write a new feature, I commit it to the repo on my computer. Because it’s a distributed version control system, my machine doesn’t just store a snapshot — it keeps the entire project history. Then, before rolling out that new experimental feature to everyone, I want to make sure it’s okay for the company, so I push all my code to Squash, the auxiliary server. After that, zxzyy can pull my changes and keep developing the feature.

![distributed version control system](/images/03_distributed_version_control.png)
