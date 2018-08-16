# PyLogger for Windows
[![Python](https://img.shields.io/badge/Python-2.7-blue.svg)](https://python.org/)
[![Windows](https://img.shields.io/badge/Works%20with-Windows%20XP%20and%20above-blue.svg)](https://www.python.org/downloads/windows/)

PyLogger is a simple, easy-to-use keylogging program for Windows.

## Installing dependencies
To run the program, you will need the following:

- Python 2.7: https://www.python.org/

- pyHook Module: https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyhook

- pythoncom Module: https://sourceforge.net/projects/pywin32/

>*The pyHook module currently has to be installed via a wheel file. Download it from the link above.*

If the program can't import the required modules, it will warn you with an error message.


## Using the program (CLI)
- #### Command Usage:
  - keylogger-2.7.py **< mode >** *[optional:startup]*
- #### Modes:
  - **local:** store the logs in a file *(by default this is set to `key.log`, but can be changed)*
  - **remote:** send the logs to a Google Form. You must specify the Form URL and Field Name in the script.
  - **email:** send the logs to an email. You must specify the SERVER, **PORT, USERNAME, PASSWORD,** and who to send the email to.)
  - **ftp:** upload logs file to an FTP account. You must specify the **SERVER, USERNAME, PASSWORD, SSL OPTION, and OUTPUT DIRECTORY.**)
- #### Optional:
  - **startup:** This will add the keylogger to Windows startup.

## Compiling
Once you have set the program up, you can [compile your program into an EXE file.](https://www.youtube.com/watch?v=lOIJIk_maO4)

This is where the `startdefaultmode` variable comes in. Change this variable to `True` to start the program without asking for arguments. This is good for hiding the keylogger, or saving time.

`defaultmode` determines what mode we start in when `startdeaultmode` is True. You can set this to any of the above modes.
