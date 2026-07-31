## Text Processing and Pipelines: 
  - means reading, filtering, transforming, and analyzing text from files or command output.

### Commands:
#### 1. sort:
    - Sorts lines in a file alphabetically, numerically, or in a custom order.
    - Basic Syntax: "sort FILE"

#### 2. uniq:
    - Removes adjacent duplicate lines (sort the file first if duplicates are not together).
    - Basic Example: "sort colors.txt | uniq"

#### 3. wc(word-count):
    - Counts the number of lines, words, characters, or bytes in a file.
    - Basic Syntax: "wc FILE"

#### 4. cut: 
    - Extracts selected columns or fields from each line of a file.
    - Basic Syntax: "cut OPTIONS FILE"

#### 5. tr:
    - Replaces, removes, squeezes, or translates characters in text.
    - Example: "echo "linux handbook" | tr 'a-z' 'A-Z'"

#### 6. tee:
    - Displays command output on the screen and saves it to a file at the same time.
    - Basic Syntax: "COMMAND | tee FILE"



| **Command** | **Purpose**                              |
| ----------- | ---------------------------------------- |
| `sort`      | Arrange lines                            |
| `uniq`      | Remove adjacent duplicate lines          |
| `wc`        | Count lines, words, characters, or bytes |
| `cut`       | Extract columns or fields                |
| `tr`        | Replace, delete, or translate characters |
| `tee`       | Display and save output simultaneously   |



## Cheat Sheet:

| **Command**                         | **Purpose**                                 |
| ----------------------------------- | ------------------------------------------- |
| `sort file`                         | Sort lines alphabetically                   |
| `sort -n file`                      | Sort lines numerically                      |
| `sort -r file`                      | Sort lines in reverse order                 |
| `sort file \| uniq`                 | Sort and remove duplicate lines             |
| `sort file \| uniq -c`              | Sort and count duplicate lines              |
| `wc -l file`                        | Count lines                                 |
| `wc -w file`                        | Count words                                 |
| `cut -d',' -f2 file.csv`            | Extract the 2nd CSV column                  |
| `tr 'a-z' 'A-Z'`                    | Convert lowercase to uppercase              |
| `tr -d '0-9'`                       | Remove digits                               |
| `tee output.txt`                    | Display output and save to a file           |
| `tee -a output.txt`                 | Append output to a file while displaying it |
| `cat file \| sort \| uniq`          | Display unique sorted lines                 |
| `cat file \| sort \| uniq \| wc -l` | Count unique lines                          |

