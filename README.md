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
2. [Getting & Managing Projects](docs/github-project-management.md)
3. [Environment Setup](docs/environment-setup.md)
4. [Running Scripts](docs/running-instructions.md)
5. [Updating the Environment](docs/updating-environments.md)

### Ops Setup Part 1
> Use the documentation to get started if you are brand new

Throughout the documentation we have included 👷 as an indicator to follow along. Watch out for our cautions ⚠️ and our tips 💡 (we might even reveal some of the magic [🧙‍♀️](https://tenor.com/EJvb.gif)). We know these docs are content heavy, but they are also for future reference as you learn more (or want to learn more). 

For your first time, we recommend using the following as a checklist as you read and walk through the docs. 

#### [Computer Setup](docs/computer-setup.md)
1. [Create a free GitHub Account](https://github.com/join)
2. Send a request to join the Saud-Learning-Services organization - email Alison or Marko who will add you to the [ls-ops](https://github.com/orgs/saud-learning-services/teams/ls-ops) team
3. [Installing everything you need on your computer](docs/computer-setup.md)
   - a) [Download Anaconda Navigator](https://www.anaconda.com/products/individual#Downloads) _(recommended for most)_
      - select the **64-Bit Graphical Installer** for your operating system. Note that some older Windows computer may need to install the **32-Bit Graphical Installer** (you can check [here](https://support.microsoft.com/en-us/windows/32-bit-and-64-bit-windows-frequently-asked-questions-c6ca9541-8dce-4d48-0415-94a3faa2e13d))
   - b) [Download GitHub Desktop](https://desktop.github.com)
   - c) [Git](https://git-scm.com/downloads) (should be included in GitHub Desktop steps)

#### [Getting & Managing Projects](docs/github-project-management.md)
4. Create a place for the projects to live: `Documents/GitHub/Sauder-Learning-Services/`
5. [Clone your first repo](docs/github-project-management.md) - setup-test👷
6. Read about Updating a Project (GitHub Desktop) -> note, because you are downloading the most recent version, there is nothing to do yet - but be aware that you should "Fetch origin" whenever you are using a script in the future (in case there are changes made).  

#### [Environment Setup](docs/environment-setup.md)
8. Create a [project-specific environment](environment-setup.md#configuring-environments) for setup-test

#### [Running Scripts](docs/running-instructions.md)
10. [Run your first project](docs/running-instructions.md)
      - try it using the project environment from [setup-test](https://github.com/saud-learning-services/setup-test)
By the end, you should be able to now clone any projects/repos that you need, and know how to run the associated Jupyter notebooks!

### Ops Setup Part 2
Once you have walked through the instructions above, and ran your first project (setup-test), you can get your computer ready for running ls-ops scripts.

1. Review steps 1-4 above - have you installed everything, joined everything, and created your place for projects to live?
2. Clone the saud-ls-ops projects into your new directory `Documents/GitHub/Sauder-Learning-Services/`
    - from https://github.com/saud-learning-services you can use the search for the tag "saud-ls-ops" or see Projects list below
    - clone each of the projects into your folder `Documents/GitHub/Sauder-Learning-Services/`
      - reminder [Cloning your first repo](docs/github-project-management.md)
      - reminder - make sure you have been added to the Saud-Learning-Services organization (step #2 above) or you may not see all of the projects.
3. Set up the [universal environment 🌎](docs/environment-setup.md#universal-environment-setup) which you can use to run any of the "saud-ls-ops" projects 
4. Try out the universal environment with the [👷 setup-test project](https://github.com/saud-learning-services/instructions-and-other-templates/blob/main/docs/environment-setup.md#testing)

## Additional Resources

- [Terminal Basics](docs/terminal-basics.md)
- [Running Scripts with Terminal & Visual Studio Code](docs/terminal-vscode-running-instructions.md)

## Projects

> All projects listed below support the universal environment 🌎

- [Canvas (Sauder) Semester Prep](https://github.com/saud-learning-services/canvas-saud-semester-prep): Generates a CSV that summarizes all Canvas courses that fall under a provided term id and account id(s).
- [Canvas Batch Change Dates](https://github.com/saud-learning-services/canvas-batch-change-dates): Batch change the start and end dates for courses listed in a CSV.
- [Canvas Subaccount Movement](https://github.com/saud-learning-services/subaccount-movement): Moves any Sauder course into a specific Canvas sub-account. Upon providing the necessary input, the script will locate the appropriate sub-account, migrate the course to it, and produce a CSV file detailing the courses and the sub-accounts.
- [Canvas Quiz Response PDFs](https://github.com/saud-learning-services/quiz-response-pdfs): Pulls quiz data from Canvas to create PDF documents containing student answers to essay questions.
- [Canvas Peer Reviews](https://github.com/saud-learning-services/canvas-peer-reviews): Create CSV tables containing peer review data; summarizing all students who've been assigned as assessors, who they are assessing and the results of any completed assessments
