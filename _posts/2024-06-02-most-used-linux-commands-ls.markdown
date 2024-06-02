---
layout: post
title:  "Most used Linux command: ls"
date:   2024-06-02 22:12:00 +1000
categories: linux
---

## ls

The `ls` command in Linux is used to list the contents of a directory. It has various options that can modify its output to show more detailed information, hidden files, sorted lists, and more. Here are several examples demonstrating different usages of the `ls` command:

### Basic Usage

1. **List Files and Directories**
   ```sh
   ls
   ```
   This command lists the files and directories in the current directory.

### Common Options

2. **List All Files Including Hidden Files**
   ```sh
   ls -a
   ```
   This command lists all files, including hidden files (those starting with a dot `.`).

3. **List in Long Format**
   ```sh
   ls -l
   ```
   This command lists files and directories in a long format, showing detailed information such as permissions, number of links, owner, group, size, and modification time.

4. **List with Human-Readable File Sizes**
   ```sh
   ls -lh
   ```
   This command is similar to `ls -l` but shows file sizes in a human-readable format (e.g., KB, MB).

5. **List Files Sorted by Modification Time**
   ```sh
   ls -lt
   ```
   This command lists files and directories sorted by modification time, with the most recently modified files listed first.

6. **List Files with a Specific Pattern**
   ```sh
   ls *.txt
   ```
   This command lists all files with a `.txt` extension in the current directory.

### Combining Options

7. **List All Files in Long Format Including Hidden Files**
   ```sh
   ls -la
   ```
   This command lists all files, including hidden files, in a long format.

8. **List All Files in Long Format with Human-Readable Sizes**
   ```sh
   ls -lah
   ```
   This command lists all files, including hidden files, in a long format with human-readable file sizes.

### Recursive Listing

9. **List Files Recursively**
   ```sh
   ls -R
   ```
   This command lists all files and directories recursively, displaying the contents of all subdirectories.

### Detailed Examples

10. **List Files with Permissions and Size in Human-Readable Format**
    ```sh
    ls -lh
    ```
    Example output:
    ```
    total 12K
    drwxr-xr-x 2 user user 4.0K Jun  1 12:00 dir1
    -rw-r--r-- 1 user user 1.2K Jun  1 12:01 file1.txt
    -rw-r--r-- 1 user user 2.3K Jun  1 12:02 file2.txt
    ```

11. **List All Files Sorted by Modification Time in Long Format**
    ```sh
    ls -lat
    ```
    Example output:
    ```
    total 12K
    drwxr-xr-x 2 user user 4.0K Jun  1 12:02 .
    -rw-r--r-- 1 user user 2.3K Jun  1 12:02 file2.txt
    -rw-r--r-- 1 user user 1.2K Jun  1 12:01 file1.txt
    drwxr-xr-x 3 user user 4.0K Jun  1 12:00 ..
    drwxr-xr-x 2 user user 4.0K Jun  1 11:59 .hidden
    ```

12. **List Files Recursively with Human-Readable Sizes**
    ```sh
    ls -lRh
    ```
    Example output:
    ```
    .:
    total 12K
    drwxr-xr-x 2 user user 4.0K Jun  1 12:00 dir1
    -rw-r--r-- 1 user user 1.2K Jun  1 12:01 file1.txt
    -rw-r--r-- 1 user user 2.3K Jun  1 12:02 file2.txt

    ./dir1:
    total 8.0K
    -rw-r--r-- 1 user user 1.1K Jun  1 12:03 file3.txt
    -rw-r--r-- 1 user user 1.1K Jun  1 12:04 file4.txt
    ```

### Summary of Options

- **`-a`**: Show all files, including hidden files.
- **`-l`**: Long listing format.
- **`-h`**: Human-readable sizes.
- **`-t`**: Sort by modification time.
- **`-R`**: Recursive listing.

By using these options and combining them as needed, you can customize the output of the `ls` command to meet your specific requirements.

