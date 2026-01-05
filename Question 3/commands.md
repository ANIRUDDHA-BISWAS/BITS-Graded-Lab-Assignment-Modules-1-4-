# Question 3 – Linux Links and Disk Usage Management

This document contains the commands executed, outputs observed, and brief explanations for each task performed to understand Linux file linking and disk usage information.

---


## 1. File Creation

### Command:
```
echo "This is sample data for link testing." > ~/sample_data.txt
```

### Explanation:
- Creates a file named sample_data.txt in the home directory.
- Writes sample text into the file.

## 2. Hard Link Creation

### Command:
```
ln ~/sample_data.txt ~/sample_hard.txt
```

### Explanation:
- Creates a hard link named sample_hard.txt.
- Both files point to the same inode on disk.

## 3. Symbolic Link Creation

### Command:
```
ln -s ~/sample_data.txt ~/sample_soft.txt
```

### Explanation:
- Creates a symbolic (soft) link named sample_soft.txt.
- The soft link points to the original file path.

## 4. Inode Verification

### Command:
```
ls -li ~/sample_data.txt ~/sample_hard.txt ~/sample_soft.txt
```

### Explanation:
- Displays inode numbers along with file details.
- Allows comparison of inode values for each file.

## 5. Inode Analysis

### Observation:
```
sample_data.txt and sample_hard.txt share the same inode number.
sample_soft.txt has a different inode number.
```

### Explanation:
- Hard links reference the same inode, meaning they point to the same data on disk.
- A symbolic link has its own inode and stores the path to the target file.

## 6. File Metadata Inspection

### Command:
```
ls -l ~/sample_data.txt
```

### Explanation:
- Displays file permissions, ownership, size, and timestamps.
- Confirms metadata details of the original file.


## 7. Disk Usage Check

### Command:
```
du -sh ~
```

### Explanation:
- Displays total disk usage of the home directory.
- -s shows a summary, and -h formats the output in human-readable units.

## 8. File Size Overview

### Command:
```
ls -lh ~
```

### Explanation:
- Lists all files in the home directory with sizes in human-readable format.
- Helps understand individual file sizes.


## 9. Link Deletion Test

### Command:
```
rm ~/sample_soft.txt
ls ~/sample_data.txt
```

### Explanation:
- Deletes the symbolic link sample_soft.txt.
- The original file sample_data.txt remains unaffected, proving soft link independence.


## 10. Disk Utility Demonstration

### Command:
```
du -h ~
df -h
```

### Explanation:
- du -h ~ shows disk usage of directories and files under the home directory.
- df -h displays overall filesystem disk space, including total, used, and available space in human-readable format.


