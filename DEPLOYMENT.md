# Deployment Guide for GitHub Pages

This guide will help you deploy your professional portfolio website to GitHub Pages.

## Prerequisites

1. **GitHub Account**: You'll need a GitHub account
2. **Git**: Installed on your local machine
3. **Ruby & Jekyll** (for local development): Optional but recommended

## Step 1: Create GitHub Repository

1. **Create a new repository** on GitHub with the name: `vineethkumar-marpadge.github.io`
   - Replace `vineethkumar-marpadge` with your actual GitHub username
   - Make sure the repository is **public**
   - Initialize with a README (you can replace it later)

## Step 2: Upload Your Site Files

### Option A: Using Git Command Line

1. **Clone your new repository**:
   ```bash
   git clone https://github.com/vineethkumar-marpadge/vineethkumar-marpadge.github.io.git
   cd vineethkumar-marpadge.github.io
   ```

2. **Copy all portfolio files** from `/Users/marpadv/vineethkumar-portfolio/` to your cloned repository directory

3. **Add, commit, and push**:
   ```bash
   git add .
   git commit -m "Initial portfolio website deployment"
   git push origin main
   ```

### Option B: Using GitHub Web Interface

1. **Upload files directly** through GitHub's web interface
2. **Drag and drop** all files from your portfolio folder
3. **Commit changes** with a descriptive message

## Step 3: Configure GitHub Pages

1. **Go to your repository** on GitHub
2. **Click on "Settings"** tab
3. **Scroll down to "Pages"** section
4. **Under "Source"**, select "Deploy from a branch"
5. **Select "main" branch** and "/ (root)" folder
6. **Click "Save"**

## Step 4: Customize Your Site

### Update Configuration

Edit `_config.yml` to match your information:

```yaml
title: Your Name - AWS Cloud Support Engineer
email: your.email@example.com
description: Your professional description
url: "https://your-username.github.io"
github_username: your-username
linkedin_username: your-linkedin-username
```

### Add Your Profile Image

✅ **Your professional photo is already included!** 
- Your image is located at `assets/images/profile.jpg`
- The image shows you in professional AWS attire with excellent quality
- It's properly optimized for web display (251KB)
- The website is configured to display it prominently on the homepage and about page

**Image specifications:**
- **Location**: `assets/images/profile.jpg`
- **Size**: Optimized for web (251KB)
- **Format**: Professional headshot in AWS branded attire
- **Usage**: Homepage hero section and About page
- **Styling**: Circular crop with AWS orange border and hover effects

### Update Contact Information

Edit `contact.md` to include your actual:
- Email address
- LinkedIn profile URL
- GitHub profile URL
- Location (if desired)

### Customize Content

Review and update all pages:
- `index.md`: Homepage content
- `about.md`: Personal and professional background
- `experience.md`: Work history and achievements
- `skills.md`: Technical expertise
- `projects.md`: Case studies and projects
- `blog.md`: Blog introduction

## Step 5: Set Up Custom Domain (Optional)

If you want to use a custom domain:

1. **Purchase a domain** from a domain registrar
2. **Create a CNAME file** in your repository root with your domain name
3. **Configure DNS** with your domain provider:
   - Add a CNAME record pointing to `your-username.github.io`
4. **Update GitHub Pages settings** to use your custom domain

## Step 6: Enable HTTPS

1. **In GitHub Pages settings**, check "Enforce HTTPS"
2. **Wait for SSL certificate** to be provisioned (may take a few minutes)

## Step 7: Test Your Site

1. **Visit your site** at `https://your-username.github.io`
2. **Test all pages** and navigation
3. **Check mobile responsiveness**
4. **Verify contact forms** work (if using external form service)

## Local Development Setup

For local development and testing:

1. **Install Ruby and Bundler**:
   ```bash
   # On macOS with Homebrew
   brew install ruby
   gem install bundler
   ```

2. **Install dependencies**:
   ```bash
   cd your-repository
   bundle install
   ```

3. **Run locally**:
   ```bash
   bundle exec jekyll serve
   ```

4. **View at** `http://localhost:4000`

## Troubleshooting

### Common Issues

1. **Site not updating**: 
   - Check GitHub Actions tab for build errors
   - Ensure all files are properly committed
   - Wait a few minutes for changes to propagate

2. **CSS not loading**:
   - Check file paths in `_config.yml`
   - Ensure `assets/css/style.scss` exists
   - Verify SCSS syntax is correct

3. **Images not displaying**:
   - Check image file paths
   - Ensure images are in `assets/images/` directory
   - Verify image file names match references

4. **404 errors**:
   - Check permalink settings in page front matter
   - Ensure navigation links match actual page URLs

### Build Errors

If you see build errors in GitHub Actions:

1. **Check the Actions tab** in your repository
2. **Review error messages** in the build log
3. **Common fixes**:
   - Fix YAML syntax errors in `_config.yml`
   - Ensure all required gems are in `Gemfile`
   - Check for typos in file names and paths

## Maintenance

### Regular Updates

1. **Keep content current**: Update experience, skills, and projects
2. **Add blog posts**: Share new insights and experiences
3. **Update dependencies**: Occasionally update gems in `Gemfile`
4. **Monitor performance**: Use Google PageSpeed Insights

### SEO Optimization

1. **Add meta descriptions** to all pages
2. **Use descriptive page titles**
3. **Include relevant keywords** naturally in content
4. **Submit sitemap** to Google Search Console

## Security Considerations

1. **Never commit sensitive information**:
   - API keys
   - Personal phone numbers
   - Private email addresses
   - Internal company information

2. **Use contact forms** instead of direct email links to prevent spam

3. **Keep dependencies updated** to avoid security vulnerabilities

## Support

If you encounter issues:

1. **Check GitHub Pages documentation**: https://docs.github.com/en/pages
2. **Jekyll documentation**: https://jekyllrb.com/docs/
3. **GitHub Community**: https://github.community/

---

**Congratulations!** Your professional portfolio is now live on GitHub Pages. Remember to keep it updated with your latest achievements and experiences.

*Your site will be available at: `https://your-username.github.io`*
