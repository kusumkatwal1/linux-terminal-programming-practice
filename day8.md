## Linux Process Management and Job Control:
      - A process is a running instance of a program.
      - "PID" = Unique ID of a process.
      - "PPID" = ID of its parent process.
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
      - eg: "pkill -TERM python3"  =  may terminate multiple matching processes.
      - Use carefully.

#### 8. killall:
      - can send a signal to processes matching a process name.
      - eg: "killall -TERM myapplication"
            - "TERM" = Gracefully stop
            - "pgrep -a name" = Check matching processes first.
            - "killall" = send a signal to processes by name

#### 9. jobs:
      - shows background or stopped jobs started by the current shell.
      - eg: "sleep 300"
            - output: "job" = "[1]+  Stopped  sleep 300"
            - "Ctrl+Z" = press it to suspend a running job.
            - "jobs" = Shows background/stopped jobs.

#### 10. bg:
      - continues a stopped job in the background.
      - eg: "sleep 300"
            - output:"bg" = "[1]+ sleep 300 &"
            - "Ctrl+Z": "Stop/suspend the current job"
            - "bg": "resume a stopped job in the background"

#### 11. fg:
      - Bring a background job to the foreground.
      - eg : "fg"
            - "Ctrl+C": "to terminate the sleep command."

#### 12. nohup:
      - Keeps a command running after you disconnect from SSH or close the terminal.
      - nohup = run a command independently of the terminal session.
      - eg: "nohup python3 server.py &"
            - "nohup" = Ignore terminal hangup
            - "&" = Run in the background
            - "Output" = Usually saved to nohup.out
    

#### 13. nice:
      - Starts a process with a different CPU scheduling priority.
      - Range: "-20 to 19"
      - "20" = "Highest priority"
      - "19" = "Lowest priority"
      - eg: "nice -n 10 sleep 100"
      - "nice" = "set process priority when starting it."
      
#### 14. renice:
      - changes the priority of an already-running process.
      - eg: "renice 10 -p 25100"
      - "10" = "New nice value"
      - "25100" = "Process ID (PID)"
      - "renice" = "change process priority."

## Command Cheat Sheet
            a. Current identity
            whoami
            
            b. Process snapshot
            ps
            
            c. All processes
            ps aux
            
            d. Full process information
            ps -ef
            
            e. Find processes
            pgrep python
            
            f. Find PID
            pidof sshd
            
            g. Live monitoring
            top
            
            h. Interactive monitoring
            htop
            
            i. Graceful termination
            kill -TERM PID
            
            j. Force termination
            kill -KILL PID
            
            k. Search and terminate by name
            pkill -TERM NAME
            
            l. Jobs
            jobs
            
            m. Background a stopped job
            bg %1
            
            n. Foreground a job
            fg %1
            
            o. Start in background
            command &
            
            p. Keep running after logout
            nohup command &
            
            q. Lower scheduling priority
            nice -n 10 command
            
            r. Change priority
            renice 10 -p PID

@Kusum Katwal
