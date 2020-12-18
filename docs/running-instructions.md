<br />
<p align="center">
  <div align="center">
    <img src="../imgs/rocket.png" alt="Logo" height="80">
  </div>

  <h3 align="center">Running Scripts</h3>

  <p align="center">
  A step-by-step guide for running Sauder LS, Canvas API projects
    <br />
  </p>
</p>

> Before you read on, ensure your computer is [setup to run scripts](computer-setup.md) and you're familiar with [how to manage projects](github-project-management.md)

⚠️ All references to **the-project** should be the name of the script or project you are running.

## Where to start

- [I HAVE NOT run this script on this computer before](#configuring-the-run-environment)
- [I HAVE successfully run it on this computer before](#running-the-script)

## Configuring the Run Environment

🌎 The very first time you run a script, you'll want to start by getting your environment set up. Think of an enironment as a bunch of packages that get stitched together to form the complete script. We give you the pieces, but you need to put it together!

⚠️ If you've already setup a universal environment, you can skip to the [next section](#running-the-script) and run from your universal environment instead (but check to make sure the project supports it)

1. Make sure your computer is [setup](computer-setup.md) to run our projects

1. Clone the project you need (i.e. make a local copy) from our GitHub. See [here](github-project-management.md) or detailed instructions on getting and managing projects.

   > 💡 we recommend cloning all of our projects into a single location like `.../Documents/GitHub/Sauder-Learning-Services`

1. Open Anaconda Navigator:

   1. Open **Anaconda Navigator** application
   2. Click on **Environments** (left panel)
   3. Click on **Import** (bottom)

   <div align="center">
      <img src="../imgs/sauder-ops-guide/anaconda-env-import.png" alt="Logo" width="600">
   </div>

1. Import Environment

   1. A small window will open, navigate to the **the-project** folder on your computer and select: `environment.yml`

      > ⚠️ Do not manually enter the project name. This will automatically be filled in when you select the `environment.yml` and will be the same name as the project foler (i.e. the-project)

      > 💡 Note that every project has their own `environment.yml` file so it's important to make sure you select the right one. You can always ensure you have the right script by checking the name field after importing the yml file

   1. Select **Import** and wait for installation to complete
      > 💡 This may take some time (upwards of 20 minutes)

   <div align="center">
      <img src="../imgs/sauder-ops-guide/anaconda-import-box.png" alt="Logo" width="600">
   </div>

Now that you have your environment setup (or are using the universal environment) go to the [next section](#running-the-script) to run the script.

## Running the Script

1. Open **Anaconda Navigator**, select the ▶ button next to **the-project** to run your environment. Then select **Open with Jupyter Notebook**, and that will launch the browser.

   > ⚠️ If you're runing via the universal environment, click the ▶ button next to that instead (but make sure the project supports it)

   <div align="center">
      <img src="../imgs/sauder-ops-guide/anaconda-run.png" alt="Logo" width="600">
   </div>

2. In the browser, navigate to the **the-project** project folder and select **the-project.ipynb**

   > 💡 This will be located wherever you cloned it on your local computer - if you used our suggested location, all projects will be in a single folder so everything is easy to find

   <div align="center">
      <img src="../imgs/sauder-ops-guide/browser-select-notebook.png" alt="Logo" width="600">
   </div>

3. Read the information notebook! Once, you've done that select **Kernal** > **Restart & Run All** to run it

   <div align="center">
      <img src="../imgs/sauder-ops-guide/notebook-start.png" alt="Logo" width="600" >
   </div>

4. If everything was done correctly, the script should now run. Most of our projects involve some user inputs so the Jupyter Notebook will prompt and guide you from here
