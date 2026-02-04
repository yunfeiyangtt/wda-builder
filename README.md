# WebDriverAgent Builder

Builds WebDriverAgent IPA using GitHub Actions (free macOS cloud build).

## Quick Start

1. **Create a new GitHub repo** named `wda-builder`
2. **Push this folder** to the repo
3. **Go to Actions tab** and run the workflow
4. **Download the IPA** from the workflow artifacts or releases

## Detailed Steps

### Step 1: Create GitHub Repository

Go to https://github.com/new and create a new repo called `wda-builder`

### Step 2: Push This Code

```bash
cd wda-builder
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/wda-builder.git
git push -u origin main
```

### Step 3: Run the Build

1. Go to your repo on GitHub
2. Click the **Actions** tab
3. Click **Build WebDriverAgent IPA**
4. Click **Run workflow** button
5. Wait ~5 minutes for build to complete

### Step 4: Download IPA

After the build completes:
- Click on the completed workflow run
- Scroll down to **Artifacts**
- Download **WebDriverAgent-IPA**
- Extract the zip to get `WebDriverAgent.ipa`

### Step 5: Install with Sideloadly

1. Open Sideloadly
2. Connect your iPhone via USB
3. Drag `WebDriverAgent.ipa` into Sideloadly
4. Enter your Apple ID and password
5. Click Start

### Step 6: Trust the App

On your iPhone:
1. Settings > General > VPN & Device Management
2. Tap your Apple ID email
3. Tap "Trust"

## Notes

- Free Apple IDs: Apps expire after 7 days, need to reinstall
- Paid Apple Developer: Apps last 1 year
- The IPA is unsigned - Sideloadly handles the signing
