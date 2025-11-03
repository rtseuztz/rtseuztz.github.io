# Saji Shunnarah - Portfolio Website

A modern, responsive portfolio website showcasing my software engineering projects and technical expertise, including Rezumake.

## 🌟 Features

- **Modern Design**: Clean, professional interface with smooth animations
- **Responsive Layout**: Optimized for all devices (desktop, tablet, mobile)
- **Project Showcase**: Detailed case studies of featured projects
- **SEO Optimized**: Built-in SEO tags and sitemap for better discoverability
- **Fast Performance**: Lightweight static site with optimized assets

## 🛠️ Built With

- **Jekyll** - Static site generator
- **HTML/CSS** - Custom styling with CSS variables
- **JavaScript** - Interactive navigation and smooth scrolling
- **GitHub Pages** - Hosting platform

## 🚀 Getting Started

### Prerequisites

- Ruby (version 2.7 or higher)
- Bundler
- Jekyll

### Installation

1. Clone the repository:
```bash
git clone https://github.com/rtseuztz/rezumake.com.git
cd rezumake.com
```

2. Install dependencies:
```bash
bundle install
```

3. Run the development server:
```bash
bundle exec jekyll serve
```

4. Open your browser and navigate to:
```
http://localhost:4000
```

## 📁 Project Structure

```
.
├── _config.yml           # Site configuration
├── _layouts/             # Custom layouts
│   ├── default.html      # Main layout template
│   └── post.html         # Project post layout
├── _includes/            # Reusable components
│   └── head.html         # HTML head section
├── _posts/               # Project posts
├── assets/
│   ├── css/
│   │   └── style.css     # Custom styles
│   ├── images/           # Project images
│   └── videos/           # Project videos/GIFs
├── index.markdown        # Homepage
└── README.md
```

## 🎨 Customization

### Colors

The site uses CSS variables for easy theming. Edit `assets/css/style.css`:

```css
:root {
  --primary-color: #2563eb;
  --secondary-color: #64748b;
  --accent-color: #0ea5e9;
  /* ... more variables */
}
```

### Content

- **Homepage**: Edit `index.markdown`
- **Projects**: Add new posts in `_posts/` directory
- **Site Info**: Update `_config.yml`

## 📝 Adding New Projects

Create a new file in `_posts/` with the format: `YYYY-MM-DD-project-name.markdown`

```markdown
---
layout: post
title: "Project Name"
date: YYYY-MM-DD HH:MM:SS -0500
categories: jekyll project
---

Your project content here...
```

## 🌐 Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the main branch.

### Manual Deployment

```bash
bundle exec jekyll build
```

The built site will be in the `_site/` directory.

## 📧 Contact

Saji Shunnarah - [sajishunnarah@gmail.com](mailto:sajishunnarah@gmail.com)

- GitHub: [@rtseuztz](https://github.com/rtseuztz)
- LinkedIn: [sajishunnarah](https://linkedin.com/in/sajishunnarah)

## 📄 License

This project is open source and available under the MIT License.

---

Built with ❤️ using Jekyll