# EX 08: Windows-basic-commands-batchscript

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

![mkdir](https://github.com/Aakashraj04/Windows-basic-commands-batchscript/assets/121117266/9fd1bc4e-1eae-40f4-90cd-b3e375ccd68b)


```
cd %userprofile%\Desktop\MyLab
```

![cd](https://github.com/Aakashraj04/Windows-basic-commands-batchscript/assets/121117266/46461fa3-7da7-4805-84d8-5ff73bfac3a9)


```
type nul > MyFile.txt

```
![myfile_txt](https://github.com/Aakashraj04/Windows-basic-commands-batchscript/assets/121117266/9f8c69cf-5762-47cc-b442-da02ccbb0a44)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
dir %userprofile%\Desktop\MyLab
```

![userprofile](https://github.com/Aakashraj04/Windows-basic-commands-batchscript/assets/121117266/f8868342-11ec-40c7-a0af-c92f66e6804c)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

```
mkdir %userprofile%\Desktop\Backup

```
![backup](https://github.com/Aakashraj04/Windows-basic-commands-batchscript/assets/121117266/945f1493-8ee2-408d-aa59-138912464919)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![Screenshot 2024-05-08 200923](https://github.com/Aakashraj04/Windows-basic-commands-batchscript/assets/121117266/15f53b1e-1cc4-47e6-9017-655b14c00e43)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Documents
```

```
move MyLab Documents
```
![move](https://github.com/Aakashraj04/Windows-basic-commands-batchscript/assets/121117266/bf3921e6-1988-42a4-b3cd-224afda8fe18)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

```

## OUTPUT

![Screenshot 2024-05-08 202436](https://github.com/Aakashraj04/Windows-basic-commands-batchscript/assets/121117266/c08073e2-a0bf-443f-b3c0-13b8a224e02c)


# RESULT:
The commands/batch files are executed successfully.

