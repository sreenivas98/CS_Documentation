 <h1>Hopper System Help</h1>

Assume a user with the below credentials:

***SLU NetID:*** hlogin01

***Default Password:*** xah48fj@icjdn

<h3>First time login</h3>

When you login in for the first time on hopper, it prompts you to change the password to a new one. To change password on the first login attempt follow the below steps.

**Step 1:** Ssh into your SLU hopper account using the below command (replace hlogin01 with your SLUNetID) and enter the default password provided to login.
```
ssh hlogin01@hopper.slu.edu
```

**Step 2:** Enter the current password i.e., the default provided password.
```
Current Password: xah48fj@icjdn
```

**Step 3:** Enter the new password that you want to set.

***Password Rules:***

        1. The password should be atleast 10 characters long.

        2. It shuold be a combination of lowercase letters, uppercase letters, numbers and symbols.

        3. The new password should not be same as your old password.
        
**Step 4:** Enter the new password again for confirmation (Both new passwrod and confirm password must match for a successful password change).

<h3>Manual Passowrd Change</h3>

To change the password manually whenever you want. Follow the below steps:

**Step 1:** Login into your hopper account by using the below command (replace hlogin01 with your SLUNetID) and then entering your password.
```
ssh hlogin01@hopper.slu.edu
```

**Step 2:** Type in the below command to change your current password to a new one.
```
passwd
```

**Step 3:** Enter your current password.

**Step 4:** Enter your new password that you want to set.

***Password Rules:***

        1. The password should be atleast 10 characters long.

        2. It shuold be a combination of lowercase letters, uppercase letters, numbers and symbols.

        3. The new password should not be same as your old password.
        
**Step 5:** Enter your new password again for confirmation (Both new passwrod and confirm password must match for a successful password change).

<h3>Basic Linux Commands</h3>

<h1>1.  ls command:</h1> 

The ls command lists files and directories in your system. Below is the syntax:

```
ls [option] [directory/folder path]
```

If you remove the path, the ls command will show the current working directory's content. Below are the list of options and their use:

1. -a: lists all files, including hidden ones.
2. -lh: converts sizes to readable formats, such as MB, GB, TB. Also displays read, write and executable access of all files/folders in the mentioned path for all the three groups(user, group, others).

<h1>2.  pwd command:</h1> 

The pwd command prints your current working directory’s path, like /home/directory/path. Below is the syntax:

```
pwd
```

<h1>3.  cd command:</h1> 

The cd command is used to navigate the Linux files and directories. Below is the syntax

```
cd [directory/folder path]
```

Depending on your current location, it requires either the full path or the directory name. For example, omit /username from /username/directory/folder if you are already within it.

Omitting the arguments will take you to the home folder. Here are some navigation shortcuts:

1. cd ~[username] - goes to another user’s home directory.
2. cd .. - switches to the previous directory.
3. cd- – switches to the previous directory and prints the path of current working directory after switching.

<h1>4.  mkdir command:</h1> 

The mkdir command is used to create one or multiple directories and set their permissions. Below is the syntax:

```
mkdir [option] [directory_name]
```

To create a folder within a directory, use the path as the command parameter. For example, mkdir music/songs will create a songs folder inside music. Here are several common mkdir command options:

1. -p: creates a directory between two existing folders. For example, mkdir -p Music/2023/Songs creates a new 2023 directory.
2. -m: sets the folder permissions. For instance, enter mkdir -m777 directory to create a directory with read, write, and execute permissions for all users.
3. -v: prints a message for each created directory.

<h1>5.  rmdir command:</h1> 

The rmdir command is used to delete an empty directory in Linux. Below is the syntax:

```
rmdir [directory_name]
```

<h1>6. rm command:</h1> 

Use the rm command to permanently delete files within a directory. Below is the syntax:

```
rm [option] [filename1] [filename2] [filename3]
```

Adjust the number of files in the command according to your needs. If you encounter an error, ensure you have the write permission in the directory.

To modify the command, add the following options:

1. -i: prompts a confirmation before deletion.
2. -f: allows file removal without a confirmation.
3. -r: deletes files and directories recursively.

***Note:*** Use the rm command with caution since deletion is irreversible. Avoid using the -r and -f options since they may wipe all your files. Always add the -i option to avoid accidental deletion.

<h1>7. cp command:</h1> 

Use the cp command to copy files or directories, including their content, from your current location to another. It has various use cases, such as:

1. Copying one file from the current directory to another folder. Specify the file name and target path:

```   
cp filename.txt /home/username/Documents
```

2. Duplicating multiple files to a directory. Enter the file names and the destination path:

```
cp filename1.txt filename2.txt filename3.txt /home/username/Documents
```

3. Copying a file’s content to another within the same directory. Enter the source and the destination file:

```
cp filename1.txt filename2.txt
```

4. Duplicating an entire directory. Pass the -R flag followed by the source and destination directory:

```
cp -R /home/username/Documents /home/username/Documents_backup
```

<h1>8. mv command</h1>

Use the mv command to move or rename files and directories. To move items, enter the file name followed by the destination directory:

```
mv filename.txt /home/username/Documents
```

Meanwhile, use the following syntax to rename a file in Linux with the mv command:

```
mv old_filename.txt new_filename.txt
```

<h1>9. touch command</h1>

The touch command lets you create an empty file in a specific directory path. Below is the syntax:

```
touch path/filename.extension
```

If you omit the path, the command will create the item in the current folder.

<h1>10. file command</h1>

The file command lets you check a file type – whether it is a text, image, or binary. Below is the syntax:

```
file [option] [filename]
```

To modify the command, add the following options:

1. -k: Add this option to display more detailed information.
2. -i: Add this option to show the file’s MIME type.

<h1>11. zip command</h1>

The zip command lets you compress items into a ZIP file with the optimal compression ratio. Below is the syntax:

```
zip [options] [zipfile] [file1] [file2] ...
```

To modify the command, add the following options:

1. -u: Use this option to add an additional file to an existing zip archive.
2. -d: Use this option to remove a file from the zip archive.
3. -m: Use this option to delete the original files after creating a zipped archive.
4. -r: Use this option to zip the directory recursively.
5. -e: We can create a password-protected zip file using the -e option with the zip command.

<h1>12. zipinfo command</h1>

Use the zipinfo command to view the content of the zip file. Below is the syntax:

```
zipinfo [zipfilename]
```

<h1>13. unzip command</h1>

The unzip command lets you extract the compressed file items into a ZIP. Below is the syntax:

```
unzip [options] [zipfile] .
```

To modify the command, add the following options:

1. -d: If you want to unzip a file to a different directory, use the -d option with the unzip command. For example, to unzip a file named students.zip to a students directory, run the following command:

```
unzip students.zip -d students
```

2. -o: If you want to overwrite the existing files without being prompted.
3. -l: Use the -l option with the unzip command to view the content of a zipped file.
4. -Z: To list the content of a zipped file with detailed information about the file, use the -Z option

<h1>14. nano, vi commands</h1>

Linux lets users edit files using a text editor like nano or vi. Below are the syntaxes:

```
nano filename
```

```
vi filename
```

If the target file doesn’t exist, these editors will create one. We recommend nano if you want to quickly edit text files. Meanwhile, use vi for scripting and programming.

<h1>15. cat command</h1>

Concatenate or cat is one of the most used Linux commands. It lists, combines, and writes file content to the standard output. Below is the syntax:

```
cat [filename]
```

There are various ways to use the cat command:

1. cat > file.txt: Creates a new file with name file.txt.
2. cat file1.txt file2.txt > file3.txt: Merges file1.txt with file2.txt and stores the output in filename3.txt.
3. tac file.txt: Displays content in reverse order.

<h1>16. grep command</h1>

The global regular expression or grep command lets you find a word by searching the content of a file. This Linux command prints all lines containing the matching strings, which is useful for filtering large log files. Below is the syntax:

```
grep [pattern/string] [filename]
```

<h1>17. head command</h1>

The head command prints the first ten lines of a text file or piped data in your command-line interface. Below is the syntax:

```
head [option] [file]
```

The head command accepts several options, such as:

1. -n: This option changes the number of lines printed. For example, head -n 5 shows the first five lines.
2. -c: This option prints the file's first customized number of bytes. For example, head -c 50 shows the first 50 bytes of data from the file.
3. -q: This option disables headers specifying the file name. 

<h1>18. tail command</h1>

The tail command displays the last ten lines of a file, which is useful for checking new data and errors. Below is the syntax:

```
tail [option] [file]
```

The tail command accepts several options, such as:

1. -n: This option changes the number of lines printed. For example, tail -n 5 shows the last five lines.
2. -c: This option prints the file's last customized number of bytes. For example, tail -c 50 shows the last 50 bytes of data from the file.

<h1>19. sort command</h1>

The sort command rearranges lines in a file in a specific order. It doesn’t modify the actual file and only prints the result as Terminal outputs. Below is the syntax:

```
sort [option] [file]
```

By default, this command will sort the lines in alphabetical order, from A to Z. To modify the sorting, use these options:

1. -r: Reverses the sorting order to descending.
2. -n: Sorts the file numerically.
3. -k: Reorders data in a specific field.

<h1>20. cut command</h1>

The cut command retrieves sections from a file and prints the result as Terminal outputs.Below is the syntax:

```
cut [option] [file]
```

Instead of a file, you can use data from standard input. To determine how the command sections the line, use the following options:

1. -b: To extract the specific bytes, you need to follow -b option with the list of byte numbers separated by comma. Range of bytes can also be specified using the hyphen(-). It is necessary to specify list of byte numbers otherwise it gives error. Tabs and backspaces are treated like as a character of 1 byte.
2. -c: To cut by character use the -c option. This selects the characters given to the -c option. This can be a list of numbers separated comma or a range of numbers separated by hyphen(-). Tabs and backspaces are treated as a character. It is necessary to specify list of character numbers otherwise it gives error with this option.
3. -f: -c option is useful for fixed-length lines. Most unix files doesn’t have fixed-length lines. To extract the useful information you need to cut by fields rather than columns. List of the fields number specified must be separated by comma. Ranges are not described with -f option. 
4. -d: Cut uses tab as a default field delimiter but can also work with other delimiter by using -d option.

<h1>21. chmod command</h1>

The chmod command modifies directory or file permissions in Linux. Below is the syntax:

```
chmod [option] [permission] [file_name]
```

<h1>22. df command</h1>

The df command is used to check a Linux system’s disk space usage in percentage and kilobyte (KB). Below is the syntax:

```
df [options] [file]
```

If you don’t specify the item, this command will display information about every mounted file system. These are some acceptable options:

1. -m: Displays information on the file system usage in MBs.
2. -k: Prints file system usage in KBs.
3. -T: Shows the file system type in a new column.

<h1>23. du command</h1>

The du command is used to check a file or directory’s storage consumption. Remember to specify the directory path when using this command. Below is the syntax:

```
du [option] [directory/file path]
```

The du command has several options, such as:

1. -s: Shows the specified folder’s total size.
2. -m: Provides folder and file information in MB.
3. -k: Displays information in KB.
4. -h: Informs the displayed folders and files’ last modification date.

<h1>24. ps command</h1>

The ps command creates a snapshot of all running processes in your system. Executing it without an option or argument will list the running processes in the shell with the following information:

Unique process ID (PID).
Type of the terminal (TTY).
Running time (TIME).
Command that launches the process (CMD).

Below is the syntax:

```
ps [option]
```

The ps command accepts several options, including:

1. -T: Displays all processes associated with the current shell session.
2. -u username: Lists processes associated with a specific user.
3. -A: Shows all the running processes.

<h1>25. top command</h1>

The top command displays running processes and the system’s real-time condition, including resource utilization. It helps identify resource-intensive processes, enabling you to disable them easily. Below is the syntax:

```
top
```
