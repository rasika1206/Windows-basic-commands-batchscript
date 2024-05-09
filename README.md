# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript      
NAME: RASIKA. M    
REG.NO: 212222230117

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

![image](https://github.com/23004513/Windows-basic-commands-batchscript/assets/138973069/1feba45d-0779-48f3-9e31-f5a0350f0a66)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/23004513/Windows-basic-commands-batchscript/assets/138973069/2f186507-dd16-4ff6-ba9d-726aa06afb18)
![image](https://github.com/23004513/Windows-basic-commands-batchscript/assets/138973069/7423c134-d5e4-4596-b6bc-ba9df42eb03d)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/23004513/Windows-basic-commands-batchscript/assets/138973069/7185c5be-7400-4896-b2a7-761467002990)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/23004513/Windows-basic-commands-batchscript/assets/138973069/1f984e02-cf25-41c7-9534-4ff073959a2a)

![image](https://github.com/23004513/Windows-basic-commands-batchscript/assets/138973069/1f6310cd-f10a-4e03-89ba-ff14f15a29cf)



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/23004513/Windows-basic-commands-batchscript/assets/138973069/a74e26cf-e31f-4372-bc5e-80c890174e37)




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

![image](https://github.com/23004513/Windows-basic-commands-batchscript/assets/138973069/a8e01095-f652-4407-896d-272deb28d452)




# RESULT:
The commands/batch files are executed successfully.
