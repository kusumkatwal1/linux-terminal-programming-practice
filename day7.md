## Users, Groups, and Privilege Management:
 #### 1: whoami:
    - Display the current logged-in user.
    - Syntax: "whoami"
    - Before running administrative commands.
    - Terminal Example: "student@linux:~$ whoami"
            - Output: "student"

 #### 2. id:
    - Display detailed identity information.
    - Syntax: "id"

 #### 3. groups:
    - Show the groups a user belongs to.
    - Syntax: "groups"

 #### 4. useradd:
    - Create a new user.
    - Syntax: "sudo useradd USERNAME"

#### 5. usermod:
    - Modify an existing user.
    - Example: Add a User to a Group: "sudo usermod -aG docker alice"
    - Here; "-a" = Append and "-G" = "Supplementary groups"

#### 6. passwd:
   - Change passwords.
   - Example: Change Your Password: "passwd"
   - Change Another User's Password: "sudo passwd alice"
    
#### 7. userdel:
   - Delete a user.
   - Remove only the Account: "sudo userdel alice"

#### 8. su:
   - Switch to another user account.
   - "su -" : if enabled, prompts for the root password.
   - "su - alice": "-" loads the target user's login environment

#### 9. sudo:
   - Run a single command with elevated privileges.
   - sudo apt update.
   - sudo whoami

## Cheat Sheet
    - whoami
    
    - id
    
    - groups
    
    - sudo useradd -m alice
    
    - sudo passwd alice
    
    - sudo usermod -aG docker alice
    
    - sudo userdel -r alice
    
    - su - alice
    
    - sudo COMMAND


