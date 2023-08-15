<!-- PROJECT LOGO -->
<br />
<p align="center">
  <div align="center">
    <img src="../imgs/github-logo.png" alt="Logo" width="80" height="80">
  </div>

  <h3 align="center">Managing Projects with GitHub</h3>

  <p align="center">
    A Guide for Managing Sauder LS Projects using GitHub
    <br />
    (VS Code and Terminal)
  </p>
</p>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [Table of Contents](#table-of-contents)
- [What is GitHub?](#what-is-github)
- [Why Use It?](#why-use-it)
- [Managing Projects Using VS Code](#managing-projects-using-vs-code)
  - [Downloading a Project (VS Code)](#downloading-a-project-vs-code)
  - [Updating a Project (VS Code)](#updating-a-project-vs-code)
- [(Optional) Managing GitHub Projects Using Terminal](#optional-managing-github-projects-using-terminal)
  - [Downloading a Project (Terminal)](#downloading-a-project-terminal)
  - [Updating a Project (Terminal)](#updating-a-project-terminal)

💡 All Sauder LS, Canvas API tools are hosted on our [GitHub](https://github.com/saud-learning-services).

## What is GitHub?

GitHub is a website that allows people to share and collaborate on software projects. All projects on GitHub use a version control system called [Git](https://git-scm.com/). For the purposes of _using_ our tools, it's enough to know that GitHub will be:

- Where you'll be downloading projects from
- How you will recieve updates

## Why Use It?

GitHub helps us with version control. Crucially, it'll help us ensure that everyone is using the most up-to-date versions of our tools. It will also help us respond to problems faster and send fixed code back to our users without creating any kind of duplication or confusion around which version is correct.

_Here's a scenario we're trying to avoid..._

Say you _manually_ download one of our tools to a folder on your computer like so:

<div align="center">
    <img src="../imgs/github_desktop/folder-single.png" alt="Logo" width="300">
</div>

Now over time, we make improvements to the tool, and let you know we've posted version 2, followed by version 3. Over time your project folder starts to look like:

<div align="center">
    <img src="../imgs/github_desktop/folder-messy.png" alt="Logo" width="300">
</div>

This has a lot of downsides:

- It makes it hard to keep track of which version is the "right" version
- Data can get lost or forgotten in folders of previous versions
- Users can miss crucial updates

GitHub solves this by allowing us all to host all our tools online and have everybody connect to the same "folder in the cloud" so to speak. This way everyone can be sure they're on the latest version of the code and any changes to the code can reach everybody.

<div align="center">
    <img src="../imgs/github_desktop/github_diagram.png" alt="Logo" width="500">
    <p>sending out updates through GitHub</p>
</div>

## Managing Projects Using VS Code

> ⚠️ Recommended for Operations team

First, you'll need a GitHub account (Don't have one? [Create one!](https://github.com/join)).

> 💡 For any Learning Services staff, get in touch to let someone from the API team and let them know you have an account and want to be added to the organization. Some projects (for LS-ops) are private and you must be a member of the organization to view them.

If not already downloaded, download [VS Code](https://desktop.github.com/). Among the things VS Code can do are: 

- write new code
- modify existing code
- run command line tasks in its integrated terminal
- download and contribute to projects hosted on GitHub

Once downloaded, open the application. It should look something like this:

<div align="center">
    <img src="../imgs/vscode-new-window.png" alt="Logo" width="500">
</div>

### Downloading Extensions
DUMMY SECTION, add extensions here (3 of them?)

### Create a local project folder
:white_check_mark: We recommend using `Documents/GitHub/Sauder-Learning-Services` to store all projects. If you haven't already, create a GitHub folder in Documents, and a Sauder-Learning-Services folder within.

- Documents can be easily found in the File Explorer (Windows) or Finder (macOS) as it is one of the default user directories.

### Downloading a Project (VS Code)

Start by launching VS Code. Select the source control icon on the left navigation menu, as seen below:

<div align="center">
    <img src="../imgs/vscode-source-control-icon.png" alt="Logo" width="800">
</div>

Next, obtain the GitHub URL of the project you are trying to get. To find this, visit a project page on GitHub and copy the link as seen below (click "Code" then clipboard icon):

> 👷 Working through the setup test? Visit that project and copy the URL as described above: [link to setup test repository](https://github.com/saud-learning-services/setup-test)

<div align="center">
    <img src="../imgs/copy-github-link.png" alt="Logo" width="800">
</div>

Back in VS Code, click on the **Clone Repository** button, which should be blue. You will be prompted to input a repository URL. This is where you paste in the URL obtained from GitHub, then press the enter key. You will then be required to select a folder to place the project in. As mentioned earlier, we recommend creating a single folder where you clone all Sauder LS GitHub Projects you need.

> 💡 We recommend using `.../Documents/GitHub/Sauder-Learning-Services` to store projects.

<div align="center">
    <img src="../imgs/clone-repository-gif.mp4" alt="Logo" width="800">
</div>
<div align="center">
    <img src="../imgs/recommended-saudls-folder.png" alt="Logo" width="800">
</div>

After cloning, this should open up a new window with the new project in the folder you've specified.

> 👷 Working through the setup test? A folder titled **setup-test** should've appeared in the location.

> 💡 Double check the suggested Local Path! We suggest `.../Documents/GitHub/Sauder-Learning-Services` to store projects.

### Updating a Project (VS Code)

:white_check_mark: _Read this - but note it won't apply your first time downloading a project because everything will be up to date!_

When we update a tool, we send those updates to GitHub where you can download or "fetch" them for your local copy.

To do this in VS Code, open up the project and follow the following sequence: **Source Control Tab > Views and More Actions... > Pull**. Note that there are many ways you can do this, including using **Pull from...** over **Pull**, but this is a quicker way to fetch any new changes from GitHub.

NEEDS GIF HERE

Your project will update to the the most recent version! Same location as before and if you had any data outputs in the project folders prior to fetching, that data will persist.

> If manually pulling from GitHub, and you're prompted to choose a branch, always choose either **main** or **master**.

> ⚠️ Please **DO NOT select Commit to main** unless you are contributing code!

> ⚠️ While we will try to communicate major updates to our team, it is advisable to "Fetch Origin" frequently (especially if you haven't used a tool in a while). This ensures it's up-to-date and only takes a few seconds.

The following section on terminal is optional. If you'd like to continue to manage tools as described above, head to the next section on environment setup.

[➡️ Next: Environment Setup](environment-setup.md)

## (Optional) Managing GitHub Projects Using Terminal

Terminal is a good way of managing GitHub projects if you are:

1. Someone who is interested in programming or computers
1. Someone who may want to contribute to one of our projects
1. Someone who is interested in the fastest possible way to manage projects

> It is also an excellent way to be the envy of all your friends as you'll look like some kind of computer genius, with capabilities nothing short of magic-like [🧙‍♀️](https://tenor.com/view/clapping-harry-potter-applause-smile-happy-gif-5297465)

Before reading on, you'll want to have read [terminal basics](./terminal-basics.md).

You'll also want to make sure that you have **Git** installed and an account on **GitHub** (the two often get confused, however they're different things):

- [Install Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [Create GitHub Account](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github/signing-up-for-a-new-github-account) and let us know you need to join the saud-learning-services organization

### Downloading a Project (Terminal)
Keep in mind that this is **OPTIONAL** for LS Ops!

Using the `cd` command, navigate to a folder where you'd like to store and run the project. 

> 💡 We recommend keeping all Sauder LS projects in a single folder for ease of management. Something like `.../Documents/GitHub/Sauder-Learning-Services` will do the trick.

Once you've navigated to the folder, you'll want to **clone** the project into it. This can be done using with running this command in terminal:

`$ git clone <URL>` (where `<URL>` is HTTPS link copied from the GitHub repo)

<div align="center">
    <img src="../imgs/github_desktop/copy-github-link.png" alt="github-link" width="800">
    <p>HTTPS links to projects can be found on the project's GitHub page</p>
</div>

### Updating a Project (Terminal)

Using the `cd` command, navigate to the folder where your copy of the project is stored

- `$ cd path/to/my-project`

Check to see what branch you are on

- `$ git branch` (the starred branch is your current branch; type **q** to exit)

If not on **main**, switch to it

- `$ git checkout main`

While on the main branch, grab the latest changes

- `$ git pull`

[➡️ Next: Environment Setup](environment-setup.md)