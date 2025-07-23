# ✅ git commit

The `git commit` command saves your **staged changes** to the local Git repository.  
Each commit creates a snapshot of your project at a specific time.

---

## 🔹 Basic Syntax

- bash
  -  `git commit -m "Your descriptive commit message"`

---

##### The -m flag allows you to write the message inline.

---

## 🔹 Example

- echo "Hello Git" > hello.txt
- git add hello.txt
- git commit -m "Add hello.txt with welcome message"

---

## 🔹 View Commit History

- git log
- git log -oneline

---

## 🔹 Edit Previous Commit Message

- If you made a typo or want to rephrase your last commit message:
  - `git commit --amend -m "New better message"`

---

## 🧪 Practice Task
- Create a file demo.txt
- Write some content in it
- Stage it: git add demo.txt
- Commit it: git commit -m "Add demo.txt with sample content"
- Check history: git log

---

## 🔁 Related Commands
- git status: Check what’s staged/untracked
- git diff: See unstaged changes
- git reset: Undo commits

