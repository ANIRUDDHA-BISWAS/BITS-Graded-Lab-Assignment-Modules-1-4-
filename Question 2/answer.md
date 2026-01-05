# Question 2 – Linux File and Directory Management

This document contains the commands executed, outputs observed, and brief explanations for each task performed as part of Linux file and directory management in the home directory.

---


## 1. Project Workspace Setup

### Command:
```
mkdir ~/documents
```

### Explanation:
- Creates a directory named documents inside the home directory.
- This directory will be used to store project-related files.

## 2. File Creation

### Command:
```
cd ~/documents
touch plan.txt
```

### Explanation:
- cd navigates into the documents directory.
- touch creates an empty file named plan.txt.

## 3. Content Addition

### Command:
```
echo "Project plan: Complete Linux lab tasks on time." > plan.txt
```

### Explanation:
- Writes sample text into the plan.txt file.
- The text serves as a short project note or reminder.

## 4. File Metadata Verification

### Command:
```
ls -l plan.txt
```

### Explanation:
- Displays file permissions, ownership, size, and modification time.
- The output shows my username as the file owner, confirming ownership.

## 5. File Duplication

### Command:
```
cp plan.txt plan_copy.txt
```

### Explanation:
- Creates a copy of plan.txt.
- The duplicated file is named plan_copy.txt.

## 6. Directory Renaming

### Command:
```
cd ~
mv documents project_documents
```

### Explanation:
- Renames the directory from documents to project_documents.
- The new name better reflects the project scope.


## 7. Archival Structure

### Command:
```
mkdir ~/project_documents/archive
```

### Explanation:
- Creates a subdirectory named archive inside project_documents.
- This directory will be used to store archived files.

## 8. File Organization

### Command:
```
mv ~/project_documents/plan_copy.txt ~/project_documents/archive/
```

### Explanation:
- Moves plan_copy.txt into the archive subdirectory.
- This helps organize active and archived files separately.


## 9. Recursive Listing

### Command:
```
ls -R ~/project_documents
```

### Explanation:
- Lists all files and subdirectories recursively.
- Displays the complete directory structure of project_documents.


## 10. Path Verification

### Command:
```
realpath ~/project_documents/archive/plan_copy.txt
```

### Explanation:
- Displays the absolute path of plan_copy.txt.
- Confirms the file’s final location after being moved.

