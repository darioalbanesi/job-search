# UX Careers Switzerland - Course Website

A comprehensive static course website for UX professionals seeking career opportunities in Switzerland.

## Website Structure

- **Homepage** (`index.html`) - Course overview and introduction
- **Job Search Guide** (`swiss-job-search.html`) - Complete guide to the Swiss UX job market
- **Market Expectations** (`ux-market.html`) - Skills analysis and employer expectations
- **CV & ATS** (`cv-ats.html`) - CV optimization for Swiss employers
- **CV Tailoring** (`tailored-cv.html`) - Customization strategies for specific roles
- **About** (`about.html`) - Agency information and services

## Features

- Fully responsive design optimized for all devices
- Professional styling suitable for recruitment agency
- ATS-friendly content structure and formatting
- Comprehensive market insights specific to Switzerland
- Practical examples and before/after comparisons

## Automatic Deployment

This repository is configured with GitHub Actions to automatically deploy to an FTP server when changes are pushed to the main branch.

### Setup FTP Deployment

To enable automatic deployment, add the following secrets to your GitHub repository:

1. Go to your GitHub repository
2. Click on **Settings** → **Secrets and variables** → **Actions**
3. Click **New repository secret** and add:

   - `FTP_SERVER` - Your FTP server hostname (e.g., `ftp.yourwebsite.com`)
   - `FTP_USERNAME` - Your FTP username
   - `FTP_PASSWORD` - Your FTP password

### Deployment Process

When you push changes to the main branch:
1. GitHub Actions automatically triggers
2. The workflow checks out the latest code
3. Files are deployed to your FTP server
4. Your live website is updated instantly

## Local Development

To make changes locally:

```bash
# Clone the repository
git clone git@github.com:darioalbanesi/job-search.git
cd job-search

# Make your changes
# Open files in your preferred editor

# Commit and push changes
git add .
git commit -m "Your commit message"
git push origin main
```

## File Structure

```
job-search/
├── index.html                 # Homepage
├── swiss-job-search.html      # Job search guide
├── ux-market.html            # Market expectations
├── cv-ats.html               # CV optimization
├── tailored-cv.html          # CV tailoring
├── about.html                # About page
├── assets/
│   └── styles.css            # Main stylesheet
└── .github/
    └── workflows/
        └── deploy.yml        # GitHub Actions deployment
```

## Technical Details

- **Framework**: Pure HTML5 + CSS3 (no JavaScript required)
- **Styling**: Custom responsive CSS with professional design
- **Deployment**: GitHub Actions with FTP deployment
- **Hosting**: Compatible with any web server or static hosting service

## Content Updates

The course content is regularly updated to reflect current Swiss UX market conditions. All updates are automatically deployed when pushed to the main branch.

---

*Created by specialized recruiters for digital UX professionals in Switzerland*