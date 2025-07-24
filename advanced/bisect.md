## 📄 bisect.md
# 🔍 git bisect – Debugging Made Easy
- git bisect helps you automatically find the commit that introduced a bug by using binary search.
- It’s like narrowing down a detective investigation — fast and smart.

---
<br>

### 🧠 When to Use
- Use git bisect when:
- A bug appeared, but you don’t know which commit caused it.
- You know a good commit (bug-free) and a bad commit (has the bug).

---
<br>


### 🔁 How It Works
- Git will:
- Check out a middle commit.
- You test the code and tell Git if the commit is good or bad.
- It continues the search until the exact bad commit is found.

---
<br>

## 🧪 Example: Find Buggy Commit
```

Step 1: Start Bisect
git bisect start

Step 2: Mark the Bad Commit (current one)
git bisect bad

Step 3: Mark a Known Good Commit
git bisect good abc1234

```

#### Git now checks out a commit in the middle.


---
<br>

### 🧹 After Each Step

- You test the code.
- Then run either:
```
git bisect good
or
git bisect bad

```
- Git will keep narrowing down the range.

---
<br>


### 🎯 When Bug is Found
- Git will show:
  `<bad_commit_hash> is the first bad commit`
- End the session:
  `git bisect reset`
- This takes you back to your original branch.


 ---
 <br>

 ### ⚡ Advanced: Automate Testing

 - You can even script the test:
   `git bisect run ./test_script.sh`

- Git will run the script after each checkout and mark it good/bad based on the exit code.

---
<br>

### 📌 Summary Commands
| Action             | Command                  |
| ------------------ | ------------------------ |
| Start bisect       | `git bisect start`       |
| Mark current bad   | `git bisect bad`         |
| Mark known good    | `git bisect good <hash>` |
| Mark tested result | `git bisect good/bad`    |
| Stop bisecting     | `git bisect reset`       |

---
<br>

### 🛠️ Real-World Tip

- Use it when you:
   - Introduce a regression.
   - Want to find root cause of issues after merges or refactoring.

















