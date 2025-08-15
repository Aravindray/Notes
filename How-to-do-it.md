# How to do it?

## Git

### How to Download git and install it?

Visit this [git-scm](https://git-scm.com/downloads) website and click _Download for Windows_ button to download it.

:LiNotebookText: Check out this video _How to Install Git_ on your google drive directory **My Drive > Videos > How to do it?**

### How to login and setup in git?

```git title:"to add name"
git config --global user.name "your_name"
```

```git title:"to add email"
git config --global user.email "your_email"
```

```git title:"to verify"
git config --list
```

## Windows

### How to add date & time in command prompt or terminal in windows PC?

This 3 arrows is called prompt *>>>* in python or c:\Users\name> in windows terminal. For more information type `prompt /?`

Once you decided the format we have to save it in registry editor. The format I chose is **Date & Time | Path >**

### How to download PC Battery Report in windows 11

Open the cmd prompt as admin and type this command

```bash
powercfg /batteryreport /output "D:\battery_report.html"
```

### How to turn off external devices wake up PC?

open device manager select _HID Keyboard Device & HID-compliant mouse_ -> go to Properties then select Power Management tab and uncheck **Allow this device to wake the computer**

### How to open MS Store using Run?

```run title:"Windows Run"
ms-windows-store:updates
```

### How to clear cache and temp files in windows PC?

- [ ] Clear Cache and Temp Files 🔁 every month 🛫 2025-09-01

Step 1: Go to Local Disk (C:) > Windows > SoftwareDistribution > Download > <span style="color:rgb(255, 0, 0)">Inside Download Deleted All</span>
Step 2: Open Run > %temp% > <red>Inside temp Deleted All</red> / Another method to open this folder is going through User Name > AppData > Local > Temp > <span style="color:rgb(255, 0, 0)">...</span>
Step 3: Open Run > temp > click continue > <span style="color:rgb(255, 0, 0)">Inside temp Deleted All</span> / Another method to open this folder is going through This PC > Local Disk (C:) > Windows > Temp > <span style="color:rgb(255, 0, 0)">...</span>
Step 4: Open Run > prefetch > click continue > <span style="color:rgb(255, 0, 0)">Inside prefetch Deleted All</span> / Another method to open this folder is going through This PC > Local Disk (C:) > Windows > Prefetch > <span style="color:rgb(255, 0, 0)">...</span>
Step 5: To reset windows store > Open Run > wsreset > <span style="color:rgb(255, 0, 0)">This will clear the cache for windows store</span>
Step 6: Go to Edge > <span style="color:rgb(255, 0, 0)">Clear browser cache and cookies</span>
Step 7: click windows key + s > type clear location history > <span style="color:rgb(255, 0, 0)">click clear</span>
Step 8: Go to CMD as administrator > type `ipconfig /flushDNS`
Step 9: Advance --- Disk Cleanup > Select Disk ><span style="color:rgb(255, 192, 0)"> recommended to watch the video in youtube for reference</span>

### How to connect WiFi FTP Server in Windows PC?

1. Open File Explorer (with Windows + E)
2. Right-Click the program and select **Add a network location**
3. New setup wizard will appear click and select **Choose a custom network location**
4. Then enter the FTP server URL ```ftp://XXX.XXX.XX.X:XXXX``` and don't forgot to **turn off "Log on Anonymously**
5. Then enter the user name, and then enter the display name.
6. A new window asks userid and password enter the password and save the password for future connections.
7. Now ready to use.

:LiNotebook: Now a days I am using _Google's QuickShare_

### How to fetch all files name from a folder and store it as desire file format (ex. csv, xlsx, txt)

1. Go to the folder where you want to file names from
2. Open the cmd prompt from that folder

```bash title:"3. execute this command"
dir /b > fileName.txt
```

### How to create / delete folder and files using windows command prompt?

**Create Folder**

To create a folder go to the desire folder and type this cmd:

```bash title:"create folder"
mkdir folderName
mkdir "folder name" # Use quoting if space separated name
mkdir folder name # If you did not use the quotation it will create two different folders
```

**Create File**

Windows cmd prompt support 3 different way to create a file within a folder

```bash title:"Using echo cmd - We have to enter the content while creating the file"
echo Text goes here > filename.extension
```

```bash title:"Using copy con cmd - Unlike echo, we only need to enter the content after we create the file"
copy con filename.extension
```

:LiNotebook: To <span style="color:rgb(0, 176, 80)">save</span> the file press <span style="color:rgb(0, 176, 80)">ctrl + z</span> or to quit hit <span style="color:rgb(0, 176, 80)">ctrl + c</span> within the prompt section.

```bash title:"Using notepad cmd - This opens the dialog box click "Yes" and enter the content within in the notepad application and save the file within the application"
notepad filename.extension
```

```bash title:"To view the content from a file use this cmd"
type filename.extension
```

**Delete Folder**

.
└── parentFolder/
    └── childFolder/

To delete a folder go to the desire folder parent directory (In this case, go to parentFolder) and enter the below cmd

```bash title:"delete folder"
rmdir childFolder
```

**Delete File**

To delete a file go to desire file location and enter the below cmd

```bash title:"delete file"
del filename.extension
```

### How to rename files bulk in a folder using windows command prompt?

**Rename Files**

For example if an old file name is "sorry.mp3" and you want to rename it as "apology.mp3" using command prompt check below cmd

```bash title:"file rename"
rename "sorry.mp3" "apology.mp3" #or
ren "sorry.mp3" "apology.mp3"
```

### What to do when blue screen error occur?

:LiNotebook: In Jan 17 2025, I faced 0xc000021a blue screen error, but SSD hard drive also crash.

1. Steps yet to add!

## Python

:LiNotebook: For more in-depth notes check out this [Python repository](https://github.com/Aravindray/Python)

### How to import modules from different folders in python?

<span style="color:rgb(255, 0, 0)">Question:</span> I have _person.py_ script inside the **JAN2024** folder and I have another folder called **FEB2024** which have _employee.py_ script I need to import _person.py_ script to use it as a base class of _employee.py_, how to import it in python?
:LiNotebook: both **JAN2024** and **FEB2024** folder are inside **Python** folder

<span style="color:rgb(0, 176, 80)">Answer:</span> The simplest way to add the file path in sys path for python to check the folder. In windows PC don't forget to add \\\\ between folder hierarchy.

```python
import sys
sys.path.append('d:\\Github\\Python\\JAN2024')
from person import Person
```

### How to create and activate virtual environment in python?

Decide your working location / directory where new virtual environment folder lives in your PC.

```bash title:"To create"
py -m venv helium
```

Above command created a new folder named as 'helium' in the selected location.

```bash title:"to activate (for windows pc)"
helium\Scripts\activate
```

From the above command an virtual environment is activated and you can notice it before your terminal prompt.

```bash title:"an env name will display before the prompt"
(helium) $>
```

To deactivate just type **deactivate**

```bash title:"to deactivate"
(helium) $> deactivate
```

```bash title:"after deactive"
$>
```

### How to uninstall pip package?

```bash title:"To uninstall pip package"
py -m pip uninstall <package_name>
```

### How to add Python profile in Windows 11 Terminal?

> [!tip]
> Need python png image in 16x16 px






