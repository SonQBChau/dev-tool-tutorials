1. Install Mingw-w64 via the SourceForge website. Click [Mingw-w64](https://sourceforge.net/projects/mingw-w64/files/Toolchains%20targetting%20Win32/Personal%20Builds/mingw-builds/installer/mingw-w64-install.exe/download) to download the Windows Mingw-w64 installer.
	 - Run the installer. 
	 - For  **Architecture**  select  **x86_64**  and then select  **Next**. 
     ![minGW](https://raw.githubusercontent.com/misc-sonchau/dev-tool-tutorials/main/images/minGW_x86.jpg)
	 - On the Installation Folder page, use the default installation folder. Copy the location to notepad as you will need it later. 
     ![minGW](https://raw.githubusercontent.com/misc-sonchau/dev-tool-tutorials/main/images/minGW_location.jpg)
	  - Select  **Next**  to start the installation.


2. Add the path to your Mingw-w64 bin folder to the Windows PATH environment variable by using the following steps:
    - In the Windows search bar, type 'settings' to open your Windows Settings.
    - Search for **Edit environment variables for your account**.
      ![settings](https://raw.githubusercontent.com/misc-sonchau/dev-tool-tutorials/main/images/windows_settings.jpg)
    - Choose the `Path` variable and then select **Edit**.
     ![settings](https://raw.githubusercontent.com/misc-sonchau/dev-tool-tutorials/main/images/windows_env.jpg)
    - Select **New** and add the Mingw-w64 destination folder path to the system path. The exact path depends on which version of Mingw-w64 you have installed and where you installed it. If you used the settings above to install Mingw-w64, then add this to the path: `C:\Program Files\mingw-w64\x86_64-8.1.0-posix-seh-rt_v6-rev0\mingw64\bin`.
    - Select **OK** to save the updated PATH. You will need to reopen any console windows for the new PATH location to be available.