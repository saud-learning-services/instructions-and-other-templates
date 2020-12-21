<br />
<p align="center">
  <div align="center">
    <img src="../imgs/earth.png" alt="Logo" height="80">
  </div>

  <h3 align="center">Universal Environment Setup</h3>

  <p align="center">
  A single environment for all Sauder LS, Canvas API Projects
    <br />
  </p>
</p>

> ⚠️ Before reading on, ensure you've covered [computer setup](computer-setup.md), [github project management](github-project-management.md), and the [running instructions](running-instructions.md) docs - and have successfully worked through the [setup-test](https://github.com/saud-learning-services/setup-test) project.

While each of our projects comes with thier own `environment.yml` file for setting a project-specific environment, we also offer a **universal environment** that can be used to run _any_ of our projects that work with Canvas.

If you setup your unversal environment correctly, you can use and update that environment exclusively instead of managing one independently for each project.

1. To start, clone [this](https://github.com/saud-learning-services/instructions-and-other-templates/tree/marko) project to your computer (Not sure how? Revisit [Managing Projects with Github](managing-projects-with-github.md))
2. Create your environment from the `universal-environment.yml` file in the `instructions-and-other-templates` folder on your computer (cloned from GitHub in Step 1)
3. Test it out by running a Jupyter Notebook from the **universal-environment** from Anaconda Navigator (or Terminal), navigate to the project that supports it on your local computer (like [Canvas Peer Reviews](https://github.com/saud-learning-services/canvas-peer-reviews)) select **Kernal** > **Restart & Run All** - If everything went well, you should hopefully see the same output as before!
