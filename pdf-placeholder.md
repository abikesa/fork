To add new PDFs in the future, the correct section to update is the `<div class="directory-structure">` block.

You’ll want to insert new entries inside it, each using the `.file-item` template. Here's a ready-to-copy **template** you can use to append new PDFs — just replace the filename and size:

```html
<div class="file-item" onclick="openPDF('new-file-name')">
    <div class="file-icon pdf-file">📄</div>
    <div>new-file-name.pdf</div>
    <div class="file-size">123,456 bytes</div>
</div>
```

### Example with a placeholder:

```html
<div class="file-item" onclick="openPDF('placeholder')">
    <div class="file-icon pdf-file">📄</div>
    <div>placeholder.pdf</div>
    <div class="file-size">42,000 bytes</div>
</div>
```

### Pro tip:

To keep things organized, append this new block just **before** the last HTML entry in your `.directory-structure` div, or sort it alphabetically if that's your convention.

Let me know if you’d like a Python or Bash script to auto-generate these blocks from `ls -lh *.pdf`.

