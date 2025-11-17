# Quick Start Guide

## ✅ Project Structure Created

Your AI/ML portfolio structure is ready! Here's what was created:

```
ari-ml-portfolio/
├── index.md                    ✅ Homepage (ready to customize)
├── _config.yml                 ✅ Jekyll configuration
├── Gemfile                     ✅ Ruby dependencies
├── .gitignore                  ✅ Git ignore rules
├── README.md                   ✅ Project documentation
│
├── projects/                   ✅ 5 project files
│   ├── rag-multi-agent.md      (detailed content)
│   ├── mcts-rag.md             (detailed content)
│   ├── deepseek-guardrails.md  (detailed content)
│   ├── databricks-recon.md     (detailed content)
│   └── gnn-fraud.md            (placeholder)
│
├── security/                   ✅ 4 security files
│   ├── llm-red-teaming.md
│   ├── prompt-injection-tdd.md
│   ├── vulnerabilities-remediation.md
│   └── trojan-mitigation.md
│
├── publications/               ✅ 4 publication files
│   ├── aws-blogs.md
│   ├── protectai-blogs.md
│   ├── medium-articles.md
│   └── talks-videos.md
│
├── diagrams/                   ✅ Diagram directory
│   └── README.md
│
└── about/                      ✅ About section
    ├── summary.md
    └── contact.md
```

## 🚀 Next Steps

### 1. Install Jekyll (if not already installed)

```bash
# Install Ruby (if needed)
brew install ruby

# Install Jekyll and Bundler
gem install bundler jekyll
```

### 2. Install Dependencies

```bash
cd ari-aiml-portfolio
bundle install
```

### 3. Run Locally

```bash
bundle exec jekyll serve
```

Then visit: **http://localhost:4000**

### 4. Customize Content

#### Update Personal Information
Edit `_config.yml`:
```yaml
title: Your Name - AI/ML Portfolio
author: Your Name
email: your.email@example.com
url: "https://yourusername.github.io"
```

#### Add Your Content
- Fill in placeholder files in `security/`, `publications/`, and `about/`
- Update `index.md` with your information
- Add your resume PDF to `about/resume.pdf`

#### Add Diagrams
Place your architecture diagrams in `diagrams/`:
- `rag-architecture.png`
- `agentic-rag-flow.png`
- `guardrail-pipeline.png`

### 5. Deploy to GitHub Pages

```bash
# Initialize git (if not already)
git init

# Add all files
git add .

# Commit
git commit -m "Initial portfolio setup"

# Create GitHub repository and push
git remote add origin https://github.com/yourusername/portfolio.git
git branch -M main
git push -u origin main
```

#### Enable GitHub Pages
1. Go to repository Settings
2. Navigate to Pages section
3. Select source: `main` branch, `/ (root)` folder
4. Save and wait for deployment
5. Visit: `https://yourusername.github.io/portfolio`

## 📝 Content Status

### ✅ Complete (Detailed Content)
- `projects/rag-multi-agent.md` - Full project writeup
- `projects/mcts-rag.md` - Full project writeup
- `projects/deepseek-guardrails.md` - Full project writeup
- `projects/databricks-recon.md` - Full project writeup

### 📝 Placeholder (Add Your Content)
- `projects/gnn-fraud.md`
- All files in `security/`
- All files in `publications/`
- All files in `about/`

## 🎨 Customization Tips

### Change Theme
Edit `_config.yml`:
```yaml
theme: minima  # Default
# Or try: jekyll-theme-cayman, jekyll-theme-minimal, etc.
```

### Add Custom CSS
Create `assets/css/style.scss`:
```scss
---
---

@import "{{ site.theme }}";

// Your custom styles here
```

### Add Navigation Menu
Edit `_config.yml`:
```yaml
header_pages:
  - index.md
  - about/summary.md
  - about/contact.md
```

## 🔧 Troubleshooting

### Jekyll won't start
```bash
# Update bundler
gem update bundler

# Reinstall dependencies
bundle install
```

### GitHub Pages not updating
- Check repository Settings > Pages
- Ensure `_config.yml` has correct `baseurl` and `url`
- Wait 2-3 minutes for deployment
- Check Actions tab for build errors

### Images not showing
- Use relative paths: `../diagrams/image.png`
- Ensure images are in `diagrams/` directory
- Check file names match exactly (case-sensitive)

## 📚 Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Guide](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)
- [Jekyll Themes](https://jekyllrb.com/docs/themes/)

## ✨ Features Included

- ✅ Responsive design (mobile-friendly)
- ✅ SEO optimized with jekyll-seo-tag
- ✅ RSS feed with jekyll-feed
- ✅ Sitemap generation
- ✅ Clean URL structure
- ✅ Easy navigation
- ✅ Professional layout

---

**Ready to launch your portfolio!** 🚀

Start by running `bundle exec jekyll serve` and visit http://localhost:4000

