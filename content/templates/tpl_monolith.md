---
publish: true
draft: true
cssclasses: ""
---

# <% tp.file.folder() %>

```dataviewjs
const folder = dv.current().file.folder;
const pages = dv.pages(`"${folder}"`).sort(p => p.file.name);

// 1. GENERATE THE VISUAL TOC
dv.header(1, "Table of Contents");
for (const page of pages) {
    if (page.file.path !== dv.current().file.path) {
        dv.paragraph(`- [[${page.file.path}|${page.file.name}]]`);
    }
}

dv.paragraph("---");

// 2. EMBED THE CONTENT
for (const page of pages) {
    if (page.file.path !== dv.current().file.path) {
        // We use H1 here so the PDF generator creates a "Bookmark" in the PDF file
        dv.header(1, page.file.name); 
        dv.paragraph(`![[${page.file.path}]]`);
        dv.paragraph('<div style="page-break-after: always;"></div>'); // Forces each note to start on a new page
    }
}
```
