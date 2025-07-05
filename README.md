# Ops Handbook Template

A template repository for creating technical documentation sites using Hugo and the Docsy theme.

## Getting Started

### 1. Create Your Repository from Template

1. Visit [Ops Handbook Template](https://github.com/xyna-bpinelab/ops-handbook)
2. Click the green "Use this template" button at the top of the repository
3. Select "Create a new repository" from the dropdown menu
4. In the "Create a new repository" page:
   - Choose your repository name
   - Add an optional description
   - Select repository visibility (Public/Private)
   - Click "Create repository from template"

### 2. Set Up Your Local Environment

1. **Clone your new repository**
```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```

2. **Start the development server**
```bash
docker compose up
```

3. **Access your site**
   - Open http://localhost:1313/YOUR_REPO_NAME/ in your browser
   - The site will automatically reload when you make changes

## Customization

### Site Configuration

Edit `config.toml` to customize:
- Site title and description
- Base URL
- Theme settings
- Language settings

### Content Management

1. **Add new pages**
   - Create Markdown files in `content/en/` and `content/ja/`
   - Follow the existing content structure

2. **Modify existing content**
   - Edit files in `content/en/` and `content/ja/`
   - Use Hugo's front matter for metadata

### Theme Customization

1. **Override theme components**
   - Copy components from `themes/docsy/layouts/` to `layouts/`
   - Modify the copied files to customize the theme

2. **Add custom assets**
   - Place custom CSS in `assets/scss/`
   - Add custom JavaScript to `assets/js/`

## Deployment

### GitHub Pages Setup

1. **Enable GitHub Pages**
   - Go to your repository's Settings
   - Click "Pages" in the left sidebar
   - Under "Source", select:
     - Branch: `gh-pages`
     - Folder: `/(root)`
   - Click "Save"

2. **Automatic Deployment**
   - The site is automatically built and deployed when you push to the `main` branch
   - GitHub Actions workflow (`.github/workflows/gh-pages.yml`) handles the deployment process
   - You can monitor the deployment status in the "Actions" tab of your repository

## Features

- Modern UI with Docsy theme
- Japanese content support
- Offline search functionality
- Syntax highlighting
- Responsive design
- Docker-based development environment
- Automated deployment with GitHub Actions

## License

This template is licensed under the [MIT License](LICENSE).

## Contributing

1. Fork this template repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request 