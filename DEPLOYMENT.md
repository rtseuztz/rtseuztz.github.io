# Deployment Guide

## Quick Start - GitHub Pages (Recommended)

The easiest way to deploy your portfolio is using GitHub Pages, which will automatically build and host your Jekyll site.

### Steps:

1. **Commit all changes:**
```bash
git add .
git commit -m "Complete portfolio overhaul with modern design"
```

2. **Push to GitHub:**
```bash
git push origin main
```

3. **Enable GitHub Pages:**
   - Go to your repository settings on GitHub
   - Navigate to "Pages" in the left sidebar
   - Under "Source", select the `main` branch
   - Click "Save"

4. **Wait for deployment:**
   - GitHub will automatically build and deploy your site
   - Your site will be live at: `https://rtseuztz.github.io`
   - This usually takes 1-2 minutes

## Local Development (Alternative Methods)

### Option 1: Using Docker (Recommended for Local Testing)

If you have Docker installed, you can run Jekyll without Ruby version conflicts:

```bash
docker run --rm -v "$PWD:/srv/jekyll" -p 4000:4000 jekyll/jekyll:latest jekyll serve
```

Then visit: `http://localhost:4000`

### Option 2: Using rbenv (Ruby Version Manager)

If you want to run locally with the correct Ruby version:

1. **Install rbenv:**
```bash
brew install rbenv ruby-build
```

2. **Install Ruby 3.1.0 or higher:**
```bash
rbenv install 3.1.0
rbenv local 3.1.0
```

3. **Install dependencies:**
```bash
gem install bundler
bundle install
```

4. **Run the server:**
```bash
bundle exec jekyll serve
```

5. **Visit:** `http://localhost:4000`

### Option 3: GitHub Codespaces

1. Open your repository on GitHub
2. Click the green "Code" button
3. Select "Codespaces" tab
4. Click "Create codespace on main"
5. Once loaded, run:
```bash
bundle install
bundle exec jekyll serve
```

## Troubleshooting

### Ruby Version Issues

The system Ruby (2.6) is too old for modern Jekyll. Solutions:
- Use GitHub Pages (no local setup needed)
- Use Docker (recommended)
- Install a newer Ruby version with rbenv or rvm

### Port Already in Use

If port 4000 is busy:
```bash
bundle exec jekyll serve --port 4001
```

### Changes Not Showing

1. Stop the server (Ctrl+C)
2. Clear the cache:
```bash
bundle exec jekyll clean
```
3. Restart the server

## What's New in Your Portfolio

### ✨ Features Added:

1. **Modern Hero Section** - Eye-catching gradient header with call-to-action buttons
2. **About Section** - Professional introduction highlighting your expertise
3. **Skills Grid** - Organized display of technical skills by category
4. **Enhanced Projects** - Beautiful card-based project showcase
5. **Contact Section** - Easy-to-find contact links with icons
6. **Responsive Design** - Perfect on all devices (mobile, tablet, desktop)
7. **Smooth Navigation** - Sticky header with smooth scrolling
8. **SEO Optimized** - Better search engine visibility
9. **Custom 404 Page** - Branded error page
10. **Professional Styling** - Modern color scheme and typography

### 📁 Files Modified/Created:

- `index.markdown` - Complete homepage redesign
- `_layouts/default.html` - Custom layout with navigation
- `_layouts/post.html` - Enhanced project post layout
- `_includes/head.html` - SEO and meta tags
- `assets/css/style.css` - Comprehensive custom styling (682 lines)
- `_posts/2025-03-03-ResumeCreator.markdown` - Enhanced project showcase
- `_config.yml` - Updated configuration with SEO
- `404.html` - Modern error page
- `README.md` - Updated documentation
- `Gemfile` - Added SEO plugins

## Next Steps

1. **Deploy to GitHub Pages** (recommended - easiest option)
2. **Add more projects** - Create new posts in `_posts/` directory
3. **Customize colors** - Edit CSS variables in `assets/css/style.css`
4. **Add images** - Place project screenshots in `assets/images/`
5. **Update content** - Personalize the About and Skills sections

## Support

If you encounter any issues:
1. Check the GitHub Actions tab for build errors
2. Ensure all files are committed and pushed
3. Verify GitHub Pages is enabled in repository settings
4. Wait a few minutes for changes to propagate

---

**Your portfolio is ready to impress! 🚀**