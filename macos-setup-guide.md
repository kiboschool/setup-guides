# MacOS Setup Guide

If you have an Apple laptop running MacOS, you should follow these
instructions to set your computer up to write, run, and debug code. 

You'll install:

1. **Homebrew**, a tool for installing and managing software
2. **Git**, a tool for managing changes to code 
3. **Iterm2**, a terminal emulator that lets you interact with files and programs via text
4. **VSCode**, a popular programming text editor you'll use to write programs
5. **Python**, the programming language we'll use for introductory programming classes at Kibo
6. **NodeJS**, the programming language and environment we'll use for introductory web development classes at Kibo

## 1. Homebrew

Homebrew is a tool for installing programs on MacOS. When you are installing software in subsequent steps, or in the future, you’ll use Homebrew.

To install Homebrew, you’ll follow these steps (copied from the Install Homebrew section on https://brew.sh/)

1. Open Terminal

Press  `⌘ Command + Space` to bring up Spotlight, then type “Terminal” and select the Terminal application to launch it

2. Install the XCode Command Line Tools

Copy and paste this line into Terminal, then hit Enter:

```sh
xcode-select --install
```

Agree to the prompts to allow the installation to proceed. This will install a
set of developer tools necessary to install other software. It won't install
XCode. You don't need to install XCode.

3. Install Homebrew

Copy and paste this line, then hit Enter:

```zsh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

This line will actually download and install Homebrew. The installer will tell
you what it is doing, and ask for confirmation several times. Use the default
settings. It may also prompt you for your computer password.

Once Homebrew has completed its install process, you can move on to the next step.

## 2. Git

Git is a version control tool. It helps software developers work together on a shared set of files. Over the course of the degree program, you’ll learn how to use Git to manage your work and collaborate with teammates. For now, you are just getting Git installed on your computer.

Run this command in Terminal to install Git:

```sh
brew install git
```

Git and its dependencies should install fairly quickly.

## 3. Iterm2

Iterm2 is a Terminal Emulator. It provides a text-based way to manage files, run programs, and develop software. You’ll use it in many of your courses to run programs and see their output.

To install Iterm2, run the following command in Terminal:

```sh
brew install --cask iterm2
```

While you wait for it to install, you can browse to the Iterm2 wiki to learn more about configuration options. 

## 4. VSCode

Visual Studio Code (VSCode) is a text editor for programming. Unlike ‘rich text’ editors like Google Docs or Microsoft Word, VSCode operates on plain text. It can highlight different keywords, and use colors to indicate different parts of syntax, but it still saves each file as just the text. If someone opened the same file with different settings, it would look different.

To install VSCode, run the following commands in Terminal:

```sh
brew install --cask visual-studio-code
```

## 5. Python

Python is a popular programming language, which we use in the introductory programming courses at Kibo. While technically you could write python programs without installing any software, it’s important that you can run Python programs too! In order to run python programs, you’ll need to install the language.

To install Python, run the following command in Terminal:

```sh
brew install python@3.10
```

There are lots of different versions of Python. This will install version `3.10`, which is the latest version of python and which is what we’ll use in class.

## 6. NodeJS

NodeJS is a JavaScript _runtime_ -- it lets you run JavaScript on your computer, like you run python, instead of just in the browser. For web development, lots of common development tools depend on NodeJS, including the automated tests for the web development classes.

To install Node, run the following command in Terminal:

```sh
brew install node
```

There are lots of different versions of Node. This will install version `20`, which is the latest stable version of Node and what we’ll use in class.

## Summary

Here’s the short version of the above steps. 

Don't do them again if you've already followed the steps!

Open Terminal (Press  `⌘ Command + Space` to bring up Spotlight, then type “Terminal” and select the Terminal application to launch it) and run these commands one at a time, in order. To run each command, copy and paste the line from here into Terminal and press Enter.

```sh
xcode-select --install
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install git
brew install --cask iterm2
brew install --cask visual-studio-code
brew install python@3.10
brew install node
```
