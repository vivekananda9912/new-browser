# Educational Browser - Computer Lab Deployment Guide

This application is packaged as a standalone Windows executable. **Student computers do NOT need Node.js, VS Code, npm, or any developer tools.**

---

## 🚀 How Students Use It (1-Click)
1. Turn on the student PC.
2. Double-click the **Educational Browser** icon on the Windows Desktop.
3. The app immediately launches full-screen in locked student mode.

---

## 📦 Where the App is Located
The standalone build is already compiled and ready inside your project at:
```text
release-builds\Educational Browser-win32-x64\
```
Inside this folder, you will find:
- `Educational Browser.exe` (The main application)
- `Create-Desktop-Shortcut.bat` (1-click script that creates the Desktop icon)

---

## 🛠️ Step-by-Step Setup on Student PCs (Takes 30 Seconds)

### Step 1: Copy the Folder to the Student PC
Copy the `Educational Browser-win32-x64` folder to the student PC via:
- USB Flash Drive, or
- Shared School Network Drive (`\\school-server\apps\`), or
- Copying to `C:\Educational Browser\`

### Step 2: Create the 1-Click Desktop Icon
Inside the folder on the student PC:
- Double-click **`Create-Desktop-Shortcut.bat`**.

That's it!
- It automatically creates an **Educational Browser** desktop icon for the student.
- It also registers the shortcut for all student accounts on that PC if administrator permissions are present.

---

## 🔄 How to Re-Build Anytime (For Future Code Changes)
Whenever you update code in your IDE and want to generate a fresh build:
```bash
npm run package-win
```
Or simply double-click **`CREATE-LAB-SHORTCUT.bat`** in the root directory.
