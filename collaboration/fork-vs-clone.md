# 🔀 Fork vs Clone in Git

When working with GitHub, understanding the difference between **fork** and **clone** is key, especially in collaborative environments.

---
<br>
<br>
<br>

## 🔧 1. What is a Fork?

A **fork** is a copy of a remote repository **on your own GitHub account**.

- 🔁 You fork when you **don’t have write access** to the original repo.
- 💡 Often used to **contribute to open-source projects**.
- 🚫 Forking doesn’t create a local copy — it stays on GitHub until you clone it.

📌 Example:
- Original: `github.com/original-user/project`
- Forked: `github.com/your-username/project`

---

## 💻 2. What is a Clone?

A **clone** is a **local copy** of any repository on your computer.

- ✅ Used to **work offline**, make changes, and push back later.
- 🔐 You can clone your own repo, someone else’s public repo, or a fork.

---  



📌 Command:

```bash
`git clone <repo-url>`

Example :
`git clone https://github.com/your-username/project.git`

```



## 📊 Fork vs Clone – Quick Comparison

| Feature              | Fork                          | Clone                      |
| -------------------- | ----------------------------- | -------------------------- |
| Location             | GitHub (remote)               | Your computer (local)      |
| Permission Needed    | No (for public repos)         | No                         |
| When to Use          | To contribute to others' code | To start local development |
| Can Push to Original | No (only via PR)              | Yes (if you have access)   |
| Creates GitHub Copy  | ✅ Yes                         | ❌ No                       |
| Creates Local Copy   | ❌ No                          | ✅ Yes                      |




### 🧠 Best Practice
 - 🔸 Fork → Clone → Create new branch → Make changes → Push → Create PR.



### ✅ Summary
- Fork = GitHub-level duplication for collaboration.
- Clone = Local copy for actual development.


