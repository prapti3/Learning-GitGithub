# 🧱 git init

`git init` is the first command you’ll run when starting a new Git project.

---

## 🔹 What it Does

It **initializes a new Git repository** in your project folder.  
This creates a hidden `.git` directory where Git stores all version history and configuration for that repo.

---

## 🔹 Syntax

- bash
`git init`

---

## 🔹 Example

- mkdir my-first-git-project
- cd my-first-git-project
- git init

---

## 🔹 What Gets Created?
After running git init, Git adds a hidden .git/ folder inside your project directory:


.git/
├── config
├── HEAD
├── refs/
├── objects/


#### 💡 Do NOT delete or modify .git/ — this is your repo’s brain!


---

## 🔹 Check if Git is Tracking
Use this command to see if Git has started tracking the folder:

- git status

---

## 🧠 Tips

- Use git init only once per project.
- If you're cloning an existing project from GitHub, you don’t need to run git init — git clone does it automatically.

---


## 🧪 Practice Task

- Create a folder git-init-demo/
- Run git init inside it
- Create a file like hello.txt
- Run
  - git add hello.txt
  - git commit -m "First commit after init"





