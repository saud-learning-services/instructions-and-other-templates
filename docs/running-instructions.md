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

      > 🧪 If using the setup-test you'll want to navigate to the **setup-test** folder you cloned earlier

   1. Select **Import** and wait for installation to complete
      > 💡 This may take some time (upwards of 20 minutes)

   <div align="center">
      <img src="../imgs/sauder-ops-guide/anaconda-import-box.png" alt="Logo" width="600">
   </div>

Now that you have your environment setup (or are using the universal environment) go to the [next section](#running-the-script) to run the script.

## Running the Script

> ⚠️ Any of our tools that interact with the Canvas LMS will require you to generate a API access token. If the project you've chosen does not work with Canvas you can likely skip step 0. You can always refer to individual setup instructions on a project's GitHub page.

0. Get Canvas Token and Save it in the `.env`

   - Login to Canvas and select **Account** > **Settings** from the menu on the left
   - Under **Approved Integrations** select **New Access Token**
   - Name it something like `sauder-api` and set the expiration to the next day
     > ⚠️ For security reasons we don't encourage setting late expiration days (keep it to a day or two)
   - Copy the token it provides you, navigate to **the-project** folder on your computer and locate the `.env` file
     > ⚠️ `.env` files are hidden by most operating systems by default. If you don't see a file called `.env` in **the-project** folder you likely need to _reveal hidden files_ (Instructions for [Windows](https://support.microsoft.com/en-us/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) / [Mac](https://setapp.com/how-to/show-hidden-files-on-mac))
   - Open the `.env` file with any application that can edit text _(like TextEdit or Notepad)_ Paste the token you copied from Canvas into the `.env`file (There will be an indicator in the file as to exactly where you should paste it)
   - Save the `.env` file after you've pasted in your token

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

> 🧪 If using the setup-test you'll hopefully now see a printout like "Hi {your-name}". If you aren't seeing this, you'll hopefully see a printout giving you an indication of what is wrong and you can try and revisit that step in the docs. If your problem persists, contact someone on the Sauder LS, Canvas API team for support.

[➡️ Next: Universal Environment Setup](universal-env-setup.md)
