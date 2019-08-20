# QEMU
### Download the x86_64 Installer
```
https://www.qemu.org/download
Select "Windows"
Note the links to Stefan Weil's site for binaries and installers.
Select the "64-bit" link.
https://qemu.weilnetz.de/w64/
Select a suitably recent w64 installer executable
Here, we chose QEMU 4.1.0
https://qemu.weilnetz.de/w64/qemu-w64-setup-20190815.exe
Select the "Save File" option prompted by Firefox
```
### Install QEMU
```
Select the Downloads icon menu item in Firefox (down-arrow).
Select the Folder icon to "Open containing folder".
Right-click on the downloaded file, qemu-w64-setup-20190815.exe, and select "Run as Administrator".
If prevented by Windows Defender, click the "More info" link and click "Run anyway".
Click "Yes" in Windows User Account Control to confirm installation.
Select the appropriate language.
Click Next, "I Agree", Next and Install.
Click Finish to complete QEMU setup.
```
### Use QEMU to Launch OS
```
Navigate to the OS project os.001 folder where os.dsk has been assembled.
Make sure os.dsk is not in use by another VM such as VirtualBox.
Run qemu-system-x86_64 -drive format=raw,file=os.dsk,index=0,if=floppy
Confirm OS launches in a QEMU window.
```
