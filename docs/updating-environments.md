<br />
<p align="center">
  <div align="center">
    <img src="../imgs/update.png" alt="Logo" height="80">
  </div>

  <h3 align="center">Updating Environments</h3>
</p>

You will occasionally have to update your environment, either due to updates in projects or the development of new projects. You can do this using Anaconda Navigator or Terminal.

> ⚠️ If you are updating the universal environment, make sure to have a up-to-date version of [this](https://github.com/saud-learning-services/instructions-and-other-templates) repo cloned on your machine (this is where you'll find the universal-environment.yml file)

> ⚠️ If you're working with a project-level environment. Make sure you have the most up-to-date version of that project on your machine (i.e. you've "Fetched Origin" on GitHub Desktop)

> Note that the `$` character in these docs is not part of the command but rather is a commonly used symbol to indicates that what follows is a terminal command.

> 💡 Running a command in terminal refers to typing out the command in the bash terminal and then hitting enter.

## Instructions for Updating in VS Code Terminal

1. Open **VS Code**
2. Since you should have the most up-to-date version of your project/repo on your machine, open the project/repo folder. You can open it from the top menu via **File > Open Folder**
3. Launch a new bash terminal from the top menu via **Terminal > New Terminal**
4. Run the command `$ conda remove {environment-name}` in terminal which removes the old environment
> 👷 eg. for setup-test, you would run `$ conda remove setup-test`
5. Run the command `$ conda env create -f environment.yml` in terminal
> 👷 eg. for setup-test, you would run `$ conda env create -f environment.yml`
6. Run the command `$ conda activate <environment-name>` in terminal to activate the new environment.
> 👷 eg. for setup-test, you would run `$ conda activate setup-test`

If you couldn't already tell, the steps basically consist of removing the old environment and then importing a new environment, not exaclty updating the same environment in place. If you need help importing the new environment (steps 5 & 6), then refer to [Environment Setup](environment-setup.md).

> ⚠️ Getting errors? Confused? Don't forget to contact the Canvas API team for support.