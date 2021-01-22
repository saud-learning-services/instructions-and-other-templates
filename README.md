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

### Use the documentation to get started if you are brand new
 
Throughout the documentation we have included 👷  as an indicator to follow along. Watch out for our cautions ⚠️  and our tips 💡 (we might even reveal some of the magic [🧙‍♀️](https://tenor.com/EJvb.gif)). We know these docs are content heavy, but they are also for future reference as you learn more (or want to learn more). Basically, by going through our docs and following along, you will be: 
1. Making sure you have the right accounts (if you see this... you have an account!)
2. [Installing everything you need on your computer](docs/computer-setup.md)
   - Anaconda Navigator
   - GitHub Desktop
   - (Git)
3. [Cloning your first repo](docs/github-project-management.md) - setup-test👷
4. Creating a [project-specific environment](environment-setup.md#configuring-environments) for setup-test
5. Creating the [universal environment 🌎](docs/environment-setup.md#universal-environment-setup)  
6. [Running your first project](docs/running-instructions.md) 
   - try it using the project environment from [setup-test](https://github.com/saud-learning-services/setup-test)
   - now try running setup-test again, but use the universal environment in Anaconda

By the end, you should be able to now clone any projects/repos that you need, and know how to run the associated Jupyter notebooks! 
## Additional Resources

- [Terminal Basics](docs/terminal-basics.md)

## Projects

> All projects listed below support the universal environment 🌎

- [Canvas Batch Change Dates](https://github.com/saud-learning-services/canvas-batch-change-dates): Batch change the start and end dates for courses listed in a CSV.
- [Canvas Subaccount Movement](https://github.com/saud-learning-services/subaccount-movement): Moves any Sauder course into a specific Canvas sub-account. Upon providing the necessary input, the script will locate the appropriate sub-account, migrate the course to it, and produce a CSV file detailing the courses and the sub-accounts.
- [Canvas Quiz Response PDFs](https://github.com/saud-learning-services/quiz-response-pdfs): Pulls quiz data from Canvas to create PDF documents containing student answers to essay questions.
- [Canvas Peer Reviews](https://github.com/saud-learning-services/canvas-peer-reviews): Create CSV tables containing peer review data; summarizing all students who've been assigned as assessors, who they are assessing and the results of any completed assessments
- [Canvas Get Group CSV](https://github.com/saud-learning-services/group-csv): Used to extract a csv file of group names and associated student user IDs in any Canvas course
- [Canvas (Sauder) Semester Prep](https://github.com/saud-learning-services/canvas-saud-semester-prep): Generates a CSV that summarizes all Canvas courses that fall under a provided term id and account id(s).
