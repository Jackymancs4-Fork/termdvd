# termdvd [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
A program that simulates the DVD video screensaver in the terminal.

Now even people without a display server can enjoy the thrill of watching the DVD icon hit the corner. Amazing!

# Compatability info
This program requires at least Python version 3.3. If you attempt to run this program on Python 3.2 or lower, it will not work. In a future release, I may get support for older Python 3 versions working. However, I have no plans for getting Python 2 support.

If you're using a Unix system (like Linux, macOS, BSD, etc.), the program should work just fine.

If you're using a Windows system, the program will only correctly work on Windows 10 or newer. This is because my program
makes heavy use of ANSI escape codes, which aren't supported on older versions of Windows. If you attempt to run this program
on one of those versions, then it will just display a bunch of jumbled text.

# Getting the application
Before downloading the program, make sure you have the correct version of Python on your machine. (see "compatibility info" above.)

To download the program, go to a command line and clone the repository using git:

`git clone https://github.com/MrCatFace8885/termdvd`

Alternatively, you can also click the green "clone or download" button, and then click "Download ZIP" if you're in a web browser.

To run the program, cd to the directory in the command line (if you used git to download it then just type `cd termdvd`), and then run the program. (type `./termdvd.py` on a Unix or Unix-like system, or `termdvd.py` on a Windows system.)

# Command line arguments
When no arguments are given to termdvd, the region where the DVD icon bounces around is set to 20 rows and 40 columns by default.
If you want the DVD screen to be a diffrent size, it can be changed by typing the row count and then the column count as command line arguments. For example:

`termdvd.py 30 60`

will make the DVD screen be 30 rows long and 60 columns wide.

If you only want to change the row count, you only need to issue one argument. For example:

`termdvd.py 30`

will set the screen to 30 rows, but keep the column count at 40. However, if you want to issue a custom column count, you will need to issue both arguments.

There's also a few optional arguments. They are:

```
-h (--help): Displays command syntax and these arguments and then exits.
-v (--version): Displays the program's version number and then exits.
-c (--no_color): Makes the DVD icon only colored white.
```
