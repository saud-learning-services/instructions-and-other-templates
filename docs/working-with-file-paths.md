# Working with file paths

A helpful [article](https://medium.com/@ageitgey/python-3-quick-tip-the-easy-way-to-deal-with-file-paths-on-windows-mac-and-linux-11a072b58d5f) on the subject. The following is essentially just a more suscint version of the contents of this article.

## Describing the problem

Microsoft Windows uses a backslash character between folder names while almost every other operating sysetem uses a forward slash

```
# Windows filenames:
C:\somefolder\somefile.txt

# Mac, Linux and most others:
/some_folder/somefile.txt
```

Writing out filepaths like the following may work on Mac and Linux based sysems, but will cause errors on windows.

```python
data_folder = "source_data/text_files/"

file_to_open = data_folder + "raw_data.txt"

f = open(file_to_open)

print(f.read())
```

## The solution: Python3's [pathlib](https://docs.python.org/3/library/pathlib.html) module

Specifiying filepaths using the following technique will work across all operating systems

```python
from pathlib import Path

data_folder = Path("source_data/text_files/")

# Note that you can add to filepaths simply by using the / character
file_to_open = data_folder / "raw_data.txt"

f = open(file_to_open)

print(f.read())
```
