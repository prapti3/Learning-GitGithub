## 📄 hooks.md
# 🪝 Git Hooks – Automate Tasks in Your Workflow
- Git hooks are scripts that run automatically when certain Git events occur. They're useful for enforcing standards, automating tasks, or integrating tools in your development lifecycle.

---
<br>

### 🔧 Where Are Hooks Stored?
- Inside your Git repo:
  - `.git/hooks/`
- This folder contains sample scripts like pre-commit.sample, post-commit.sample, etc.
- To activate a hook:
  1. Remove the .sample extension
  2. Make the file executable

    - `chmod +x pre-commit`
 
  ---
  <br>

## 🧩 Types of Git Hooks
#### Hooks are divided into client-side and server-side.

### 🔹 Client-Side Hooks (on developer's machine)

| Hook                 | Triggered When…                        | Use Case                              |
| -------------------- | -------------------------------------- | ------------------------------------- |
| `pre-commit`         | Before a commit is created             | Lint code, run tests                  |
| `prepare-commit-msg` | Before the commit message editor opens | Auto-fill message with ticket ID      |
| `commit-msg`         | After commit message is entered        | Validate commit format (e.g. JIRA ID) |
| `pre-push`           | Before pushing to a remote             | Run tests before push                 |
| `post-commit`        | After commit is created                | Send notification, log info           |


### 🔹 Server-Side Hooks (on Git server)

| Hook           | Triggered When…           | Use Case                        |
| -------------- | ------------------------- | ------------------------------- |
| `pre-receive`  | Before a push is accepted | Enforce policy, reject bad code |
| `update`       | During push               | Check ref updates               |
| `post-receive` | After a push is accepted  | Trigger CI/CD, send email       |

---
<br>


### ✍️ Example: A pre-commit Hook
- Create a file at .git/hooks/pre-commit:

```
#!/bin/sh
echo "Running pre-commit checks..."
npm run lint
if [ $? -ne 0 ]; then
  echo "❌ Lint failed. Commit aborted."
  exit 1
fi
```

---
<br>

- Make it executable:
```
chmod +x .git/hooks/pre-commit
```

- Now every commit runs linting first.

---
<br>

## 🚫 Limitations
- Hooks are not shared across systems by default (not version controlled).
- Solutions: use Husky (for JS projects) or custom scripts to set up hooks on clone.


---
<br>

## 🚀 Tools for Managing Hooks


| Tool                                                                 | Description                                   |
| -------------------------------------------------------------------- | --------------------------------------------- |
| [Husky](https://typicode.github.io/husky)                            | Easily manage Git hooks in JS projects        |
| [lefthook](https://evilmartians.com/chronicles/introducing-lefthook) | Language-agnostic hook manager                |
| [pre-commit](https://pre-commit.com/)                                | Framework for multi-language pre-commit hooks |


---
<br>


## 📌 Summary
- Git hooks are scripts triggered by Git events.
- They help automate tasks like linting, testing, or formatting.
- You need to manually install or manage them per system/repo.



