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

3) Displaying My User and Group Information :
```bash
id
```
The command `id` shows us a way to see what groups you belong to.
In Linux, users are organized into groups. These groups determine the permissions and access rights a user has.

- `uid`- Your User ID (a unique numerical identifier).
- `gid`- Your primary Group ID.
- `groups`- All the groups you are a member of.

*) Every process runs under the user who started it 
*) File access depends on ownership and permissions protecting user's private file

## Users :
*) Each user has a Home directory : usually (home/username)
*) Home directories store personal files and configurations
*) Users are identified internally by a UID (User ID)

## Groups:
*) Groups are collection of user's
*) Group's simplify permission management for multiple users
*) Groups are identified by a GID (Group ID)

4) 
   
