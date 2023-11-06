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

**Step 3:** Enter your current password password.

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

1. cd ~[username]:  goes to another user’s home directory.
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
