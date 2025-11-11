# How to Publish Your PDFs and References

This guide will help you publish your existing clickable references table and PDF files to this repository.

## Step 1: Add Your PDF Files

1. Copy all your PDF files to the `pdfs/` directory in this repository
2. You can organize them in subdirectories if you have many files, for example:
   - `pdfs/2024/`
   - `pdfs/papers/`
   - `pdfs/reports/`

## Step 2: Update the References Table

If you already have a references table HTML file:

### Option A: Replace the entire index.html
1. Replace the `index.html` file with your existing HTML file
2. Make sure all PDF links point to the `pdfs/` directory (e.g., `pdfs/your-file.pdf`)

### Option B: Copy your table into the existing index.html
1. Open your existing HTML references table
2. Copy the table rows (the `<tr>` elements)
3. Paste them into the `index.html` file, replacing the example rows
4. Ensure the PDF links are correct (e.g., `href="pdfs/your-file.pdf"`)

## Step 3: Commit and Push Your Changes

```bash
# Add all new files
git add pdfs/ index.html

# Commit your changes
git commit -m "Add reference PDFs and update table"

# Push to GitHub
git push origin main
```

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/[your-username]/TLC-References`
2. Click on **Settings** at the top of the page
3. Scroll down to the **Pages** section in the left sidebar
4. Under **Source**, select **GitHub Actions** (this will use the workflow we've set up)
5. Wait a few minutes for the deployment to complete

## Step 5: Access Your Published References

Once GitHub Pages is deployed, your references will be available at:

```
https://[your-username].github.io/TLC-References/
```

You can share this URL with anyone, and they'll be able to:
- View your references table
- Click on any reference to download or view the PDF

## Example Table Row

Here's how to add a reference to your table:

```html
<tr>
    <td>Document Title Here</td>
    <td>Author Name(s)</td>
    <td>2024</td>
    <td class="description">Brief description of what this document contains.</td>
    <td><a href="pdfs/your-file.pdf" class="pdf-link" target="_blank">View PDF</a></td>
</tr>
```

## Tips for Links

- **Relative paths**: Use `pdfs/filename.pdf` for files in the pdfs folder
- **Subdirectories**: Use `pdfs/2024/filename.pdf` if you organized files in subdirectories
- **No spaces**: Avoid spaces in filenames (use hyphens or underscores instead)

## Troubleshooting

### PDFs not loading?
- Check that the file path in your HTML matches the actual location of the PDF
- Make sure the PDF file was committed and pushed to GitHub
- Verify that GitHub Pages is enabled in your repository settings

### Changes not showing up?
- GitHub Pages can take a few minutes to update after you push changes
- Try clearing your browser cache or opening the page in an incognito/private window

## Need Help?

If you encounter issues, please open an issue in this repository with details about the problem.
