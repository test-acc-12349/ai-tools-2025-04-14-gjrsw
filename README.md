# AI Tools Directory 🤖

> The ultimate directory of AI tools and resources for professionals, developers, and enthusiasts.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Netlify Status](https://api.netlify.com/api/v1/badges/YOUR-BADGE/deploy-status)](https://app.netlify.com/)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Support & Resources](#support--resources)

## Overview

AI Tools Directory is a modern, responsive directory website showcasing artificial intelligence tools and resources in a clean, three-column grid layout. Built with HTML, CSS, and JavaScript, it offers easy customization and quick deployment options.

## Features

- 🎯 Responsive 3-column grid layout
- 🔍 Search functionality
- 🏷️ Category filtering
- 💨 Fast loading times
- 📱 Mobile-friendly design
- 🎨 Customizable styling
- 🔄 Easy content updates

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- Git
- Text editor (VS Code recommended)

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ai-tools-directory.git

# Navigate to project directory
cd ai-tools-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
ai-tools-directory/
├── src/
│   ├── assets/
│   │   ├── images/
│   │   └── styles/
│   ├── data/
│   │   └── tools.json
│   ├── js/
│   │   └── main.js
│   └── index.html
├── public/
├── package.json
└── README.md
```

## Customization Guide

### Adding Directory Items

Edit `src/data/tools.json`:

```json
{
  "tools": [
    {
      "name": "Tool Name",
      "description": "Tool description",
      "category": "Category",
      "url": "https://example.com",
      "image": "tool-image.png"
    }
  ]
}
```

### Modifying Categories

Update the categories array in `src/js/main.js`:

```javascript
const categories = [
  'All',
  'ChatBots',
  'Image Generation',
  'Text Analysis'
];
```

### Updating Hero Section

Modify the hero section in `src/index.html`:

```html
<section class="hero">
  <h1>Your New Title</h1>
  <p>Your new description</p>
</section>
```

### Customizing Colors

Edit `src/assets/styles/variables.css`:

```css
:root {
  --primary-color: #your-color;
  --secondary-color: #your-color;
  --text-color: #your-color;
  --background-color: #your-color;
}
```

## Deployment

### Netlify Deployment

1. Push your repository to GitHub
2. Login to Netlify
3. Click "New site from Git"
4. Select your repository
5. Configure build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
6. Click "Deploy site"

### Vercel Deployment

```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel
```

## Custom Domain Setup

1. Purchase domain from preferred registrar
2. Add domain in deployment platform:
   ```
   Custom Domains → Add Custom Domain → yourdomain.com
   ```
3. Configure DNS settings:
   - Type: A Record
   - Name: @
   - Value: [Your deployment platform IP]
   - TTL: 3600

## Troubleshooting

### Common Issues

1. **Images not loading**
   - Check image paths in `tools.json`
   - Verify images are in correct directory
   - Ensure proper image formats (PNG/JPG)

2. **Search not working**
   - Clear browser cache
   - Check console for JavaScript errors
   - Verify search input ID matches JS selector

3. **Styling issues**
   - Validate CSS syntax
   - Check browser compatibility
   - Inspect element for CSS conflicts

## Support & Resources

- 📖 [Documentation Wiki](https://github.com/yourusername/ai-tools-directory/wiki)
- 🐛 [Issue Tracker](https://github.com/yourusername/ai-tools-directory/issues)
- 💬 [Community Discord](https://discord.gg/yourserver)
- 📧 [Support Email](mailto:support@example.com)

### Useful Links

- [HTML Best Practices](https://www.w3schools.com/html/html5_syntax.asp)
- [CSS Grid Guide](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [JavaScript Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by [Your Name](https://github.com/yourusername)