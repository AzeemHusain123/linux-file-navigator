# 🗂️ Linux File Navigator – C Based File Management System

**Semester:** 4th  
**Course:** Operating Systems (OS)  
**Language:** C  
**Platform:** Linux (Tested on Ubuntu 22.04)  
**Author:** Azeem Husain  

---

## 🧠 Overview

This project is a **Linux-based command-line File Navigator** built in **C**, designed to simulate a lightweight file management system.  
It allows the user to perform common file operations such as creating, copying, moving, deleting, and renaming files, as well as checking and modifying permissions — all from within a single terminal program.

The project demonstrates:
- File and directory manipulation using system calls  
- Working with `dirent.h`, `sys/stat.h`, and `unistd.h`  
- OS-level permission handling and directory traversal  
- Modular C programming with structured functions  

---

## ⚙️ Features

✅ List files in the current directory  
✅ Create new files  
✅ Copy or move files between directories  
✅ Delete or rename files  
✅ Search for files by name  
✅ Change current working directory  
✅ Check file permissions  
✅ Modify file permissions (octal mode)  
✅ Simple and user-friendly command-line interface  

---

## 🧩 Code Structure

| Function | Description |
|-----------|-------------|
| `list_files()` | Displays all files in the given directory |
| `copy_file()` | Copies a file to a destination or directory |
| `move_file()` | Moves a file (implemented using `rename()`) |
| `delete_file()` | Deletes a specified file after confirmation |
| `rename_file()` | Renames a file |
| `search_file()` | Searches for a specific file name in the directory |
| `create_file()` | Creates a new file in the current directory |
| `check_file_permission()` | Displays file permissions for user/group/others |
| `change_permissions()` | Changes file permissions using octal input (e.g. `755`) |

---

## 🛠️ How to Compile and Run

### **Option 1 – Using gcc manually**
```bash
gcc project.c -o file_navigator
./file_navigator
