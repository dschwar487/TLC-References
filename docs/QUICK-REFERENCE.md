# Quick Reference: Adding a New PDF Reference

## Step 1: Add Your PDF
Place your PDF file in the `pdfs/` directory:
```bash
cp /path/to/your/document.pdf pdfs/your-document.pdf
```

## Step 2: Add a Table Row
Open `index.html` and add a new row in the `<tbody>` section:

```html
<tr>
    <td>Your Document Title</td>
    <td>Author Name(s)</td>
    <td>2024</td>
    <td class="description">Brief description of the document.</td>
    <td><a href="pdfs/your-document.pdf" class="pdf-link" target="_blank">View PDF</a></td>
</tr>
```

## Step 3: Commit and Push
```bash
git add pdfs/your-document.pdf index.html
git commit -m "Add new reference: Your Document Title"
git push origin main
```

## Step 4: View Changes
After a few minutes, your changes will be live at:
```
https://dschwar487.github.io/TLC-References/
```

## Template
Copy and paste this template for each new reference:

```html
<tr>
    <td>TITLE_HERE</td>
    <td>AUTHOR_HERE</td>
    <td>YEAR_HERE</td>
    <td class="description">DESCRIPTION_HERE</td>
    <td><a href="pdfs/FILENAME_HERE.pdf" class="pdf-link" target="_blank">View PDF</a></td>
</tr>
```

## Tips
- Keep PDF filenames simple and without spaces (use hyphens or underscores)
- Make descriptions concise but informative
- List multiple authors separated by commas
- Check that your PDF path matches the actual filename
