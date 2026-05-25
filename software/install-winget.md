# Windows Package Manager
https://github.com/microsoft/winget-cli

## How to download
1. Open the provided link.
2. Click on `Releases`.
3. Scroll to the end where the `Assets` are found.
4. Click on the file with `.msixbundle` extension to download the WinGet installer.

## Dependencies
On some systems it might be necessary to also download some dependencies that are not present on all Windows versions. To do so:
1. In the `Assets` you will also find a ZIP file named `DesktopAppInstaller_Dependencies.zip`.
2. Download and extract the files.
3. Put all extracted files into a folder called `Dependencies` in the same path as the WinGet installer (the `.msixbundle` file).

### Windows 10
It seems like for Windows 10 the dependencies are not automatically detected and installed, so a manual install is required.
To do so just follow the `How to install` steps for each dependency and then install WinGet.

## How to install
1. Open Windows PowerShell.
2. Navigate with the CD command to the folder where the file is located.
3. Type the following command replacing the "file_name" with the actual file name that you just downloaded:
	`Add-AppXPackage -Path .\file_name.msixbundle`
