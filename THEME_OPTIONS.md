# Jekyll Theme Options for Your Portfolio

Comprehensive guide to choosing and implementing themes for your data science portfolio.

---

## 🎨 Quick Theme Comparison

| Theme | Difficulty | Best For | Features | Setup Time |
|-------|-----------|----------|----------|------------|
| **Minimal** (current) | ⭐ Easy | Simple portfolios | Clean, fast | 5 min |
| **Slate** | ⭐ Easy | Professional look | Dark theme | 5 min |
| **Cayman** | ⭐ Easy | Modern design | Bold headers | 5 min |
| **al-folio** | ⭐⭐⭐ Advanced | Academic/Research | Publications, CV, blog | 30 min |
| **Minimal Mistakes** | ⭐⭐ Moderate | Feature-rich sites | Blog, search, TOC | 20 min |
| **Beautiful Jekyll** | ⭐⭐ Moderate | Personal sites | Easy customization | 15 min |

---

## Theme Category 1: GitHub-Supported Themes

### ✅ Advantages:
- ✓ Instant setup (just change one line)
- ✓ No additional dependencies
- ✓ Fast build times
- ✓ Always compatible with GitHub Pages

### 📝 How to Use:

In `_config.yml`, change line 6:
```yaml
theme: jekyll-theme-[NAME]
```

---

### 1. Minimal (Current Default) ⭐

**When to Use:** You want something simple and clean

**Pros:**
- Very fast loading
- Easy to customize
- Mobile-responsive
- Great for text-heavy content

**Cons:**
- Basic styling
- Limited layout options
- No built-in blog features

**Setup:**
```yaml
theme: jekyll-theme-minimal
```

**Preview:** [Demo](https://pages-themes.github.io/minimal/)

---

### 2. Slate ⭐

**When to Use:** Professional, modern look with dark theme

**Pros:**
- Beautiful dark design
- Professional appearance
- Good for tech portfolios
- Built-in navigation

**Cons:**
- Dark theme might not suit everyone
- Less customization options

**Setup:**
```yaml
theme: jekyll-theme-slate
```

**Preview:** [Demo](https://pages-themes.github.io/slate/)

---

### 3. Cayman ⭐

**When to Use:** Bold, eye-catching design

**Pros:**
- Striking gradient header
- Clean content area
- Call-to-action friendly
- Modern look

**Cons:**
- Fixed color scheme
- Less suitable for academic style

**Setup:**
```yaml
theme: jekyll-theme-cayman
```

**Preview:** [Demo](https://pages-themes.github.io/cayman/)

---

### 4. Architect ⭐

**When to Use:** Architectural/structural feel

**Pros:**
- Unique sidebar design
- Professional layout
- Good for project showcases

**Cons:**
- Specific design aesthetic
- May need color adjustments

**Setup:**
```yaml
theme: jekyll-theme-architect
```

**Preview:** [Demo](https://pages-themes.github.io/architect/)

---

### 5. Leap Day ⭐

**When to Use:** You want a sidebar with navigation

**Pros:**
- Fixed sidebar navigation
- Easy to navigate
- Clean content area

**Cons:**
- Sidebar takes up space
- Less content width

**Setup:**
```yaml
theme: jekyll-theme-leap-day
```

**Preview:** [Demo](https://pages-themes.github.io/leap-day/)

---

### 6. Hacker ⭐

**When to Use:** Retro terminal/coding aesthetic

**Pros:**
- Unique "hacker" look
- Dark theme
- Great for developer portfolios

**Cons:**
- Niche aesthetic
- May not look "professional" to all audiences

**Setup:**
```yaml
theme: jekyll-theme-hacker
```

**Preview:** [Demo](https://pages-themes.github.io/hacker/)

---

## Theme Category 2: Remote Themes (Advanced)

### ✅ Advantages:
- ✓ More features and options
- ✓ Regular updates
- ✓ Large communities
- ✓ Professional designs

### ⚠️ Considerations:
- Takes longer to build (5-10 minutes)
- More complex setup
- May need additional plugins

### 📝 How to Use:

In `_config.yml`:
1. Comment out or remove `theme:` line
2. Add `remote_theme:` line
3. Add required plugins

---

### 1. al-folio ⭐⭐⭐ (HIGHLY RECOMMENDED for Research)

**When to Use:** Academic portfolio, publications showcase, research projects

**Perfect For:**
- PhD students
- Postdocs
- Research scientists
- Academic job market

**Features:**
- ✓ Beautiful publication listings
- ✓ Project galleries
- ✓ News/announcements section
- ✓ CV page
- ✓ Blog with categories
- ✓ Dark mode toggle
- ✓ BibTeX integration
- ✓ Google Scholar integration
- ✓ Responsive design

**Setup:**

1. **Use the provided config file:**
   - Rename `_config_alfolio.yml` to `_config.yml` (backup the old one)

2. **Or manually edit `_config.yml`:**
```yaml
remote_theme: alshedivat/al-folio

plugins:
  - jekyll-remote-theme
  - jekyll-paginate-v2
  - jekyll-scholar
  # ... other plugins
```

3. **Update your Gemfile:**
```ruby
gem "jekyll-remote-theme"
gem "jekyll-paginate-v2"
gem "jekyll-scholar"
```

**Additional Setup:**
- Create `_bibliography/papers.bib` for publications
- Create `_projects/` folder for project pages
- Create `_news/` folder for announcements

**Preview:** [Demo](https://alshedivat.github.io/al-folio/)

**Why I Recommend This:**
- Specifically designed for researchers
- Beautiful publication rendering
- Strong in academic community
- Regularly maintained

---

### 2. Minimal Mistakes ⭐⭐

**When to Use:** Feature-rich personal site with blog

**Features:**
- ✓ Multiple layout options
- ✓ Built-in search
- ✓ Table of contents
- ✓ Author profiles
- ✓ Social sharing
- ✓ Comments (Disqus)
- ✓ Analytics ready

**Setup:**
```yaml
remote_theme: "mmistakes/minimal-mistakes"

plugins:
  - jekyll-remote-theme
  - jekyll-paginate
  - jekyll-sitemap
  - jekyll-gist
  - jekyll-feed
  - jekyll-include-cache
```

**Preview:** [Demo](https://mmistakes.github.io/minimal-mistakes/)

**Good For:**
- Technical blogs
- Portfolio with blog
- Tutorial sites

---

### 3. Beautiful Jekyll ⭐⭐

**When to Use:** Simple, beautiful personal website

**Features:**
- ✓ Easy to customize
- ✓ Blog ready
- ✓ Responsive
- ✓ Syntax highlighting
- ✓ Social icons

**Setup:**
```yaml
remote_theme: "daattali/beautiful-jekyll"

plugins:
  - jekyll-remote-theme
  - jekyll-paginate
```

**Preview:** [Demo](https://beautifuljekyll.com/)

**Good For:**
- Personal blogs
- Simple portfolios
- Non-technical audiences

---

### 4. Academic Pages ⭐⭐⭐

**When to Use:** Academic job market, similar to al-folio

**Features:**
- ✓ CV page
- ✓ Publications
- ✓ Teaching portfolio
- ✓ Talk listings
- ✓ Portfolio items

**Setup:**
```yaml
remote_theme: "academicpages/academicpages.github.io"

plugins:
  - jekyll-remote-theme
  - jekyll-paginate
```

**Preview:** [Demo](https://academicpages.github.io/)

**Good For:**
- Academic job seekers
- Professor portfolios
- Research-focused sites

---

### 5. Chirpy ⭐⭐

**When to Use:** Modern technical blog

**Features:**
- ✓ Modern UI
- ✓ Dark/light mode
- ✓ Built-in search
- ✓ Category/tag archives
- ✓ Syntax highlighting
- ✓ Table of contents

**Setup:**
```yaml
remote_theme: "cotes2020/jekyll-theme-chirpy"

plugins:
  - jekyll-remote-theme
  # ... other plugins
```

**Preview:** [Demo](https://chirpy.cotes.page/)

**Good For:**
- Technical blogs
- Developer portfolios
- Tutorial sites

---

## 🎯 My Recommendation for You

Based on your profile as a PhD candidate in computational chemistry with data science focus:

### Option 1: Start with Minimal (Current) ⭐
**Why:** 
- Get your content online quickly
- Focus on substance over style
- Easy to customize
- Fast and reliable

**When to upgrade:** After you have all content in place

---

### Option 2: Upgrade to al-folio ⭐⭐⭐
**Why:**
- Purpose-built for research portfolios
- Beautiful publication rendering
- Professional academic appearance
- Industry standard for PhD portfolios

**Best if:** You want the most impressive academic portfolio

---

### Option 3: Use Slate for Professional Look ⭐
**Why:**
- Professional appearance
- Dark theme = modern/tech-savvy
- Still simple to maintain
- One-line change from current setup

**Best if:** You're targeting industry positions

---

## 🔄 How to Switch Themes

### For GitHub-Supported Themes:

1. Edit `_config.yml`
2. Change this line:
```yaml
theme: jekyll-theme-[new-theme-name]
```
3. Commit and push
4. Wait 2-5 minutes

### For Remote Themes:

1. Backup your current `_config.yml`
2. Use the theme's template or documentation
3. Update plugins list
4. Commit and push
5. Wait 5-10 minutes (longer first time)

---

## 🛠️ Testing Themes Locally

Want to try before deploying?

```bash
# In your portfolio directory
bundle install
bundle exec jekyll serve

# View at: http://localhost:4000
# Change theme in _config.yml
# Refresh browser
```

---

## ⚖️ Decision Matrix

Answer these questions:

1. **How quickly do you need it online?**
   - Immediately → Minimal (current)
   - Can wait 1 hour → Any GitHub theme
   - Have time to customize → al-folio or Minimal Mistakes

2. **Who's your primary audience?**
   - Academia → al-folio or Academic Pages
   - Industry (Tech) → Slate or Hacker
   - Industry (General) → Minimal or Cayman
   - Mixed → Minimal Mistakes

3. **How much customization do you want?**
   - Minimal → GitHub themes
   - Some → Remote themes
   - Maximum → al-folio (but steeper learning curve)

4. **Will you blog regularly?**
   - Yes → al-folio, Minimal Mistakes, or Chirpy
   - Occasionally → Beautiful Jekyll
   - No → Minimal or Slate

5. **Technical comfort level?**
   - Beginner → GitHub themes (Minimal, Slate, Cayman)
   - Intermediate → Minimal Mistakes, Beautiful Jekyll
   - Advanced → al-folio, Academic Pages

---

## 📚 Additional Resources

### Theme Galleries:
- [Jekyll Themes](https://jekyllthemes.io/github-pages-themes)
- [Jamstack Themes](https://jamstackthemes.dev/ssg/jekyll/)
- [Jekyll Theme Showcase](https://jekyllrb.com/showcase/)

### Documentation:
- [GitHub Pages Themes](https://pages.github.com/themes/)
- [Jekyll Documentation](https://jekyllrb.com/docs/themes/)
- [Remote Theme Plugin](https://github.com/benbalter/jekyll-remote-theme)

---

## 💡 Final Tips

1. **Start simple, upgrade later**
   - Content > Design initially
   - Can always change theme later

2. **Mobile matters**
   - Test on phone/tablet
   - All recommended themes are responsive

3. **Performance counts**
   - Simpler themes = faster loading
   - Important for SEO and user experience

4. **Backup before changing**
   - Keep copy of working `_config.yml`
   - Easy to revert if needed

5. **Check examples**
   - Look at other academics' portfolios
   - See what themes they use
   - Learn from their layouts

---

**Still unsure? Start with Minimal (current setup), get your content online, then decide if you want to upgrade!**
