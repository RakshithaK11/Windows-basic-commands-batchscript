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
![image](https://github.com/user-attachments/assets/df6c841f-acba-400b-8810-4fc72229fcfc)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/user-attachments/assets/e3c6d033-7e73-4373-91f2-0c2756381335)

type nul > MyFile.txt
![image](https://github.com/user-attachments/assets/cc582b6c-f3bf-477f-abc3-1f2296718f75)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![image](https://github.com/user-attachments/assets/650f9e55-20d8-41b8-9b39-4794697dcea2)

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup
![image](https://github.com/user-attachments/assets/83250b7b-3377-4608-9b94-906f0572c33a)
copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/user-attachments/assets/45539041-7692-43b0-b768-c0f43973b17c)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
![image](https://github.com/user-attachments/assets/29af956e-5209-425b-b090-a34d0fbe5aaa)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
![image](https://github.com/user-attachments/assets/4d2d4d0c-0be4-47f7-96cc-5cfcb76fc14f)
# COMMENT:

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!



## OUTPUT
![image](https://github.com/user-attachments/assets/b8cba86c-0555-4bc7-9d4c-5da9e836aa27)

# RESULT:
The commands/batch files are executed successfully.

