<!-- PROJECT LOGO -->
<br />
<p align="center">
  <div align="center">
    <img src="../imgs/terminal-icon.png" alt="Logo" width="80" height="80">
  </div>

  <h3 align="center">Terminal Basics</h3>

  <p align="center">
    A short explanation of what terminal is and some important commands
    <br />
  </p>
</p>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [What is Terminal?](#what-is-terminal)
- [Getting Terminal Set Up](#getting-terminal-set-up)
- [Example Task Scenario](<#example-scenario-(tasks)>)
  - [Accomplishing the Task (without Terminal)](<#accomplishing-the-task-(without-terminal)>)
  - [Accomplishing the Task (with Terminal)](<#accomplishing-the-task-(with-terminal)>)
- [(Basic) Essential Commands](<#(basic)-essential-commands>)
  - [`ls`](#ls)
  - [`cd`](#cd)
  - [`mkdir`](#mkdir)
  - [`touch`](#touch)

## What is Terminal?

Terminals, also known as command lines or consoles, allow us to accomplish and automate tasks on a computer without the use of a graphical user interface (_source: [IT Connect](https://itconnect.uw.edu/learn/workshops/online-tutorials/web-publishing/what-is-a-terminal/)_)

## Getting Terminal Set Up

If you are on Mac or Linux computers, you should have terminal already installed. On windows computers, the command line uses slightly different syntax so getting set up will require a few extra steps.

[This article](https://medium.com/danielpadua/git-bash-with-vscode-593d5998f6be) explains how to get terminal set up on windows

> Note this will involve installing [Visual Studio Code](https://code.visualstudio.com/download) as well as [Git/Git Bash](https://git-scm.com/downloads) (which you may already have installed if you use Git or GitHub)

In order to illustrate how terminal works, let's walk through a _very simple_ example scenario

## Example Scenario (tasks)

1. Make a folder on the Desktop titled `My Folder`
2. Make a folder inside `My Folder` called `Contents`
3. Make a file in `My Folder/Contents` called `foo.txt`
4. Make another file in `My Folder/Contents` called `bar.txt`
5. Go back to `My Folder` and download in one of our projects from our [GitHub](https://github.com/saud-learning-services)
6. Check that `My Folder` contains two subfolders: `Contents` and the project we just cloned

### Accomplishing the Task (without Terminal)

> Note I am going to describe the process using Mac OS, however it will look almost identical on Windows or Linux machines.

1. Open Finder application and navigate to `Desktop`
2. Right click and select **New Folder**, title it **my-folder**
3. Go to **my-folder**, right click and select **New Folder**, title it **Contents**
4. Open textEdit application and make new file called `foo.txt`, write nothing and save to **Contents**
5. In textEdit application, make another new file called `bar.txt`, write nothing and save to **Contents**
6. Open GitHub Desktop and go through the steps described [here](./github-project-management.md#how-to-get-projects-using-github-desktop)
7. Reopen Finder and double check the contents of **my-folder** for `Contents` and the project we just cloned

The steps above involve 3 separate applications, lots of navigating between applications and a lot of extra steps

### Accomplishing the Task (with Terminal)

1. Open terminal application
1. run `$ cd Desktop`
1. run `$ mkdir my-folder`
1. run `$ cd my-folder`
1. run `$ mkdir Contents`
1. run `$ touch foo.txt`
1. run `$ touch bar.txt`
1. run `$ cd ..`
1. run `$ git pull <PROJECT-URL>` (where project URL is the actual URL for the project)
1. run `ls` (to list folder contents)

That may seem like _more_ steps, but consider what would take more time, doing all the subtasks in the non-terminal section or simply typing the commands in the terminal section?

> For more info on the `git` command and using terminal for Git/GitHub, see [here](./github-project-management.md)

## (Basic) Essential Commands

An important thing to realize about terminal is that you are always _somewhere_ -- ie. in some folder on a computer. When you first launch, this will be the HOME folder. As you navigate through, this will change.

### `ls`

Running `ls` will list the contents of the current folder (subfolders and files)

### `cd`

`cd` stands for change directory
You can use it to enter a immediate subdirectory from the current directory

- `$ cd my-subfolder`

Or you can provide a whole filepath to go to any directory

- `$ cd "Desktop/My Folder/Contents"`

You can also `cd` **out** of a given directory to a parent directory

- `$ cd ..` (see how this was used in the example above)

### `mkdir`

`mkdir` will create a folder:

- `$ mkdir my-new-folder-name`

### `touch`

`touch` will create a new file

- `$ touch my-new-file.txt`
- `$ touch my-new-python-file.python`
