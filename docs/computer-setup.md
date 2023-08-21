<!-- PROJECT LOGO -->
<br />
<p align="center">
  <div align="center">
    <img src="../imgs/computer.png" alt="Logo" width="80" height="80">
  </div>

  <h3 align="center">Computer Setup</h3>

  <p align="center">
    Installing the Tools Needed to Run Sauder LS Projects
    <br />
  </p>
</p>

> 💡 Note that the `$` character in these docs is not part of the command but rather is a commonly used symbol to indicates that what follows is a terminal command. By "running a command", we mean typing that command and then pressing the _enter_ key. If ever stuck working in terminal, visit [Terminal Basics](terminal-basics.md).

The basic tools for working with any Sauder LS Canvas API project are:
- Tools for getting/updating projects
- An environment to run the project in
- A place to manage environments and install extensions needed to run projects

Let us start by installing [Git](https://git-scm.com/downloads). Installing Git comes with Git Bash, a commonly used command-line interface (CLI). This will be useful when we start using VS Code later in this document.
- :white_check_mark: Install the latest version of [Git](https://git-scm.com/downloads)

> 💡Git Bash offers a more consistent experience across different operating systems (Windows, macOS, Linux) and offers additional features and capabilities compared to the default Windows Command Prompt. In other words, it's much easier to use!

[GitHub](https://github.com) - not to be confused with Git - is our tool for distributing projects and managing updates. We discuss GitHub in more detail in a later section ([Managing Projects with GitHub](github-project-management.md)). For now, you'll need to:
-  :white_check_mark: [Create a free GitHub account](https://github.com/join)
-  :white_check_mark: **For LS-Ops:** Contact someone on the Canvas API team to be added to the saud-learning-services/ls-ops team on GitHub (need this to access certain projects)

[Miniconda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html) is our tool for installing the conda package and environment management system. We will cover more on environments later in [Environment Setup](environment-setup.md). Downloading Miniconda gives you a lightweight foundation for using conda and Python, allowing you to build a custom environment suited to your requirements.
- :white_check_mark: [Download Miniconda](https://docs.conda.io/en/latest/miniconda.html) but make sure it's the right version for your device! After the download has finished, run the installer and accept the **default configuration** for all steps.

<div align="center">
    <img src="../imgs/miniconda-installation.png" alt="Logo" width="600">
</div>

Once Miniconda is installed, open the _Start Menu_. Typically, you can find the menu button along the top or bottom of your screen in the form of the Windows icon (Windows OS) or Apple icon (macOS). Click on the icon and search for the program called _Anaconda Prompt (miniconda3)_. When this opens you will see a prompt similar to `(base) C:\Users\your_name`. Type the following to check that your installations are working:
- :white_check_mark: Run the command `$ python --version` (a version number should print out)
- :white_check_mark: Run the command `$ conda --version` (a version number should print out)
- If the installation was successful, the output should look similar to this:

<div align="center">
    <img src="../imgs/anaconda-prompt-check.png" alt="Logo" width="600">
</div>

We can make the Anaconda Prompt available from the Git Bash terminal by default, allowing us to use Git and conda simultaneously. Open the _Anaconda Prompt (miniconda3)_ program again and run this command to configure Git Bash:
- :white_check_mark: Run the command `conda init bash` which should look similar to this:

<div align="center">
    <img src="../imgs/conda-initialize-bash.png" alt="Logo" width="500">
</div>

Visual Studio Code (more commonly known as VS Code) is a popular code editor allowing us to write new code, modify existing code, or run command line tasks in its integrated terminal. All our projects are built to run in both Jupyter notebooks and directly in terminal. Follow the steps below to download and configure VS Code:
- :white_check_mark: [Download Visual Studio Code](https://code.visualstudio.com/download)
- :white_check_mark: Launch VS Code, then launch a new terminal in VS Code. Do this by selecting from the top menu **Terminal > New Terminal**.
<div align="center">
    <img src="../imgs/where-vscode-terminal.png" alt="Logo" width="600">
</div>
- :white_check_mark: Select the (Git) Bash command-line interface for the terminal (top right in the photo below). Then, run the commands `$ git --version`, `$ conda --version`, and `$ python --version` (version numbers should print out). The end result should look similar to this:
<div align="center">
    <img src="../imgs/vscode-terminal.png" alt="Logo" width="600">
</div>
- :white_check_mark: (still working in VS Code Bash terminal) Run the command `$ conda install jupyter` and respond with the `yes` or `y` command to all configuration options. This allows users to work with Jupyter Notebook and other Jupyter-related components within your conda environment.

Once you have successfully done all the above, you're ready to start downloading and running projects.

We've provided a 👷 [Setup Test Project](https://github.com/saud-learning-services/setup-test) on our GitHub that you can use throughout the remainder of the documentation to ensure you have everything up and running correctly. These documents serve as a step-by-step on how to get this project running on your machine, so that you can apply this same process to all subsequent projects.

Once everything is configured correctly, you should see an output of "Hey {your-name-on-canvas}":

<div align="center">
    <img src="../imgs/test-output.png" alt="Logo" width="350">
</div>

Keep following along to reach that final step!

> 💡Getting errors? Recheck if you downloaded the wrong version of Miniconda for your device and retrace your steps to see if you configured Git Bash correctly when working with the _Anaconda Prompt (miniconda3)_ program. These appear to be the most common issues which may come up.
> ⚠️ Still confused? Don't forget to contact the Sauder Canvas API team for support.

[➡️ Next: VS Code Setup](vscode-setup.md)