# Setting up your local coding environment

## Concepts

For this project, we expect you to look at this concept:

[Struggling with the sandbox? Try this: Using Docker & WSL on your local host](../../alx-pre_course/resources/sandbox_struggles.md)

Most of the projects in this program are supposed to be done in a Linux (Ubuntu) environment.

For that matter, you will need to set up a similar environment for that purpose. It is for this reason
that we have the sandboxes but to be able to work locally even when you do not have internet
access, we highly recommend that you set up your own local coding environment.

This project is therefore a guide for you to set up the necessary coding environment irrespective
of the operating system that you are using. Once you have set this up, you can stop using the
Sandboxes and just use your local environment.

## Guide to running Ubuntu 20.04 on different operating systems

**Windows** You have **three** options for running Ubuntu on Windows:

- **WSL:** `WSL (Windows Subsystem for Linux)` is a feature that allows you to run Linux distributions natively on Windows.
WSL is the easiest option to set up and use, and it provides a good introduction to Ubuntu.
- **Vagrant:** `Vagrant` is a tool for creating and managing virtual machines. It is a good option if you need to run Ubuntu for development or testing purposes, as it allows you to create isolated environments that are easy to replicate and share.
- **Docker:** `Docker` is a tool for containerizing applications. It is a good option if you need to run Ubuntu for specific tasks, such as running a web server or database. But also remember using docker will need an installation of WSL.

**macOS** If you have:

- a Mac with an Apple Silicon chip, you can only use Docker to run `Ubuntu`.
- a Mac with an Intel chip, you can use `Vagrant` or `Docker`.

This project introduces you to all the available options. Go through them and choose the one that works for you.

### Vagrant - or - how to code in your local computer

Sandboxes are great, but you can also do your ALX assessments on your local computer - having a virtual machine (VM) is the perfect tool for that.

Let’s dig into `Vagrant` today!

Also:

- This project **can’t be done in Sandboxes** - it can be done only in your local computer.

## Resources

**Read or watch:**

- [Virtual machine](https://en.wikipedia.org/wiki/Virtual_machine)
- [man uname](https://linux.die.net/man/1/uname)

## Learning Objectives

At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

## General

- What is a virtual machine
- What is Vagrant
- Who wrote Vagrant
- What is Ubuntu
- What does “Ubuntu” mean
- How to use VMs with Vagrant
- What does the command `uname` do

## Copyright - Plagiarism

- You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.
- You will not be able to meet the objectives of this or any following project by copying and pasting someone else’s work.
- You are not allowed to publish any content of this project.
- Any form of plagiarism is strictly forbidden and will result in removal from the program.

## Requirements

### General

- A `README.md` file at the root of the repo, containing a description of the repository
- A `README.md` file, at the root of the folder of this project (i.e. `0x00-vagrant`), describing what this project is about

## More Info

### Install `git`

If `git` is not already installed on your terminal:

```shell
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git
```

### Basic usage

At the end of this project you should be able to reproduce and understand these command lines:

```shell
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main
```

### Warning

This project **can’t be done in Sandboxes** - it can be done only in your local computer. Please refer to our concept pages for your operating system.

#### Quiz questions

**Question #0**

What is a virtual machine?

- [ ] A set of servers for software development
- [x] An emulation of a computer system
- [ ] A system for developing virtual reality

**Question #1**

Ubuntu is a ____ distribution.

- [ ] Windows
- [ ] MacOS
- [x] Linux

**Question #2**

How do you launch a WSL distribution?

- [x] `wsl --distribution <distribution name>`
- [ ] `start wsl <distribution name>`
- [ ] `wsl run <distribution name>`

**Question #3**

What is the difference between a WSL distribution and a Linux distribution? _Select all correct answers?_

- [x] A WSL distribution is a special type of Linux distribution that is designed to run on Windows.
- [x] A WSL distribution is a regular Linux distribution that is packaged to run on Windows using the Windows Subsystem for Linux (WSL).
- [x] A WSL distribution is a lightweight version of a Linux distribution that is designed to be used on resource-constrained devices.

**Question #4**

[Fun question] Are you aware that all ALX products (the Intranet, the Checker, Sandboxes, Kimba,,,) are built and developed under several docker containers?

- [ ] No I didn’t, this is interesting!
- [x] Yes

**Question #5**

What is the difference between a Docker image and a Docker container?

- [ ] A Docker container is a runtime instance of a Docker image.
- [x] Docker image is like a blueprint, while a Docker container is like a house built from the blueprint.
- [x] A Docker image is immutable, meaning that it cannot be changed once it is created.
- [x] A Docker image is a lightweight, standalone, executable package of software that includes everything needed to run an application
- [x] A Docker image is a snapshot of a Docker container in a specific state.
- [x] A Docker image is a blueprint or template for creating a Docker container.
- [ ] A Docker image is a running instance of a Docker container.
- [x] A Docker container is a running instance of a Docker image.

**Question #6**

Select all correct definitions of Docker

- [x] A containerization platform
- [x] A tool that packages an application and all its dependencies together into a standardized unit for software development
- [x] A software development kit (SDK) for building and running distributed applications
- [ ] A software platform that uses OS-level virtualization to deliver software in packages called containers

**Question #7**

Where can you get help with WSL? _Select all correct answers_

- [x] The Microsoft Store
- [x] [The WSL Stack Overflow tag](https://stackoverflow.com/questions/tagged/wsl)
- [x] [The Microsoft Docs](https://learn.microsoft.com/en-us/windows/wsl/)
- [x] [The WSL GitHub repository](https://github.com/microsoft/WSL)
- [ ] The Windows Help app

**Question #8**

What is the correct definition of WSL? _Select all correct answers_

- [x] Windows Subsystem for Linux
- [x] A way to run Linux distributions on Windows without the need for a virtual machine
- [ ] A web service that allows users to create and share online surveys
- [x] A compatibility layer for running Linux binary executables natively on Windows 10

**Question #9**

Which is the correct way of accessing a Linux environment for coding? Select all correct answers

- [x] Use a Linux emulator
- [x] Install Linux on your computer
- [x] Use a Linux emulator
- [ ] Use a Linux debugger
- [x] Use a virtual machine to run Linux
- [x] Use a Linux container
- [x] Use a cloud-based Linux environment
- [ ] Use a Linux compiler
- [ ] Use a Linux chroot

### Tasks

>
> #### 0. Create and setup your Git and GitHub account
>
> You will need Git for this project, you might have to [install it](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) on your computer if it’s not done yet.
>
> - Configure your basic info (name, email) on your local machine – they will be part of your commits. [Tips](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)
>
> On [GitHub.com](https://github.com/):
>
> - Using the graphic interface on the website, create the repository (if it’s not done yet)
>   - Description: `This is my first repository as a full-stack engineer`
>   - Public repo: `zero_day`
>   - No `README`, `.gitignore`, or license
>
> On your computer, open a terminal and do the following:
>
>  - Navigate to your home directory. [Tips](https://linuxconfig.org/single-linux-command-to-return-to-home-directory)
>  - Create a directory `zero_day`. [Tips](https://help.ubuntu.com/community/Beginners/BashScripting)
>  - Navigate to this new directory. [Tips](https://askubuntu.com/questions/232442/how-do-i-navigate-between-directories-in-terminal)
>  - Initialize git and add the remote origin
>  - Create a file `README.md` with Emacs (or other command line editors) and write a small [Markdown](https://wordpress.com/support/markdown-quick-reference/) text to present this project. This file is mandatory in projects
>  - Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin (Note: You will probably need to set your login/password to push to the remote server)
>
> Good job!
>
> You pushed your first file in your first repository of the first task of your first School project.
>
> **Repo**:
>
> > - GitHub repository: `zero_day`
> > - File: `README.md`
>

>
> #### 1. Hello Ubuntu
>
> Inside the `zero_day` repo, create a new directory called `0x00-vagrant`. Add a `README.md` file to this directory.
>
> `ssh` into your Ubuntu VM. What does the command `uname` print when you run it without any option?
>
> Type your answer into a file in the `0x00-vagrant` directory and push it to GitHub. Name your file accordingly as shown below.
>
> **Repo**:
>
> > - GitHub repository: `zero_day`
> > - Directory: `0x00-vagrant`
> > - File: `0-hello_ubuntu`
>
