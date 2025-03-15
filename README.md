# clash-for-ubuntu

A repo that set up `Clash For Windows` as an application on Ubuntu >=22.04

## **Currently I am using [Sing-Box](https://github.com/GUI-for-Cores/GUI.for.SingBox), please visit the link if you are interested.**

## Download

We can download the linux version of CFW from [Clash.for.Windows-0.20.39-x64-linux.tar.gz](https://clashforwindows.org/clash-for-windows-download/)

## Modify the Script

1. There's a `cfw_launcher.sh` in this repo, which executes the executable file `cfw` in `.tar.gz` that we just downloaded, please modify the path in this script to fit your case.

2. Make the script executable:

    ```bash
    chmod +x cfw_launcher.sh
    ```

## Modify the Desktop Entry File

1. There's a `cfw.desktop` in this repo as well. Replace `/path/to/cfw_launcher.sh` with the actual path to your script. You need to specify an icon by replacing `/path/to/icon.png` with the path to an image file (e.g., [PNG](https://clashforwindows.org/wp-content/uploads/2022/09/1663501512-favicon.png)) for your application icon.

2. Make the file executable:

    ```bash
    chmod +x cfw.desktop
    ```

3. Move the file to make it accessible to your desktop environment:

    ```bash
    mv cfw.desktop ~/.local/share/applications/
    ```

4. Refresh the Desktop Environment: You may need to log out and log back in or restart your desktop environment to see the new application launcher.

## Config Your CFW as usual

Now, you should be able to find your CFW Launcher in the application menu or search for it using the specified name. Clicking on the launcher should execute your cfw_launcher.sh script. Then you can config your CFW as usual.
