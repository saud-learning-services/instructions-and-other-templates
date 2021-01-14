# GitHub Workflows

> A place for the Canvas API team to share resources and discuss improvements/changes to make to our GitHub process

## Resources

- [Understanding the Github Flow](https://guides.github.com/introduction/flow/#:~:text=GitHub%20flow%20is%20a%20lightweight,and%20why%20GitHub%20flow%20works.): Excellent high-level description of the _branch -> edit -> review -> merge_ workflow that I use (Note for our purposes we ignore the "Deploy") **@marko**

- [Git Workflow](https://github.com/jamiebuilds/git-workflow): Enjoyed this article by **@jamiebuilds** on GitHub discussion tips for small-team GitHub workflow. Could be good to implement _some_ of these ideas, especially if we see bigger projects (i.e. more people contributing). Things I like:
  - Having a `main` branch that "is always working and deployable" - never work on `main`
  - Having a `staging` or `development` branch that we merge off of - " it should be ahead of the latest release to master and should attempt to always be working"
  - Creating `feature` branches for changes. These are short-lived branches and eventually get merged into `staging`. If they successfully get merged into staging without breaking things, they can be merged into master (by only myself or Alison)
