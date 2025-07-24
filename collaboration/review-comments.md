# 📝 Review Comments in Pull Requests

**Review comments** are feedback left by collaborators or maintainers during a Pull Request (PR) review process. They help improve code quality, maintain consistency, and ensure alignment with project standards.

---
<br>

## 📌 Types of Review Comments

1. ✅ **Approval** – "Looks good to me (LGTM)"
2. ⚠️ **Suggestions** – Recommendations to improve code readability, performance, or maintainability.
3. ❌ **Required Changes** – Critical issues that must be fixed before merging.
4. 💬 **General Discussions** – Open-ended feedback, questions, or clarifications.

---
<br>

## 🔁 Responding to Review Comments

| Action            | What You Should Do                                     |
|-------------------|--------------------------------------------------------|
| ✅ Agree           | Apply the change, commit, and reply with a comment.   |
| ❓ Unsure          | Ask for clarification politely.                        |
| ❌ Disagree        | Provide a logical explanation and discuss respectfully.|

---
<br>

## 🧪 Example Workflow

### 1. Create a Pull Request  
```bash
git checkout -b feature/login
# make changes
git add .
git commit -m "Added login form validations"
git push origin feature/login


```
<br>

### 2. Reviewer Comments

- 🔴 Line 42: Consider using `async/await` instead of `.then()`.
- 🟡 Rename variable `x` to something more descriptive.

<br>

### 3. Make Changes & Push Again
```
# Apply changes
git add .
git commit --amend OR git commit -m "Refactored login logic"
git push origin feature/login
```

<br>

### 4. Reply to Comments

- On the PR page:
- Click “Reply” under each comment.
- Mark as “Resolved” if addressed.


<br> 

### 💡 Best Practices
```
- 💬 Always reply to comments — even if you agree silently.
- 🧹 Avoid ignoring feedback; clarify if you need more info.
- 🧠 Learn from review feedback — it's a great way to grow.
- 🧪 Run tests before pushing changes.
- ✅ Keep your commits clean and relevant to the feedback.
```


<br> 

### ✅ Good Comment Responses
```
- "Thanks! Updated as per suggestion ✅"
- "Used async/await instead of .then() – much cleaner now."
- "I kept the original logic because XYZ, open to further suggestions."
```


<br> 


### 📢 Summary

| Term           | Meaning                                             |
| -------------- | --------------------------------------------------- |
| Review Comment | Feedback on code changes in a PR                    |
| Resolved       | Issue is fixed, acknowledged, or no longer relevant |
| Reply          | Your response to the comment                        |
| Approve        | Reviewer agrees with the code and allows merging    |


---
<br> 



# 👥 Code reviews = Collaboration
- ⭐⭐ Treat them as learning + improvement sessions, not personal criticism.







