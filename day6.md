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

#### 1.ls -l:
  - Use ls -l to display file and directory permissions.

#### 2.chmod(Change Mode):
  - It changes permissions.
  - Basic Syntax: "chmod PERMISSIONS FILE"

| **Symbol** | **Meaning**               |      
| ---------- | ------------------------- |
| `u`        | User (Owner)              |
| `g`        | Group                     |
| `o`        | Others                    |
| `a`        | All (User, Group, Others) |
| `+`        | Add permission            |
| `-`        | Remove permission         |
| `=`        | Set exact permission      |  

\
| **Value** | **Meaning**   |
| --------- | ------------- |
| `777`     | Full access   |
| `755`     | Owner full    |
| `700`     | Owner only    |
| `644`     | Standard file |
| `600`     | Private file  |




#### 3.chgrp:

#### 4.umask:
