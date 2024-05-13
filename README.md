# EX 08: Windows-basic-commands-batchscript

## DATE:

## AIM:
To execute Windows basic commands and batch scripting

## DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




## WINDOWS COMMANDS:

## Exercise 1: Basic Directory and File Operations

Create a directory named "MyLab" on the desktop.

## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

```
mkdir %userprofile%\Desktop\MyLab

```

![alt text](<Screenshot 2024-05-07 192819.png>)

```
cd %userprofile%\Desktop\MyLab
```

![alt text](<Screenshot 2024-05-07 192917.png>)

```
type nul > MyFile.txt

```
![alt text](myfile.png)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
dir %userprofile%\Desktop\MyLab
```

![alt text](<Screenshot 2024-05-07 193029.png>)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

```
mkdir %userprofile%\Desktop\Backup

```
![alt text](backup.png)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![alt text](<Screenshot 2024-05-07 193122.png>)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Documents
```

```
move MyLab Documents
```
![alt text](<Screenshot 2024-05-07 193431.png>)

## COMMAND AND OUTPUT


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

```

## OUTPUT

![alt text](<Screenshot 2024-05-07 203226.png>)

# RESULT:
The commands/batch files are executed successfully.

