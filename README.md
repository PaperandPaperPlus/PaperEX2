# PaperEX Website

This is the official website for PaperEX, a sustainable paper packaging solutions company.

## GitHub Pages Deployment

This website is configured to deploy automatically to GitHub Pages when changes are pushed to the main branch.

### Setup Instructions

1. **Enable GitHub Pages:**
   - Go to your repository settings
   - Navigate to "Pages" section
   - Under "Source", select "GitHub Actions"

2. **Repository Structure:**
   - The website files are in the root directory
   - `index.html` is the main entry point
   - All assets are in the `assets/` folder
   - `.nojekyll` file tells GitHub Pages this is not a Jekyll site

3. **Deployment:**
   - The site will automatically deploy when you push to the main branch
   - Check the "Actions" tab for deployment status
   - The site will be available at `https://yourusername.github.io/repository-name`

### Local Development

To run the website locally:

1. Use a local server (like Live Server in VS Code)
2. Or use Python's built-in server:
   ```bash
   python -m http.server 8000
   ```
3. Open `http://localhost:8000` in your browser

### File Structure

```
├── index.html          # Main HTML file
├── assets/             # All website assets
│   ├── static/        # CSS files
│   ├── entries/       # JavaScript files
│   └── *.png, *.jpg   # Images
├── .nojekyll          # Tells GitHub Pages this isn't Jekyll
└── .github/workflows/  # GitHub Actions configuration
```

### Troubleshooting

If assets don't load on GitHub Pages:
- Ensure all paths use relative paths (starting with `./` not `/`)
- Check that the `.nojekyll` file exists
- Verify the GitHub Actions workflow is running successfully
- Check the browser's developer console for 404 errors