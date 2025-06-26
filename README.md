# 💾 Automated Backup Script 🛡️

This Python script automatically backs up a specified folder (`data`) by compressing its contents into a timestamped `.zip` file and saving it to a `backups` folder. It also logs every action to `backup.log`.

---

## 📂 Features

- 🗂️ Backs up an entire folder (recursive)
- 🕓 Adds timestamps to each backup
- 🗜️ Compresses files into `.zip` format
- 📜 Generates a log of every file backed up
- 📁 Saves backups in a dedicated folder

---

## 🧰 Folder Structure

```

project/
├── backup\_script.py
├── data/                # 📂 Source folder to back up
│   └── test.txt         # 🧪 Sample file to test backup
├── backups/             # 📦 Backup output (auto-created)
└── backup.log           # 📜 Log file (auto-generated)

````

> ✅ Make sure your `data/` folder exists before running the script!

---

## ⚙️ How It Works

1. Reads files from the `data/` directory
2. Creates a `.zip` file named like `backup_YYYYMMDD_HHMMSS.zip`
3. Saves the backup in `backups/`
4. Logs each backed-up file into `backup.log`

---

## 🚀 How to Run

### 🔹 Step-by-step:

1. 🐍 Make sure Python 3 is installed.
2. 🧪 Ensure you have the `data/` folder with files (e.g., `test.txt`).
3. ▶️ Run the script:

```bash
python backup_script.py
````

### ✅ Output:

* A `.zip` file in the `backups/` folder
* Log entries in `backup.log`
* Example terminal output:

  ```
  ✅ Backup successful: backups/backup_20250621_164530.zip (0.01 MB)
  ```

---

## 📝 test.txt Sample Content

```
This is a test file for the automated backup script.
Today's date is 21st June 2025.
The script should back this file up into a zip file.
```

---

## 🔍 Logs

Every backup operation and file archived is logged in `backup.log` like:

```
2025-06-21 16:45:30 - INFO - Backed up: data/test.txt as test.txt
2025-06-21 16:45:30 - INFO - Backup created: backup_20250621_164530.zip (0.01 MB)
```

---

## 📌 Customization

* Change the folder to back up:

  ```python
  SOURCE_FOLDER = "your_folder_name"
  ```

* Change the backup destination:

  ```python
  BACKUP_FOLDER = "your_backup_folder"
  ```

---

## 📬 Feedback

Have improvements or suggestions? Open a pull request or drop a comment!

---

Made with 🧠 + 💼 by \Sohail-Ansari

