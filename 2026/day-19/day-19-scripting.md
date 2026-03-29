⏰ CRONTAB (Scheduler)
🧠 Basics
Cron = automatic task runner
Background me kaam karta hai
📌 Format
minute hour day_of_month month day_of_week command
🎯 Important Points
* = every value
Always use full path
Cron ka environment limited hota hai
Logs manually handle karne padte hain
⚙️ Commands
crontab -e → edit
crontab -l → list
crontab -r → remove
💾 BACKUP (Data Safety)
🧠 Basics
Backup = data copy banana
Data loss se bachata hai
🎯 Important Points
Always use timestamp (date-time)
Compression use karo (storage save)
Backup location alag rakho
Regular schedule (cron use karo)
📦 Types
Full backup
Incremental backup
Differential backup
🔄 ROTATION (Cleanup System)
🧠 Basics
Old backups delete karna
Storage manage karna
🎯 Important Points
mtime → file age check
Fixed retention policy (e.g. 7 days)
Sirf specific files delete karo (pattern use karo)
Automation zaroori (cron)
🔁 REDIRECTION (IMPORTANT)
🧠 Basics
Output aur error ko control karna
🎯 Points
> → overwrite
>> → append
2> → error
2>&1 → error + output same jagah
🔒 STRICT MODE (VERY IMPORTANT)
🧠 Basics
Script ko safe banata hai
🎯 Points
set -e → error pe stop
set -u → undefined variable error
set -o pipefail → pipe fail detect

👉 DevOps me always use karo

🧠 GENERAL BEST PRACTICES
Always use absolute paths
Logging maintain karo
Scripts ko executable banao
Test before cron
Small reusable functions likho
🎯 ONE-LINE MEMORY CHEAT 💯
Cron → schedule
Backup → copy data
Rotation → delete old
Redirection → output control
Strict mode → safety
