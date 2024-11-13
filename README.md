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
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/300ac1fb-d49d-42ac-9da2-e4b36910ece8)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/80144692-1c89-4a49-8869-2149dbd515eb)
```
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/9f935902-0e38-4c6b-900f-e2082ced566b)

List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/b191f0a1-4c98-4ccb-a9ad-cfee97c372a0)
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/a43d717a-29ea-4c1f-984c-8b73bf8b30fb)
```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/292ba609-1a81-4193-9ebb-aad289ce4608)
Move the "MyLab" directory to the "Documents" folder.
## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![image](https://github.com/user-attachments/assets/f93278a0-b6e5-43e1-a303-499ce480bd72)
## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
## OUTPUT
![image](https://github.com/user-attachments/assets/8f1a1ce0-5b23-4df6-a496-7bf08a215614)
## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
![image](https://github.com/user-attachments/assets/ba76cde2-582e-4893-b55d-26b3abfb305b)
# RESULT:
The commands/batch files are executed successfully.

