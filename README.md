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
![image](https://github.com/PRASHANTHRATHI/Windows-basic-commands-batchscript/assets/145743120/dcfa2c58-68ed-41bb-b22a-e4cb8dc37efd)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/PRASHANTHRATHI/Windows-basic-commands-batchscript/assets/145743120/71816c0f-89e0-400a-a27f-3afe406a9244)

```
type nul > MyFile.txt
```
![image](https://github.com/PRASHANTHRATHI/Windows-basic-commands-batchscript/assets/145743120/a380b4b4-4ebf-467a-9b84-4bff0ec9d5d2)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/PRASHANTHRATHI/Windows-basic-commands-batchscript/assets/145743120/d73a216d-621a-4906-b579-eaf8c3e0aa1b)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```

![image](https://github.com/PRASHANTHRATHI/Windows-basic-commands-batchscript/assets/145743120/4946e87f-e4d3-4ed1-a60c-0813ce641821)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/PRASHANTHRATHI/Windows-basic-commands-batchscript/assets/145743120/5e6e287d-bdfc-4c8e-845f-b45357fe0001)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```

![image](https://github.com/PRASHANTHRATHI/Windows-basic-commands-batchscript/assets/145743120/5f8c70f2-a02a-4e78-9979-5ba50222429a)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

# COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
# OUTPUT:
![image](https://github.com/PRASHANTHRATHI/Windows-basic-commands-batchscript/assets/145743120/d1ea5ee3-e477-42ef-8d42-7a52f2c43501)


# COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!

```
## OUTPUT

![image](https://github.com/PRASHANTHRATHI/Windows-basic-commands-batchscript/assets/145743120/3bfc87f5-7075-4179-ae67-c14f22701e9a)


# RESULT:
The commands/batch files are executed successfully.

