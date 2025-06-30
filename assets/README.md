# Assets Directory

This directory contains all static assets for the portfolio website.

## Structure

```
assets/
├── css/           # Stylesheets and SCSS files
├── documents/     # PDF files, resume, and other documents
├── fonts/         # Custom fonts (if any)
├── images/        # Profile photos, icons, and other images
└── js/            # JavaScript files (if any)
```

## File Organization

- **CSS**: All styling files including the main `style.scss`
- **Documents**: Resume PDF and any other downloadable documents
- **Images**: Profile photos, favicons, project screenshots
- **Fonts**: Custom web fonts (currently empty)
- **JS**: JavaScript files for enhanced functionality (currently empty)

## Usage

All assets are referenced using Jekyll's `relative_url` filter:
```liquid
{{ '/assets/images/profile.jpg' | relative_url }}
{{ '/assets/documents/resume.pdf' | relative_url }}
```

This ensures proper URL generation for both local development and GitHub Pages deployment.
