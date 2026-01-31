# Permissions - Shell Scripts

This directory contains shell scripts that demonstrate various file and directory permission operations in Unix/Linux systems.

## Scripts Description

### 0. I am Betty
**Script:** `0-iam_betty`  
**Description:** Switches the current user to the user "betty".  
**Command:** Uses the `su` command to switch to user betty.  
**Usage:** `./0-iam_betty`

### 1. Who am I
**Script:** `1-who_am_i`  
**Description:** Prints the effective username of the current user.  
**Command:** Uses the `whoami` command.  
**Usage:** `./1-who_am_i`

### 2. Groups
**Script:** `2-groups`  
**Description:** Prints all the groups the current user is part of.  
**Command:** Uses the `groups` command.  
**Usage:** `./2-groups`

### 3. New owner
**Script:** `3-new_owner`  
**Description:** Changes the owner of the file "hello" to the user "betty".  
**Command:** Uses `chown betty hello`.  
**Usage:** `sudo ./3-new_owner`

### 4. Empty!
**Script:** `4-empty`  
**Description:** Creates an empty file called "hello".  
**Command:** Uses `touch hello`.  
**Usage:** `./4-empty`

### 5. Execute
**Script:** `5-execute`  
**Description:** Adds execute permission to the owner of the file "hello".  
**Command:** Uses `chmod u+x hello`.  
**Usage:** `./5-execute`

### 6. Multiple permissions
**Script:** `6-multiple_permissions`  
**Description:** Adds execute permission to owner and group owner, and read permission to other users for the file "hello".  
**Command:** Uses `chmod u+x,g+x,o+r hello`.  
**Usage:** `./6-multiple_permissions`

### 7. Everybody!
**Script:** `7-everybody`  
**Description:** Adds execution permission to owner, group owner, and other users for the file "hello".  
**Command:** Uses `chmod a+x hello` (without commas).  
**Usage:** `./7-everybody`

### 8. James Bond
**Script:** `8-James_Bond`  
**Description:** Sets file permissions to 007 (owner: no permission, group: no permission, others: all permissions).  
**Command:** Uses `chmod 007 hello`.  
**Usage:** `./8-James_Bond`

### 9. John Doe
**Script:** `9-John_Doe`  
**Description:** Sets the mode of the file "hello" to `-rwxr-x-wx` (octal 753).  
**Command:** Uses `chmod 753 hello`.  
**Usage:** `./9-John_Doe`

### 10. Look in the mirror
**Script:** `10-mirror_permissions`  
**Description:** Sets the mode of "hello" to match "olleh"'s mode.  
**Command:** Uses `chmod --reference=olleh hello`.  
**Usage:** `./10-mirror_permissions`

### 11. Directories
**Script:** `11-directories_permissions`  
**Description:** Adds execute permission to all subdirectories of the current directory for all users without changing regular files.  
**Command:** Uses `find . -maxdepth 1 -type d -exec chmod a+x {} \;`.  
**Usage:** `./11-directories_permissions`

### 12. More directories
**Script:** `12-directory_permissions`  
**Description:** Creates a directory called "my_dir" with permissions 751 (rwxr-x--x).  
**Command:** Uses `mkdir -m 751 my_dir`.  
**Usage:** `./12-directory_permissions`

### 13. Change group
**Script:** `13-change_group`  
**Description:** Changes the group owner of "hello" to "school".  
**Command:** Uses `chgrp school hello`.  
**Usage:** `sudo ./13-change_group`

### 14. Owner and group
**Script:** `14-change_owner_and_group`  
**Description:** Changes owner to "vincent" and group owner to "staff" for all files and directories in the working directory.  
**Command:** Uses `chown -R vincent:staff .`.  
**Usage:** `sudo ./14-change_owner_and_group`

### 15. Symbolic links
**Script:** `15-symbolic_link_permissions`  
**Description:** Changes owner to "vincent" and group owner to "staff" for the symbolic link "_hello".  
**Command:** Uses `chown -h vincent:staff _hello`.  
**Usage:** `sudo ./15-symbolic_link_permissions`

### 16. If only
**Script:** `16-if_only`  
**Description:** Changes owner of "hello" to "vincent" only if it is owned by "guillaume".  
**Command:** Uses conditional check with `stat` and `chown`.  
**Usage:** `sudo ./16-if_only`
