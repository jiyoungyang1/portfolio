# 🎨 Al-Folio Theme Setup Guide

Complete guide to deploy your portfolio using the al-folio theme - perfect for research portfolios!

---

## 🌟 Why Al-Folio?

You chose the **BEST** theme for academic/research portfolios!

**Features you'll love:**
- ✨ Beautiful publication rendering from BibTeX
- 📊 Automatic CV generation from JSON/YAML
- 📝 Blog with Distill-style posts
- 🌓 Built-in dark/light mode
- 📱 Fully responsive
- 🔍 SEO optimized
- 🎨 Professional academic design

**Example sites you liked:**
- https://carolinacarreira.github.io
- https://trandangtrungduc.github.io
- https://dineshnatesan.com/cv/

---

## 🚀 Deployment Method (EASIEST)

The easiest way is to fork the al-folio repository and let GitHub Actions automatically build and deploy your site.

### Step 1: Fork the Repository (5 minutes)

1. **Go to al-folio repository:**
   https://github.com/alshedivat/al-folio

2. **Click "Fork" button** (top right)

3. **IMPORTANT:** Rename the repository:
   - Go to Settings → General
   - Change repository name to: `yourusername.github.io`
   - Replace `yourusername` with your GitHub username
   - Click "Rename"

4. **Keep only main branch:**
   - When forking, uncheck other branches
   - You only need the `main` branch

---

### Step 2: Enable GitHub Actions (2 minutes)

You need to enable GitHub Actions to automatically build your site

1. **In your forked repository:**
   - Click the "Actions" tab
   - Click "I understand my workflows, go ahead and enable them"

2. **Configure Pages:**
   - Go to Settings → Pages
   - Source: "GitHub Actions" (should be selected automatically)
   - Click Save

---

### Step 3: Configure Basic Settings (5 minutes)

**Edit `_config.yml` directly on GitHub:**

1. Click on `_config.yml` file
2. Click the pencil icon (✏️) to edit
3. Update these critical fields:

```yaml
# Around line 17-25:
title: Ji-Young Yang
first_name: Ji-Young
middle_name: 
last_name: Yang
email: jiyoung.jane.yang@gmail.com

# Around line 35-37:
url: https://yourusername.github.io  # ⚠️ CHANGE THIS!
baseurl:  # Leave empty

# Around line 95-105:
# Social integration
github_username: yourusername  # ⚠️ CHANGE THIS!
linkedin_username: yourlinkedin  # ⚠️ CHANGE THIS!
twitter_username: # Optional
orcid_id: # Add your ORCID
scholar_userid: # Add your Google Scholar ID
researchgate_username: # Add if you have one
```

4. Scroll down and click "Commit changes"
5. Add commit message: "Update basic configuration"
6. Click "Commit changes"

---

### Step 4: Wait for Deployment (3-10 minutes)

After pushing changes, al-folio will automatically re-deploy your webpage

1. **Go to Actions tab**
2. Watch the "Deploy" workflow run
3. Wait for green checkmark ✅
4. Takes about 3-5 minutes first time

5. **Visit your site:**
   - Go to: `https://yourusername.github.io`
   - You should see the al-folio demo site with your name!

---

## 📝 Customization Roadmap

### Phase 1: Basic Info (First Hour)

**1. Update About Page**

Edit `_pages/about.md`:

```markdown
---
layout: about
title: about
permalink: /
subtitle: PhD Candidate | Computational Drug Discovery | Data Science

profile:
  align: right
  image: prof_pic.jpg  # Add your photo later
  image_circular: false
  address: >
    <p>University of Ulm</p>
    <p>Ulm, Germany</p>

news: true  # includes a list of news items
latest_posts: false
selected_papers: true # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom
---

PhD candidate with expertise in advanced biological data analysis and 
molecular dynamics (MD) simulations, focusing on protein characterization 
and drug formulation development. My research emphasizes protein-cosolute 
interactions using analytical chemistry and computational techniques.

With a global academic and professional journey spanning South Korea and 
Germany, I bring interdisciplinary skills and industry-academic experience 
to drive innovation in pharmaceutical research and development.
```

**2. Add Your Publications**

Edit `_bibliography/papers.bib`:

```bibtex
@article{Yang2025diffusion,
  title={An Expression for the Diffusion Interaction Parameter for Pharmaceutical Formulations: Insights from Kirkwood-Buff Theory},
  author={Yang, Ji Young and Smiatek, Jens},
  journal={Physical Chemistry Chemical Physics},
  year={2025},
  publisher={Royal Society of Chemistry},
  selected={true}
}

@article{Yang2024multidomain,
  title={Multidomain Protein−Urea Interactions: Differences in Binding Behavior Lead to Different Destabilization Tendencies for Monoclonal Antibodies},
  author={Yang, Ji Young and Burkert, Oliver and Mizaikoff, Boris and Smiatek, Jens},
  journal={Journal of Physical Chemistry B},
  volume={128},
  number={42},
  pages={10408--10416},
  year={2024},
  publisher={ACS Publications},
  doi={10.1021/acs.jpcb.4c04598},
  url={https://pubs.acs.org/doi/10.1021/acs.jpcb.4c04598},
  selected={true}
}

@article{Yang2024impact,
  title={Impact of Urea on Monoclonal Antibodies: Multiple Destabilization and Aggregation Effects for Therapeutic Immunoglobulin G Proteins},
  author={Yang, Ji Young and Burkert, Oliver and Mizaikoff, Boris and Smiatek, Jens},
  journal={ACS Omega},
  volume={9},
  number={5},
  pages={5517--5522},
  year={2024},
  publisher={ACS Publications},
  doi={10.1021/acsomega.3c09755},
  url={https://pubs.acs.org/doi/10.1021/acsomega.3c09755}
}

@article{Ho2022combination,
  title={Combination of Explainable Machine Learning and Conceptual Density Functional Theory: Applications for the Study of Key Solvation Mechanisms},
  author={Ho, I-Ting and Matysik, Milena and Herrera, Liliana Montano and Yang, Jiyoung and Guderlei, Ralph Joachim and Laussegger, Michael and Schrantz, Bernhard and Hammer, Regine and Miranda-Quintana, Ramón Alain and Smiatek, Jens},
  journal={Physical Chemistry Chemical Physics},
  volume={24},
  pages={28314--28324},
  year={2022},
  publisher={Royal Society of Chemistry}
}

@article{Yang2020artificial,
  title={Artificial Neural Networks for the Prediction of Solvation Energies Based on Experimental and Computational Data},
  author={Yang, Jiyoung and Knape, Matthias J and Burkert, Oliver and Mazzini, Virginia and Jung, Alexander and Craig, Vincent SJ and Miranda-Quintana, Ramón Alain and Bluhmki, Erich and Smiatek, Jens},
  journal={Physical Chemistry Chemical Physics},
  volume={22},
  pages={24359--24364},
  year={2020},
  publisher={Royal Society of Chemistry},
  doi={10.1039/D0CP03701J},
  url={https://pubs.rsc.org/en/content/articlelanding/2020/cp/d0cp03701j}
}
```

**3. Update CV**

Al-folio supports CV generation from JSON Resume or YAML format

Option A: Use `_data/cv.yml` (easier):

```yaml
- title: General Information
  type: map
  contents:
    - name: Full Name
      value: Ji-Young Yang
    - name: Languages
      value: Korean (Native), English (Fluent C1-C2), German (Fluent C1)

- title: Education
  type: time_table
  contents:
    - title: PhD in Analytical Chemistry
      institution: University of Ulm, Germany
      year: 2020 - Present
      description:
        - Industrial PhD in collaboration with Boehringer Ingelheim
        - Focus on protein-cosolute interactions and ML for drug formulation
        
    - title: MSc in Bioinformatics/Molecular Biology
      institution: University of Applied Sciences Mittweida, Germany
      year: 2018 - 2020
      
    - title: BEng in Bioengineering
      institution: Incheon National University, South Korea
      year: 2012 - 2017

- title: Experience
  type: time_table
  contents:
    - title: PhD Researcher
      institution: Boehringer Ingelheim & University Ulm
      year: 2020 - Present
      description:
        - Developed ML models for spectral deconvolution
        - Set up automated liquid handling workflows
        - MD simulations of antibody interactions
```

---

### Phase 2: Projects & Content (Second Hour)

**1. Create Project Pages**

Create files in `_projects/`:

File: `_projects/md_simulations.md`
```markdown
---
layout: page
title: Molecular Dynamics Simulations
description: Protein-cosolute interactions and antibody characterization
img: assets/img/md_project.jpg  # Add image later
importance: 1
category: research
---

### Overview
Comprehensive MD simulation studies investigating...

### Tools Used
- GROMACS
- NAMD
- OpenMM
- MDAnalysis

### Key Publications
{% cite Yang2024multidomain Yang2024impact %}
```

**2. Add News Items**

Create files in `_news/`:

File: `_news/publication_2024.md`
```markdown
---
layout: post
date: 2024-10-01
inline: true
---

New publication in J. Phys. Chem. B on multidomain protein-urea interactions!
```

---

### Phase 3: Advanced Features (Later)

**1. Add Blog Posts** (optional)
- Create files in `_posts/`
- Format: `YYYY-MM-DD-title.md`

**2. Add Profile Photo**
- Upload to `assets/img/prof_pic.jpg`
- Update in `_pages/about.md`

**3. Customize Colors**
- Edit `_sass/_themes.scss`
- Change color scheme

---

## 🔧 Important Al-Folio Files

```
your-repo/
├── _config.yml                 # Main configuration ⚠️ UPDATE THIS!
├── _pages/
│   ├── about.md               # Home/About page
│   ├── publications.md        # Auto-generated from BibTeX
│   ├── projects.md            # Projects grid
│   └── cv.md                  # CV page
├── _bibliography/
│   └── papers.bib             # Your publications ⚠️ UPDATE THIS!
├── _data/
│   ├── cv.yml                 # CV content ⚠️ UPDATE THIS!
│   └── repositories.yml       # GitHub repos to display
├── _projects/                 # Individual project pages
├── _news/                     # News announcements
├── assets/
│   ├── img/                   # Images (add your photo here!)
│   └── json/resume.json       # Alternative CV format
└── _posts/                    # Blog posts (optional)
```

---

## 📋 Customization Checklist

### Essential (Do First):
- [ ] Update `_config.yml` (name, email, URL, social media)
- [ ] Edit `_pages/about.md` with your intro
- [ ] Add publications to `_bibliography/papers.bib`
- [ ] Update `_data/cv.yml` with your CV
- [ ] Add profile photo to `assets/img/`

### Important (This Week):
- [ ] Create project pages in `_projects/`
- [ ] Add news items in `_news/`
- [ ] Update social media links
- [ ] Add Google Scholar ID
- [ ] Add ORCID ID

### Optional (When Ready):
- [ ] Write blog posts
- [ ] Customize colors/theme
- [ ] Add teaching section
- [ ] Add talks/presentations
- [ ] Set up analytics

---

## 🎨 Customization Options

### Change Color Theme

Edit `_sass/_themes.scss`:

```scss
// Find the theme colors section (around line 30)
$theme-color: #007bff;  // Change to your preferred color

// Dark mode colors
$theme-color-dark: #3498db;
```

### Enable/Disable Features

In `_config.yml`:

```yaml
# Around line 140-160
enable_darkmode: true          # Dark mode toggle
enable_navbar_social: true     # Social icons in navigation
enable_project_categories: true # Project categories
enable_medium_zoom: true       # Image zoom
enable_progressbar: true       # Page load progress bar
enable_tooltips: true         # Tooltips on hover
```

---

## 🆘 Troubleshooting

### Site Not Building?

Common issues include plugin compatibility

1. **Check Actions tab** for error messages
2. **Verify _config.yml syntax** (YAML is sensitive to spaces!)
3. **Ensure URL is correct:** `https://yourusername.github.io`
4. **Wait 5-10 minutes** - first build takes longer

### Publications Not Showing?

1. Check BibTeX syntax in `papers.bib`
2. Ensure `scholar_userid` is set if using Google Scholar
3. Verify `enabled: true` for jekyll-scholar in `_config.yml`

### 404 Error?

1. Repository name must be `yourusername.github.io`
2. Check Settings → Pages is configured correctly
3. Wait 10 minutes for gh-pages bot

---

## 💡 Pro Tips

1. **Start with demo content**
   - Get site live first
   - Replace demo content gradually
   - Don't delete everything at once!

2. **Use the examples**
   - Look at demo files as templates
   - Copy structure, change content
   - Check other al-folio sites for inspiration

3. **Commit often**
   - Small changes are easier to debug
   - Can roll back if something breaks
   - Actions tab shows each build

4. **Test locally** (advanced)
   - Install Docker
   - Run: `docker compose up`
   - View at: `localhost:8080`

---

## 📚 Resources

**Official Documentation:**
- GitHub Repo: https://github.com/alshedivat/al-folio
- Installation: https://github.com/alshedivat/al-folio/blob/main/INSTALL.md
- Customization: https://github.com/alshedivat/al-folio/blob/main/CUSTOMIZE.md
- FAQ: https://github.com/alshedivat/al-folio/blob/main/FAQ.md

**Community:**
- Discussions: https://github.com/alshedivat/al-folio/discussions
- Issues: https://github.com/alshedivat/al-folio/issues
- Examples: https://github.com/alshedivat/al-folio#user-community

**Your Examples:**
- https://carolinacarreira.github.io
- https://trandangtrungduc.github.io
- https://dineshnatesan.com/cv/

---

## 🎯 Quick Start Summary

1. **Fork** al-folio repository
2. **Rename** to `yourusername.github.io`
3. **Enable** GitHub Actions
4. **Edit** `_config.yml` (name, email, URL)
5. **Wait** 5-10 minutes
6. **Visit** your site!
7. **Customize** gradually

---

## 🚀 Your Action Plan

### Today (30 minutes):
1. Fork and rename repository
2. Enable GitHub Actions
3. Update `_config.yml`
4. Wait for deployment
5. Celebrate! 🎉

### This Week (2-3 hours):
1. Add all publications
2. Update About page
3. Fill in CV
4. Add profile photo
5. Create project pages

### This Month:
1. Write blog posts (optional)
2. Add all projects
3. Customize colors
4. Add news items
5. Share your portfolio!

---

**Al-folio is the perfect choice for your research portfolio!** 🌟

The theme will make your work look professional and organized. Take your time customizing - the default looks great already!

---

**Need help?** Check the FAQ or ask in GitHub Discussions!

Good luck! 🚀
