# GitHub Pages Setup Instructions

This file contains instructions for enabling GitHub Pages for this repository after the PR is merged.

## Prerequisites

This repository is now configured with:
- ✅ Hugo static site generator
- ✅ Custom theme
- ✅ Sample content
- ✅ GitHub Actions workflow for automatic deployment

## Steps to Enable GitHub Pages

After merging this PR to the `main` branch, follow these steps:

### 1. Enable GitHub Pages

1. Go to your repository on GitHub: https://github.com/rockifanze/rockifanze.com
2. Click on **Settings** tab
3. Scroll down to the **Pages** section in the left sidebar
4. Under **Source**, select **GitHub Actions**
5. The workflow will automatically run on the next push to `main`

### 2. Wait for Deployment

- After merging to `main`, the GitHub Actions workflow will automatically trigger
- You can monitor the deployment in the **Actions** tab
- The first deployment typically takes 1-2 minutes

### 3. Access Your Site

Once deployed, your site will be available at:
**https://rockifanze.github.io/rockifanze.com/**

## Troubleshooting

### If the site doesn't deploy:

1. Check the **Actions** tab for any workflow errors
2. Ensure GitHub Pages is enabled and set to "GitHub Actions" as the source
3. Verify the `main` branch has the latest changes

### If the site displays incorrectly:

1. Check that the `baseURL` in `hugo.toml` matches your GitHub Pages URL
2. Ensure the theme files are present in the `themes/simple/` directory

## Making Updates

To update the site:

1. Edit content in the `content/` directory
2. Commit and push to `main` branch
3. The site will automatically rebuild and deploy

## Local Development

To preview changes locally before pushing:

```bash
hugo server
```

Then visit http://localhost:1313

## Additional Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)
