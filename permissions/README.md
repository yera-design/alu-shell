cat > README.md << 'EOF'
# ALU Shell Scripting Projects

This repository contains shell scripting exercises for the ALX Software Engineering program.

## Project Structure

### 1. `permissions/` - File and Directory Permissions
Scripts demonstrating various file and directory permission operations.

**Scripts:**
- **0-iam_betty** - Switches current user to user "betty"
- **1-who_am_i** - Prints effective username of current user
- **2-groups** - Prints all groups current user is part of
- **3-new_owner** - Changes owner of file "hello" to user "betty"
- **4-empty** - Creates an empty file called "hello"
- **5-execute** - Adds execute permission to owner of file "hello"
- **6-multiple_permissions** - Adds execute to owner/group, read to others for "hello"
- **7-everybody** - Adds execute permission to all users for "hello"
- **8-James_Bond** - Sets permissions to 007 (owner: none, group: none, others: all)
- **9-John_Doe** - Sets permissions to 753 (rwxr-x-wx) for "hello"
- **10-mirror_permissions** - Sets "hello" permissions to match "olleh"
- **11-directories_permissions** - Adds execute to all subdirectories for all users
- **12-directory_permissions** - Creates directory "my_dir" with permissions 751
- **13-change_group** - Changes group owner of "hello" to "school"
- **14-change_owner_and_group** - Changes owner to "vincent" and group to "staff" for all files
- **15-symbolic_link_permissions** - Changes owner/group of symbolic link "_hello" to vincent/staff
- **16-if_only** - Changes owner of "hello" to "vincent" only if owned by "guillaume"
