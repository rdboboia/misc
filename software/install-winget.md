# Windows Package Manager
https://github.com/microsoft/winget-cli

## How to download
1. Open the provided link.
2. Click on `Releases`.
3. Scroll to the end where the `Assets` are found.
4. Click on the file that with `.msixbundle` extension to download the installer.

# Dependencies
On some systems it might be necessary to first install WinGet's dependencies first. To do so:
1. In the `Assets` you will also find a ZIP file named `DesktopAppInstaller_Dependencies.zip`.
2. Download and extract the file.
3. Follow the `How to install` steps to install each file.
4. Finally, install WinGet.

## How to install
1. Open Windows PowerShell.
2. Navigate with the CD command to the folder where the file is located.
2. Type the following command replacing the "file_name" with the actual file name that you just downloaded:
	`Add-AppXPackage -Path .\file_name.msixbundle`
