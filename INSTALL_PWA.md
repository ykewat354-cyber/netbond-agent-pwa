# Install PWA Version (Easiest Method!)

This is the **fastest way** to get the app on your phone - no APK building needed!

## Option 1: Host on GitHub Pages (Free, 5 minutes)

### Step 1: Create GitHub Repo
1. Go to https://github.com/new
2. Create a new public repository (e.g., `netbond-agent-pwa`)

### Step 2: Upload Files
Upload these files to your repo:
- `index.html`
- `manifest.json`
- `sw.js`
- `icon-192.png` (create or use any 192x192 PNG)
- `icon-512.png` (create or use any 512x512 PNG)

### Step 3: Enable GitHub Pages
1. Go to repo Settings → Pages
2. Source: Deploy from branch → main → root
3. Save

### Step 4: Access on Phone
1. You'll get a URL like: `https://yourusername.github.io/netbond-agent-pwa/`
2. Open this URL in Chrome on your OPPO K13

### Step 5: Install PWA
1. Chrome will show "Add to Home Screen" prompt
2. Or tap: Menu (⋮) → Install App / Add to Home Screen
3. App icon appears on your home screen!

---

## Option 2: Host on Netlify (Free, 3 minutes)

### Step 1: Go to Netlify Drop
https://app.netlify.com/drop

### Step 2: Upload Folder
1. Put all PWA files in a folder
2. Drag and drop the folder to Netlify Drop
3. Get instant live URL

### Step 3: Install on Phone
Same as GitHub Pages - open URL and add to home screen

---

## Option 3: Host on Render/Railway (Free)

1. Create account on https://render.com or https://railway.app
2. Create new "Static Site"
3. Connect GitHub repo or upload files
4. Get live URL
5. Install on phone

---

## Option 4: Local Testing (No Hosting)

### Using Python
```bash
cd netbond-pwa
python -m http.server 8000
```

Then on your phone (if on same WiFi):
1. Find your PC's IP: `ipconfig` (Windows) or `ifconfig` (Linux/Mac)
2. Open: `http://YOUR_PC_IP:8000`
3. Add to home screen

---

## How to Use the App

1. **Open app** from home screen
2. **Login** with netBond.in credentials
3. **Set filters**: Platform, Device, Max Price
4. **Tap "Start Listing"** - loads netBond.in with filters
5. **Tap "Analyze with AI"** - get AI summary
6. **Copy/Save** analysis

---

## Add Claude API Key

First time using AI analysis:
1. Tap "Analyze with AI"
2. Enter your Claude API key when prompted
3. Key is saved locally (encrypted on device)

Get API key from: https://console.anthropic.com/

---

## PWA vs APK Comparison

| Feature | PWA | APK |
|---------|-----|-----|
| Installation | Instant (from browser) | Build + install |
| Size | ~50KB | ~5-10MB |
| Updates | Automatic | Rebuild + reinstall |
| Offline | Limited | Full |
| Browser automation | WebView | Full Playwright |
| Best for | Quick setup | Full features |

---

## Troubleshooting

**"Add to Home Screen" not showing:**
- Use Chrome (not Firefox)
- Visit site multiple times
- Some Android launchers hide the option

**App not loading:**
- Check HTTPS (required for PWA)
- Clear browser cache
- Try incognito mode

**API calls failing:**
- Check API key is valid
- Ensure internet connection
- Check browser console for errors

---

## Next Steps

For your OPPO K13, I recommend:
1. **Start with PWA** (5 min setup)
2. Test all features
3. If you need more power, build the APK later

Enjoy! 🎉
