A script to copy files from the phone camera to local disk. Uses shell to access the MTP files.
More info on [source blog here](https://plusontech.com/2019/01/05/weekend-powershell-script-copy-files-from-phone-camera-by-month/).
```PowerShell
cd D:\Repository\phone-2-backup\;
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned -Force
.\copy.ps1 -MTPSourcePath "Galaxy S9\Phone\DCIM\Camera" -TargetPath "D:\Backup\Telefon\Camera";
.\copy.ps1 -MTPSourcePath "Galaxy S9\Phone\DCIM\Screenshots" -TargetPath "D:\Backup\Telefon\Screenshots";
.\copy.ps1 -MTPSourcePath "Galaxy S9\Phone\Voice Recorder" -TargetPath "D:\Backup\Telefon\Voice Recorder"
.\copy.ps1 -MTPSourcePath "Galaxy S9\Phone\ACRCalls" -TargetPath "D:\Backup\Telefon\ACRCalls"
```