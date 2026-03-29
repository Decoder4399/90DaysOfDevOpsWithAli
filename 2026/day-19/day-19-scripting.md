# 🧠 DevOps Shell Scripting Revision Notes (Cron, Backup, Rotation)

---

## ⏰ CRONTAB (Scheduler)

### Basics

* Cron = automatic task runner (background me chalta hai)
* Repetitive tasks automate karta hai

### Format

```
minute hour day_of_month month day_of_week command
```

### Key Points

* `*` = every value
* Always use **absolute/full path**
* Cron ka environment limited hota hai (PATH issue aa sakta hai)
* Output by default store nahi hota → logging zaroori

### Commands

* `crontab -e` → edit cron jobs
* `crontab -l` → list cron jobs
* `crontab -r` → remove all cron jobs

---

## 💾 BACKUP (Data Safety)

### Basics

* Backup = data ki copy banana
* Data loss se protection

### Key Points

* Always use **timestamp (date-time)** in backup names
* Compression use karo (space save hota hai)
* Backup location **source se alag** rakho
* Regular backup schedule (cron ke through)

### Types

* Full Backup → sab kuch copy
* Incremental → sirf changes copy
* Differential → last full backup ke baad ka data

---

## 🔄 ROTATION (Cleanup System)

### Basics

* Old backups/logs delete karna
* Storage manage karna

### Key Points

* `mtime` → file age check karta hai
* Retention policy define karo (e.g. 7 days)
* Specific files target karo (pattern use karo)
* Automation via cron zaroori

---

## 🔁 OUTPUT REDIRECTION

### Basics

* Output aur error ko control karna

### Key Points

* `>` → overwrite
* `>>` → append
* `2>` → error output
* `2>&1` → error + normal output same jagah

---

## 🔒 STRICT MODE (Script Safety)

### Basics

* Script ko safe aur predictable banata hai

### Key Points

* `set -e` → error aate hi script stop
* `set -u` → undefined variable error
* `set -o pipefail` → pipe me kisi bhi command ka fail detect

👉 DevOps me **recommended best practice**

---

## 🧠 GENERAL BEST PRACTICES

* Always use **absolute paths**
* Proper logging maintain karo
* Script ko executable banao (`chmod +x`)
* Cron me use karne se pehle manual test karo
* Reusable functions likho
* Error handling include karo

---

## 🎯 QUICK MEMORY CHEAT

* Cron → Schedule automate
* Backup → Data copy
* Rotation → Old data delete
* Redirection → Output control
* Strict mode → Script safety

---
