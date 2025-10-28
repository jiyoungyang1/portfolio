# Ji-Young Yang - Data Science Portfolio

This is the source code for my professional portfolio website, hosted on GitHub Pages.

## About This Portfolio

A showcase of my research in:
- Molecular Dynamics Simulations
- Advanced Spectroscopic Data Analysis  
- Data Science in Drug Development
- Patent & Clinical Analytics

## Website Structure

```
├── index.md              # Home page
├── about.md             # About me and background
├── research.md          # Research projects and areas
├── publications.md      # Publications and presentations
├── skills.md            # Technical skills
├── contact.md           # Contact information
├── _config.yml          # Jekyll configuration
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```

## Setup Instructions

### Option 1: Quick Setup (Recommended for Beginners)

1. **Create a new repository on GitHub:**
   - Go to https://github.com/new
   - Name it: `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
   - Make it public
   - Don't initialize with README

2. **Upload these files:**
   - Click "uploading an existing file"
   - Drag and drop all files from this folder
   - Commit the changes

3. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: main / (root)
   - Click Save

4. **Customize your content:**
   - Edit `_config.yml` and update:
     - `url` with your actual GitHub Pages URL
     - `author` information
     - LinkedIn and GitHub usernames
   - Update social media links in `contact.md`
   - Add your photo (optional)

5. **Visit your site:**
   - Go to `https://yourusername.github.io`
   - It may take a few minutes for the first deployment

### Option 2: Advanced Setup (With Local Development)

#### Prerequisites
- Git installed
- Ruby 2.7 or higher
- Bundler gem

#### Steps

1. **Clone or create the repository:**
```bash
git clone https://github.com/yourusername/yourusername.github.io.git
cd yourusername.github.io
```

2. **Install dependencies:**
```bash
bundle install
```

3. **Run locally:**
```bash
bundle exec jekyll serve
```

4. **View in browser:**
   - Open http://localhost:4000

5. **Make changes:**
   - Edit any `.md` files
   - Changes auto-reload in browser

6. **Push to GitHub:**
```bash
git add .
git commit -m "Update portfolio content"
git push origin main
```

## Customization Guide

### Changing the Theme

The default theme is `jekyll-theme-minimal`. To change:

1. **For GitHub-supported themes:**
   - Edit `_config.yml`
   - Change `theme: jekyll-theme-minimal` to another theme:
     - `jekyll-theme-slate`
     - `jekyll-theme-architect`
     - `jekyll-theme-cayman`
     - See full list: https://pages.github.com/themes/

2. **For any GitHub-hosted theme:**
   - Edit `_config.yml`
   - Add: `remote_theme: owner/repository`
   - Example: `remote_theme: alshedivat/al-folio`
   - Comment out the `theme:` line

### Popular Themes for Academic/Research Portfolios

- **al-folio**: `remote_theme: alshedivat/al-folio-jekyll-theme`
- **Minimal Mistakes**: `remote_theme: mmistakes/minimal-mistakes`
- **Academic**: `remote_theme: academicpages/academicpages.github.io`

### Adding Your Photo

1. Create an `assets/images/` folder
2. Add your photo (e.g., `profile.jpg`)
3. Reference in your pages:
```markdown
![Ji-Young Yang](/assets/images/profile.jpg)
```

### Adding Your CV

1. Create an `assets/` folder
2. Add your CV PDF: `assets/CV_JI_YOUNG_YANG.pdf`
3. Link to it: `[Download CV](/assets/CV_JI_YOUNG_YANG.pdf)`

### Updating Content

Simply edit the `.md` files:
- Use Markdown syntax
- Front matter at the top of each file:
```yaml
---
layout: default
title: Page Title
---
```

## Troubleshooting

### Site not showing up?
- Wait 5-10 minutes after first push
- Check Settings → Pages for error messages
- Ensure repository name is `yourusername.github.io`

### Theme not working?
- Check `_config.yml` syntax
- For remote themes, ensure you have `jekyll-remote-theme` in plugins
- Try the default theme first: `theme: jekyll-theme-minimal`

### Local build errors?
```bash
bundle update
bundle exec jekyll serve --trace
```

## Important Updates to Make

Before publishing, update these:

### In `_config.yml`:
- [ ] `url` - Your GitHub Pages URL
- [ ] `author` fields - Your information
- [ ] `linkedin` - Your LinkedIn username
- [ ] `github` - Your GitHub username

### In `contact.md`:
- [ ] LinkedIn profile URL
- [ ] GitHub profile URL
- [ ] Research profile links (ResearchGate, Google Scholar, ORCID)
- [ ] Remove optional sections you don't want

### In all pages:
- [ ] Replace `#` placeholder links with actual URLs
- [ ] Add your actual photo
- [ ] Update any [brackets] with your information

## Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)
- [Jekyll Themes](https://jekyllthemes.io/github-pages-themes)

## License

Feel free to fork this repository and adapt it for your own use. Please credit the original if you use substantial portions of the content structure.

## Contact

If you find issues with the template:
- Open an issue on GitHub
- Or contact me at: jiyoung.jane.yang@gmail.com

---

**Built with ❤️ using Jekyll and GitHub Pages**
