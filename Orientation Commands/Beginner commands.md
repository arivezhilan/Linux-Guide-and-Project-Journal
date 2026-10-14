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

   
