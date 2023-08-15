<!-- PROJECT LOGO -->
<br />
<p align="center">
  <div align="center">
    <img src="imgs/sauder-logo.png" alt="Logo" height="50">
  </div>

  <h3 align="center">Sauder Canvas API Guide</h3>

  <p align="center">
  A home for the documentation and guides needed to work with Sauder LS, Canvas API Projects
    <br />
  </p>
</p>

<!-- LINKS TO ALL DOCS -->

## Documentation

1. [Computer Setup](docs/computer-setup.md) _(start here if you are new to our projects)_
2. [Running Scripts in Visual Studio Code Terminal](docs/terminal-vscode-running-instructions.md)
3. [Getting & Managing Projects](docs/github-project-management.md)
4. [Environment Setup](docs/environment-setup.md)
5. [Running Scripts](docs/running-instructions.md)
6. [Updating the Environment](docs/updating-environments.md)

### Ops Setup Part 1
> Use the documentation to get started if you are brand new

Throughout the documentation we have included 👷 as an indicator to follow along with setup-test. Watch out for our cautions ⚠️ and our tips 💡 (we might even reveal some of the magic [🧙‍♀️](https://tenor.com/EJvb.gif)). We know these docs are content heavy, but they are also for future reference as you learn more (or want to learn more). 

For your first time, we recommend using the following as a checklist as you read and walk through the docs. You will notice :white_check_mark: in each of the docs that correspond to the steps listed below in Part 1. 

#### [Computer Setup](docs/computer-setup.md)
1. [Create a free GitHub Account](https://github.com/join)
2. Send a request to join the Saud-Learning-Services organization - email the ops manager who will add you to the [ls-ops](https://github.com/orgs/saud-learning-services/teams/ls-ops) team.
3. [Installing everything you need on your computer](docs/computer-setup.md)
   - a) [Git](https://git-scm.com/downloads) (should be included in GitHub Desktop steps)
   - b) [Download Miniconda](https://docs.conda.io/en/latest/miniconda.html) _(recommended for most)_

#### [Running Scripts in Visual Studio Code Terminal](docs/terminal-vscode-running-instructions.md)
4. [Download VS Code](https://code.visualstudio.com/download)
5. Download Python Extension Pack and Jupyter extensions in VS Code, which can both be found in the Extensions _(Ctrl+Shift+X)_ tab in VS Code.
6. Download the GitHub Pull Requests and Issues extensions in VS Code. See step 5 for where to find this.
7. Practice how to clone a repository using the extension downloaded in step 6.
THIS IS WHERE WE REALLY HAVE TO START REARRANGING ORDER

#### [Getting & Managing Projects](docs/github-project-management.md)
6. [Create a place for the projects to live](docs/github-project-management.md#create-a-local-project-folder): `Documents/GitHub/Sauder-Learning-Services/`
7. [Clone your first repo](https://github.com/saud-learning-services/instructions-and-other-templates/blob/main/docs/github-project-management.md#white_check_mark-1-start-from-github-desktop) - setup-test👷
8. Read about an [alternative way to clone a project](https://github.com/saud-learning-services/instructions-and-other-templates/blob/main/docs/github-project-management.md#2-start-from-the-github-organization). 
9. [Read about Updating a Project](docs/github-project-management.md#updating-a-project-vs-code).

#### [Environment Setup](docs/environment-setup.md)
10. Create a [project-specific environment](docs/environment-setup.md#configuring-environments) for setup-test.

#### [Running Scripts](docs/running-instructions.md)
11. [Run your first project](https://github.com/saud-learning-services/instructions-and-other-templates/blob/main/docs/running-instructions.md#running-the-script)
      - try it using the project environment from [setup-test](https://github.com/saud-learning-services/setup-test)
By the end, you should be able to now clone any projects/repos that you need, and know how to run the associated Jupyter notebooks!

### Ops Setup Part 2
Once you have walked through the instructions above, and ran your first project (setup-test), you can get your computer ready for running ls-ops scripts.

1. Review steps 1-4 above - have you installed everything, joined everything, and created your place for projects to live?
2. Clone all of the saud-ls-ops projects into your new directory `Documents/GitHub/Sauder-Learning-Services/`
    - a) from https://github.com/saud-learning-services you can use the search for the tag "saud-ls-ops" or see Projects list below
    - b) clone each of the projects into your folder `Documents/GitHub/Sauder-Learning-Services/`
      - ⚠️ Reminder how to clone: [Cloning your first repo](docs/github-project-management.md)
      - ⚠️ make sure you have been added to the Saud-Learning-Services organization (step #2 above) or you may not see all of the projects.
3. Set up the [universal environment 🌎](docs/environment-setup.md#universal-environment-setup) which you can use to run any of the "saud-ls-ops" projects 
4. Try out the universal environment with the [👷 setup-test project](https://github.com/saud-learning-services/instructions-and-other-templates/blob/main/docs/environment-setup.md#testing)

## Additional Resources

- [Terminal Basics](docs/terminal-basics.md)

## Projects

> All projects listed below support the universal environment 🌎

- [Canvas (Sauder) Semester Prep](https://github.com/saud-learning-services/canvas-saud-semester-prep): Generates a CSV that summarizes all Canvas courses that fall under a provided term id and account id(s).
- [Canvas Batch Change Dates](https://github.com/saud-learning-services/canvas-batch-change-dates): Batch change the start and end dates for courses listed in a CSV.
- [Canvas Subaccount Movement](https://github.com/saud-learning-services/subaccount-movement): Moves any Sauder course into a specific Canvas sub-account. Upon providing the necessary input, the script will locate the appropriate sub-account, migrate the course to it, and produce a CSV file detailing the courses and the sub-accounts.
- [Canvas Quiz Response PDFs](https://github.com/saud-learning-services/quiz-response-pdfs): Pulls quiz data from Canvas to create PDF documents containing student answers to essay questions.
- [Canvas Peer Reviews](https://github.com/saud-learning-services/canvas-peer-reviews): Create CSV tables containing peer review data; summarizing all students who've been assigned as assessors, who they are assessing and the results of any completed assessments
