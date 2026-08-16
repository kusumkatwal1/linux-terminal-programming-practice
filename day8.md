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
  - Sends a signal to a process.
  - Basic syntax: "kill PID"
  - eg: "kill 24321"

#### 7. pkill:
  - Sends signals to processes matching a name or other selection criteria.
  - eg: "pkill -TERM python3"  =>  may terminate multiple matching processes.
  - Use carefully.

#### 8. killall:
  - can send a signal to processes matching a process name.
  - eg: "killall -TERM myapplication"
      - "TERM" → Gracefully stop
      - "pgrep -a name" → Check matching processes first.
      - "killall" = send a signal to processes by name

#### 9. jobs:
  - shows background or stopped jobs started by the current shell.
  - eg: "sleep 300"
      - "Ctrl+Z" → press it to suspend a running job.
      - "jobs": Shows background/stopped jobs.

#### 10. bg:

#### 11. fg:

#### 12. nohup:
  - keeps a command running after you disconnect from SSH or close the terminal.
  - nohup = run a command independently of the terminal session.
  - eg: "nohup python3 server.py &"
      - "nohup" → Ignore terminal hangup
      - "&" → Run in background
      - "Output" → Usually saved to nohup.out
    

#### 13. nice:

#### 14. renice:


