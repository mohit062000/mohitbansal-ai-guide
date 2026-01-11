# GitHub Pages Deployment Guide

## 🚀 Your Site
**Live URL:** https://mohit062000.github.io/mohitbansal-ai-guide/

## ✨ What's New

Your site now features:
- **Dynamic Repository Detection** - Automatically uses your GitHub username and repo
- **Modern Gradient Design** - Purple gradient background with clean white content cards
- **Smooth Animations** - Fade-in effects and smooth scrolling
- **Responsive Layout** - Works perfectly on mobile and desktop
- **Professional Styling** - Bootstrap 5 with custom CSS enhancements

## 🔧 How It Works

The `generate_json.py` script now:
1. Detects your repository info from git config automatically
2. Uses your username (`mohit062000`) and repo name dynamically
3. Generates a beautiful, modern HTML page with your branding
4. Creates JSON API endpoints for all guides

## 📝 Local Testing

```bash
# Build the site
make site-build

# Run local server
make site-run

# Visit http://localhost:9090
```

## 🔄 Deployment

The site deploys automatically via GitHub Actions when you:
1. Push to `main` branch
2. Create a release

### Manual Deployment
1. Go to https://github.com/mohit062000/mohitbansal-ai-guide/actions
2. Click "CI/CD" workflow
3. Click "Run workflow"
4. Select `main` branch

## 🎨 Customization

To customize the look:
- Edit `.github/scripts/generate_json.py`
- Modify the `<style>` section in the HTML template
- Change colors, fonts, or layout as needed

### Current Color Scheme
- Primary: `#667eea` (Purple)
- Secondary: `#764ba2` (Dark Purple)
- Gradient: `linear-gradient(135deg, #667eea 0%, #764ba2 100%)`

## 📦 What Gets Generated

```
site/
├── index.html          # Main landing page (styled)
├── api.json           # API index
├── version-badge.json # Version badge for shields.io
└── api/
    ├── guide.json     # Main guide content
    └── guides/
        ├── languages/ # Language-specific guides
        ├── patterns/  # Pattern guides
        └── platforms/ # Platform guides
```

## 🔗 Key Features

1. **Auto-detection** - No hardcoded URLs, works with any fork
2. **Beautiful UI** - Modern, professional design
3. **Fast Loading** - Optimized with CDN resources
4. **SEO Friendly** - Proper meta tags and structure
5. **Mobile Ready** - Responsive Bootstrap layout

## 🐛 Troubleshooting

If the site doesn't update:
1. Check GitHub Actions status
2. Verify GitHub Pages is enabled (Settings → Pages)
3. Ensure source is set to "GitHub Actions"
4. Wait 2-3 minutes for deployment to complete

## 📚 Resources

- [Original Guide](https://dwmkerr.github.io/ai-developer-guide/)
- [GitHub Pages Docs](https://docs.github.com/en/pages)
- [Bootstrap 5 Docs](https://getbootstrap.com/docs/5.3/)
