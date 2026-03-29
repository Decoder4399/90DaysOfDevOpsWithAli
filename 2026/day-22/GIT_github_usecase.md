# 🚀 Git & GitHub Cheatsheet (Beginner → Advanced)

---

# 🧠 WHAT IS GIT?

* Git = Version Control System
* Code ka history track karta hai
* Changes ko save, compare aur restore karne me help karta hai

---

# 🌐 WHAT IS GITHUB?

* GitHub = cloud platform for Git repositories
* Code store, share aur collaborate karne ke liye use hota hai

---

# ⚙️ SETUP COMMANDS

```bash
git config --global user.name "Your Name"
```

👉 Git ko batata hai kaun commit kar raha hai

```bash
git config --global user.email "your@email.com"
```

👉 commit ke saath email attach hota hai

```bash
git config --list
```

👉 current configuration dekhne ke liye

---

# 📁 REPOSITORY COMMANDS

```bash
git init
```

👉 new Git repository initialize karta hai

```bash
git clone <repo-url>
```

👉 remote repository ko local machine pe copy karta hai

---

# 🔄 BASIC WORKFLOW COMMANDS

```bash
git status
```

👉 current changes aur state show karta hai

```bash
git add <file>
```

👉 specific file ko staging area me add karta hai

```bash
git add .
```

👉 sabhi changes ko staging me add karta hai

```bash
git commit -m "message"
```

👉 staged changes ko save karta hai (snapshot banata hai)

---

# 🔍 HISTORY & LOGS

```bash
git log
```

👉 commit history show karta hai

```bash
git log --oneline
```

👉 short format me history

```bash
git diff
```

👉 changes compare karta hai

---

# 🔙 UNDO & RESET

```bash
git reset --soft HEAD~1
```

👉 last commit remove karta hai, changes safe rehte hain

```bash
git reset --hard HEAD~1
```

👉 last commit aur changes dono delete ⚠️

```bash
git checkout -- <file>
```

👉 file ko previous state me laata hai

---

# 🌿 BRANCHING

```bash
git branch
```

👉 saare branches list karta hai

```bash
git branch <branch-name>
```

👉 new branch create karta hai

```bash
git checkout <branch-name>
```

👉 branch switch karta hai

```bash
git checkout -b <branch-name>
```

👉 create + switch ek saath

```bash
git merge <branch-name>
```

👉 branch ko current branch me merge karta hai

---

# 🌐 REMOTE (GITHUB)

```bash
git remote add origin <repo-url>
```

👉 remote repository connect karta hai

```bash
git remote -v
```

👉 remote URLs show karta hai

---

# ⬆️ PUSH & ⬇️ PULL

```bash
git push -u origin main
```

👉 local commits ko GitHub pe upload karta hai

```bash
git push
```

👉 latest changes push karta hai

```bash
git pull
```

👉 remote se latest changes fetch + merge karta hai

```bash
git fetch
```

👉 sirf changes download karta hai (merge nahi karta)

---

# 🔁 REBASE (ADVANCED)

```bash
git rebase main
```

👉 current branch ko main ke upar reapply karta hai (clean history)

---

# ⚔️ MERGE CONFLICT

* Jab same line multiple jagah change ho jaye
* Manual resolve karna padta hai

---

# 🧹 STASH (TEMP SAVE)

```bash
git stash
```

👉 temporary changes save karta hai

```bash
git stash pop
```

👉 saved changes wapas laata hai

---

# 🏷️ TAGS

```bash
git tag v1.0
```

👉 version mark karta hai

---

# 🧠 IGNORE FILES

```bash
.gitignore
```

👉 unwanted files ko ignore karta hai (logs, node_modules, etc.)

---

# 👥 COLLABORATION FLOW

1. clone repository
2. new branch create
3. changes karo
4. add + commit
5. push
6. pull request create
7. merge

---

# ⚠️ BEST PRACTICES

* small commits karo
* clear commit messages likho
* direct main branch pe kaam mat karo
* pull before push
* .gitignore use karo

---

# 🎯 QUICK MEMORY CHEAT

* init → start repo
* clone → copy repo
* add → stage changes
* commit → save changes
* push → upload
* pull → update
* branch → parallel work
* merge → combine
* stash → temporary save

---

# 💥 FINAL RULE

👉 "Commit often, push safely, and never break main branch"

---
