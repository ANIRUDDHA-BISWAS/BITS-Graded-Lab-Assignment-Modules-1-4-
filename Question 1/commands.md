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


## 7. Log Investigation

### Command:
```
grep "admin" log.txt
```

### Explanation:
- Searches for the word "admin" inside the file log.txt.
- Displays only the lines that contain the matching word.

## 8. System Information Check

### Command:
```
uname -r
```

### Explanation:
- Displays the Linux kernel version currently running on the system.


## 9. Network Connectivity Test

### Command:
```
ping -c 4 www.google.com
```

### Explanation:
- Sends 4 ICMP packets to www.google.com.
- Receiving replies confirms that the system has active network connectivity.


## 10. System Health Awareness

### Command:
```
uptime
```

### Explanation:
- Shows how long the system has been running (uptime).
- Displays the number of logged-in users.
- Shows system load averages for the last 1, 5, and 15 minutes, indicating system workload.
