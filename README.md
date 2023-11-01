<h1>Hopper System Help</h1>

Assume a user with the below credentials:

***SLU NetID:*** hlogin01

***Default Password:*** xah48fj@icjdn

<h3>First time login</h3>

When you login in for the first time on hopper, it prompts you to change the password to a new one. To change password on the first login attempt follow the below steps.

**Step 1:** Ssh into your SLU hopper account using the below command (replace hlogin01 with your SLUNetID) and enter the password  v.
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

**1.**
