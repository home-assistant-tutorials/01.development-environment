# Tutorial 01 - Home Assistant - The Develoment Environment

This repository is the first one of a series of tutorials addressing differnt
parts of the development with Home Assistant seen with the eye of the skilled 
user. Each tutorial is shipped as a standalone github repository holding the
code alongside with the README (if any).

## The Development Environment

Today development is often done within Docker containers to get the same
environment for all develpers. This is as useful to get the same environment for
all users of a tutorial. The recommended method to run Home Assistant itself is
based upon Docker Conainers, the "Home Assistant Operating System".

While there are different containers around, lets go directly into the lion's
den and use [the development container of the Home Assistant
core](https://github.com/home-assistant/core). It is well elaborated and most
likely up-to-date. Let's address the downside of this approach, too. It is a
large one. However, it is good to know the handling on the long run and you will
be able reuse this container for most of the future tutorials.

## Prerequisites

### Machine and Operating System

A contemporary machine being able to run Docker conatainers and VS Code.
Windows, Linux and Mac OS should do as Operating System equally well.

### Internet accesss

Just to mention it.

### Docker

Docker should have been set up for your machine. You should know how to run it.

### Visual Studio Code

*VS Code* should have been set up for your machine and you should have figured
*out how to use it.

The development container for core development is integrated with *VS Studio
Code*. It does automate most of the setup for you. There is also a manual setup
and you may use other editors. I hold to *VS Code* for this tutorial. Vim users
will find a well done plugin with vim bindings in *VS Code* and they get the IDE
on top for free.

### Shell

Even within *VS Code* you should know how to use a Linux shell. Inside the
cointainer you may get offered *zsh*. In case type `bash` to enter a *Bash*.

### Git

You should know how to use *Git* on the commandline. While *VS Code* offers a
graphical interface to *Git* it is difficult to really understand the usage
without a fundamental background.

### Github account

You should have registerd for a Github account to be able to fork your own
instances of differnt parts of the tutorial.

### JavaScript

To follow along the tutorials you should have a basic experience with JavaScript and understand it's implementation of the class concept.

### Python

Will depend upon the tutorial.

### Installation

### Mounting
