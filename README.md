# Tutorial 01 - Home Assistant - The Develoment Environment

This repository is the first one of a series of tutorials addressing differnt
parts of the development with Home Assistant seen with the eye of the skilled 
user. Each tutorial is shipped as a standalone github repository holding the
code alongside with the README (if any).

## The Development Environment

Today development is often done within *Docker containers* to get the same
environment for all developers. This is as useful to get the same environment for
all users of a tutorial. The recommended method to run Home Assistant itself is
based upon *Docker Containers*, the *"Home Assistant Operating System"*.

While there are different containers around, let's go directly into the lion's
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

Begin be setting up the container as instructed by [the documenttion
here](https://developers.home-assistant.io/docs/development_environment). You
actually have to visit the page and to use the given form, to start up your
container.

![instructions](img/instructions-for-dev-container.png)

This may take a while depending upon your connections. Open the terminal window at the bottom of *VS Code* to follow along the process of the installation.

![log of setup](img/process-of-container-setup.png)

In the dashboard of the *Docker Desktop* you can observe, how a bootstrapping container is setting up the development container.

![bootstrapping](img/bootstrapping.png)

It gets a crazy `NAME` assigned. In my case it is `blissful_gagarin`. You
recoginize the right container by the `IMAGE` name. It contains the name you
assigned to your fork on Github. Assign the container a meaningful name in the
shell of your host machine in analogy to my example:

```bash
docker rename blissful_gagarin ha.tutorial
```

![starting ha](img/starting-ha.png)

Follow the instructions to start Home Assistant. Open the command palette of *VS
Code*. Select `Tasks: Run Task`. Select `Run Home Assistant Core`. Follow along
in the terminal window, if everything goes well.

You can ignore a warning regarding the version of Python. Home Assistant wants
to support older versions to a certain extend. When time has come, the core team
will update the container.

![deprecation warnig](img/deprecation-waring.png)

Go ahead to the port `8123` of your local machine to set up an account for the admin. The typical URL is `http://localhost:8123`.

### Mounting
