

### First we need to install chocolatey


Chocolatey is a popular package manager for Windows that simplifies the process of installing, updating, and managing software applications. It allows users to automate the installation of a wide range of software with a single command, making it efficient and convenient. Chocolatey provides access to a vast repository of pre-packaged software packages, which can be easily installed, updated, or removed using command-line instructions. This tool streamlines software management on Windows systems, enhancing productivity and reducing the manual effort required for software maintenance.

???+ warning "Requirements"
    * Windows 7 or newer version of Windows Operating System (Recommended Windows 10 or 11)
    * PowerShell v2+
    * .NET Framework 4+ 

???+ info "Installation Process"
    * Start Powershell with Administrator rights (Run as Administrator)
    If you already have choco installed in your device, run the following command in your powershell 

!!! danger "This will remove chocolatey from your computer! For re-installing only!"
    ```powershell title="Powershell as Administrator"
    rm -Path "C:\ProgramData\chocolatey" -Recurse -Force
    rm -Path "C:\ProgramData\ChocolateyHttpCache" -Recurse -Force
    ```
**Lets understand what you did with above command:** 

- `#!powershell rm`: It deletes files or directories in this case it deletes the chocolatey directory.
- `#!powershell -erroraction 'silentlycontinue'`: This part of the command tells PowerShell to continue executing the script without displaying an error message if the removal encounters an error (e.g., if the directory doesn't exist).

**Run the following command in Powershell to install CHOCOLATEY**

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; iwr https://community.chocolatey.org/install.ps1 -UseBasicParsing | iex
```

# Introduction
### Here's a small introduction of the programs installed on my computer

## Programs:
1. Powershell core
2. Git
3. VSCode
4. Putty
5. Firefox
6. Greenshot
7. Google drive file stream
8. Google Chrome
9. Notepad++
10. Winscp
11. 7zip
12. Paint.net
13. WinDirStat
14. Zoom
15. Sudo
16. Vmrc
17. VMware Horizon Client
18. Github Desktop
19. Docker Desktop
20. OBS Studio
21. Discord


***To install mentioned programs, run this script in Powershell***

```powershell

choco install powershell-core git vscode putty greenshot notepadplusplus winscp discord 7zip paint.net windirstat zoom sudo vmrc vmware-horizon-client github-desktop obs-studio docker-desktop google-drive-file-stream googlechrome curl powertoys -y

``` 


## Here's a screenshot from my terminal, after running the command "hostname"
![hostname](https://github.com/user-attachments/assets/cd6defc3-84f1-410c-b3d0-e404072ee2ac)
