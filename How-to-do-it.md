# How to do it?

## Git

### How to Download git and install it?

Visit this [git-scm](https://git-scm.com/downloads) website and click _Download for Windows_ button to download it.

:LiFileVideo: Check out this video _How to Install Git_ on your google drive directory **My Drive > Videos > How to do it?**

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

Open device manager select _HID Keyboard Device & HID-compliant mouse_ -> go to Properties then select Power Management tab and uncheck **Allow this device to wake the computer**

### How to open MS Store using Run?

```run title:"Windows Run"
ms-windows-store:updates
```

### How to clear cache and temp files in windows PC?

- [ ] Clear Cache and Temp Files 🔁 every month 🛫 2025-09-01

Step 1: Go to Local Disk (C:) > Windows > SoftwareDistribution > Download > <span style="color:rgb(255, 0, 0)">Inside Download Deleted All</span>
Step 2: Open Run > %temp% > <span style="color:rgb(255, 0, 0)">Inside temp Deleted All</span> / Another method to open this folder is going through User Name > AppData > Local > Temp > <span style="color:rgb(255, 0, 0)">...</span>
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

```py
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

> [!warning]
> Need python png image in 16x16 px

![[How to add python in windows 11 terminal profile.png]]

### How to check python installed packages with pip?

```bash
pip list
```

### How to run jupyter lab in windows terminal?

```bash
jupyter lab
```

## Database

### How to Install MySql on Windows 11?

First Go to this website -> [Microsoft Visual C++ Redistributable](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170) and download X64 Architecture file which ends like this vc_redist.x64.exe and Install it.

Then go to [MySql Webiste](https://dev.mysql.com/downloads/installer/) and download the installer (My system is 64 bit)

Then download the Windows (x86, 32-bit), MSI Installer with maximum MB (the second one)

Don't need to sign in just click download without sign in.

⚠ :LiNotebook: Don't Change Window Service Name - default is MYSQL80, Again do not change the name

:LiFileVideo: Check out this video _How to Install MySQL Note-Do NOT Change Win Service Name MYSQL80_ on your google drive directory **My Drive > Videos > How to do it?**

### How to Install PostgreSQL on Windows 11?

1. Go to [PostgreSQL download](https://www.postgresql.org/download/) page, select [OS](https://www.postgresql.org/download/windows/) (mine is Windows)
2. Then select [download the installer](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)
3. Then decide your version and architecture which your PC support when click the download icon a file like this _postgresql-17.x-x-windows-x64.exe_ will start downloading.
4. Install it (while installing set your root user password)

:LiFileVideo: Check out this video _How to Install PostgreSQL_ on your google drive directory **My Drive > Videos > How to do it?**

### How to run psql in terminal on windows 11 with docker container?

1. Run the container
2. Then execute this command `docker exec -it blog_db psql -U blog`

### How to Install Redis using docker?

1. Use this cmd to install the latest version of redis in your pc `$> docker pull redis`
2. Then you need to start the container with `$> docker run -it --rn --name redis -p 6379:6379 redis`
3. While the server is running, open the another terminal window and to start the redis client use this cmd `$> docker exec -it redis sh` to initialize
4. Then you will see the **#** hash symbol, start the redis client with `# redis-cli` then you will see the redis client shell prompt, like this `127.0.0.1:6379>`, you can start executing the redis commands directly from the shell.
5. user `exit` to quit the redis client terminal.

## JavaScript

### How to Install NodeJS on Windows 11 PC?

Check out this article [Install NodeJS on Windows](https://learn.microsoft.com/en-us/windows/dev-environment/javascript/nodejs-on-windows)

First Download <abbr title="Node Version Manager">NVM</abbr> from [NVM For Windows](https://github.com/coreybutler/nvm-windows#installation--upgrades) click Download Now!

![[NVM Select Download Now.png]]

then select nvm-setup.exe to download and then install it.

After that open PowerShell as Admin, and check the available version with this command `nvm list available` and choose the LTS version you needed, then install the node js with this command `nvm install <version>` (replacing `<version>` with the **number**, ie: `nvm install 12.14.0`). To confirm the download use this command to check the installed version number with this command `nvm ls` and check the 9th, 10th and 11th points from the above attached article.

:LiFileVideo: Check out this video _How to Install NodeJS_ on your google drive directory **My Drive > Videos > How to do it?**

### How to run JavaScript file in terminal using node?

Just like python file, you go the file location in command prompt and type below command

```bash title:"run js"
node filename.js
```

## Linux - WSL

### How to Install WSL2 on Windows 11?

## Docker

### How to Install Docker on Windows 11?

Visit this [Docker](https://www.docker.com/products/docker-desktop/) official website and hover _Download Docker Desktop_ button and select the operating system to download it.

:LiFileVideo: Check out this video _How to Install Docker_ on your google drive directory **My Drive > Videos > How to do it?**

## Excel

### Some Excel Formula

- `=IF(G2="D",4,IF(G2="C",3,IF(G2="B",2,IF(G2="A",1))))`
- `=IF(G2="09:00 A.M.-10:30 A.M.",1,IF(G2="01:30 P.M.-03:00 P.M.",2))`
- `=VLOOKUP(A2,Sheet3!A:B,2,0)`
- `=TRIM(SUBSTITUTE(A2,CHAR(160),))`
- `=text(vlookup(a2, range, 2,0),"dd/mm/yyyy")`
- `=concat(range&"$$") then press f9`
- `=offset($x$3,1,match($b2,$x$3:$ac$3,0)-1,79,1)`
- `=TEXTJOIN("##",TRUE,IF(A2:A189=I2,B2:B189,"")`

## Visual Studio Code

### How to turn off copilot suggestions in VS Code?

```json
{
"github.copilot.editor.enableAutoCompletions": false,
}
```

Above settings didn't available at all, so I just disable the copilot extension.

### Helpful Shortcuts

Cursor preview - <img width="15" height="15" src="https://img.icons8.com/ios/50/text-cursor.png" alt="text-cursor"/>

**For Delete**

1. Delete a letter - use `Backspace` to delete a letter from left side of the cursor & use `Delete` to delete a letter from right side of the cursor.
2. Delete a word - use `Ctrl + Backspace` to delete a word from left side of the cursor & use `Ctrl + Delete` to delete a word from right side of the cursor.
3. In VS code to delete a current line - use `shift + Delete` (that is blinking cursor - entire line).

**For Fold & Unfold**

1. Fold ( `Ctrl+Shift+[` ) folds the innermost uncollapsed region at the cursor.
2. Unfold ( `Ctrl+Shift+]` ) unfolds the collapsed region at the cursor.
3. Toggle Fold ( `Ctrl+K Ctrl+L` ) folds or unfolds the region at the cursor.
4. Fold Recursively ( `Ctrl+K Ctrl+[` ) folds the innermost uncollapsed region at the cursor and all regions inside that region.
5. Unfold Recursively ( `Ctrl+K Ctrl+]` ) unfolds the region at the cursor and all regions inside that region.
6. Fold All ( `Ctrl+K Ctrl+0` ) folds all regions in the editor.
7. Unfold All ( `Ctrl+K Ctrl+J` ) unfolds all regions in the editor.
8. Fold Level X ( `Ctrl+K Ctrl+2 for level 2` ) folds all regions of level X, except the region at the current cursor position.
9. Fold All Block Comments ( `Ctrl+K Ctrl+/` ) folds all regions that start with a block comment token.

**For Remove Hyperlink**

`Ctrl + Shift (+ Fn) + F9`