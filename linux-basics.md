## Linux Basics:
  Learn what Linux is, why it is used, and how the terminal works.
### # Navigating the Linux Filesystem:
  - means moving between directories and finding files on a Linux system.
  - "directories" = "folders". i.e "**/ directory**"
### # Major Commands:
  #### 1. PWD:
    - pwd: Shows your current/working directory.
    - syntax: "pwd"
    - eg:
        - input: pwd
        - output: /home/student
  
  #### 2. List(ls):
    - ls: It displays a list of files and directories.
    - syntax: "ls" || "ls -l" =>detailed info || "ls -a"=> hidden files
    - eg:
        - input: ls
        - output: Documents Downloads linux-project Pictures
  
  #### 3.Change Directory(cd):
    - cd: It moves you from one directory to another.
    - syntax: "cd .. i.e. (one-directory)" || "cd or cd~ i.e (home_directory)" || "cd / i.e. (root_dir)" || "cd - i.e. (previous_directory)."
    - eg:
        - input: cd Documents
        - /Documents$ pwd
        -  /home/student/Documents
      
  #### 4. Make Directory(mkdir):
     - mkdir: It creates a new directory.
     - syntax: "mkdir"
     - eg:
           mkdir linux-lab
     
  #### 5.Touch(file create)
    -It creates an empty file.
    - syntax: "touch"
    - eg: touch file1.txt file2.txt file3.txt  (can create multiple at the same time)

## Complete Terminal Session
  a.student@linux:~$ pwd
  - /home/student
  
  b.student@linux:~$ mkdir -p linux-handbook/{notes,scripts,exercises,projects}
  
  c.student@linux:~$ cd linux-handbook
  
  d. student@linux:~/linux-handbook$ touch README.md notes/linux-basics.md scripts/hello.sh
  
  e. student@linux:~/linux-handbook$ ls
  - README.md  exercises  notes  projects  scripts
  
  f. student@linux:~/linux-handbook$ ls notes
  - linux-basics.md
  
  g.student@linux:~/linux-handbook$ ls scripts
  - hello.sh
