# Bash (Bourne Again SHell) Practice
[Source](https://ryanstutorials.net/linuxtutorial/)
## The Command Line
- dashes (-) represent an option which help to modify a command

- Commands are stored in history and can be entered again using the up or down arrow. move left or right to edit.

### Common Commands

| Syntax | Description | Options | Description |
| ------ | ----------- | ------- | ----------- |
| ls [options][location]| show list of all files in current directory, ignores hidden (.) items| -l | long list |
| ... | ... | /etc | list directory contents |
| ... | ... | -a | list hidden items |
| pwd | print working directory | ... | ... |
| file [path] | shows file type | ... | ... |
| man < command > | works like a encyclopedia | -k < search term > | help you find a command |
| mkdir [options] < name of directory > | make new directory | -p | make parent |
| ... | ... | -v | results |
| rmdir [options] < name of directory > | remove **empty** directory | ... | ... |
| touch [options] < filename > | create new file | ... | ... |
| cp [options] < source > < destination > | copy | ... | ... |
| mv [options] < source > < destination > | move or rename | ... | ... |
| rm [options] < file > | remove file | -r | remove non-empty directory |
| ... | ... | -i | interactive prompt |

### More About Long List (-l)

### Example

| -/d | permissions | # of blocks | owner | privilege | filesize | last modification date/time | name |
|---- | ----------- | ----------- | ----- | --------- | -------- | --------------------------- | ---- |
| - | rw-r--r-- | 1 | dgomez | staff | 813 | Sep 13 08:23 | bash.md |
| - | rw-r--r-- | 1 | dgomez | staff | 0 | Sep  6 15:11 | class-01.md |
| d | rwxr-xr-x | 3 | dgomez | staff | 96 | Sep  6 15:13 | prework |

Notes: - indicates file, d indicates directory

**command:** ls -l /etc

**output:** lrwxr-xr-x@ 1 root  wheel  11 Jun 15 05:08 /etc -> private/etc

above starts with l. what is l??

## Basic Navigation
### Paths
Absolute paths specify a location (file or directory) in relation to the root directory and they always begin with a / whereas relative paths specify a location (file or directory) in relation to where we currently are in the system and they don't start with a slash.

- / stands for root directory
- ~ stands for home directory
- . stands for current directory
- .. stands for parent directory
- cd by itself takes you to home directory

### Interesting stuff

- /etc has config files
- /var/log has logs of system programs
- programs are located in /bin or /usr/bin

## More About Files

- Everything is a file??
- Unlike Windows, Linux is and extensionless system and it is case-sensitive
- anything inside quotes is treated as a single item
- you can use escape characters(backslash) e.g., Holiday\ Photos is the same as 'Holiday Photos'

## Manual Pages

use /search + ENTER to find specific words while in manual pages, press n for next

## File Manipulation
 see common commands mkdir through rm

## Cheat Sheet

kill < process id > - very useful for killing a port
SUDO for admin privileges

# Other Interests
## Grep and Regular Expressions
## Scripting

## Things I Learned
- Using multiple terminal windows for different purposes will come in handy
- / stands for root
- hidden files begin with a .
- use q to exit
- long hand options begin with double (--)
- short hand options with single (-)
- both cp and r are recursive

### macOS short-cuts
- command+space -> opens Spotlight (search tool)

