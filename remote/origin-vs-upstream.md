# 🌐 origin vs upstream in Git

When working with **forked repositories**, you’ll often deal with two remotes:
- `origin`
- `upstream`

Let’s understand the difference between them and when to use each.

---

## 🔹 What is `origin`?

- `origin` is the **default remote name** Git gives to the **repository you cloned**.
- It usually points to **your own copy** of the repo.

```bash
git remote add origin https://github.com/your-username/repo.git

Used for:
Pushing and pulling your own changes.

```

## 🔹 What is upstream?
- upstream is a name you manually assign to the original repository you forked from.
- It points to the main source repo — maintained by someone else (e.g., open-source project).

`git remote add upstream https://github.com/original-owner/repo.git`


### ✅ Used for:
- Fetching updates from the original repo, so you can stay in sync.


---

```
🧪 Example Scenario

 - You forked a repo and cloned it:
   
git clone https://github.com/your-username/repo.git
cd repo/
git remote add upstream https://github.com/original-owner/repo.git


1. git fetch upstream               # Get updates from original repo
2. git checkout main
3. git merge upstream/main          # Merge upstream changes
4. git push origin main             # Push merged changes to your fork


```

### 🧠 Check Your Remotes

`git remote -v`

### Output Examples : 
- origin    https://github.com/your-username/repo.git (fetch)
- origin    https://github.com/your-username/repo.git (push)
- upstream  https://github.com/original-owner/repo.git (fetch)
- upstream  https://github.com/original-owner/repo.git (push)

### 📝 When Do You Use This?

1. When working with forked repos (e.g., contributing to open source).
2. To sync your fork (origin) with the original project (upstream).
3. To avoid getting out of date with the latest updates from the source.

---

### ✅  Quick Commands Recap 

1. Add upstream remote
`git remote add upstream <url>`

2. Fetch latest from upstream
`git fetch upstream`

3. Merge upstream changes
`git merge upstream/main`

4. Push to your origin
`git push origin main`










