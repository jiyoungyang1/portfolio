# Portfolio Setup Guide

Complete step-by-step guide to deploy your portfolio to GitHub Pages.

## 🎯 Quick Start (5 Minutes)

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **+** button (top right) → **New repository**
3. **Important:** Name it exactly: `yourusername.github.io`
   - Replace `yourusername` with your actual GitHub username
   - Example: If your username is `jyyang`, name it `jyyang.github.io`
4. Set to **Public**
5. **Do NOT** check "Add a README file"
6. Click **Create repository**

### Step 2: Upload Your Portfolio Files

**Option A: Direct Upload (Easiest)**

1. On your new repository page, click **uploading an existing file**
2. Drag and drop ALL files from the `jiyoung-portfolio` folder:
   - `index.md`
   - `about.md`
   - `research.md`
   - `publications.md`
   - `skills.md`
   - `contact.md`
   - `_config.yml`
   - `Gemfile`
   - `.gitignore`
   - `README.md`
3. Add commit message: "Initial portfolio setup"
4. Click **Commit changes**

**Option B: Using Git (If you're familiar with command line)**

```bash
# Navigate to your portfolio folder
cd /path/to/jiyoung-portfolio

# Initialize git
git init
git add .
git commit -m "Initial portfolio setup"

# Link to your GitHub repository
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. In your repository, click **Settings** (top navigation)
2. Scroll down and click **Pages** (left sidebar)
3. Under **Source**:
   - Select **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **Save**
5. Wait 2-5 minutes for deployment

### Step 4: Verify Your Site

1. After a few minutes, refresh the Pages settings
2. You'll see: "Your site is live at `https://yourusername.github.io`"
3. Click the link to view your portfolio!

---

## ✏️ Customization (Essential Steps)

### 1. Update `_config.yml`

Open `_config.yml` and change:

```yaml
# Line 8: Update with YOUR GitHub URL
url: "https://yourusername.github.io"  # ← Change this!

# Lines 25-29: Update YOUR information
author:
  name: Ji-Young Yang  # Keep or change
  linkedin: your-linkedin-username  # ← Change this!
  github: your-github-username  # ← Change this!
  email: jiyoung.jane.yang@gmail.com  # Keep or change
```

### 2. Update Contact Links

Open `contact.md` and update:

- LinkedIn URL (line ~33)
- GitHub URL (line ~39)
- Add your Google Scholar, ResearchGate, ORCID links

### 3. Add Your Photo (Optional but Recommended)

1. Create folders: `assets/images/`
2. Add your photo: `assets/images/profile.jpg`
3. In `index.md`, add at the top:
```markdown
![Ji-Young Yang](/assets/images/profile.jpg)
```

### 4. Add Your CV PDF (Optional)

1. Create folder: `assets/`
2. Upload: `assets/CV_JI_YOUNG_YANG.pdf`
3. Update links in pages where you reference your CV

---

## 🎨 Theme Options

### Current Theme: Minimal (Default)

The portfolio uses Jekyll's minimal theme - simple and clean.

### Want to Change Theme?

#### Option 1: GitHub Supported Themes (Easiest)

In `_config.yml`, change line 6:

```yaml
# Current:
theme: jekyll-theme-minimal

# Change to one of these:
theme: jekyll-theme-slate          # Dark professional
theme: jekyll-theme-architect      # Modern design
theme: jekyll-theme-cayman         # Clean and bold
theme: jekyll-theme-leap-day       # Sidebar navigation
```

[See all themes →](https://pages.github.com/themes/)

#### Option 2: al-folio Theme (Best for Research)

For academic/research portfolios, al-folio is excellent:

1. **Backup your current `_config.yml`:**
   - Rename it to `_config_minimal.yml`

2. **Use the al-folio config:**
   - Rename `_config_alfolio.yml` to `_config.yml`

3. **Update the new config file:**
   - Change `url` to your GitHub Pages URL
   - Update all `your-username` placeholders
   - Add your Google Scholar, ORCID IDs

4. **Commit and push changes**

**Note:** al-folio has more features but takes longer to build (5-10 minutes)

---

## 📝 Making Updates

### Method 1: Edit Directly on GitHub (Easiest)

1. Go to your repository
2. Click on any file (e.g., `index.md`)
3. Click the **pencil icon** (Edit)
4. Make your changes
5. Scroll down → **Commit changes**
6. Wait 1-2 minutes for site to rebuild

### Method 2: Local Development (Advanced)

**Prerequisites:**
- Git installed
- Ruby 2.7+ installed
- Basic command line knowledge

**Setup:**

```bash
# Clone your repository
git clone https://github.com/yourusername/yourusername.github.io.git
cd yourusername.github.io

# Install dependencies
bundle install

# Run locally
bundle exec jekyll serve

# Open browser to: http://localhost:4000
```

**Make changes:**
1. Edit files in your text editor
2. Save changes - site auto-reloads in browser
3. When satisfied:
```bash
git add .
git commit -m "Updated research section"
git push origin main
```

---

## 🔧 Common Issues & Solutions

### Issue 1: Site Shows 404 Error

**Solution:**
- Repository name must be exactly: `yourusername.github.io`
- Wait 5-10 minutes after first deployment
- Check Settings → Pages for error messages

### Issue 2: Theme Not Applying

**Solution:**
- Ensure `theme:` line in `_config.yml` is correct
- For remote themes, you need `jekyll-remote-theme` plugin
- Try reverting to `jekyll-theme-minimal` first

### Issue 3: Build Failed

**Check:**
1. Go to **Actions** tab in your repository
2. Click on the failed workflow
3. Look for error messages
4. Common causes:
   - Syntax error in `_config.yml`
   - Missing required plugins
   - Invalid markdown syntax

**Fix:**
- Check `_config.yml` syntax (use a YAML validator)
- Ensure all files are properly formatted
- Revert last changes if necessary

### Issue 4: Links Not Working

**Solution:**
- Use relative links: `/about` not `about.html`
- Check for typos in filenames
- Ensure all `.md` files are in root directory

---

## 📋 Content Checklist

Before publishing, make sure you've updated:

### Essential:
- [ ] `_config.yml` - URL and author information
- [ ] `contact.md` - All social media links
- [ ] Replace all `#` placeholder links
- [ ] Update `yourusername` throughout

### Recommended:
- [ ] Add your profile photo
- [ ] Upload your CV PDF
- [ ] Add research images/figures
- [ ] Update publication links with actual DOIs
- [ ] Remove any placeholder text in [brackets]

### Optional:
- [ ] Set up custom domain
- [ ] Add Google Analytics
- [ ] Create a blog section
- [ ] Add project galleries

---

## 🎓 Learning Resources

- **Markdown Guide:** https://www.markdownguide.org/
- **Jekyll Documentation:** https://jekyllrb.com/docs/
- **GitHub Pages Help:** https://docs.github.com/en/pages
- **Jekyll Themes:** https://jekyllthemes.io/

---

## 💡 Pro Tips

1. **Start Simple:** Use minimal theme first, then customize
2. **Test Locally:** If making major changes, test locally first
3. **Commit Often:** Small, frequent commits are easier to debug
4. **Backup:** Keep a backup of working `_config.yml`
5. **Mobile Test:** View your site on phone/tablet
6. **SEO:** Use descriptive page titles and meta descriptions

---

## 🆘 Need Help?

1. **Check the [Jekyll Documentation](https://jekyllrb.com/docs/)**
2. **Search [Stack Overflow](https://stackoverflow.com/questions/tagged/jekyll)**
3. **Ask on [Jekyll Forum](https://talk.jekyllrb.com/)**
4. **GitHub Pages [Community](https://github.community/)**

---

## 🚀 Next Steps

After your basic site is live:

1. **Add More Content:**
   - Blog posts
   - Project pages with images
   - Detailed case studies

2. **Enhance SEO:**
   - Add meta descriptions
   - Create sitemap (automatic with plugin)
   - Submit to Google Search Console

3. **Analytics:**
   - Set up Google Analytics
   - Track visitor statistics

4. **Custom Domain (Optional):**
   - Purchase domain (e.g., jiyoungyang.com)
   - Configure in repository settings
   - Update DNS records

---

**Good luck with your portfolio! 🎉**

If you get stuck, don't hesitate to reach out or check the troubleshooting section above.
