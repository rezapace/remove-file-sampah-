# Junk File Remover

This script will delete junk files on Windows 10 with a single click. The junk files that will be deleted are located in the following directories:

- `C:\Windows\Prefetch`
- `C:\Users\R\AppData\Local\Temp`
- `C:\Windows\Temp`

## Script Explanation

```powershell
Get-ChildItem -Path "C:\Windows\Temp" *.* -Recurse | Remove-Item -Force -Recurse
```
The above script will delete all files with any extension in the `C:\Windows\Temp` directory and its subdirectories.

```powershell
Get-ChildItem -Path "C:\Users\R\AppData\Local\Temp" *.* -Recurse | Remove-Item -Force -Recurse
```
The above script will delete all files with any extension in the `C:\Users\R\AppData\Local\Temp` directory and its subdirectories.

```powershell
Get-ChildItem -Path "C:\Windows\Prefetch" *.* -Recurse | Remove-Item -Force -Recurse
```
The above script will delete all files with any extension in the `C:\Windows\Prefetch` directory and its subdirectories.

```powershell
Clear-RecycleBin -Force
```
The above script will delete all files in the recycle bin.

## How to Use

1. Open PowerShell by right-clicking on the Start Menu and selecting "Windows PowerShell".
2. Copy the script above and paste it into PowerShell.
3. Press Enter to run the script.
4. Wait until the process is complete.
5. The junk files in the specified directories will be deleted.

This structure provides a clear and concise explanation of the script, making it easy to understand and follow.