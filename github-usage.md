**Date:** 09 July 2025
# Deleting a GitHub Repository
I have a Repo I don't need (created at the beginning of the account when I didn't know how to use it...)
## ⚠️ Before Starting 
- Deleting a repository is permanent
- All code, issues, pull request (I have no idea what that is...), and wiki data will be deleted.
- Make sure to back up anything important first!
## 🧨 How to Delete a GitHub Repository (via the website):
1. Go to https://github.com and log into your account.
2. Open the **repository you want to delete**.
3. Click on the Settings tab
   (⚠️ *This is a tab inside the repo*, not your account settings)
4. Scroll all the way to the **bottom of the Settings** page.
5. Under the **"Danger Zone"**, you’ll see: 
*🗑️ Delete this repository*
6. Click “Delete this repository”
7. GitHub will ask you to type the repo’s full name to confirm (e.g., yourusername/reponame).
8. Click **“I understand the consequences, delete this repository”**

All of this steps make it seam like a big deal. Will be carful from now on ✍️.

---

# How to Commit Only One File in GitHub Desktop
1. Open GitHub Desktop
2. In the left sidebar, under the “Changes” tab, you’ll see a list of all files that have been modified.
3. Uncheck the ones you don’t want to include in the current commit:
   - Click the checkboxes to deselect any files you don’t want to commit yet.
   - Leave only the file(s) you want to commit checked ✅
4. At the bottom, write your commit message.
5. Click “Commit to main” (or whatever branch you're on).
6. When you’re ready, click “Push origin” to upload your change to GitHub.com.

I had to Google that because I didn't know...

---

**Date:** 17 July 2025

# Add a GitHub repository from the website to the GitHub Desktop app

## ✅ Option 1: If you already own the repository (your repo)

1. Open GitHub Desktop.
2. Go to File > Clone Repository…
3. In the “GitHub.com” tab, you’ll see your repositories listed.
4. Select the repo you want to clone to your local machine.
5. Choose the local path (where the folder will be saved).
6. Click Clone.

## ✅ Option 2: If the repo is not yours but public (e.g., from someone else)
### A. First, fork or copy the URL:

1. On GitHub.com, go to the repository page.
2. Click the green “Code” button.
3. Copy the HTTPS URL (e.g., https://github.com/username/repo-name.git).

### B. Then, in GitHub Desktop:
1. Open GitHub Desktop.
2. Go to File > Clone Repository…
3. Select the “URL” tab.
4. Paste the URL you copied.
5. Choose where to save it on your computer.
6. Click Clone.

---

**Date:** 20 July 2025

I keep getting a folder for the cache when running code in PyCharm using other txt files so this is the way of ignoring the changes 
each time in the GitHub desktop app. 

# 🧾 How to Create a .gitignore File in PyCharm (Step by Step)

## ✅ Step 1: Open Your Project in PyCharm
Make sure you're inside the GitHub project or folder where you want Git to ignore files (like __pycache__/).

## 📝 Step 2: Create the .gitignore File
Option A: If it doesn’t exist yet
1. In the Project view (left panel), right-click on your root project folder.
2. Click New > File.
3. Name the file:

``` .gitignore ```

(Make sure it starts with a dot and has no extension)

4. Click OK or press Enter.

## ✏️ Step 3: Add ignore rules
1. Once the file is created, PyCharm will open it. Now add lines like:
```
bash

# Ignore Python cache files and folders
__pycache__/
*.pyc
*.pyo
*.pyd

# Ignore virtual environments (if you have one)
venv/
env/

# Ignore IDE/project settings (optional)
.idea/
.vscode/
You can write one rule per line.
```

## ✅ Step 4: Save the File
Just press Ctrl + S (or Cmd + S on Mac), or PyCharm will auto-save it after a few seconds.

## 🧹 Step 5: (Optional) Stop Tracking Existing Files
If you had already committed __pycache__/, Git is still tracking it. You can stop that with:

1. Open PyCharm's terminal at the bottom (Alt + F12 or click the Terminal tab).
2. Run this command:
```
bash

git rm -r --cached __pycache__/
```
Then commit the change:
```
bash

git commit -m "Remove __pycache__ and add .gitignore"
```

---

**Date:** 