# 🚫 .gitignore

The `.gitignore` file tells Git **which files or folders to ignore** — meaning they won’t be tracked or committed.

This is useful for:
- Temporary files
- Build output
- API keys or secret files
- IDE/project settings

---

## 🔹 Syntax

Create a `.gitignore` file in your root directory:

- bash
`touch .gitignore`

---

## 🔹 Add Patterns to ignore Files or Folders

1. Ignore all .log files
`*.log`
2. Ignore a folder named /build
`build/`
4. Ignore specific file
`secrets.txt`
4. Ignore all .class files in any folder
`*.class`

---

## Example .gitignore

1. Java files to ignore
`*.class`
2. IntelliJ IDEA
`.idea/`
`*.iml`
3. Logs
`*.log`
4. OS files
`.DS_Store`
`Thumbs.db`
5. Build directory
`target/`


---

## 🔹 Important Notes
- Files already tracked by Git won’t be ignored unless you remove them.
- To force Git to re-evaluate .gitignore after a file is already tracked:
  `git rm --cached filename`
- Example : `git rm --cached secrets.txt`

---

## 🧪 Practice Task
1. Create a .gitignore file
2.  Add:
  - temp.txt | logs/ | *.log
3. Create those files/folders
4. Run git status — they should be missing from staged changes
5. Add other files and commit as usual

---

## 🔁 Related Commands

- git rm --cached: Remove tracked file but keep it locally
- git status: Shows ignored files if you use --ignored
`git status --ignored`

