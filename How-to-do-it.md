## Table of Content

- [Style Block](#style-block)
- [How to do it?](#how-to-do-it)
    - [How to login and setup in git?](#how-to-login-and-setup-in-git)
    - [How to add date \& time in command prompt or terminal in windows PC?](#how-to-add-date--time-in-command-prompt-or-terminal-in-windows-pc)
    - [How to download PC Battery Report in windows 10/11](#how-to-download-pc-battery-report-in-windows-1011)
    - [How to turn off external devices wake up PC?](#how-to-turn-off-external-devices-wake-up-pc)
    - [How to import modules from different folders in python?](#how-to-import-modules-from-different-folders-in-python)
    - [How to open MS Store using Run?](#how-to-open-ms-store-using-run)
    - [How to clear cache and temp files in windows PC?](#how-to-clear-cache-and-temp-files-in-windows-pc)
    - [How to install MySql in windows 11?](#how-to-install-mysql-in-windows-11)
    - [How to create and activate virtual environment in python?](#how-to-create-and-activate-virtual-environment-in-python)
    - [How to Install NodeJS on Windows 11 PC?](#how-to-install-nodejs-on-windows-11-pc)
    - [How to connect WiFi FTP Server in Windows PC?](#how-to-connect-wifi-ftp-server-in-windows-pc)
    - [How to fetch all files name from a folder and store it as desire file format (ex. csv, xlsx, txt)](#how-to-fetch-all-files-name-from-a-folder-and-store-it-as-desire-file-format-ex-csv-xlsx-txt)
    - [How to create / delete folder and files using windows command prompt?](#how-to-create--delete-folder-and-files-using-windows-command-prompt)
    - [How to rename files bulk in a folder using windows command prompt?](#how-to-rename-files-bulk-in-a-folder-using-windows-command-prompt)
    - [How to uninstall pip package?](#how-to-uninstall-pip-package)
    - [How to Install PostgreSQL on Windows 11?](#how-to-install-postgresql-on-windows-11)
    - [How to Install WSL2 on Windows 11?](#how-to-install-wsl2-on-windows-11)
    - [How to Install Docker on Windows 11?](#how-to-install-docker-on-windows-11)
    - [How to run JavaScript file in terminal using node?](#how-to-run-javascript-file-in-terminal-using-node)
    - [How to add Python profile in Windows 11 Terminal?](#how-to-add-python-profile-in-windows-11-terminal)
    - [How to check python installed packages with pip?](#how-to-check-python-installed-packages-with-pip)
    - [What to do when blue screen error occur?](#what-to-do-when-blue-screen-error-occur)
    - [Some Excel Formula](#some-excel-formula)
- [Helpful Shortcuts](#helpful-shortcuts)
    - [Editor Shortcuts](#editor-shortcuts)
- [World of Open Source! (My favorite)](#world-of-open-source-my-favorite)
  - [Development \& Programming](#development--programming)
    - [Operating System](#operating-system)
    - [For Web Development](#for-web-development)
      - [Programming Languages](#programming-languages)
      - [Frameworks](#frameworks)
    - [Database Management System](#database-management-system)
      - [SQL](#sql)
      - [NoSQL](#nosql)
    - [Web Browser](#web-browser)
  - [Creativity and Graphic Design](#creativity-and-graphic-design)
      - [Photoshop \& Illustrator](#photoshop--illustrator)
      - [3D Modeling](#3d-modeling)
      - [Video Editing](#video-editing)
      - [Video Recording](#video-recording)
      - [Fonts](#fonts)
  - [Productivity](#productivity)
    - [Office Suites](#office-suites)

<br>

# Style Block

<style>
  red {color: Red}
  green {color: Green}
</style>

# How to do it?

### How to login and setup in git?

To add name
```git
git config --global user.name "your_name"
```
To add email
```git
git config --global user.email "your_email"
```
To verify

```git
git config --list
```

### How to add date & time in command prompt or terminal in windows PC?

This 3 arrows is called prompt >>> in python or c:\Users\name> in windows terminal. For more information type **prompt /?**.

Once you decided the format we have to save it in registry editor. The format I chose is Date & Time | Path >

### How to download PC Battery Report in windows 10/11

Open the cmd prompt as admin and type this command

```command line interface
powercfg /batteryreport /output "D:\battery_report.html"
```

### How to turn off external devices wake up PC?

open device manager select _HID Keyboard Device & HID-compliant mouse_ go to Properties then select Power Management tab and uncheck **Allow this device to wake the computer**

### How to import modules from different folders in python?

Question: I have _person.py_ script inside the **JAN2024** folder and I have another folder called **FEB2024** which have _employee.py_ script I need to import _person.py_ script to use it as a base class of _employee.py_, how to import it in python?<br>
Note: both **JAN2024** and **FEB2024** folder are inside **Python** folder

Answer: The simplest way to add the file path in sys path for python to check the folder. In windows PC don't forget to add **\\\\** between folder hierarchy.

```python
import sys
sys.path.append('d:\\Github\\Python\\JAN2024')
from person import Person
```

### How to open MS Store using Run?

```command line interface
ms-windows-store:updates
```

### How to clear cache and temp files in windows PC?

Recursive Task for every month first day or week ҉

Step 1: Go to Local Disk (C:) > Windows > SoftwareDistribution > Download > <red>Inside Download Deleted All</red> <br>
Step 2: Open Run > %temp% > <red>Inside temp Deleted All</red> <br> Another method to open this folder is going through User Name > AppData > Local > Temp > <red>...</red> <br>
Step 3: Open Run > temp > click continue > <red>Inside temp Deleted All</red> <br> Another method to open this folder is going through This PC > Local Disk (C:) > Windows > Temp > <red>...</red> <br>
Step 4: Open Run > prefetch > click continue > <red>Inside prefetch Deleted All</red> <br> Another method to open this folder is going through This PC > Local Disk (C:) > Windows > Prefetch > <red>...</red>  <br>
Step 5: To reset windows store > Open Run > wsreset > <red>This will clear the cache for windows store</red> <br>
Step 6: Go to Edge > <red>Clear browser cache and cookies</red> <br>
Step 7: click windows key + s > type clear location history > <red>click clear</red> <br>
Step 8: Go to CMD as administrator > <red>type ```ipconfig /flushDNS```</red> <br>
Step 9: Advance --- Disk Cleanup > Select Disk > recommended to watch the video in youtube for reference

### How to install MySql in windows 11?

First Go to this website -> [Microsoft Visual C++ Redistributable](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170) and download X64 Architecture file which ends like this vc_redist.x64.exe and Install it.

Then go to [MySql Webiste](https://dev.mysql.com/downloads/installer/) and download the installer (My system is 64 bit)

Then download the Windows (x86, 32-bit), MSI Installer with maximum MB (the second one)

Don't need to sign in just click download without sign in.

**Important Note:** Don't Change Window Service Name - default is MYSQL80, Again do not change the name

### How to create and activate virtual environment in python?

Decide your working location / directory where new virtual environment folder lives in your PC.

- To Create
```command line interface
$> py -m venv helium
```
Above command created a new folder named as 'helium' in the selected location.

- To Activate (for windows PC)
```command line interface
$> helium\Scripts\activate
```
From the above command an virtual environment is activated and you can notice it before your terminal prompt.

- Preview
```cmd
(helium) $>
```

To deactivate just type **deactivate**

- To deactivate

**Before**
```cmd
(helium) $> deactivate
```

**after**
```cmd
$>
```

### How to Install NodeJS on Windows 11 PC?

Check out this article [Install NodeJS on Windows](https://learn.microsoft.com/en-us/windows/dev-environment/javascript/nodejs-on-windows)

First Download <abbr title="Node Version Manager">NVM</abbr> from [NVM For Windows](https://github.com/coreybutler/nvm-windows#installation--upgrades) click Download Now! refer the below image,

![Image](https://github.com/Aravindray/Notes/blob/main/assets/NVM%20Select%20Download%20Now.png)

then select nvm-setup.exe to download and then install it.

After that open PowerShell as Admin, and check the available version with this command ```nvm list available``` and choose the LTS version you needed, then install the node js with this command ```nvm install <version>``` (replacing ```<version>``` with the **number**, ie: ```nvm install 12.14.0```). To confirm the download use this command to check the installed version number with this command ```nvm ls``` and check the 9th, 10th and 11th points from the above attached article.

**author_note:** You can view the google drive video about how to install NodeJS

### How to connect WiFi FTP Server in Windows PC?

1. Open File Explorer (with Windows + E)
2. Right-Click the program and select **Add a network location**
3. New setup wizard will appear click and select **Choose a custom network location**
4. Then enter the FTP server URL ```ftp://XXX.XXX.XX.X:XXXX``` and don't forgot to **turn off "Log on Anonymously**
5. Then enter the user name, and then enter the display name.
6. A new window asks userid and password enter the password and save the password for future connections.
7. Now ready to use.

**Note:** Now a days I am using _Google's QuickShare_

### How to fetch all files name from a folder and store it as desire file format (ex. csv, xlsx, txt)

**By Using cmd prompt**
1. Go to the folder where you want to file names from
2. Open the cmd prompt from that folder
3. Then type the below command
```cmd
dir /b > fileName.txt
```

### How to create / delete folder and files using windows command prompt?

**Create Folder**

To create a folder go to the desire folder and type this cmd:

```cmd
> mkdir folderName
> mkdir "folder name" # Use quoting if space separated name
> mkdir folder name # If you did not use the quotation it will create two different folders
```

**Create File**

Windows cmd prompt support 3 different way to create a file within a folder

1. Using *echo* cmd - We have enter the content while creating the file.

```cmd
> echo Text goes here > filename.extension
```

2. Using *copy con*  cmd - Unlike echo, we only need to enter the content after we create the file.

```cmd
> copy con filename.extension
```

Note: To save the file press ctrl + z or to quit hit ctrl + c within the prompt section.

3. Using *notepad* cmd - This opens the dialog box click "Yes" and enter the content within in the notepad application and save the file within the application.

```cmd
> notepad filename.extension
```

**NOTE:** To view the content from a file use this cmd:

```cmd
> type filename.extension
```

**Delete Folder**

To delete the folder go to the desire folder parent directory and enter the below cmd:

```cmd
> rmdir folderName
```

**Delete File**

To delete a file go to desire file location and enter the below cmd:

```cmd
del filename.extension
```

### How to rename files bulk in a folder using windows command prompt?

**Rename Files**

For example if an old file name is "sorry.mp3" and you want to rename it as "apology.mp3" using command prompt check below cmd

```cmd
> rename "sorry.mp3" "apology.mp3"
or
> ren "sorry.mp3" "apology.mp3"
```

### How to uninstall pip package?

```cmd
py -m pip uninstall <package_name>
```

### How to Install PostgreSQL on Windows 11?

1. Go to [PostgreSQL download](https://www.postgresql.org/download/) page, select [OS](https://www.postgresql.org/download/windows/) (mine is Windows)
2. Then select [download the installer](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)
3. Then decide your version and architecture which your PC support when click the download icon a file like this _postgresql-17.2-3-windows-x64.exe_ will start downloading.
4. Install it (while installing set your root user password)

**author_note:** You can view the google drive video about how to install PostgreSQL

### How to Install WSL2 on Windows 11?

### How to Install Docker on Windows 11?

### How to run JavaScript file in terminal using node?

Just like python file, you go the file location in command prompt and type below command

```cmd
$> node filename.js
```

### How to add Python profile in Windows 11 Terminal?

It is just simple, check out this below image, __Note:__ Need python png image in 16x16 px

![Image](https://github.com/Aravindray/Notes/blob/main/assets/How%20to%20add%20python%20in%20windows%2011%20terminal%20profile.png)

### How to check python installed packages with pip?

Just type below command in terminal

```py
$> pip list
```

### What to do when blue screen error occur?

**author_notes:** In Jan 17 or 18 2025, I faced 0xc000021a blue screen error, but SSD hard drive also crash.

1. Steps yet to add!

### Some Excel Formula

- =IF(G2="D",4,IF(G2="C",3,IF(G2="B",2,IF(G2="A",1))))
- =IF(G2="09:00 A.M.-10:30 A.M.",1,IF(G2="01:30 P.M.-03:00 P.M.",2))
- =VLOOKUP(A2,Sheet3!A:B,2,0)
- =TRIM(SUBSTITUTE(A2,CHAR(160),))
- =text(vlookup(a2, range, 2,0),"dd/mm/yyyy")
- =concat(range&"$$") then press f9
- =offset($x$3,1,match($b2,$x$3:$ac$3,0)-1,79,1)
- =TEXTJOIN("##",TRUE,IF(A2:A189=I2,B2:B189,"")

# Helpful Shortcuts

### Editor Shortcuts

Cursor preview - <img width="15" height="15" src="https://img.icons8.com/ios/50/text-cursor.png" alt="text-cursor"/>

**For Delete**

1. Delete a letter - use ```Backspace``` to delete a letter from left side of the cursor & use ```Delete``` to delete a letter from right side of the cursor.
2. Delete a word - use ```Ctrl + Backspace``` to delete a word from left side of the cursor & use ```Ctrl + Delete``` to delete a word from right side of the cursor.
3. In VS code to delete a current line - use ```shift + Delete``` (that is blinking cursor - entire line).

**For Fold & Unfold**

1. Fold (Ctrl+Shift+[) folds the innermost uncollapsed region at the cursor.
2. Unfold (Ctrl+Shift+]) unfolds the collapsed region at the cursor.
3. Toggle Fold (Ctrl+K Ctrl+L) folds or unfolds the region at the cursor.
4. Fold Recursively (Ctrl+K Ctrl+[) folds the innermost uncollapsed region at the cursor and all regions inside that region.
5. Unfold Recursively (Ctrl+K Ctrl+]) unfolds the region at the cursor and all regions inside that region.
6. Fold All (Ctrl+K Ctrl+0) folds all regions in the editor.
7. Unfold All (Ctrl+K Ctrl+J) unfolds all regions in the editor.
8. Fold Level X (Ctrl+K Ctrl+2 for level 2) folds all regions of level X, except the region at the current cursor position.
9. Fold All Block Comments (Ctrl+K Ctrl+/) folds all regions that start with a block comment token.

**For Remove Hyperlink**

```Ctrl + Shift (+ Fn) + F9```

# World of Open Source! (My favorite)

## Development & Programming

### Operating System

- Linux

### For Web Development

#### Programming Languages

- Python
- JavaScript
- HTML
- CSS
- GIT

#### Frameworks

- React
- Django

### Database Management System

#### SQL

- MySQL
- PostgreSQL

#### NoSQL

- MongoDB

### Web Browser

- Mozilla

## Creativity and Graphic Design

#### Photoshop & Illustrator

- GIMP
- Inkscape
- Krita (for digital painting)
- Penpot
- Figma (Freemium)

#### 3D Modeling

- Blender

#### Video Editing

- ?

#### Video Recording

- OBS Studio

#### Fonts

- [Fontget](https://www.fontget.com/)
- [DaFont](https://www.dafont.com/)
- [Google Fonts](https://fonts.google.com/)
- [Font Bundles](https://fontbundles.net/free-fonts)
- [Font squirrel](https://www.fontsquirrel.com/)
- [1001 Free Fonts](https://www.1001freefonts.com/)

## Productivity

### Office Suites

- LibreOffice
- WPS (Freemium)
