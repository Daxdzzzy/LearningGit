# **Learning Git**
## Table of Contents
  1. [Basic Operations](#1-basic-operations)  
    1.1. [File Operations](#11-file-operations)  
    1.2. [Text Operations](#12-text-operations)  
    1.3. [Directory Operations](#13-directory-operations)  
    1.4. [SSH, System Info & Network Operations](#14-ssh-system-info--network-operations)  
    1.5. [Process Monitoring Operations](#15-process-monitoring-operations)
  2. [Basic Shell Programming](#2-basic-shell-programming)  
    2.1. [Variables](#21-variables)  
    2.2. [Array](#22-array)  
    2.3. [String Substitution](#23-string-substitution)  
    2.4. [Other String Tricks](#24-other-string-tricks)  
    2.5. [Functions](#25-functions)  
    2.6. [Conditionals](#26-conditionals)  
    2.7. [Loops](#27-loops)  
    2.8. [Regex](#28-regex)  
    2.9. [Pipes](#29-pipes)  
  3. [Tricks](#3-tricks)  
  4. [Debugging](#4-debugging)  
  5. [Multi-threading](#5-multi-threading)
## Table of contents
1. [Why I create this?](#1-why-i-create-this)
2. [Control Version system](#2-getting-started)
   1. [Local Version Control System](#21-local-version-control-system)

## 1. Why I create this?
I'm learning git from scratch so made this repo to practice as I go.
You'll find notes, terms, and concepts that I'm learning from the book Pro Git and its HTML version at [Learn Git](https://git-scm.com/learn)

## 2. Getting Started
First of all, let's talk about version control, is a system that records changes to a file over time. Doesn't matter if you screw things up because you can roll it back or if you lose a file with this you can easily recover it.

### 2.1. Local Version Control System
A simple local VCS without RCS is just copying files into another folder with a timestamp in the name. This is super simple but super risky because you can forget where you are or overwrite the wrong file. To solve this problem, programmers built local VCSs a simple database on your computer that tracks all your file changes. A popular one was RCS, which saves the differences between file versions so it can rebuild any version at any point in time.

![local version control system](/images/LVC.png)
