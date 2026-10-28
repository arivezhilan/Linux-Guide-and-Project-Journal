# Basic Starting Commands 
---
1) To display a message on the terminal :
```bash
echo "Hello World"
```
The command `echo` precisely tells what string of text to display provided as an argument inside the quotes , back to the terminal.

---
2) What's my account username :
```bash
whoami
```
The command `whoami` displays the username of the account currently running your terminal commands.

---
3) Displaying My User and Group Information :
```bash
id
```
The command `id` shows us a way to see what groups you belong to.
In Linux, users are organized into groups. These groups determine the permissions and access rights a user has.

- `uid`- Your User ID (a unique numerical identifier).
- `gid`- Your primary Group ID.
- `groups`- All the groups you are a member of.

- Every process runs under the user who started it.
- File access depends on ownership and permissions protecting user's private file.

## Users :
- Each user has a Home directory : usually (home/username)
- Home directories store personal files and configurations
- Users are identified internally by a UID (User ID)

## Groups:
- Groups are collection of user's
- Group's simplify permission management for multiple users
- Groups are identified by a GID (Group ID)

---
4) Display where exactly i'am :
```bash
pwd
```
- In Linux a core concept is that everything is treated as file . files are organised within a hierarchical structure known as file system
- Entire file system starts from single top level directory called the root directory
- The location of any file or directory is described by its path. A path is a sequence of directories that leads from starting point to a specific destination .  

The Command `pwd` Displays the full path of directory you are currently in starting from root .

---
5) Display Files & Folders :
```bash
ls
```
The command `ls` will list the directories and files in current directory 

- `ls /Home/Documents` - can specify path to list contents of different directory
- `ls -a` - to view hidden files on the folder
- `ls -l` - shows list of files in long format , detailed info of file permission , owner , group , file size etc .
- `ls -r` - sorting in reverse order
- `ls -la` - combining command flag to see list of hidden files in long format .
- `ls ~` - This command lists the contents of the home directory, which may be different from the current working directory .

---
6) Move to a different folder : 
```bash
cd
```
The command `cd` uses paths to change or specify destination .

- Absolute path :- This is the full path starting from root directory (/) . /home/username/desktop
- Relative path :- Relative to your current location in the file system . desktop/

`cd /home/username/desktop/pictures` - command moves directly to the pictures directory .

Navigating to a cd folder : if your are already in a directory and want to move to a subdirectory you can use a relative path .

Current location is `/home/username/desktop/pictures` and the pictures directory contains folder named Hawaii , you can navigate into it with `cd Hawaii` - we have only used Folders name because we are already in parents directory .

Navigation shortcuts :-

- `cd .` - Current directory ( . )
- `cd ..` - parent directory ( .. )
- `cd ~` - Home directory ( ~ )
- `cd -` - Previous directory ( - )

---
7) Creating an Empty file :
```bash
touch
```
The command `touch myfile` - a new empty file created called " my file " will appear in current directory .

`touch file1.txt file2.txt file3.log` - can create multiple empty files at once .

---
8) Reading a file :
```bash
cat
```
The command `cat` displays the content of a single file directory on the terminal 
- example : `cat myfile.txt`

`cat txtfile1 txtfile2` : Command reads the file in order , it will display the contents of txtfile 1 & then txtfile2 in order .

---
#) Creating New files and writing or reading the content : 

Operator ( > ) to create 

`cat > newfile.txt` - creates new file and write text into a file directory .

Also the command `less` views text file that are too large to fit on a single screen . it displays text in a paged format , allowing to navigate thru a file page by page without loading the entire file into memory .
- Navigation : arrow keys up & down to navigate line by line or page by page .
- Help menu : `h` to display help summary & Exit : `q` - quits and goes back to shell .

---
9) Finding what a command does, its syntax, and the options it supports :
```bash
help
```
The command `help` provides info about other bash built in commands .
`help echo` : displays summary of syntax and list of available options .

`ls --help` : provides summary of the command .
`help` mainly works with shell built-ins, such as `cd`, `echo`, `read`, and `exit`. For external programs such as `ls`, use `man ls` or `ls --help`

---
10) Display the documentation for commands :
```bash
man
```
The command `man`It displays the documentation for commands, programs, and system functions, explaining how they work, their options, and how to use them .

`man ls` accessing a manual for `ls` command .

---
11) Whats that command :
```bash
whatis
```
The command `whatis` displays concise one line description of commands directly .

---
*) Difference between help, man, and --help

| Command | Description | Example |
|---------|-------------|---------|
| `help`    | Help for Bash built-in commands  | `help cd` |
| `man`    | Opens a command's manual page | `man ls` |
| `--help`   | Often displays a command's usage and options | `ls --help` |

   
