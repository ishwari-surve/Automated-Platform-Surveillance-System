# Automated Platform Surveillance System

A Python-based automation project designed to continuously monitor system resources and generate detailed surveillance logs at scheduled intervals.

The application collects information about CPU usage, RAM usage, Disk usage, Network activity, and Running Processes, then stores the collected information in timestamped log files for future analysis and monitoring.

---

##  Features

### System Monitoring
* CPU Usage Monitoring
* RAM Usage Monitoring  
* Disk Usage Monitoring (All Partitions)
* Network Activity Monitoring (Sent/Received)

### Process Monitoring
* Process ID (PID)
* Process Name
* Username
* Process Status
* Process Creation Time
* CPU Consumption per Process
* Memory Consumption per Process

### Automated Logging
* Generates timestamped log files
* Stores logs in user-defined directory
* Creates structured surveillance reports
* Prevents log file overwrites

### Scheduler Support
* Periodic execution using schedule library
* User-defined monitoring intervals
* Continuous background monitoring
* Lightweight & efficient

### Command Line Interface
* Help option (`--h`)
* Usage option (`--u`)
* User-defined time interval
* User-defined log directory

---

## Technologies Used

* **Python 3.x**
* **psutil** - System and process monitoring
* **schedule** - Job scheduling
* **os** - File system operations
* **sys** - Command line arguments
* **time** - Timestamp generation & formatting

---

##  Project Structure
```bash
Automated-Platform-Surveillance-System/
│
├── surveillance.py
├── requirements.txt
├── logs/
│ ├── SysAudit_2026-08-31_21-00-00.log
│ ├── SysAudit_2026-08-31_21-00-00.log
│ └── SysAudit_2026-08-31_21-00-00.log
│
└── README.md
```


---

##  Installation

### Clone Repository
```bash
git clone https://github.com/YourUsername/Automated-Platform-Surveillance-System.git
```

### Navigate to Repository
```bash
cd Automated-Platform-Surveillance-System
```

### Install Required Packages
```bash
pip install -r requirements.txt
```

Or install manually:
```bash
pip install psutil
pip install schedule
```

---

##  Usage

### Display Help
```bash
python surveillance.py --h
```
Shows project description and features.

### Display Usage
```bash
python surveillance.py --u
```
Shows how to run the script.

### Start Surveillance
```bash
python surveillance.py 5 SystemLogs
```

**Parameters:**
* `5` → Time interval in minutes
* `Logs` → Directory where log files will be created

The application will automatically generate a surveillance log every 5 minutes.

**Example:** Monitor every 10 minutes
```bash
python surveillance.py 10 SystemLogs
```

---

##  Sample Log Report
```bash
---- Automated Platform Surveillance System -----
Log created at : Thu Feb 07 21:00:00 2026
SYSTEM REPORT

CPU Usage : 18 %
RAM Usage : 45 %

Disk Usage Report:
C:\ -> 62 % used
D:\ -> 51 % used

Network Usage:
Sent : 245.32 MB
Recv : 512.64 MB

PROCESS REPORT
PID : 1234
Name : chrome.exe
Username : Admin
Status : running
Start Time : 2026-02-07 10:15:30
CPU % : 5.20
Memory % : 8.45
PID : 5678
Name : python.exe
Username : Admin
Status : running
Start Time : 2026-02-07 09:45:12
CPU % : 2.10
Memory % : 12.30
End of Log File
```
---

##  Learning Objectives

This project demonstrates:

* Python Automation & Scripting
* System Monitoring & Resource Tracking
* Process Management
* Scheduler Implementation
* Command Line Programming
* File Handling & I/O Operations
* Log Generation
* Exception Handling
* Operating System Utilities
* Data Collection & Analysis
* Object-Oriented Concepts

---

##  Future Enhancements

* Email Notifications for alerts
* PDF Report Generation
* CSV Export for data analysis
* Real-Time Dashboard
* GUI Application with Tkinter
* Database Storage (SQLite/MySQL)
* Process Filtering & Monitoring
* Resource Threshold Alerts
* Cloud Log Storage
* Process Kill Functionality

---

##  Use Cases

* System Administration
* Server Monitoring
* Resource Utilization Analysis
* Performance Optimization
* Process Tracking & Management
* Infrastructure Health Checks
* Development & Automation Learning
* Educational Projects
* System Auditing

---

##  How It Works

**Step 1:** User runs the script with time interval and directory
**Step 2:** Script creates folder if it doesn't exist
**Step 3:** Scheduler registers periodic job
**Step 4:** Every N minutes:
   - Collects system metrics (CPU, RAM, Disk, Network)
   - Scans all running processes
   - Generates timestamped log file
   - Writes structured report
**Step 5:** Logs accumulate for analysis

---

##  Requirements

* Python 3.6 or higher
* pip (Python package manager)
* Windows/Linux/macOS

---

##  Author

**Ishwari Vijaykumar Surve**

---

##  Repository Highlights
- Real-Time System Monitoring
- Automated Log Generation  
- Process Surveillance
- Scheduler-Based Execution
- Command Line Support
- Timestamped Reports
- Exception Handling
- Python Automation Project
- Production-Ready Code

---

##  License

This project is developed for **educational, learning, and portfolio purposes**.






