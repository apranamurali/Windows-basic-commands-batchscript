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
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/Aaron-0111/Windows-basic-commands-batchscript/assets/149347631/e95d419b-e1e0-46e4-b15a-526b5e311bd7)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/Aaron-0111/Windows-basic-commands-batchscript/assets/149347631/696b13b0-15a4-4eee-b1a9-42f7d7f0178c)
![image](https://github.com/Aaron-0111/Windows-basic-commands-batchscript/assets/149347631/bfd7435b-0d86-405e-a12a-26f3db05c13c)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/Aaron-0111/Windows-basic-commands-batchscript/assets/149347631/b4ac4df6-a5a8-4111-a724-d0790156e9f0)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/Aaron-0111/Windows-basic-commands-batchscript/assets/149347631/2f32ee2c-a44a-4c2e-85c7-51782fec0ad8)
![image](https://github.com/Aaron-0111/Windows-basic-commands-batchscript/assets/149347631/5e32ab54-ab74-4bc0-9368-c9c08a21d276)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/Aaron-0111/Windows-basic-commands-batchscript/assets/149347631/244dd6b7-8a61-4a1b-8a00-086fc2c61ee6)


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

![image](https://github.com/Aaron-0111/Windows-basic-commands-batchscript/assets/149347631/2dc920d8-968a-4998-867d-501afcafc1b3)




# RESULT:
The commands/batch files are executed successfully.

