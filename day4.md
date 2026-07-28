## Searching for Files and Text:
  - Searching in Linux means locating(Files/Directories/Commands/File names/Text inside files/Log entries/Configuration values)

### Command:
#### 1. Find:
  - Searches directories and their subdirectories and checks the filesystem directly.
  - Basic Syntax: "find STARTING_PATH CONDITIONS"
  - eg: "find ~/search-lab -name "linux-notes.txt"


#### 2. Locate:
  - Searches for paths using a prebuilt database.
  - Basic Syntax: "locate SEARCH_TERM"
  - eg: "locate app.conf"


#### 3.Grep: 
  - Searches for text patterns.
  - It can search: a single file/Multiple files/Entire directory trees/Command output/Logs/Configuration files/Source code.
  - Basic Syntax: "grep PATTERN FILE"
