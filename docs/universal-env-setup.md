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

> 💡 The universal environment is called **sauder-canvas-api**

While each of our projects comes with thier own `environment.yml` file for setting a project-specific environment, we also offer a universal environment, named **sauder-canvas-api**, that can be used to run _any_ of our projects that work with Canvas.

If you setup your universal environment correctly, you can use and update only that environment instead of managing one independently for each project.

> ⚠️ Every project that works with the universal environment will say "**supports universal environment 🌎**" on its GitHub page

### Installation (sauder-canvas-api)

1. Clone [this](https://github.com/saud-learning-services/instructions-and-other-templates/tree/marko) project to your computer (Not sure how? Revisit [Managing Projects with Github](managing-projects-with-github.md))
2. In Anaconda Navigator, import the `universal-environment.yml` file in the `instructions-and-other-templates` folder (cloned from GitHub in Step 1)
3. You should now see a new environment called **sauder-canvas-api** in your environments list. Select the ▶ button, then **Open with Jupyter Notebook**. Your browser should open automatically.
4. In the browser, navigate to a project that supports the universal environment and select the jupyter notebook (.ipynb file)
   > 🧪 We recommend using the [setup-test](https://github.com/saud-learning-services/setup-test) project to check your universal environment is set up correctly
5. Select **Kernal** > **Restart & Run All**. The notebook should run without errors if everything was done correctly

[➡️ Next: Updating Environments](updating-environments.md)
