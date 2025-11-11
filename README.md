# TLC-References

A repository for hosting and sharing clickable PDF references through GitHub Pages.

## Overview

This repository contains a clickable references table (HTML) that links to local PDFs, making them accessible remotely from any computer with internet access.

## Quick Start

### 1. Add Your PDFs

Upload your PDF files to the `pdfs/` directory:

```bash
git add pdfs/your-document.pdf
git commit -m "Add reference PDF"
git push
```

### 2. Update the References Table

Edit `index.html` and add your references to the table. Follow this pattern:

```html
<tr>
    <td>Your Document Title</td>
    <td>Author Name(s)</td>
    <td>2024</td>
    <td class="description">Brief description of the document.</td>
    <td><a href="pdfs/your-document.pdf" class="pdf-link" target="_blank">View PDF</a></td>
</tr>
```

### 3. Enable GitHub Pages

1. Go to your repository Settings
2. Navigate to "Pages" in the left sidebar
3. Under "Source", select the `main` branch
4. Click "Save"

Your references will be available at: `https://[your-username].github.io/TLC-References/`

## Accessing Your References

Once GitHub Pages is enabled, your references table will be accessible at:

```
https://[your-username].github.io/TLC-References/
```

Anyone with this URL can view the references table and access the PDFs.

## File Structure

```
TLC-References/
├── index.html          # Main references table (clickable HTML)
├── pdfs/              # Directory for PDF files
│   └── .gitkeep       # Placeholder file
├── docs/              # Optional: Additional documentation
└── README.md          # This file
```

## Tips

- **PDF Naming**: Use descriptive, URL-friendly filenames (e.g., `smith-2024-analysis.pdf`)
- **File Size**: Be mindful of PDF file sizes; GitHub has a 100MB per-file limit
- **Organization**: For many PDFs, consider organizing them into subdirectories (e.g., `pdfs/2024/`, `pdfs/category/`)
- **Updates**: Any changes pushed to the main branch will automatically update the GitHub Pages site

## Customization

You can customize the appearance of the references table by editing the CSS in the `<style>` section of `index.html`.

## Support

For issues or questions, please open an issue in this repository.