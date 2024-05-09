# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

NAME:MOHAN RAJ.C

REG.NO:212223040114

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
mkdir %userprofile%\Desktop\MyLab

![325487824-1feba45d-0779-48f3-9e31-f5a0350f0a66](https://github.com/Mohanraj2006/Windows-basic-commands-batchscript/assets/152195759/f8f5df15-67e6-409c-bc21-f642bb6a92cf)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![325488323-2f186507-dd16-4ff6-ba9d-726aa06afb18](https://github.com/Mohanraj2006/Windows-basic-commands-batchscript/assets/152195759/71bc5c55-8783-4a01-8d56-cb9b62b3b227)

![325488368-7423c134-d5e4-4596-b6bc-ba9df42eb03d](https://github.com/Mohanraj2006/Windows-basic-commands-batchscript/assets/152195759/35ae9b93-4484-404b-bb49-b5b2b313da59)




List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![325488521-7185c5be-7400-4896-b2a7-761467002990](https://github.com/Mohanraj2006/Windows-basic-commands-batchscript/assets/152195759/ff60edf8-fe8d-4e57-947e-1a8322df1856)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![325488716-1f984e02-cf25-41c7-9534-4ff073959a2a](https://github.com/Mohanraj2006/Windows-basic-commands-batchscript/assets/152195759/56d22c08-1bdf-4793-a370-071642601e3e)

![325488745-1f6310cd-f10a-4e03-89ba-ff14f15a29cf](https://github.com/Mohanraj2006/Windows-basic-commands-batchscript/assets/152195759/10ab6fd5-2275-4f96-bf5c-5f45e610c158)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![325488849-a74e26cf-e31f-4372-bc5e-80c890174e37](https://github.com/Mohanraj2006/Windows-basic-commands-batchscript/assets/152195759/4c38d465-e4d1-463e-b72d-1b50251367d0)

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

![325489059-a8e01095-f652-4407-896d-272deb28d452](https://github.com/Mohanraj2006/Windows-basic-commands-batchscript/assets/152195759/9f9ffe89-d4b5-4566-ad0e-179406e9e88e)


# RESULT:
The commands/batch files are executed successfully.

