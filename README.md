WSL Stack
=========

Stack for working with containerized Linux distros, including graphical
applications within Windows.

WSL 2
-----

WSL 2 requires Windows 10 1903 or higher on x64 systems.

1. Install WSL.
Run as Administrator:
```PowerShell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
2. Enable Virtual Machine Platform.
Run as Administrator:
```PowerShell
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```
*Note:* These first two steps can be performed by adding these commands to
an answer file for an unattended Windows install.
3. Restart.
4. Download and install the [Linux kernel update package](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi).
5. Set WSL 2 as the default version.
Run as Administrator:
```PowerShell
wsl --set-default-version 2
```

Docker
------

X Window System
---------------

