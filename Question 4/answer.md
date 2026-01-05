# Question 4 – System Monitoring and Process Management

This document contains the commands executed, outputs observed, and brief explanations for each task performed related to system monitoring, processes, memory, and disk usage.

---


## 1. System Uptime Verification

### Command:
```
uptime
```

### Explanation:
- Displays how long the system has been running since the last boot.
- Also shows the number of logged-in users and load average.

## 2. User Process Listing

### Command:
```
ps -u $USER
```

### Explanation:
- Lists all processes currently running under the logged-in user account.
- Displays process IDs, terminal, CPU time, and command names.

## 3. CPU Usage Analysis

### Command:
```
top -u $USER
```

### Explanation:
- Displays real-time process activity for the current user.
- The process with the highest %CPU value is consuming the most CPU resources.

## 4. Background Process Execution

### Command:
```
sleep 300 &
jobs
```

### Explanation:
- sleep 300 & starts a background process that runs for 300 seconds.
- jobs confirms that the background process is currently running.

## 5. Process Priority Management

### Command:
```
ps -o pid,ni,cmd -u $USER
renice 5 -p <PID>
ps -o pid,ni,cmd -u $USER
```

### Explanation:
- Displays the current niceness (priority) of user processes.
- renice changes the priority of the selected process.
- The updated niceness value confirms the priority change.

## 6. Memory Usage Monitoring

### Command:
```
free -h
```

### Explanation:
- Displays memory usage in a human-readable format.
- Shows total, used, free, shared, buffered, and available memory.


## 7. Disk Space Inspection

### Command:
```
df -h ~
```

### Explanation:
- Displays disk space usage of the filesystem where the home directory resides.
- Shows total, used, available space, and usage percentage.

## 8. Shell Identification

### Command:
```
echo $SHELL
```

### Explanation:
- Displays the name and path of the shell currently in use by the user.

## 9. Output Redirection

### Command:
```
uname -a > system_report.txt
```

### Explanation:
- Redirects the output of the system information command into system_report.txt.
- The file stores system details without displaying them on the terminal.

## 10. Disk Usage Visualization

### Command:
```
ncdu ~
```

### Explanation:
- ncdu provides an interactive disk usage analyzer.
- It shows directory-wise disk usage and helps identify large files and folders visually.



