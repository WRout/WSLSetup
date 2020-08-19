##WSL Setup
>https://www.windowscentral.com/install-windows-subsystem-linux-windows-10

1. Open Settings
2. Click on "Apps"
3. On the right hand side, click on "Programs and Features"
4. Click "Turn Windows features on or off" to the left hand side
5. Find and check the "Windows Subsystem for Linux" option
6. Click the "OK" button
7. Click the "Restart now" button

##Installing Linux distros using Microsoft Store:

1. Open Microsoft Store
2. Search for a Linux distribution you would like to install
(Recommended; Ubuntu, Kali)
3. Select the distro of Linux to install on your device
4. Click the "Get" or "Install" button
5. Click the "Launch" button
6. **Create a username for the Linux distro and press the enter key**
7. **Create a password for the Linux distro and press the enter key**
*(Step 6 & 7 are VERY important. These steps will be creating a user account
for the subsystem. Make sure you remember the password, since it will be
required for every sudo use)*
8. Repeat password and press the enter key to confirm

##Linux Subsystem Viewing:
>https://solarianprogrammer.com/2017/04/16/windows-susbsystem-for-linux-xfce-4/

1. Launch subsystem
2. Navigate to home directory by typing: "cd ~"
3. Open ".bashrc" file by typing: "nano .bashrc". Use arrow keys to locate
bottom of the ".bashrc" file. Type in (at the bottom): "export DISPLAY=:0.0".
Save the ".bashrc" file by typing: "CTRL+X", "Y", and hitting the enter key.
4. Download VcXSrv on main computer, (*https://sourceforge.net/projects/vcxsrv/*)
5. Locate VcXSrv install file, create shortcut for "xlaunch.exe"
6. Install xfce4 by typing: "sudo apt install xfce4"
(If xfce4 fails to install, type: "sudo apt-get update")
7. Close and re-open subsystem window
8. Open "xlaunch.exe"
(Following instructions are for xlaunch boot)
9. In Display settings, select "One large window"
10. Hit Next. In the Client Startup, select "Start no client"
11. Hit Next. In the Extra Settings, select "Disable access control"
12. Finish the boot process
13. Relocate subsystem window. Type: "xfce4-session"
14. XLaunch window should boot up with Xfce session
