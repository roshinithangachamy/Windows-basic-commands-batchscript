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
![376103705-51be50b9-009d-4a34-9e07-73e41332a414](https://github.com/user-attachments/assets/a59bf44e-16af-4a90-a0d7-098fbab12551)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![376103770-c573ec08-0f89-427e-a648-919d5fe8150a](https://github.com/user-attachments/assets/fa8813c6-feeb-415e-93cf-7677f0df6856)

![376103788-239f273a-61ab-4e43-961e-6ebedc793e5d](https://github.com/user-attachments/assets/4ecc883b-02f1-49cb-ad4d-8c0437f99c21)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![376103844-c77b2551-bffa-49d2-ab84-60e7d221b068](https://github.com/user-attachments/assets/91e0cf60-fdf3-4987-8d73-48f4111271c5)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![376103932-a0f80ef5-e8f6-4cbd-b96b-e5cce11e902c](https://github.com/user-attachments/assets/156d4423-4163-4d7f-bbeb-ea8ec1dde82e)
![376103945-08a33477-ac70-4c67-94cc-752c203ee715](https://github.com/user-attachments/assets/bd25177f-3a51-4a6b-8a09-e1d243f818eb)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![376104010-0dd978e0-e0d6-4a93-a619-83d965a0bfd2](https://github.com/user-attachments/assets/22b175a0-8b2e-4085-9b6d-1dde324c7e2f)

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

![376104140-ddf657d3-b54a-44c7-8393-615d081e9043](https://github.com/user-attachments/assets/e58fad14-1744-48d2-a5f3-7f8d59c420fb)

# RESULT:
The commands/batch files are executed successfully.

