# YouTube Redirect via GitHub Pages

A simple, permanent redirect to your YouTube video that hides upload timestamps.

## 🚀 Quick Setup

1. **Replace the video ID** in `index.html`:
   - Find `YOUR_VIDEO_ID_HERE` (appears 3 times)
   - Replace with your actual YouTube video ID (e.g., `dQw4w9WgXcQ`)

2. **Upload to GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: YouTube redirect"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to your repository → Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` / `(root)`
   - Click Save

4. **Your redirect URL will be**:
   ```
   https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
   ```

## 📝 How to Change the Redirect Later

Simply edit `index.html` and update **line 9** where it says:
```javascript
const YOUTUBE_VIDEO_ID = 'YOUR_VIDEO_ID_HERE';
```

Change `YOUR_VIDEO_ID_HERE` to your new video ID. That's it! The rest updates automatically.

Then commit and push:
```bash
git add index.html
git commit -m "Update redirect to new video"
git push
```

The redirect will update automatically (may take a few seconds).

## 💡 Tips

- Use **Unlisted** YouTube videos to hide upload timestamps from viewers
- The redirect works immediately and hides all timing information
- The link is permanent as long as your GitHub repo exists
- Works on all devices and browsers

## 🎯 Example

If your video ID is `abc123xyz`, your redirect URL will be:
- GitHub: `https://maneeshvaddi.github.io/pitch/`
- Redirects to: `https://youtu.be/abc123xyz`
- No timestamp visible to viewers!

