# Securily Macro Recorder

<div align="center">
  <img src="src/assets/securily-logo.png" alt="Securily Logo">
  <p>
    **Efficient. Intuitive. Secure.**<br>
    Securily Macro Recorder is an advanced tool designed to help you automate the recording of application login steps and general application workflows that require security testing.<br>
    Perfect for pentesters and vulnerability scanners to streamline the process of testing web and software applications.
  </p>
  <a href="https://github.com/securily/SecurilyMacroRecorder/releases"><img alt="Download Securily Macro Recorder" src="https://img.shields.io/github/downloads/securily/SecurilyMacroRecord/total?label=Downloads"/></a>
</div>

# Overview
Securily Macro Recorder is a derivative work of the open-source <a href="https://github.com/LOUDO56/PyMacroRecord">PyMacroRecord project</a>, licensed under the GNU General Public License v3.0. This version has been rebranded and modified for security testing purposes, specifically to help customers record login steps and application workflows for vulnerability scanning and penetration testing.

# Features
- **Intuitive Interface**: Easy to use, no coding required.
- **Perfect for Security Testing**: Record login flows and application steps for pentesting.
- **Full Control**: Adjust playback speed, repeat actions, and set intervals between steps.
- **Save and Share**: Save your recordings and share them with security teams or pentesters.
- **Universal File Format**: Export recordings as `.json` files for cross-platform compatibility.
- **Custom Hotkeys**: Define custom hotkeys for recording and playback.
- **Cross-Platform**: Available for Windows, macOS, and Linux.

# How Does It Work?
1. **Start Recording**: Click the red button to start recording. Move your mouse, type on your keyboard—everything is captured.  
2. **Stop Recording**: Click the black square to stop.  
3. **Playback**: Play your recorded actions by pressing the green play button.  
4. **Stop Playback**: Stop the playback using the `F3` key.

# Use Case: Security Testing
The Securily Macro Recorder is perfect for security testing. By capturing complex application workflows and login procedures, it allows pentesters to run automated tests with recorded scripts, ensuring the security of various components in an application, including login mechanisms, data entry, and other critical processes.

# Installation
Follow the steps below to install and use Securily Macro Recorder on your platform:

- Download the latest source code [here](https://github.com/securily/SecurilyMacroRecorder).
- Extract the archive.
- Install dependencies with `pip3 install -r requirements.txt`.
- (Linux users: You may need to install Tkinter manually and remove `win10toast` from `requirements.txt`.)
- Run the application with `python3 main.py`.

There is also a separate branch for Windows-specific builds, available [here](https://github.com/securily/SecurilyMacroRecorder/tree/windows).

# How does this work?
To start recording, you simply have to press the red button\
From there, you can move your mouse, click, and type on your keyboard, and everything will be recorded. (You can choose what will be recorded.)
\
\
Then, to stop the recording, you simply click on the black square.\
To play a recording, you just need to click on the green play icon
And to stop the playback, press the `f3` key (By default).


# Showcase

## Windows






https://github.com/LOUDO56/PyMacroRecord/assets/117168736/ac77b7b6-02d0-4c12-a71a-65119c4acc59


## macOS





https://github.com/LOUDO56/PyMacroRecord/assets/117168736/2e8d8a85-c96b-4906-b8d9-b91de2c3d35b








## Linux






https://github.com/LOUDO56/PyMacroRecord/assets/117168736/25ab7c60-9f48-425f-bd5f-68c8b76e4c9c







# For bug reports or update requests
If you encounter a bug or want to request an update, simply create an issue [here](https://github.com/LOUDO56/PyMacroRecord/issues)

# For people who don't have windows or don't want to use exe file
- First, if you didn't already, install [Python](https://www.python.org/downloads/)
- Download the last source code release [here](https://github.com/LOUDO56/PyMacroRecord/releases)

- Extract it wherever you want.
- Open the terminal and type `cd <PATH TO SOFTWARE FOLDER>`
- Type the command:
  ```bash
  pip3 install -r requirements.txt
  ```
  - If you are on **Linux**, you might need to install Tkinter manually, commands to install are [here](https://www.geeksforgeeks.org/how-to-install-tkinter-on-linux/)
  - You need to remove the **win10toast** from `requirements.txt` if you are not on windows or else you won't be able to install the depedencies
  - Mac Users, you must add terminal to accessibility and input monitoring settings in system preferences to allow mouse and keyboard inputs.
  - (Optional) If you want these package to be on virtual environment follow these step [here](https://stackoverflow.com/a/41799834)
- Finally, do `cd src` and type: `python3 main.py`
- And boom! The software is now ready to use.

# Build (Windows)
To build the application, I use PyInstaller.

You need to be on home directory, not on src.

Then, use that command for onefile output (upx is optional).
```
pyinstaller --noconfirm --onefile --windowed --icon "src/assets/logo.ico" --name "PyMacroRecord-portable" --contents-directory "." --upx-dir upx --add-data "src/assets;assets/" --add-data "src/hotkeys;hotkeys/" --add-data "src/macro;macro/" --add-data "src/utils;utils/" --add-data "src/windows;windows/" --add-data "src/langs;langs"  "src/main.py"
```

For onedir output, use that command (upx is optional).

```
pyinstaller --noconfirm --onedir --windowed --icon "src/assets/logo.ico" --name "PyMacroRecord" --contents-directory "." --upx-dir upx --add-data "src/assets;assets/" --add-data "src/hotkeys;hotkeys/" --add-data "src/macro;macro/" --add-data "src/utils;utils/" --add-data "src/langs;langs" --add-data "src/windows;windows/"  "src/main.py"
```

# Support
Developing software is not an easy task. If you really like this project, please consider making a donation to the original <a href="https://github.com/LOUDO56/PyMacroRecord">Author</a>
\
\
By making a donation, your name will appear in the "Donors" section of the PyMacroRecord software and among the last 5 donors on the [PyMacroRecord](https://www.pymacrorecord.com) website as a thank you!

# License

This program is under [GNU General Public License v3.0](https://github.com/LOUDO56/PyMacroRecord/blob/main/LICENSE.md)

# Special Thanks

- Fooinys, who playtested my program.
- <a href="https://github.com/Lenochxd">Lenoch</a>, for code enhancement.
- <a href="https://github.com/takiem">Takiem</a> for the Italian and Brazilian-Portuguese translation.
- <a href="https://github.com/DennyClarkson">DennyClarkson</a> for the Chinese-Simplified translation.