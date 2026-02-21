# 📱 How to Get Your MoneyManager APK via GitHub (Free!)

---

## 🔧 STEP 1 — Create GitHub Account
1. Go to https://github.com
2. Click "Sign up"
3. Enter your email, password, username
4. Verify your email
5. You're in! ✅

---

## 📁 STEP 2 — Create a New Repository
1. Click the **"+"** button (top right) → "New repository"
2. Repository name: `MoneyManager`
3. Set to **Public**
4. Click **"Create repository"**

---

## 📤 STEP 3 — Upload the Project Files

### Option A: Upload via GitHub Website (Easiest)
1. Extract the **MoneyManager_App.zip** on your PC
2. On your new GitHub repo page, click **"uploading an existing file"**
3. Drag and drop ALL files and folders from the extracted folder
4. Important: Make sure the `.github/workflows/build.yml` file is included!
5. Scroll down, click **"Commit changes"**

### Option B: Use Git (if you have it installed)
```bash
cd MoneyManager
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOURUSERNAME/MoneyManager.git
git push -u origin main
```

---

## ⚙️ STEP 4 — Watch GitHub Build Your APK

1. Go to your repository on GitHub
2. Click the **"Actions"** tab (top menu)
3. You'll see **"Build MoneyManager APK"** running (yellow circle = in progress)
4. Wait about **5-10 minutes**
5. When it turns **green ✅** — your APK is ready!

---

## 📥 STEP 5 — Download Your APK

1. Click on the completed workflow run (green checkmark)
2. Scroll down to **"Artifacts"** section
3. Click **"MoneyManager-APK"** to download
4. You'll get a ZIP file — extract it
5. Inside is your **app-debug.apk** file! 🎉

---

## 📲 STEP 6 — Install on Your Android Phone

### Transfer the APK to your phone:
- Email it to yourself and open on phone
- Upload to Google Drive, open on phone
- Send via WhatsApp/Telegram to yourself
- USB cable copy

### Install on phone:
1. Open **File Manager** on phone
2. Find the APK file
3. Tap it → **Install**
4. If blocked: Settings → Apps → Special Access → Install Unknown Apps → Allow

---

## 🔄 BONUS: Re-build anytime you make changes!

Every time you push new code to GitHub, it automatically builds a new APK!
You can also manually trigger a build:
1. Go to Actions tab
2. Click "Build MoneyManager APK"
3. Click "Run workflow" button

---

## ❓ Common Issues

**"Gradle build failed"**
→ Check the Actions log for the error message and share it — I can fix it!

**"Workflow not running"**
→ Make sure the file is at exactly: `.github/workflows/build.yml`

**"Can't upload folders on GitHub website"**
→ Use git commands instead (Option B in Step 3)

---

Good luck! 🚀 Once you have the APK, enjoy your Money Manager app!
