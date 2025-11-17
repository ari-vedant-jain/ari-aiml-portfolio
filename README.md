# AI/ML Portfolio

A professional portfolio showcasing AI/ML projects, security research, and technical publications.

## 📁 Project Structure

```
ari-ml-portfolio/
│
├── index.md               # Homepage
├── _config.yml            # Jekyll configuration
│
├── projects/              # Project case studies
│   ├── rag-multi-agent.md
│   ├── mcts-rag.md
│   ├── deepseek-guardrails.md
│   ├── databricks-recon.md
│   └── gnn-fraud.md
│
├── security/              # Security research
│   ├── llm-red-teaming.md
│   ├── prompt-injection-tdd.md
│   ├── vulnerabilities-remediation.md
│   └── trojan-mitigation.md
│
├── publications/          # Publications & talks
│   ├── aws-blogs.md
│   ├── protectai-blogs.md
│   ├── medium-articles.md
│   └── talks-videos.md
│
├── diagrams/              # Architecture diagrams
│   ├── rag-architecture.png
│   ├── agentic-rag-flow.png
│   └── guardrail-pipeline.png
│
└── about/                 # About & contact
    ├── summary.md
    ├── resume.pdf
    └── contact.md
```

## 🚀 Getting Started

### Local Development

1. Install Jekyll:
```bash
gem install bundler jekyll
```

2. Create a Gemfile:
```ruby
source "https://rubygems.org"
gem "github-pages", group: :jekyll_plugins
gem "jekyll-feed"
gem "jekyll-seo-tag"
gem "jekyll-sitemap"
```

3. Install dependencies:
```bash
bundle install
```

4. Run locally:
```bash
bundle exec jekyll serve
```

5. Visit `http://localhost:4000`

### GitHub Pages Deployment

1. Push to GitHub repository
2. Enable GitHub Pages in repository settings
3. Select source: `main` branch, `/ (root)` folder
4. Site will be published at `https://yourusername.github.io/repo-name`

## 📝 Content Guidelines

### Adding New Projects

1. Create a new `.md` file in the `projects/` directory
2. Use the following front matter:
```yaml
---
layout: default
title: Project Title
---
```
3. Add project link to `index.md`

### Adding Diagrams

1. Place PNG files in `diagrams/` directory
2. Reference in markdown: `![Description](../diagrams/filename.png)`
3. Recommended size: 1200x800 pixels

### Updating Resume

1. Place PDF in `about/` directory
2. Update link in `index.md` and `about/summary.md`

## 🎨 Customization

### Theme

Edit `_config.yml` to change theme:
```yaml
theme: minima  # or jekyll-theme-cayman, etc.
```

### Colors & Styling

Create `assets/css/style.scss` to override theme styles.

### Navigation

Edit `_config.yml` header_pages to customize navigation menu.

## 📄 License

This portfolio structure is open source. Content is © Your Name.

## 📫 Contact

- Email: your.email@example.com
- LinkedIn: [Your Profile](#)
- GitHub: [@yourusername](#)

