# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS: 

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-04-25 112001](https://github.com/aswethaashok/Windows-basic-commands-batchscript/assets/149987410/04b939cc-be72-4fce-98e6-1d96c1e8b6d6)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2024-04-25 112410](https://github.com/aswethaashok/Windows-basic-commands-batchscript/assets/149987410/d3328cab-2d17-4efd-b736-cfe6cef4cedb)

![Screenshot 2024-04-25 112453](https://github.com/aswethaashok/Windows-basic-commands-batchscript/assets/149987410/a72820db-5967-472c-b6ae-bf08ceeaeace)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-04-25 112534](https://github.com/aswethaashok/Windows-basic-commands-batchscript/assets/149987410/11847b48-2dfb-49f1-90b6-4912c9c9d016)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2024-04-25 112639](https://github.com/aswethaashok/Windows-basic-commands-batchscript/assets/149987410/561d2b39-0dd3-423d-9503-9264fcacf815)

![Screenshot 2024-04-25 112639](https://github.com/aswethaashok/Windows-basic-commands-batchscript/assets/149987410/3da0083b-77b0-4aec-b583-86d70d6d90c4)


## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![Screenshot 2024-04-25 112750](https://github.com/aswethaashok/Windows-basic-commands-batchscript/assets/149987410/06a53612-1394-46c4-bbab-7d6b8e19955d)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT

![Screenshot 2024-04-25 112915](https://github.com/aswethaashok/Windows-basic-commands-batchscript/assets/149987410/359df3da-ad00-44a6-b6d8-663bea5dfc6e)




# RESULT:
The commands/batch files are executed successfully.

