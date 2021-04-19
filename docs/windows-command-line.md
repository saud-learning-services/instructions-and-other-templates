# Running scripts in the Windows command line

The windows command line, [cmd.exe](https://en.wikipedia.org/wiki/Cmd.exe), is the counterpart of [COMMAND.COM](https://en.wikipedia.org/wiki/COMMAND.COM) in [DOS](https://en.wikipedia.org/wiki/DOS) and [Windows 9X](https://en.wikipedia.org/wiki/Windows_9x) systems. It is analogous to the Unix shells used in Unix-like systems.

## Some important commands

- `cd` _change directory_
- `cd ..` _change to parent directory_
- `w:` _access another drive, type the drive name followed by ":" (in this case W)_
  ```
  1. C:\Users\MyUser>W:
  2. W:\>_
  ```
- `dir` _view the contents of a folder_
- `mkdir` _make a new folder_

Commands concerning conda environments or running python scripts work in the same way as unix-like systems.

```
C:\Users\MyUser>conda env create -f environment.yml    # create environment from environment.yml file in current working directory
C:\Users\MyUser>conda activate my-envirionment         # activate environment named my-environment
C:\Users\MyUser>python my_script.py                    # run my_script.py
```

## Recommendations

- I found that cmd doesn't like when you use emoji's and icons in your print statements 😔
- You need to use [colorama](https://pypi.org/project/colorama/) to work with [termcolor](https://pypi.org/project/termcolor/) ([READ](https://stackoverflow.com/questions/21858567/why-does-termcolor-output-control-characters-instead-of-colored-text-in-the-wind))

## Running scripts with Task Scheduler

The [Task Scheduler](https://en.wikipedia.org/wiki/Windows_Task_Scheduler) app on Windows systems provides the ability to schedule and launch computer programs or scripts at pre-defined times or at specifed intervals.

In order to use Task Scheduler to run our python scripts, we need a [batch file](https://en.wikipedia.org/wiki/Batch_file) or `.bat` file. In this file, we'll write instructions to setup our environment, run our script and print to the console.

For example

```
@echo off
echo Please wait...
echo ================
echo activating conda environment...
call C:\Users\MyUser\Anaconda3\Scripts\activate.bat module-progress         # i.e call path-to-env env-name
echo ================
echo running script...
python C:\Users\MyUser\Documents\saud-learning-services\project-name\my_script.py      # path to entrypoint
echo end
pause

```

In order to easily keep track of I'd save this file in the project root folder

Open task scheduler, **right-click** on a folder (or create a new one) on the left panel time to store your task. Select **Create Basic Task...**

<div align="center">
    <img src="../imgs/task-scheduler/1.png" alt="one" width="600">
</div>

Give your task a name and description, select next

Select the frequency you'd like the automation to run, select next

<div align="center">
    <img src="../imgs/task-scheduler/2.png" alt="two" width="400">
</div>

Adjust when the run is triggered

<div align="center">
    <img src="../imgs/task-scheduler/3.png" alt="three" width="400">
</div>

Select **Start a program**

<div align="center">
    <img src="../imgs/task-scheduler/4.png" alt="four" width="400">
</div>

Select **Browse..** and locate your `.bat` file

<div align="center">
    <img src="../imgs/task-scheduler/5.png" alt="five" width="400">
</div>

Review and select **Finish**

<div align="center">
    <img src="../imgs/task-scheduler/6.png" alt="six" width="400">
</div>

> ⚠️ Be mindful of storing credentials like tokens. For automation like this to work tokens will need to be active for long stretches of time, making it all the more important to store these somewhere secure.
