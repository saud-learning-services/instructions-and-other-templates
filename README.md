<!-- PROJECT LOGO -->
<br />
<p align="center">
  <div align="center">
    <img src="imgs/sauder-logo.png" alt="Logo" height="50">
  </div>

  <h3 align="center">Sauder Canvas API Projects Guide</h3>

  <p align="center">
    Centre of Documentation and Guides Needed to Work With Sauder LS Projects!
    <br />
  </p>
</p>

<!-- LINKS TO ALL DOCS -->

## Documentation

1. [Computer Setup](docs/computer-setup.md) _(start here if you are new to our projects, and follow in chronological order)_
2. [Visual Studio Code Setup](docs/vscode-setup.md)
3. [Managing Projects with GitHub](docs/github-project-management.md)
4. [Environment Setup](docs/environment-setup.md)
5. [Running Scripts](docs/running-instructions.md)

### Ops Setup

Throughout the documentation we have included this symbol 👷 as an indicator to follow along with setup-test. Watch out for our cautions ⚠️ and our tips 💡 (we might even reveal some of the magic [🧙‍♀️](https://tenor.com/EJvb.gif)). We know these docs are content heavy, but they are also for future reference as you learn more (or want to learn more). 

💡 For your first time, we recommend using the following as a checklist as you read and walk through the docs. You will notice :white_check_mark: in each of the docs correspond to the steps listed below. Do note that this checklist is the compressed version of all the steps, and isn't exactly beginner-friendly. For more detailed instructions, feel free to jump into any of the docs as you work through the checklist.

> 💡 Note that the `$` character in these docs is not part of the command but rather is a commonly used symbol to indicates that what follows is a terminal command. By "running a command", we mean typing that command and then pressing the _enter_ key. If ever stuck working in terminal, visit [Terminal Basics](terminal-basics.md).

#### [Computer Setup](docs/computer-setup.md)
- :white_check_mark: Install the latest version of [Git](https://git-scm.com/downloads).
- :white_check_mark: Create a free [GitHub Account](https://github.com/join).
- :white_check_mark: Send a request to join the Saud-Learning-Services organization on GitHub - email the ops manager who will add you to the [ls-ops](https://github.com/orgs/saud-learning-services/teams/ls-ops) team.
- :white_check_mark: Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html). Make sure you're downloading the right version.
- :white_check_mark: Open up the _Anaconda Prompt (miniconda3)_ program, and run the following commands: `$ git --version`, `$ python --version`, `$ conda --version`, and `conda init bash`.
- :white_check_mark: Download [Visual Studio Code](https://code.visualstudio.com/download).
- :white_check_mark: Open up VS Code, and launch a new Bash terminal. Run the command `$ conda install jupyter` and respond with `y` to all configuration options.

#### [Visual Studio Code Setup](docs/vscode-setup.md)
- :white_check_mark: Open up VS Code, and launch a new Bash terminal. Run the following commands, which should all output version numbers: `$ git --version`, `$ conda --version`, and `$ python --version`.
- :white_check_mark: Install the _Jupyter_ extension in VS Code.
- :white_check_mark: Install the _GitHub Pull Requests and Issues_ extension in VS Code.

#### [Managing Projects with GitHub](docs/github-project-management.md)
- :white_check_mark: [Create a local project folder for all the projects to live in.](docs/github-project-management.md#create-a-local-project-folder) We recommend creating `.../Documents/GitHub/Sauder-Learning-Services/` to serve that purpose.
- :white_check_mark: [Clone a repository from GitHub into VS Code](docs/github-project-management.md#cloning-a-project-vs-code). We recommend trying this for the first time with the 👷 [setup test project](https://github.com/saud-learning-services/setup-test).
- :white_check_mark: [Read through how to update a project in VS Code](docs/github-project-management.md#updating-a-project-vs-code). Note that you will not have to do any updating when you run through this checklist for the first time, as you already have the most recent project version on locally on your device.
- :white_check_mark: Read or try the [alternate way](docs/github-project-management.md#optional-managing-github-projects-using-terminal) to do the previous two checkpoints using the integrated terminal in VS Code. This is an optional step, but highly recommended if you are comfortable or interested in working in terminal.

#### [Environment Setup](docs/environment-setup.md)
- :white_check_mark: Open up the project which we want to create an environment for in VS Code.
- :white_check_mark: Run `$ conda env create -f environment.yml` in a Bash terminal from the directory containing the environment.yml file. This command creates an environment using the environment.yml file in the current directory.
- :white_check_mark: Activate the environment just created by running the command `$ conda activate <environment-name>` in that same Bash terminal. Wait for installation to complete.

#### [Running Scripts](docs/running-instructions.md)
- :white_check_mark: Generate a Canvas token and note it somewhere. ⚠️ For security reasons, set the expiration date to the next day and discard the token once you no longer need it. Skip this step if your project does not work with Canvas.
- :white_check_mark: Assign your token to the `.env` file and save the file. Skip this step if the project does not mention a `.env` on its GitHub page, or if the project does not work with Canvas at all.
- :white_check_mark: Open the folder where your project is located in VS Code, then open a new Bash terminal. Run the command `$ jupyter notebook` or `$ jupyter-notebook` in the terminal, which should open the project in the browser.
- :white_check_mark: Now working in browser, select the `.ipynb` file for your project.
- :white_check_mark: Read the information contained in the `.ipynb` file, and then select **Kernel** > **Restart & Run All** to run the entire Jupyter notebook. Follow any prompts given to you after running the file (eg pasting the Canvas token).
💡 We recommend restarting the kernel and clearing all outputs after you're done with the Jupyter notebook. Select **Kernel** > **Restart & Clear Output** before closing the Jupyter notebook/exiting the browser.

By this point, you should be able to now clone any projects/repos that you need, and know how to run the associated Jupyter notebooks!

#### Recommended Steps to Install a [Universal Environment](docs/environment-setup.md#universal-environment-setup) 🌎
> 💡 This is highly recommended, as the universal environment 🌎 allows you to run any of our projects working with the Canvas API.
- :white_check_mark: Install the universal environment 🌎 using the same steps above for "Environment Setup" section above. This [repository](https://github.com/saud-learning-services/instructions-and-other-templates) can be used to clone the project for the universal environment to your local device.
- :white_check_mark: Test **canvas-universal-env** 🌎 using the same steps in the "Running Scripts" section directly above. We recommend trying this out with the 👷 setup-test project.

## Additional Resources

- [Terminal Basics](docs/terminal-basics.md) - this is especially useful for working in VS Code terminal, which is used often in the documentation provided.

## Sample Projects

> All projects listed below support the universal environment 🌎 - test them out at your own convenience!

- [Canvas (Sauder) Semester Prep](https://github.com/saud-learning-services/canvas-saud-semester-prep): Generates a CSV that summarizes all Canvas courses that fall under a provided term id and account id(s).
- [Canvas Batch Change Dates](https://github.com/saud-learning-services/canvas-batch-change-dates): Batch change the start and end dates for courses listed in a CSV.
- [Canvas Quiz Response PDFs](https://github.com/saud-learning-services/quiz-response-pdfs): Pulls quiz data from Canvas to create PDF documents containing student answers to essay questions.