## 📄 tag.md
# 🔖 git tag – Mark Important Points in Git History
- Tags are used to mark specific points in Git history — like releases (v1.0, v2.1, etc.).

<br>

### 🎯 Why Use Tags?
- Highlight important commits (like release versions).
- Easily reference or go back to specific versions.
- Tags are useful for CI/CD, deployment, and versioning.

---

### 🏷️ Types of Tags
| Type            | Description                                                                 |
| --------------- | --------------------------------------------------------------------------- |
| **Lightweight** | A simple pointer to a commit.                                               |
| **Annotated**   | Includes metadata (tagger, date, message). Recommended for release tagging. |


---
<br>

### ✨ Create a Tag
```
#### ✅ Lightweight Tag 
`git tag v1.0`

#### ✅ Annotated Tag
`git tag -a v1.0 -m "Release version 1.0"`

#### 🔍 View Tags
`git tag`
- To filter:
`git tag -l "v1.*"`
```


---


### 📌 Tag a Specific Commit
`git tag -a v1.1 <commit-hash> -m "Tagging v1.1"`


### ⬆️ Push Tags to Remote
1. Push a single tag:
   - `git push origin v1.0`
2. Push all tags:
   - `git push origin --tags`


---
<br>

### 🧽 Delete Tags
1. Locally:
   - ` git tag -d v1.0`
2. From remote:
   - `git push origin --delete tag v1.0`

---
<br>


### 🛫 Checkout a Tag (Detached HEAD)

`git checkout v1.0`
- You are now in a detached HEAD state (not on a branch).

---
<br>


### 🧠 Pro Tip
- Use annotated tags for anything you want to share or publish.
- Tags don’t move automatically — they are fixed to a commit.


---
<br>

### 📁 Example Workflow
```
git tag -a v2.0 -m "Stable release v2.0"
git push origin v2.0
```

## Done! You’ve versioned your project cleanly.







  
