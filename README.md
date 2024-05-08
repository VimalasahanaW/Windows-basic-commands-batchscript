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
![image](https://github.com/VimalasahanaW/Windows-basic-commands-batchscript/assets/144870812/3da6a15b-b84f-4b8e-8739-081770b5193e)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/VimalasahanaW/Windows-basic-commands-batchscript/assets/144870812/927ff308-6976-44ec-b9a2-99fd73d49039)
![image](https://github.com/VimalasahanaW/Windows-basic-commands-batchscript/assets/144870812/33153c03-6bab-4c98-ad35-5e89584de362)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/VimalasahanaW/Windows-basic-commands-batchscript/assets/144870812/6938436d-aad7-4171-9a5f-7ef471b69c78)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/VimalasahanaW/Windows-basic-commands-batchscript/assets/144870812/ace345c3-6bab-48f5-b0ad-e0b5bf62da26)
![image](https://github.com/VimalasahanaW/Windows-basic-commands-batchscript/assets/144870812/9c957336-3b66-4a19-8759-e1e67153cddc)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/VimalasahanaW/Windows-basic-commands-batchscript/assets/144870812/3528ac80-c89e-4b40-8ba8-07a8b66d026b)

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

![image](https://github.com/VimalasahanaW/Windows-basic-commands-batchscript/assets/144870812/58393c32-e7a7-4ceb-a06a-2b3ae4a05208)




# RESULT:
The commands/batch files are executed successfully.

