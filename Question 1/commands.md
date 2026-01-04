# Question 1 – Linux Environment Verification  

This document contains the commands executed, outputs observed, and brief explanations for each task performed as part of the basic Linux environment verification.

---

## 1. User Identity Verification

### Command:
```
whoami
groups
```

### Explanation:
- whoami displays the username of the currently logged-in user.  
- groups shows all the groups that the user account belongs to.  
- My login ID appears in the output, confirming user identity.

## 2. Workspace Validation

### Command:
```
pwd
ls -l
```

### Explanation:
- pwd prints the current working directory.
- ls -l lists all files and directories in long format, showing permissions, owner, size, and modification time.

## 3. Environment Confirmation File

### Command:
```
echo "Linux user environment verified" > user_info.txt
```

### Explanation:
- This command creates a file named user_info.txt.
- The specified text is written into the file.

## 4. File Integrity Check

### Command:
```
wc -m user_info.txt
```

### Explanation:
- wc -m counts the total number of characters present in the file.
- This verifies the content length of user_info.txt.

## 5. Learning the Tools (mkdir Manual)

### Command:
```
man mkdir
```

### Useful Option Identified:
```
mkdir -p dir1/dir2/dir3
```

### Explanation:
- The -p option creates parent directories automatically.
- It also prevents errors if the directory already exists.

## 6. Home Directory Inspection

### Command:
```
ls ~ | sort
```

### Explanation:
- ls ~ lists all files and directories in the home directory.
- sort arranges the output alphabetically.






