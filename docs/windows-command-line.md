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
