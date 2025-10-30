# YouTube Redirect via GitHub Pages

A simple, permanent redirect to your YouTube video that hides upload timestamps.

## 🚀 Quick Setup

1. **Replace the destination URL** in `index.html`:
   - Find line 9: `const REDIRECT_URL = 'https://youtu.be/YOUR_VIDEO_ID_HERE';`
   - Replace the entire URL with your destination (e.g., `'https://youtu.be/dQw4w9WgXcQ'` or any other URL)

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
const REDIRECT_URL = 'https://youtu.be/YOUR_VIDEO_ID_HERE';
```

Replace the entire URL with your new destination URL. That's it! The rest updates automatically.

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

If your YouTube video URL is `https://youtu.be/abc123xyz`, your redirect will be:
- GitHub: `https://maneeshvaddi.github.io/youtube-redirect/`
- Redirects to: `https://youtu.be/abc123xyz`
- No timestamp visible to viewers!

You can redirect to any URL - YouTube videos, websites, or any other link!

