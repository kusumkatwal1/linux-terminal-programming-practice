## Viewing File Contents
  - means reading the contents of a file directly from the Linux terminal.

### Commands:
#### 1. cat(Concatenate):
    - commonly used to display files, but its original purpose is to combine file contents.
    - Syntax: "cat FILE" || Display Multiple Files => "cat linux.txt handbook.txt"


#### 2. less:
    - less opens a file in an interactive viewer(to move/jumpy/search/read large file).
    - Basic Syntax: "less FILE"
    - Eg: "less handbook.txt"
    - use "q" to exit command.


#### 3. head:
    - displays the beginning of a file(first 10 line).
    - Basic Syntax: "head FILE"

#### 4. tail:
    - tail displays the end of a file(last 10 lines).
    - Basic Syntax: "tail FILE"
    - To stop: "Ctrl+C"


| **Situation**                                          | **Recommended Command** |
| ------------------------------------------------------ | ----------------------- |
| Read a short file or combine files                     | `cat`                   |
| Read a long file interactively or search while reading | `less`                  |
| Preview the beginning of a file or check CSV headers   | `head`                  |
| Inspect the latest lines or recent errors              | `tail`                  |
| Monitor a changing log file                            | `tail -f` or `tail -F`  |




@Kusum Katwal
