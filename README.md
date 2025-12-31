# Feast

A static website for a restaurant delivery marketplace that empowers restaurants, couriers, and customers without the crippling fees. This project is a migration from a previously Django-based application to a fully static website, designed for simplicity, performance, and easy deployment using GitHub Pages.

## Badges

[![Static Website](https://img.shields.io/badge/Website-Static-green.svg)](https://github.com)
[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-blue.svg)](https://pages.github.com/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## Installation

Since this is a static website, no build process is required. Simply clone the repository and open `index.html` in your browser:

```bash
  git clone https://github.com/your-username/lets_feast.git
  cd lets_feast
```

Then open `index.html` in your web browser, or serve it using a local web server:

```bash
  # Using Python
  python -m http.server 8000
  
  # Using Node.js (if you have http-server installed)
  npx http-server
```

## Deployment

This project is configured for automatic deployment to GitHub Pages using GitHub Actions.

### Setting up GitHub Pages

1. **Enable GitHub Pages in repository settings:**
   - Go to your repository on GitHub
   - Navigate to **Settings** → **Pages**
   - Under **Source**, select **"GitHub Actions"** (not "Deploy from a branch")
   - Save the settings

2. **Push your code:**
   - The workflow will automatically trigger on push to `main` or `master` branch
   - You can also manually trigger it from the **Actions** tab → **Deploy to GitHub Pages** → **Run workflow**

3. **Check deployment status:**
   - Go to the **Actions** tab to see the workflow status
   - Once successful, your site will be available at:
     - `https://[your-username].github.io/lets_feast/`
     - Or `https://[your-org].github.io/lets_feast/` if it's an organization repository

4. **Troubleshooting:**
   - Ensure GitHub Pages is set to use **"GitHub Actions"** as the source (not a branch)
   - Check the Actions tab for any workflow errors
   - Wait a few minutes after the workflow completes for DNS propagation
   - Clear your browser cache if you see a 404 error

## Appendix

### Technology Stack

- **HTML5** - Semantic markup and structure
- **Tailwind CSS** (CDN) - Utility-first CSS framework for styling
- **JavaScript (Vanilla)** - Client-side interactivity and functionality
- **Bootstrap 5** - Additional UI components and utilities
- **Bootstrap Icons** - Icon library
- **Owl Carousel 2** - Image and content carousel
- **Swiper** - Touch slider component
- **GitHub Pages** - Static site hosting and deployment
- **Plausible Analytics** - Privacy-friendly web analytics

### Project Structure

```
lets_feast/
├── css/
│   ├── fonts.css          # Custom font definitions
│   ├── index.css          # Page-specific styles
│   └── styles.css         # Global styles
├── fonts/
│   ├── mortend-extended/  # Mortend Extended font family
│   └── neusa-next/        # Neusa Next font family
├── img/
│   ├── logos/             # Brand logos and icons
│   └── stock/             # Stock images and photos
├── js/
│   ├── apis/
│   │   └── blog.js        # Blog API integration
│   ├── inquiry/
│   │   └── inquiry.js     # Contact form handling
│   ├── utils/
│   │   ├── common.js      # Common utility functions
│   │   ├── constants.js   # Application constants
│   │   ├── elements.js    # DOM element utilities
│   │   └── images.js      # Image handling utilities
│   ├── base.js            # Base application logic
│   ├── carousel.js        # Carousel functionality
│   ├── home.js            # Home page specific scripts
│   └── trix.js            # Trix editor integration
├── json/
│   └── phone-codes.json   # Country phone codes data
├── index.html             # Main HTML file
└── README.md              # Project documentation
```

## Authors

- [@dunosis](https://www.dunosis.com) - Made by Dunosis
