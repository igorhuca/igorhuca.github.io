# Igor Huca's Personal Blog

A personal blog built with Jekyll 4 and hosted on GitHub Pages. This blog covers topics in technology, programming, career development, and personal insights.

## 🚀 Quick Start

### Prerequisites
- Ruby 2.7+
- Bundler gem

### Local Development

1. Clone this repository:
```bash
git clone https://github.com/igorhuca/igorhuca.github.io.git
cd igorhuca.github.io
```

2. Install dependencies:
```bash
bundle install
```

3. Start the development server:
```bash
bundle exec jekyll serve --livereload
```

4. Open your browser to `http://localhost:4000`

## 📝 Creating Content

### New Blog Post
Create a new file in `_posts/` with the format: `YYYY-MM-DD-title.md`

```markdown
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD HH:MM:SS -0000
categories: category1 category2
tags: [tag1, tag2, tag3]
excerpt: "Brief description of your post"
---

Your content here...
```

### New Page
Create a new `.md` file in the root directory:

```markdown
---
layout: page
title: "Page Title"
permalink: /page-url/
---

Your page content...
```

## 🎨 Customization

### Site Configuration
Edit `_config.yml` to customize:
- Site title and description
- Author information
- Social media links
- SEO settings

### Styling
- Main styles: `assets/css/style.scss`
- Custom layouts: `_layouts/`
- Reusable components: `_includes/`

### Features
- ✅ Responsive design
- ✅ SEO optimized
- ✅ Social media meta tags
- ✅ RSS feed
- ✅ Syntax highlighting
- ✅ Comment system ready (Giscus placeholder)

## 📁 Project Structure

```
├── _config.yml          # Site configuration
├── _posts/              # Blog posts
├── _layouts/            # Page templates
├── _includes/           # Reusable components
├── assets/              # CSS, images, files
├── about.md             # About page
├── index.md             # Homepage
└── README.md            # This file
```

## 🚀 Deployment

This blog is configured for GitHub Pages deployment:

1. Push your changes to the `main` branch
2. GitHub Pages will automatically build and deploy your site
3. Your blog will be available at `https://igorhuca.github.io`

### Manual Deployment
```bash
bundle exec jekyll build
# Upload _site/ contents to your web server
```

## 🔧 Development Commands

```bash
# Start development server
bundle exec jekyll serve

# Start with live reload
bundle exec jekyll serve --livereload

# Build for production
bundle exec jekyll build

# Clean build files
bundle exec jekyll clean
```

## 📱 GitHub Pages Setup

1. Create a repository named `igorhuca.github.io`
2. Push this code to the `main` branch
3. Go to Settings > Pages
4. Select "Deploy from a branch" and choose `main`
5. Your site will be live at `https://igorhuca.github.io`

## 🛠 Customization Tips

### Adding Comments (Giscus)
1. Enable Discussions in your GitHub repository
2. Visit [giscus.app](https://giscus.app) to generate configuration
3. Replace the placeholder in `_layouts/post.html`

### Google Analytics
Add your GA4 measurement ID to `_config.yml`:
```yaml
google_analytics: G-XXXXXXXXXX
```

### Custom Domain
1. Add a `CNAME` file with your domain
2. Configure DNS at your domain provider
3. Update `url` in `_config.yml`

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Issues and pull requests are welcome! Please feel free to contribute to this project.

---

**Happy blogging!** 🎉