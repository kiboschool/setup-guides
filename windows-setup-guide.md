# Windows Setup Guide

[Watch a walkthrough of this setup
guide](https://www.loom.com/share/c7ff1f619c5844bab568c0c3d681d8b2)

If you have a Windows 10 or Windows 11 laptop, you should follow these
instructions to set your computer up to write, run, and debug code. 

You'll install:

1. **Scoop**, a tool for installing and managing software
2. **Git**, a tool for managing changes to code 
3. **Cmder**, a terminal emulator that lets you interact with files and programs via text
4. **VSCode**, a popular programming text editor you'll use to write programs
5. **Python**, the programming language we'll use for introductory programming classes at Kibo

## 1. Scoop

Scoop is a tool for installing programs on Windows. When you are installing software in subsequent steps, or in the future, you’ll use Scoop.

To install Scoop, you’ll follow these steps (copied from the Quickstart Guide on https://scoop.sh/):

1. Open a Powershell Terminal

Press the  `⊞ Win`   (the Windows Key), then type “Powershell” and select the Powershell application to launch it

2. Copy and paste this line into Powershell, then hit Enter:

```powershell
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```

Since this changes some permissions on your computer, you'll have to enter 'y'
to accept the changes.

3. Copy and paste this line, then hit Enter:

```powershell
irm get.scoop.sh | iex
```

This line will actually download and install scoop. Scoop will take several minutes to install.

While you wait, you can read more about Scoop on its homepage. Note any questions you have about what terms mean, about particular software, or about how Scoop works.

Once Scoop has completed its install process, you can move on to the next step.

## 2. Git

Git is a version control tool. It helps software developers work together on a shared set of files. Over the course of the degree program, you’ll learn how to use Git to manage your work and collaborate with teammates. For now, you are just getting Git installed on your computer.

Run this command in Powershell to install Git:

```powershell
scoop install git
```

Git and its dependencies should install fairly quickly.

## 3. Cmder

Cmder is a Terminal Emulator. It provides a text-based way to manage files, run programs, and develop software. You’ll use it in many of your courses to run programs and see their output.

To install Cmder, run the following command in Powershell:

```powershell
scoop install cmder
```

While you wait for it to install, you can browse to the Cmder wiki to learn more about configuration options for cmder.

## 4. VSCode

Visual Studio Code (VSCode) is a text editor for programming. Unlike ‘rich text’ editors like Google Docs or Microsoft Word, VSCode operates on plain text. It can highlight different keywords, and use colors to indicate different parts of syntax, but it still saves each file as just the text. If someone opened the same file with different settings, it would look different.

To install VSCode, run the following commands in Powershell:

```powershell
scoop bucket add extras
```

```powershell
scoop install vscode
```

The first line (scoop bucket add extras) adds a “bucket” to scoop. It’s a new set of software programs and packages that scoop knows how to install. The second line actually installs vscode.

## 5. Python

Python is a popular programming language, which we use in the introductory programming courses at Kibo. While technically you could write python programs without installing any software, it’s important that you can run Python programs too! In order to run python programs, you’ll need to install the language.

To install Python, run the following command in Powershell

```powershell
scoop install python
```

There are lots of different versions of Python. This will install the latest version (`3.10` as of this writing) , which is what we’ll use in class.

## Summary

Here’s the short version of the above steps. 

Don't do them again if you've already followed the steps!

Open Powershell ( `⊞ Win` then search “Powershell”), and run these commands one at a time, in order. To run each command, copy and paste the line from here into Powershell and press Enter.

```powershell
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh | iex
scoop install git
scoop install cmder
scoop bucket add extras
scoop install vscode
scoop install python
```
