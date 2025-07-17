# Personal Academic Website

This is the source code for my personal academic website built with Hugo and the PaperMod theme.

## 🚀 Quick Start

### Prerequisites
- [Hugo](https://gohugo.io/getting-started/installing/) (Extended version)
- [Git](https://git-scm.com/)

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/noor01/noor01.github.io.git
cd noor01.github.io
```

2. Initialize and update the theme submodule:
```bash
git submodule update --init --recursive
```

3. Start the development server:
```bash
hugo server -D
```

4. Open your browser and navigate to `http://localhost:1313`

## 📁 Project Structure

```
├── .github/workflows/    # GitHub Actions for deployment
├── archetypes/           # Content templates
├── assets/css/           # Custom CSS
├── content/              # Website content
│   ├── papers/           # Research papers
│   ├── courses/          # Teaching materials
│   └── tools/            # Tools and datasets
├── layouts/              # Custom layouts
├── static/               # Static files (images, PDFs, etc.)
├── themes/PaperMod/      # Hugo theme (git submodule)
└── config.yml            # Site configuration
```

## 🛠️ Customization

### Personal Information
Update the following in `config.yml`:
- `baseURL`: Your GitHub Pages URL
- `title`: Your name
- `author`: Your name
- Social media links in `socialIcons`
- Profile information in `homeInfoParams`

### Adding Content

#### Papers
```bash
hugo new papers/my-paper.md
```

#### Courses
```bash
hugo new courses/my-course.md
```

#### Tools
```bash
hugo new tools/my-tool.md
```

### Styling
- Custom CSS: `assets/css/extended/custom.css`
- The theme uses CSS variables for easy customization

## 🚀 Deployment

This site is automatically deployed to GitHub Pages using GitHub Actions when you push to the main branch.

### Setup GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages" section
3. Select "GitHub Actions" as the source
4. The workflow will automatically build and deploy your site

## 📝 Content Management

### Front Matter Examples

**Paper:**
```yaml
---
title: "Paper Title"
date: 2024-01-15
authors: ["Your Name", "Co-Author"]
publication: "Conference Name"
abstract: "Brief description"
tags: ["tag1", "tag2"]
url_pdf: "paper.pdf"
url_code: "https://github.com/user/repo"
---
```

**Tool/Dataset:**
```yaml
---
title: "Tool Title"
date: 2024-01-15
author: "Your Name"
description: "Brief description"
tags: ["tag1", "tag2"]
categories: ["Tools"]
url_download: "download-link"
url_code: "github-link"
---
```

## 🎨 Theme

This website uses the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme, which is:
- Fast and lightweight
- Responsive design
- Dark/light mode support
- SEO friendly
- Academic-focused modifications

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📧 Contact

For questions or suggestions, please open an issue or contact me through the social media links on the website.

## 🔗 Links

- [Live Website](https://noor01.github.io)
- [Hugo Documentation](https://gohugo.io/documentation/)
- [PaperMod Theme](https://github.com/adityatelange/hugo-PaperMod)
- [GitHub Pages](https://pages.github.com/) 