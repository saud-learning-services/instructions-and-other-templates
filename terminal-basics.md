# Terminal Basics

## What is terminal?

Terminals, also known as command lines or consoles, allow us to accomplish and automate tasks on a computer without the use of a graphical user interface (*source: [IT Connect](https://itconnect.uw.edu/learn/workshops/online-tutorials/web-publishing/what-is-a-terminal/)*)

In order to illustrate how terminal works, let's walk through an example use-case

### The task

1. Make a folder on the Desktop titled `My  Folder`
2. Make a folder inside `My Folder` called `Contents`
3. Make a file in `My Folder/Contents` called `foo.txt`
4. Make another file in  `My Folder/Contents` called `bar.txt`
5. Go back to `My Folder` and download in one of our projects from our [GitHub](https://github.com/saud-learning-services)
6. Check that `My Folder` contains two subfolders: `Contents` and the project we just cloned

### Accomplishing the task without terminal
> Note I am going to describe the process using Mac OS, however it will look almost identical on Windows or Linux machines.

1. Open Finder application and navigate to `Desktop`
2. Right click and select **New Folder**, title it **my-folder**
3. Go to **my-folder**, right click and select **New Folder**, title it **Contents**
4. Open textEdit application and make new empty file called `foo.txt` in **Contents**, Save
5. In textEdit application, make another new file called `bar.txt` in **Contents**, Save
6. Open GitHub Desktop and go through the several steps described [here](./github-project-management.md#how-to-get-projects-using-github-desktop)
7. Reopen Finder and double check the contents of **my-folder**

The steps above involve 3 separate applications, lots of navigating between applications and a lot of extra steps

### Accomplishing the task with terminal

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

That may seem like *more* steps, but consider what would take more time, doing all the subtasks in the non-terminal section or simply typing the commands in the terminal section?

> For more info on the `git` command and using terminal for Git/GitHub, see [here](./github-project-management.md)

**Below are some common commands for getting started with Terminal**

*Note that there are endless possibilies when it comes to terminal, this is merely meant to get someone started with the basics*

### `ls`

Running `ls` will list the contents of the current folder (subfolders and files). When you open terminal, it will start in your HOME folder. 

### `cd`

`cd` stands for change directory. 
You can use it to enter a immediate subdirectory from the current directory:
* `$ cd my-subfolder`
Or you can provide a whole filepath to go to any directory:
* `$ cd "Desktop/My Folder/Contents"`
You can also `cd` **out** of a given directory to a parent directory
* `$ cd ..` (see how this was used in the example above)


### `mkdir`

`mkdir` will create a folder
* `$ mkdir my-new-folder-name`

### `touch`

`touch` will create a new file
* `$ touch my-new-file.txt`
* `$ touch my-new-python-file.python`