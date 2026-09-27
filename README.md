# Book Creator

A lightweight, browser-based book writing and publishing tool built as a **single HTML file**. Book Creator lets you write, organize, format, illustrate, read, save, import, and export books directly from your browser without a backend server or database. The project is designed to be simple to download, easy to run, and useful on both desktop and mobile browsers.

> **Repository:** https://github.com/trackbeatz/Book-Creator

---

## ✨ Features

### 📚 Book writing
- Create and manage multiple books.
- Set the book title and author.
- Add, rename, reorder, and delete chapters.
- Edit chapter content with the built-in rich-text editor.
- Insert images directly into chapter content.
- Organize the book from the chapter sidebar and table of contents.

### 📖 Preface / front matter
- Add a dedicated **Preface** before Chapter 1.
- Edit the preface separately from the chapters.
- The preface appears before Chapter 1 in the reader.
- The preface is included in supported exports.
- Existing books without a preface are automatically given an empty preface area.

### 🖼️ Front and back cover images
- Add a custom **front cover photo**.
- Add a custom **back cover photo**.
- Replace or remove cover photos at any time.
- Images are inserted as actual image data rather than external links.
- Cover images are displayed in the book reader and included in supported exports.
- If no custom cover is supplied, the app can continue using its built-in cover presentation.

### 📝 Rich text and images
- Format text while writing.
- Insert images into book content.
- Upload images from your device.
- Image data is stored with the book/project so the image does not depend on an external image URL.

### 📥 Import
- Import plain-text (`.txt`) content.
- Import EPUB (`.epub`) books.
- Open Book Creator project files (`.json`).
- Imported books can be edited and exported again.

### 📤 Export

Export your book in several formats:
- **HTML** — a standalone web-readable book.
- **EPUB** — for compatible ebook readers and publishing workflows.
- **TXT** — plain-text version of the book.
- **Print / PDF** — use the browser print dialog and choose **Save as PDF** when available.
- **JSON project** — preserve your editable Book Creator project for backup or later editing.

### 📱 Responsive interface
The interface is designed to work across desktop and mobile screen sizes, making it possible to write or review a book from a phone, tablet, or computer.

### 💾 Browser-based storage
Books are stored locally in the browser using browser storage. No account or remote database is required by the application. Because browser storage is device/browser-specific, **export your project as JSON regularly if the book is important**.

---

## 🚀 Quick Start

There are two easy ways to use Book Creator.

### Option 1 — Download ZIP from GitHub
This is the easiest method if you do not use Git.

1. Open the repository: https://github.com/trackbeatz/Book-Creator
2. Click the green **Code** button.
3. Click **Download ZIP**.
4. Extract the downloaded ZIP file.
5. Open the extracted project folder.
6. Open `index.html` in a modern web browser.
7. Book Creator will load in the browser.

GitHub documents **Download ZIP** as the way to download a snapshot of a repository without installing Git.

### Option 2 — Clone with Git
If you have Git installed, open Terminal, Command Prompt, PowerShell, or Git Bash and run:

```bash
git clone https://github.com/trackbeatz/Book-Creator.git
cd Book-Creator
```

Then open `index.html` in your browser.

Cloning gives you a local Git repository, which makes it easier to receive future changes and contribute changes back to GitHub.

---

## 🧰 Requirements

Book Creator is intentionally simple.

### Required
- A modern web browser.
- JavaScript enabled.
- A device capable of opening an HTML file.

### Recommended browsers
Use a current version of one of these browsers:
- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Apple Safari

No Node.js, Python, database, API key, or backend server is required for the normal application workflow.

---

## ▶️ Running the Application

### Simplest method
After downloading the repository, open:

```text
index.html
```

The application runs directly in the browser.

### Optional: run with a local web server
If your browser restricts some functionality when an HTML file is opened directly with `file://`, run a small local server instead.

If Python is installed:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

This is optional. You do not normally need a server to use the application.

---

# 📘 How to Use Book Creator

## 1. Start a new book
When Book Creator opens, create or select a book from the library. Enter the basic book information, such as:
- Book title
- Author name
- Chapters
- Other available book metadata

Your book becomes the workspace in which you can add the front cover, preface, chapters, images, and back cover.

---

## 2. Add the front cover photo
To add a custom front cover:
1. Open your book.
2. Find the **Front Cover** controls in the sidebar.
3. Click **Add / Change Front Cover**.
4. Select an image from your device.
5. The selected image is stored with the book as image data.
6. Open the reader to preview the front cover.

You can replace the image later by choosing **Add / Change Front Cover** again.

### Recommended cover preparation
For the best results, use a high-quality portrait image that matches the shape of the book you are creating. For example:
- Book cover artwork
- Author-designed cover
- Photograph
- Illustration
- Brand or publisher artwork

Avoid extremely large images when possible because large embedded images can make the project and exported files larger.

---

## 3. Add the back cover photo
To add a custom back cover:
1. Open your book.
2. Click **Add / Change Back Cover**.
3. Select your back-cover image.
4. Preview the book in the reader.
5. The back cover appears after the chapters.

You can replace or remove it whenever you want. If you do not add a custom back cover, the application can still provide its normal back-cover presentation.

---

## 4. Write the preface
The preface is separate from the chapters and is designed to appear **before Chapter 1**.

To write it:
1. Click **Edit Preface**.
2. Enter the preface title if you want to change it.
3. Write or paste your preface into the editor.
4. Apply formatting as needed.
5. Save your changes through the normal Book Creator workflow.
6. Open the reader and confirm that the preface appears before Chapter 1.

A typical book structure is now:

```text
Front Cover
   ↓
Preface
   ↓
Chapter 1
   ↓
Chapter 2
   ↓
Chapter 3
   ↓
...
   ↓
Back Cover
```

The preface is therefore treated as front matter rather than as Chapter 1.

---

## 5. Create chapters
Use the chapter controls to:
1. Add a new chapter.
2. Give it a title.
3. Write the chapter content.
4. Format the text.
5. Insert images if needed.
6. Continue adding chapters until the book is complete.

The chapter list provides a quick way to move between sections.

---

## 6. Insert images into a chapter
To insert an image inside chapter content:
1. Open the chapter you want to edit.
2. Place the cursor where the image should appear.
3. Use the image insertion control.
4. Select an image from your device.
5. The image is inserted into the chapter content.
6. Continue writing around the image.

This is different from the front and back cover controls: chapter images belong to the chapter itself, while cover images belong to the book's cover pages.

---

# 👀 Reading and Previewing the Book

Use the built-in reader to preview the finished book. The reader presents the book in reading order:
1. Front Cover
2. Preface, when one exists
3. Chapter 1
4. Chapter 2
5. Additional chapters
6. Back Cover

The reader also provides navigation through the book's table of contents. This makes it useful for checking the final order before exporting.

---

# 📤 Exporting Your Book

Open the **Export** menu to choose the format you need.

## HTML export
HTML export creates a standalone web-readable version of the book. Use HTML when you want:
- A browser-readable copy.
- A portable web version.
- A version that can be opened without the Book Creator editor.

The exported HTML includes the book structure and supported cover/preface content.

## EPUB export
EPUB is useful for ebook readers and ebook publishing workflows. The EPUB structure includes the book's reading order and can include:
- Front cover
- Preface
- Chapters
- Back cover
- Navigation/table of contents

## TXT export
TXT creates a plain-text representation of the book. This is useful for:
- Simple backups
- Copying text into another application
- Archiving the manuscript
- Sharing the raw text

Rich formatting and images are not preserved as visual elements in plain text.

## Print / PDF
Choose the print option and use your browser's print dialog. For browsers that provide it, select:

```text
Destination → Save as PDF
```

Review the print preview before saving the PDF, especially if the book contains images or custom page layouts.

## JSON project export
JSON is the most important backup format when you want to continue editing the book later. Use it to preserve the editable project rather than only the final manuscript.

A good backup habit is:

```text
Write → Export JSON → Continue writing → Export JSON again
```

---

# 📥 Importing Books

## Import a TXT file
Use the TXT import option to bring plain-text material into Book Creator. This is useful when you already have a manuscript in a `.txt` file. After importing, review the chapter structure and formatting because plain text contains limited formatting information.

## Import an EPUB
Use the EPUB import option to bring supported EPUB content into Book Creator. After importing:
1. Review the title and author.
2. Check the preface.
3. Check every chapter.
4. Check the images and cover presentation.
5. Correct formatting where necessary.
6. Export the book again when finished.

## Import a JSON project
Use the JSON project import/open option to restore a Book Creator project. This is the recommended method for continuing work on a previously exported Book Creator project.

---

# 💾 Saving and Backups

Book Creator stores its working library in the browser's local storage. That means the same book may not automatically appear if you:
- Switch browsers.
- Switch devices.
- Clear browser data.
- Use private/incognito browsing.
- Delete the site's stored data.

### Recommended backup strategy
For important books, regularly export a `.json` project file. Keep copies of the JSON project somewhere safe, such as:
- Your computer
- An external drive
- Cloud storage
- A private backup folder

You can also export HTML, EPUB, and TXT versions as additional backups.

---

# 🖼️ Working With Cover Images

Cover images are stored as image data inside the project rather than as a reference to an external website. This means the book does not depend on an image URL remaining online. The application also processes uploaded cover images so they can be used within the book without requiring a separate image-hosting service.

### Good practice
Use optimized images whenever possible:
- Prefer clear, high-resolution artwork.
- Avoid unnecessarily huge files.
- Use portrait-oriented artwork for book covers.
- Keep important text away from the extreme edges of the image.
- Check the reader preview before exporting.

---

# 📁 Project Structure

The repository is intentionally minimal:

```text
Book-Creator/
├── index.html      # Main Book Creator application
└── README.md       # Project documentation
```

The main application is contained in `index.html`, including its HTML, CSS, and JavaScript. There is no separate frontend build system required for the normal project.

---

# 🔧 Development

Because the application is a single HTML file, development is straightforward.

1. Clone the repository.
2. Open `index.html` in a text editor or code editor.
3. Make your changes.
4. Open the file in a browser.
5. Test writing, images, covers, preface, import, and export functionality.
6. Commit your changes with Git.

For example:

```bash
git clone https://github.com/trackbeatz/Book-Creator.git
cd Book-Creator
```

Then edit:

```text
index.html
```

---

# 🔄 Updating an Existing Local Copy

If you cloned the repository with Git, you can retrieve new changes with:

```bash
git pull origin main
```

If you have local changes that conflict with incoming changes, Git may ask you to resolve the conflict before completing the update.

---

# 🌐 How to Download Book Creator From GitHub

## On a computer
1. Go to: https://github.com/trackbeatz/Book-Creator
2. Click **Code**.
3. Select **Download ZIP**.
4. Extract the ZIP file.
5. Open the extracted `Book-Creator` folder.
6. Open `index.html`.
7. Start creating your book.

GitHub's official documentation describes this method as downloading a snapshot of the repository.

## Using Git

```bash
git clone https://github.com/trackbeatz/Book-Creator.git
```

Then:

```bash
cd Book-Creator
```

And open `index.html`.

GitHub's documentation explains that cloning creates a complete local copy of the repository and its Git history.

## On Android
The easiest approach is usually:
1. Open the repository in Chrome.
2. Tap **Code**.
3. Tap **Download ZIP**.
4. Open the downloaded ZIP using your file manager.
5. Extract the folder.
6. Open `index.html` with a browser or an HTML/code editor that supports running local web files.

If your Android browser or file manager does not allow local HTML files to run correctly, use a local development server or an Android code editor that provides a local preview/server.

---

# 🛠️ Troubleshooting

## The book is not saving
The application uses browser storage. Check that:
- JavaScript is enabled.
- You are not using a private/incognito window if you need persistent storage.
- Browser storage has not been disabled.
- You have not cleared the site's stored data.

Most importantly, export the project as JSON so you have an independent backup.

## My book disappeared
If the browser's local storage was cleared, the local library may no longer be available. Restore the book from a previously exported JSON project file.

## My cover image is missing
Try the following:
1. Reopen the book.
2. Add the cover image again.
3. Confirm it appears in the reader.
4. Export the project as JSON.
5. Reopen the exported project if necessary.

## The EPUB does not look exactly like the editor
EPUB readers use their own rendering engines and styles. Always test the exported EPUB in the target ebook reader before publishing.

## PDF layout looks different
PDF output through the browser print system depends on the browser's print engine and print settings. Check:
- Paper size
- Margins
- Scale
- Background graphics
- Headers and footers
- Orientation

Use the print preview before saving the final PDF.

## The page does not open correctly
Make sure you are opening the actual application file:

```text
index.html
```

If direct `file://` access causes browser restrictions, serve the folder locally:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

---

# 🔒 Privacy

Book Creator is designed as a client-side browser application. The normal writing workflow does not require a user account, remote database, or server-side book storage.

Your locally stored books remain in your browser's storage until you remove the browser data or otherwise lose that local storage. When you export a book, the resulting file is saved to your device through the browser's download functionality.

Do not put sensitive information into a book unless you understand where your browser and exported files are being stored.

---

# 🤝 Contributing

Contributions are welcome. A typical contribution workflow is:

```bash
git clone https://github.com/trackbeatz/Book-Creator.git
cd Book-Creator
```

Create a branch:

```bash
git checkout -b feature/my-improvement
```

Make and test your changes, then:

```bash
git add .
git commit -m "Add my improvement"
git push origin feature/my-improvement
```

You can then open a pull request on GitHub.

When contributing, please test the following areas when your change affects them:
- Book creation
- Chapter editing
- Preface editing
- Front cover image
- Back cover image
- Chapter images
- JSON import/export
- TXT import/export
- EPUB import/export
- HTML export
- Print/PDF workflow
- Mobile layout

---

# 🗺️ Suggested Book-Creation Workflow

For a new book, the following workflow is recommended:

```text
1. Create the book
   ↓
2. Enter title and author
   ↓
3. Add front cover
   ↓
4. Write the preface
   ↓
5. Create Chapter 1
   ↓
6. Create the remaining chapters
   ↓
7. Add chapter images where needed
   ↓
8. Add the back cover
   ↓
9. Read the complete book in the built-in reader
   ↓
10. Export JSON backup
   ↓
11. Export EPUB / HTML / TXT / PDF as required
   ↓
12. Test the exported files
```

---

# 📋 Example Book Structure

A finished book can be organized like this:

```text
My Book
│
├── Front Cover
│
├── Preface
│
├── Chapter 1 — The Beginning
│
├── Chapter 2 — The Journey
│
├── Chapter 3 — The Challenge
│
├── Chapter 4 — The Solution
│
├── Chapter 5 — The Ending
│
└── Back Cover
```

---

# 📌 Important Notes

- Book Creator is a browser application, not a traditional desktop installation package.
- The main application is contained in `index.html`.
- Local browser storage is convenient but should not be treated as the only backup of an important book.
- Use JSON project exports for editable backups.
- Exported EPUB, HTML, TXT, and PDF files should be checked before publishing or distributing them.
- EPUB and PDF rendering can vary between readers, browsers, operating systems, and publishing platforms.

---

# 📜 License

No explicit license is currently documented in the repository. If you plan to redistribute, modify, or publish the project, add an appropriate `LICENSE` file to the repository and state the permitted usage here.

---

# ❤️ Book Creator

Create it. Write it. Illustrate it. Read it. Export it.

**Repository:** https://github.com/trackbeatz/Book-Creator
