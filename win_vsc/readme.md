# C++ Dev Environment With VSCode & Windows

## Subject
Setting up a development environment in Windows can be difficult. Still, there
are advantages to setting up your own dev envrionment v. installing overbloated
IDEs. In this tutorial, we will discuss how to set up a general dev-environment
for C++ on Windows using Visual Studio Code. We will be using the G++ compiler.
As an added bonus, we will go over installing Git and managing your GitHub repo
through vscode.

## Requirements
The following is assumed about your environment:
* You are on a Windows machine compatible with VSCode, Git, and MinGW
* You are familiar with downloading files and navigating windows directories

## Install [VSCode](https://code.visualstudio.com/)
* When installing VSCode, I recommend checking the following boxes in addition to the default settings. This is OPTIONAL though.
    * Add "Open With Code" action to Windows Explorer file context menu
    * Add "Open With Code" action to Windows Explorer directory context menu
    * Add to PATH (requires shell restart)
* The first two options allow you to open VSCode by right clicking in a folder or file. The third option lets you open VSCode from command line using the command `code [folder_path]`.

## Install [MinGW-W64](https://sourceforge.net/projects/mingw-w64/files/)
MinGW is a package of GNU elements for developers on Windows. If that last
sentence didn't make sense, don't worry its not important. What *is* important
is that MinGW comes with the option to install the G++ compiler. This is the
compiler of choice for many c++ developers and the one we will be using.
(Note: MinGW-W64 is a newer, actively maintained version of MinGW. This
tutorial was originally written for MinGW but MinGW-W64 has wider compatibility
and easier installation.)
* Under `Architecture` select `x86_64`
* NOTE which directory MinGW is installed to, it should contain a folder called `mingw64\bin\`
* Add MinGW's `bin\` folder to your `PATH`
* On Windows 10, PATH can be modified by following these steps
    1. In Search, search for and then select: Edit the system environment variables
    2. Click Environment Variables. In the section System Variables, find the PATH environment variable and select it. Click Edit. If the PATH environment variable does not exist, click New.
    3. In the Edit System Variable (or New System Variable) window, click "new" to add a new line to the PATH, then enter the path of MinGW's bin folder (C:\\\wherever\i\installed\it\mingw64\bin\\). Click OK. Close all remaining windows by clicking OK.

## Add extension "Code Runner" to VSCode
The Code Runner extension is a quick and convienent method of executing your
code inside of VSCode. It works for numerous languages, including c++. Of
course, you have MinGW installed and G++, so you don't *need* code runner. But
I highly recommend it.
* Click the `extensions` button on the left (it looks like 4 cubes with one drifting away)
* Search for and select Code Runner from the list
* Click `install` near the top of the page
* To run your code, right click while in the cpp file and select "Run Code"
* If you wish to compile multiple files and not simply execute the one you have open, [see this tutorial](https://github.com/jeremyglebe/dev_tool_tutorials/tree/master/vsc_mf)
* To configure additional settings, you'll need to go to your preferences 
    * Open your project's folder in Visual Studio Code
    * Click `file` in the top left
    * Select `preferences`, then `settings` in the drop down menu
        * This should open a new tab within vscode
    * In the search bar, type in the setting you wish to change
* You may want to configure these settings (optional):
    * `Code-runner: Run in Terminal` check this box to allow for interaction with your program. By default it goes to a non-interactive output which can block things like `cin` from getting keyboard input
    * `Code-runner: Save All Files Before Run` check this box to automatically make sure your files are saved when clicking `Run Code`
    * `Code-runner: File Directory As Cwd` check this box to automatically compile from the directory your file is in. This will prevent *a lot* of errors. Otherwise it might say that the file you're trying to compile can't be found (if you're in a folder with multiple projects inside)
