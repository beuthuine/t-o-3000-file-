# 🔍 Find in Files (Parallel Algorithm Project)

**Course:** Parallel Algorithms  
**Language:** C++  
**Student:** *[Your Name]*  

---

## 🧩 Overview
This project demonstrates how to process large datasets efficiently using C++.  
It simulates an admin searching through thousands of log files for a specific keyword.

It includes **two main programs**:

1. **`GenerateLogs.cpp`** – Automatically generates 3,000 log files with simulated server data.  
2. **`FindInFiles.cpp`** – Provides an interactive console interface that allows the user to:
   - Enter a **search keyword**
   - Specify a **directory path** containing the log files
   - Display **file name**, **line number**, and **log line content** for each match
   - Write all results to `ketqua.txt`

---

## 🧱 Program Features

### 🧮 GenerateLogs.cpp
- Creates a `logs/` directory.
- Generates 3,000 log files named:
log_1.txt, log_2.txt, ..., log_3000.txt

lua
Sao chép mã
- Each file contains **20,000 log lines**.
- Randomly inserts lines like:
User action: login by 99 - success on line XXXX

graphql
Sao chép mã

### 🔍 FindInFiles.cpp
- Provides a **console-based "Find in Files" interface**:
=================== FIND IN FILES ===================
Find what: login by 99
Directory (log folder): D:\logs

kotlin
Sao chép mã
- Displays each result in this format:
logs\log_50.txt - line 9999 - User action: login by 99 - success on line 9999

yaml
Sao chép mã
- Saves all matches into `ketqua.txt`.
- Prints progress summary when finished.

---

## 🧠 Example Output
=================== FIND IN FILES ===================
Find what: login by 99
Directory (log folder): D:\logs

Searching for "login by 99" in directory: D:\logs
logs\log_50.txt - line 9999 - User action: login by 99 - success on line 9999
logs\log_100.txt - line 9999 - User action: login by 99 - success on line 9999
✅ Scanned 3000 files. Results saved to: ketqua.txt

yaml
Sao chép mã

---

## 🛠️ Build & Run Instructions

### 🪟 Using Visual Studio Developer Command Prompt
1. Open **Developer Command Prompt for VS 2022**
2. Go to your project directory:
   ```bash
   cd /d D:\FindInFiles
Compile:

bash
Sao chép mã
cl /EHsc GenerateLogs.cpp
cl /EHsc FindInFiles.cpp
Run the programs:

bash
Sao chép mã
GenerateLogs
FindInFiles
