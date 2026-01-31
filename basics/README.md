# Shell Basics Scripts

This directory contains shell scripts for ALX shell basics exercises.

## Script Descriptions

### **0-current_working_directory**
**What it does:** Prints the absolute path of the current working directory  
**Command used:** `pwd`

### **1-listit**
**What it does:** Lists files and directories in current directory  
**Command used:** `ls`

### **2-bring_me_home**
**What it does:** Changes directory to home directory  
**Command used:** `cd ~`

### **3-listfiles**
**What it does:** Lists files in long format  
**Command used:** `ls -l`

### **4-listmorefiles**
**What it does:** Lists all files (including hidden) in long format  
**Command used:** `ls -la`

### **5-listfilesdigitonly**
**What it does:** Lists files with numeric user and group IDs  
**Command used:** `ls -la -n`

### **6-firstdirectory**
**What it does:** Creates a directory in /tmp  
**Command used:** `mkdir /tmp/my_first_directory`

### **7-movethatfile**
**What it does:** Moves a file to a directory  
**Command used:** `mv /tmp/betty /tmp/my_first_directory/betty`

### **8-firstdelete**
**What it does:** Deletes a file  
**Command used:** `rm /tmp/my_first_directory/betty`

### **9-firstdirdeletion**
**What it does:** Deletes a directory  
**Command used:** `rm -rf /tmp/my_first_directory`

### **10-back**
**What it does:** Changes to previous directory  
**Command used:** `cd -`

### **11-lists**
**What it does:** Lists files in multiple directories  
**Command used:** `ls -la`, `ls -la ..`, `ls -la /boot`

### **12-file_type**
**What it does:** Displays file type  
**Command used:** `file /tmp/iamafile`

### **13-symbolic_link**
**What it does:** Creates symbolic link to /bin/ls  
**Command used:** `ln -s /bin/ls __ls__`

### **14-copy_html**
**What it does:** Copies HTML files to parent directory  
**Command used:** `cp -u *.html ..`

### **15-lets_move**
**What it does:** Moves files starting with uppercase letters  
**Command used:** `mv [A-Z]* /tmp/u/`

### **16-clean_emacs**
**What it does:** Deletes backup files ending with ~  
**Command used:** `rm *~`

### **17-tree**
**What it does:** Creates nested directories  
**Command used:** `mkdir -p welcome/to/school`

## Requirements
- All scripts are exactly 2 lines
- All scripts start with `#!/bin/bash`
- All files end with a newline
- Scripts are executable

## How to Run
```bash
# Make all scripts executable
chmod +x *

# Run any script
./0-current_working_directory
