# 🌿 Main vs Develop Branch in Git

In a collaborative Git workflow like Git Flow, two key branches are used:
- `main`: production-ready branch
- `develop`: development integration branch

---
<br>

## 🔹 `main` Branch

### ✅ Purpose
- Represents the **stable** and **deployable** version of the code.
- Contains only tested, reviewed, and production-ready commits.

### 🚀 When to Use
- Deploying to production.
- Hotfixes or emergency patches.

### 🛑 Best Practices
- Never commit directly to `main`.
- All merges should come through pull requests (usually from `develop` or hotfix branches).

---
<br>


## 🔸 `develop` Branch

### 🔧 Purpose
- Integration branch for ongoing **development work**.
- Collects all feature branches and bug fixes before going to `main`.

### 👨‍💻 When to Use
- Creating new features or updates.
- Team collaboration before production deployment.

### 🛠️ Best Practices
- Frequently merged with feature branches.
- Regularly updated with `main` to avoid conflicts.

---
<br>

## 🔁 Workflow Example

```mermaid
gitGraph;
   commit id: "Initial commit";
   branch main;
   commit id: "Production v1.0";
   branch develop;
   commit id: "Add login";
   commit id: "Fix login bug";
   checkout main;
   merge develop;
   commit id: "Release v1.1";

```

### 📌 Summary Table :

| Branch    | Purpose                  | Stability | Who works on it       | When to merge      |
| --------- | ------------------------ | --------- | --------------------- | ------------------ |
| `main`    | Stable, production-ready | ✅ High    | Release Managers      | After full testing |
| `develop` | Staging for new features | ⚠️ Medium | Developers & QA teams | Feature complete   |


---
<br>


### ✅ Example Commands : 

```
# Switch to develop and create a feature
git checkout develop
git checkout -b feature/ui-redesign

# After testing, merge into develop
git checkout develop
git merge feature/ui-redesign

# After QA approval, merge into main
git checkout main
git merge develop
```


---
<br>

### 📚 Final Tips

- Think of main as what’s live and develop as what’s coming next.
- Always test changes in develop before promoting to main.
- If using GitHub, protect main with branch protection rules.





















