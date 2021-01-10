## Open Terminal in Mac
Choose one of the following methods:
- Cmd + Space to open Search bar and type in Terminal
- Click the Terminal icon in the Dock
- Double-click the Terminal icon in Applications> Utilities.

## Log on to a CSE machine from Mac

1. Open the Terminal and type `ssh euid@cse01.cse.unt.edu` (replace "euid" with *your* actually euid)

*The first time you start SFTP a message similar to this will appear, You will have to accept a certificate to complete the connection.*

*At the prompt, Are you sure you want to continue connecting (yes/no)?, type yes and press return.*

2. At the password prompt, type your password and press return. The sftp prompt will appear: sftp>



## Transfer files from a CSE machine to Mac
**Make sure exit the SSH firstly (close it) before transfer files by using SFTP. Otherwise you may lose your files.**

Start SFTP
1. Open the Terminal
2. At the Terminal prompt, type `sftp euid@cse01.cse.unt.edu`
3. At the password prompt, type your password and press <return>. The sftp prompt will appear: sftp>
<br>
##### Upload from the Mac to UNIX
At the sftp prompt, type, put filename return
<br>
##### Download from UNIX to the Mac
At the sftp prompt, type, get filename return
<br>
##### Quit SFTP
At the sftp prompt, type quit and press return
