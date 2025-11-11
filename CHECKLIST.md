# Setup Checklist for Publishing Your PDFs

Follow these steps to get your references table online:

## Initial Setup

- [ ] **Merge this PR** into the main branch
- [ ] **Clone or pull** the latest changes from main branch

## Add Your Content

- [ ] **Upload PDFs** to the `pdfs/` directory
  - Copy all your PDF files into this folder
  - Use descriptive filenames without spaces (e.g., `author-year-title.pdf`)
  
- [ ] **Update index.html** with your references
  - Open `index.html` in a text editor
  - Find the `<tbody>` section
  - Replace the sample rows with your actual references
  - Use the template in `docs/table-row-template.html` for each new row
  - Verify that PDF filenames in the HTML match your actual files

- [ ] **Test locally** (optional)
  - Open `index.html` in a web browser
  - Click on the PDF links to make sure they work

## Publish to GitHub

- [ ] **Commit your changes**
  ```bash
  git add pdfs/ index.html
  git commit -m "Add my reference PDFs and update table"
  git push origin main
  ```

## Enable GitHub Pages

- [ ] **Go to repository Settings**
  - Navigate to: `https://github.com/dschwar487/TLC-References/settings`
  
- [ ] **Enable GitHub Pages**
  - Click on "Pages" in the left sidebar
  - Under "Source", select **GitHub Actions**
  - Click "Save"
  
- [ ] **Wait for deployment** (2-5 minutes)
  - Go to the "Actions" tab to watch the deployment progress
  - Once complete, you'll see a green checkmark

## Verify Your Site

- [ ] **Visit your published site**
  - Go to: `https://dschwar487.github.io/TLC-References/`
  - Verify the table displays correctly
  - Test clicking on a few PDF links
  
- [ ] **Share the URL**
  - Share `https://dschwar487.github.io/TLC-References/` with others
  - They can now access your references from anywhere!

## Future Updates

When you need to add or update references:

1. Add new PDFs to the `pdfs/` directory
2. Add corresponding rows to `index.html`
3. Commit and push to main branch
4. GitHub Pages will automatically update within a few minutes

---

**Need Help?** See `INSTRUCTIONS.md` for detailed guidance or `docs/QUICK-REFERENCE.md` for quick tips.
