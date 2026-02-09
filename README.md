# PDF Reader & Information Extractor

A web-based PDF reader and information extraction tool that allows you to upload multiple PDF files and extract key information including:

- **Policy Numbers** (POLICY NO)
- **Class of Insurance**
- **Invoice Numbers** (VP/NP format)
- **Total Premium Amounts** (PHP currency)
- **Custom information extraction** using keywords or regex patterns

## Features

- 📄 Upload multiple PDF files at once
- 🔍 Extract invoice numbers and corresponding totals
- 📋 Extract policy information (Policy No, Class of Insurance)
- 🎯 Custom extraction with keywords or regex patterns
- 📊 Document statistics and analysis
- 💾 All processing happens in your browser (no server required)

## How to Deploy to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in (or create an account)
2. Click the **"+"** icon in the top right → **"New repository"**
3. Name your repository (e.g., `pdf-reader` or `pdf-extractor`)
4. Choose **Public** (required for free GitHub Pages)
5. **Don't** initialize with README (we'll upload files manually)
6. Click **"Create repository"**

### Step 2: Upload Files

#### Option A: Using GitHub Web Interface

1. In your new repository, click **"uploading an existing file"**
2. Drag and drop these files:
   - `index.html` (your PDF reader app)
   - `README.md` (this file - optional)
3. Scroll down and click **"Commit changes"**

#### Option B: Using Git Command Line

```bash
# Navigate to your project folder
cd c:\Users\ziwei.yee

# Initialize git (if not already done)
git init

# Add files
git add index.html README.md

# Commit
git commit -m "Initial commit: PDF Reader app"

# Add your GitHub repository as remote (replace YOUR_USERNAME and REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab (top menu)
3. Scroll down to **"Pages"** section (left sidebar)
4. Under **"Source"**, select:
   - Branch: **main** (or **master**)
   - Folder: **/ (root)**
5. Click **"Save"**
6. Wait a few minutes for GitHub to deploy

### Step 4: Access Your Site

Your site will be available at:
```
https://YOUR_USERNAME.github.io/REPO_NAME/
```

For example, if your username is `johndoe` and repository is `pdf-reader`:
```
https://johndoe.github.io/pdf-reader/
```

## Usage

1. Open the deployed website
2. Upload PDF files (drag & drop or click to browse)
3. View extracted information:
   - Policy Numbers
   - Class of Insurance
   - Invoice Numbers and Totals
4. Use custom extraction to find specific information
5. Click **"Reset"** button to clear and upload new files

## Notes

- All PDF processing happens in your browser - files are never uploaded to any server
- Works best with text-based PDFs (scanned PDFs may not extract text properly)
- Supports multiple PDF uploads for batch processing
- Extracts PHP currency amounts (₱)

## Troubleshooting

**Site not loading?**
- Wait 5-10 minutes after enabling GitHub Pages
- Check repository Settings → Pages to ensure it's enabled
- Make sure `index.html` is in the root folder

**PDFs not processing?**
- Ensure PDFs contain extractable text (not just images)
- Try with smaller PDF files first
- Check browser console for errors (F12)

## License

Free to use and modify for your team.
