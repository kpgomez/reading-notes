# Bash (Bourne Again SHell) Practice
[Source](https://ryanstutorials.net/linuxtutorial/)
## The Command Line
dashes (-) represent an option which help to modify a command

Commands are stored in history and can be entered again using the up or down arrow. move left or right to edit.
### Command Commands
| Syntax | Description | Options | Description |
|--------|-------------|---------|-------------|
| ls [options][location]| show list of all files in current directory| -l |long list|
|||/etc|list directory contents|

|pwd| print working directory|...|

### More About Long List (-l)

#### Example
-rw-r--r--@ 1 dgomez  staff  813 Sep 13 08:23 bash.md
-rw-r--r--  1 dgomez  staff    0 Sep  6 15:11 class-01.md
-rw-r--r--  1 dgomez  staff    0 Sep  6 15:12 class-02.md
-rw-r--r--  1 dgomez  staff    0 Sep  6 15:12 class-03.md
-rw-r--r--  1 dgomez  staff    0 Sep  6 15:12 class-04.md
drwxr-xr-x  3 dgomez  staff   96 Sep  6 15:13 prework

- indicates file
d indicates directory
next 9 characters indicate permissions such as read-write, read-only, etc
number indicates number of blocks
dgomez is owner of the file or directory
staff is group or privilege of owner
813 is the filesize
Sep 13 08:23 last file modification date and time
bash.md is the name of the file or directory

command: ls -l /etc

output: lrwxr-xr-x@ 1 root  wheel  11 Jun 15 05:08 /etc -> private/etc

above starts with l. what is l??

### Paths
Absolute paths specify a location (file or directory) in relation to the root directory and they always begin with a / whereas relative paths specify a location (file or directory) in relation to where we currently are in the system and they don't start with a slash.

## Basic Navigation
## More About Files
## Manual Pages
## File Manipulation
## Cheat Sheet

# Other Interests
## Grep and Regular Expressions
## Scripting

## Things I Learned
- Using multiple terminal windows for different purposes will come in handy

### macOS short-cuts
- command+space -> opens Spotlight (search tool)

