# GitHub Deployment Instructions

## Option 1: Using GitHub Website (Easiest)

1. **Create a new repository on GitHub**
   - Go to https://github.com/new
   - Repository name: `ages-fertility-tutorial` (or your preferred name)
   - Description: "Fertility Preservation in Endometriosis - Clinical Tutorial for AGES"
   - Make it Public
   - Click "Create repository"

2. **Upload files**
   - Click "uploading an existing file"
   - Drag and drop ALL 7 files:
     - index.html
     - background-video.mp4
     - fertile-logo.png
     - whatsapp-profile.png
     - whatsapp-icon.png
     - amh-normogram.png
     - README.md
   - Add commit message: "Initial commit - AGES Fertility Preservation Tutorial"
   - Click "Commit changes"

3. **Enable GitHub Pages**
   - Go to repository Settings
   - Scroll to "Pages" section (left sidebar)
   - Source: Select "Deploy from a branch"
   - Branch: Select "main" and "/ (root)"
   - Click "Save"
   - Wait 1-2 minutes for deployment

4. **Your tutorial will be live at:**
   ```
   https://[your-username].github.io/ages-fertility-tutorial/
   ```

## Option 2: Using Git Command Line

```bash
# Navigate to the folder with all files
cd /path/to/ages-fertility-tutorial

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit - AGES Fertility Preservation Tutorial"

# Add your GitHub repository as remote
git remote add origin https://github.com/[your-username]/ages-fertility-tutorial.git

# Push to GitHub
git branch -M main
git push -u origin main
```

Then enable GitHub Pages in repository settings as described in Option 1, step 3.

## Option 3: Add to Existing AGES Website

If you already have an AGES website repository:

1. Create a new folder: `/fertility-preservation-tutorial/`
2. Upload all files to this folder
3. Link to it from your main website:
   ```html
   <a href="/fertility-preservation-tutorial/">Fertility Preservation Tutorial</a>
   ```

## Updating Your Tutorial

To update content:
1. Edit the files locally
2. Upload updated files to GitHub (via website or git push)
3. Changes will appear on your live site within 1-2 minutes

## Troubleshooting

**Video not playing?**
- GitHub has a 100MB file limit. Your video is 506KB, so it's fine!
- Make sure the video file is in the same folder as index.html

**WhatsApp contact not working?**
- Update the phone number in index.html (search for "61XXXXXXXXX")
- Replace with your actual WhatsApp number with country code

**Images not loading?**
- Verify all image files are in the same folder as index.html
- File names are case-sensitive!

## Need Help?

Contact GitHub Support or refer to:
https://docs.github.com/en/pages
