# PDF Diff: Compare two PDFs and highlight differences.

- No installation required
- Fast, easy, and free
- Files are processed locally in your browser -- nothing is uploaded or saved

> **Disclaimer:** Please do not fully rely on this tool as it has limitations. If you find any issues or have ideas for improvement, feel free to contribute. PRs are welcome!

## Usage

### Option 1: GitHub Pages
Use the link hosted by GitHub Pages: [link](https://leolee7.github.io/PDF_diff/)  
### Option 2: Open locally
```
git clone https://github.com/LeoLee7/PDF_diff.git
cd PDF_diff
open pdf_diff_app.html
```

### Test Case

![alt text](/assets/test_case.jpg)
This test case is created by a nervous Ph.D. student named Li.
<br>  


<br>  

### Use it: Drop two PDFs and click Compare.  
![alt text](/assets/upload.jpg)





## What It Does

### Visual Diff (default view)
Renders both PDFs side by side with changes highlighted directly on the page images.
- Changed words are highlighted (red on the original, green on the modified)
- Changed or new figures/images are detected and marked with a dashed border
- Position shifts from layout reflow (e.g., Overleaf spacing adjustments) are ignored
- Each page shows a count of how many changes were found

### Text Diff
Side-by-side text comparison with three levels of granularity.
- Lines that differ get a colored sidebar
- Within those lines, only the changed words are highlighted
- Within those words, only the changed characters are highlighted.
- Synced scrolling between left and right panels

### Diff Navigation
A floating navigator (bottom right) lets you jump between pages with changes.

### Download
Click "Download PDF" to generate a merged side-by-side report. Each page places the original and modified versions horizontally so you can share or print the comparison.

## Known Limitations
- The visual overlay highlights at the word level. For character-level precision, use the Text Diff tab.
- PDF text extraction may occasionally split or merge words differently than expected, causing minor false positives.
- It may also miss some changes entirely.
- Large PDFs (50+ pages) may be slow since all processing runs in the browser.
