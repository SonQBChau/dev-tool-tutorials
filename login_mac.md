## Open Terminal in Mac
Choose one of the following methods:
- Cmd + Space to open Search bar and type in Terminal
- Click the Terminal icon in the Dock
- Double-click the Terminal icon in Applications> Utilities.

## Log on to a CSE machine from Mac

1. Open the Terminal and type `ssh euid@cse01.cse.unt.edu` (replace "euid" with *your* euid)
2. At the password prompt, type your password and press return.

*The first time you login a message will appear, you will have to accept a certificate to complete the connection.*

  ![terminal](https://raw.githubusercontent.com/misc-sonchau/dev-tool-tutorials/main/images/mac_terminal.png)



## Transfer files from a CSE machine to Mac
**Make sure exit the SSH firstly (type `exit`) before transfer files by using SFTP. Otherwise you may lose your files.**

1. Open the Terminal
2. At the Terminal prompt, type `sftp euid@cse01.cse.unt.edu`
3. At the password prompt, type your password and press <return>. The sftp prompt will appear: sftp>

![terminal](https://raw.githubusercontent.com/misc-sonchau/dev-tool-tutorials/main/images/mac_sftp.png)

**Note**: *To find out your working directory, you can use the command `pwd`*

*If prompt for access, click Ok*

##### Upload files
The command to upload files to a remote server, is:

`put path_to_local_file`

For example, this command will put the file called "hello.cpp" from **Downloads directory**, into the **working directory** in the remote server

`put /Users/sonchau/Downloads/hello.cpp`
<br>

##### Download from UNIX to the Mac
The command to download files off of a remote server, is:

`get path_to_remote_file path_to_local_file`

For example, this command will download the file called "hello.cpp" from the **Lab01 directory** on the remote server into **Downloads directory** on my Mac.

`get Lab01/hello.cpp /Users/sonchau/Downloads/`
<br>
##### Quit SFTP
At the sftp prompt, type exit and press return
