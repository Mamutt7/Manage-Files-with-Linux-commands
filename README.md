# Manage-Files-with-Linux-commands

Scenario
In this scenario, you need to ensure that the /home/analyst directory is properly organized.

You have to make a few changes to the /home/analyst directory and the files it contains.

You also have to edit a file to record the changes or updates you make to the directory.

```bash
home
└── analyst
    ├── notes
    │   ├── Q3patches.txt
    │   └── tempnotes.txt
    ├── reports
    │   ├── Q1patches.txt
    │   └── Q2patches.txt
    └── temp
```

You need to modify the /home/analyst directory to the following directory and file structure:

```bash
home
└── analyst
    ├── logs
    ├── notes
    │   └── tasks.txt    
    └── reports
        ├── Q1patches.txt
        └── Q2patches.txt
        └── Q3patches.txt
```
Here’s how you’ll do this: First, you’ll create a new subdirectory called logs in the /home/analyst directory. Next, you’ll remove the temp subdirectory. Then, you’ll move the Q3patches.txt file to the reports subdirectory and delete the tempnotes.txt file. Finally, you’ll create a new .txt file called tasks in the notes subdirectory and add a note to the file describing the tasks you've performed.

You’ll need to use the commands learned in the video lesson to complete these steps.


Task 1. Create a new directory
First, you must create a dedicated subdirectory called logs, which will be used to store all future log files.

1. Create a new subdirectory called logs in the /home/analyst directory.
2. List the contents of the /home/analyst directory to confirm that you’ve successfully created the new logs subdirectory.

The output should list the original three directories and the new logs subdirectory:

```bash
logs notes reports temp
```
![image](https://github.com/user-attachments/assets/755ca1c8-1cbb-4713-8135-785136ccd49f)


Task 2. Remove a directory
Next, you must remove the temp directory, as you’ll no longer be placing items in it.

1. Remove the /home/analyst/temp directory.
2. List the contents of the /home/analyst directory to confirm that you have removed the temp subdirectory.

The temp directory should no longer be listed:

```bash
logs notes reports
```
![image](https://github.com/user-attachments/assets/70286984-9e67-4175-adcd-525174d1ff01)

Task 3. Move a file
The Q3patches.txt file contains notes taken on third-quarter patches and is now in the correct reporting format.

You must move the  Q3patches.txt file from the notes directory to the reports directory.

1. Navigate to the /home/analyst/notes directory.
2. Move the Q3patches.txt file from the /home/analyst/notes directory to the /home/analyst/reports directory.
3. List the contents of the /home/analyst/reports directory to confirm that you have moved the file successfully.

When you list the contents of the reports directory, it should show that three quarterly report files are now in the reports directory:
```bash
Q1patches.txt Q2patches.txt Q3patches.txt 
```
![image](https://github.com/user-attachments/assets/1f233460-2a86-4f36-b730-ef00efad28af)


Task 4. Remove a file
Next, you must delete an unused file called tempnotes.txt from the /home/analyst/notes directory.

1. Remove the tempnotes.txt file from the /home/analyst/notes directory.
2. List the contents of the /home/analyst/notes directory to confirm that you’ve removed the file successfully.
No files should be listed in the notes directory.

![image](https://github.com/user-attachments/assets/40f55871-8b4e-4834-9fe3-aa291e65b4ac)


Task 5. Create a new file
Now, you must create a file named tasks.txt in the /home/analyst/notes directory that you’ll use to document completed tasks.

1. Use the touch command to create an empty file called tasks.txt in the /home/analyst/notes directory.
2. List the contents of the /home/analyst/notes directory to confirm that you have created a new file.
A file called tasks.txt should now exist in the notes directory:
```bash
tasks.txt
```
![image](https://github.com/user-attachments/assets/f43c6c33-e2e3-4e4f-b341-ac3cfddc9c77)


Task 6. Edit a file
Finally, you must use the nano text editor to edit the tasks.txt file and add a note describing the tasks you’ve completed.

1. Using the nano text editor, open the tasks.txt file that is located in the /home/analyst/notes directory.

2. Copy and paste the following text into the text input area of the nano editor:
```bash
  Completed tasks
  1. Managed file structure in /home/analyst
```
3. Press CTRL+X to exit the nano text editor.
This triggers a prompt asking Save modified bufferer?

4. Press Y to confirm that you want to save the new data to your file. (Answering "no" will discard changes.)

5. Press ENTER to confirm that File Name to Write is tasks.txt.

6. Use the clear command to clear the Bash shell window and remove any traces of the nano text input area.

7. Display the contents of the tasks.txt file to confirm that it contains the updated task details.

This file should now contain the contents of the tasks.txt file that you added and saved in previous steps:
```bash
  Completed tasks
  1. Managed file structure in /home/analyst
```

![image](https://github.com/user-attachments/assets/5f849c6c-4bfa-4c60-a5a0-a695c12498a1)

# Conclusion
You now have practical experience in using basic Linux Bash shell commands to

create and remove directories,
copy, move, and remove files, and
edit files with the nano text editor.
