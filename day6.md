## Linux File Permissions and Ownership:
    - Linux permissions control who can:
      - Read (r)
      - Write (w)
      - Execute (x)
    - Three permission categories:
        - rwx
        - r-x
        - r--
          
      - represents:
        - Owner
        - Group
        - Others

| **Letter** | **Meaning**   | **Allows**                             |
| ---------- | ------------- | -------------------------------------- |
| `r`        | Read          | View and copy file contents            |
| `w`        | Write         | Modify and delete file contents*       |
| `x`        | Execute       | Run a file or enter a directory (`cd`) |
| `-`        | No permission | No access                              |



#### Commands:

#### 1. ls -l:
    - Use "ls -l" to display file and directory permissions.
  
      | **Symbol** | **Meaning**   |
      | ---------- | ------------- |
      | `-`        | Regular file  |
      | `d`        | Directory     |
      | `l`        | Symbolic link |


#### 2. chmod(Change Mode):
    - It changes permissions.
    - Basic Syntax: "chmod PERMISSIONS FILE"
    - Example: "chmod 755 script.sh"
    - & without number: "chmod u+x script.sh"
  
| **Symbol** | **Meaning**               |
| ---------- | ------------------------- |
| `u`        | User (Owner)              |
| `g`        | Group                     |
| `o`        | Others                    |
| `a`        | All (User, Group, Others) |
| `+`        | Add permission            |
| `-`        | Remove permission         |
| `=`        | Set exact permission      |

    
#### permission values:
| **Value** | **Meaning**   |
| --------- | ------------- |
| `777`     | Full access   |
| `755`     | Owner full    |
| `700`     | Owner only    |
| `644`     | Standard file |
| `600`     | Private file  |




#### 3. chown(Change Owner):
    - It changes file ownership.
    - Syntax: "chown OWNER FILE"
    - Requires administrative privileges.
    - Eg: "sudo chown alice:developers project.txt"

#### 4.chgrp(Change Group):
    - Syntax: "chgrp developers notes.txt"

#### 5. umask:
    - Determines the default permissions for newly created files and directories.
    - Check it: "umask"
    - eg:
        umask 077
        
        Create a file:
        
        touch private.txt
        
        Check:
        
        ls -l


## Conclusion:
| **Command** | **Purpose**             |
| ----------- | ----------------------- |
| `ls -l`     | View permissions        |
| `chmod`     | Change permissions      |
| `chown`     | Change owner            |
| `chgrp`     | Change group            |
| `umask`     | Set default permissions |


## Cheat Sheet:
    ls -l
    
    chmod 755 script.sh
    
    chmod 644 file.txt
    
    chmod +x script.sh
    
    chmod -R 755 directory
    
    chown alice file.txt
    
    chown alice:developers file.txt
    
    chgrp developers file.txt
    
    umask
    
    umask 077
