## Linux Process Management and Job Control:
  - A process is a running instance of a program.
  - PID → Unique ID of a process.
  - PPID → ID of its parent process.
  - Processes form a parent-child tree.
  - PID 1 is usually systemd on modern Linux

## Commands:
 #### 1. ps(process status):
  - ps displays information about processes, or when you need a snapshot of running processes.
  - eg: "ps aux" or "ps -ef"

        | **Column** | **Meaning**   |
        | ---------- | ------------- |
        | `PID`      | Process ID    |
        | `TTY`      | Terminal      |
        | `TIME`     | CPU time used |
        | `CMD`      | Command       |

 
 #### 2. pgrep:
   - searches for processes by name or other attributes and returns their PIDs.
   - ex: "pgrep python"

 #### 3. pidof:
   - finds the PID of a running program.
   - eg: "pidof sshd"

 #### 4. top:
   - Continuously monitors running processes and system resources.
   - eg: "top"
   - "q": to quit

#### 5. htop:
  - User-friendly interactive process viewer; may need to be installed first.
  - eg: "htop"
  - Use "F10" or "q" to exit.

#### 6. kill:

#### 7. pkill:

#### 8. killall:

#### 9. jobs:

#### 10. bg:

#### 11. fg:

#### 12. nohup:

#### 13. nice:

#### 14. renice:


