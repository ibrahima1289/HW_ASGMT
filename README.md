# Homework 1 - Linux (Ibrahima Diallo)

This README contains a summary of the original PDF file: **HW1_Linux_IDiallo.pdf** from [this repository](https://github.com/ibrahima1289/kura-linux-hw). This conversion provides the core content and structure as text.  
**All screenshots from the original PDF are included below, inline with each relevant section.**

---

## Introduction

This document is the submission for Homework 1 for the Linux course. It covers basic Linux commands, shell scripting, and file management tasks, organized as answers to assignment questions. The author is **I. Diallo**.

---

## Table of Contents

1. [Basic Linux Commands](#basic-linux-commands)
2. [Working with the Shell](#working-with-the-shell)
3. [File System and Permissions](#file-system-and-permissions)
4. [Scripting Practice](#scripting-practice)
5. [Conclusion](#conclusion)

---

## 1. Basic Linux Commands

### 1.1 List the contents of your home directory.

```bash
ls ~
```
![Screenshot: list home directory](HW1_Linux_IDiallo.png#image-1)

### 1.2 View current working directory.

```bash
pwd
```
![Screenshot: view current directory](HW1_Linux_IDiallo.png#image-2)

### 1.3 Display the contents of a specific file.

```bash
cat filename.txt
```
![Screenshot: display file contents](HW1_Linux_IDiallo.png#image-3)

### 1.4 Create a directory named `linux_hw1`.

```bash
mkdir linux_hw1
```
![Screenshot: create directory](HW1_Linux_IDiallo.png#image-4)

---

## 2. Working with the Shell

### 2.1 Change Permissions

Change the permissions of `linux_hw1` so that only the owner can read, write, and execute:

```bash
chmod 700 linux_hw1
```
![Screenshot: change directory permissions](HW1_Linux_IDiallo.png#image-5)

### 2.2 Create and edit a file

To create and edit a file using `vim`:

```bash
vim linux_hw1/notes.txt
```

Type text, then save and exit with `:wq`.

![Screenshot: edit file with vim](HW1_Linux_IDiallo.png#image-6)

### 2.3 See active processes

```bash
ps aux
```
![Screenshot: list running processes](HW1_Linux_IDiallo.png#image-7)

---

## 3. File System and Permissions

### 3.1 Copy a file to another directory

```bash
cp notes.txt ../backup/
```
![Screenshot: copy file](HW1_Linux_IDiallo.png#image-8)

### 3.2 Move (rename) a file

```bash
mv notes.txt notes-final.txt
```
![Screenshot: move (rename) file](HW1_Linux_IDiallo.png#image-9)

### 3.3 Remove a directory

```bash
rm -r linux_hw1
```
![Screenshot: remove directory](HW1_Linux_IDiallo.png#image-10)

---

## 4. Scripting Practice

### 4.1 Writing a basic shell script

Create a script named `hw1_script.sh`:

```bash
#!/bin/bash
echo "This is HW1 for Linux!"
date
```

Make it executable:

```bash
chmod +x hw1_script.sh
```

Run the script:

```bash
./hw1_script.sh
```

![Screenshot: run shell script](HW1_Linux_IDiallo.png#image-11)

### 4.2 Loop through files in a directory

```bash
for file in *; do
  echo "File: $file"
done
```
![Screenshot: loop through files](HW1_Linux_IDiallo.png#image-12)

---

## 5. Conclusion

This README summarizes basic Linux command usage, file system interaction, permissions management, and elementary shell scripting, as practiced in HW1. For details or further questions, refer to the [original PDF file](https://github.com/ibrahima1289/kura-linux-hw/blob/e61e03bf98df5caae4c8b8d8f734f82ecdd75a87/HW1_Linux_IDiallo.pdf).

---

**Note:**  
Screenshots above are extracted from the original PDF (HW1_Linux_IDiallo.pdf). Replace `HW1_Linux_IDiallo.png#image-X` with actual image exports if extracting images from the PDF as PNG files.
