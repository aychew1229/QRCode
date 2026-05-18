# Bulk QR Code Generator

**Generate hundreds of QR codes in seconds — offline, free, and browser-based.**

A free, offline, single-file web tool for generating bulk QR codes from student ID data — built for Microsoft Publisher 2021 Mail Merge workflows.

> No installation. No internet required after first load. No data ever leaves your device.

![Preview](https://img.shields.io/badge/Offline-Ready-22d36e?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-Any%20Browser-4a9eff?style=flat-square)

[![Live Demo](https://img.shields.io/badge/🚀%20Launch%20Live%20Demo-Click%20Here-f5a623?style=for-the-badge)](https://aychew1229.github.io/QRCODE/)

---

## What It Does

Microsoft Publisher 2021 cannot read dynamic or formula-generated images during Mail Merge. It needs real `.png` files stored locally on your computer, and a column in your Excel sheet pointing to their exact file path.

This tool solves both problems in one step:

- Generates individual `.png` QR codes for every column in your list
- Packages them into a single downloadable `.zip` archive
- Updates your Excel file with a `QrCode` column containing the exact local file path for each student (e.g. `D:\qrcodes\DTU0000.png`)

---

## Features


| Feature | Description |
|---|---|
| 📤 **Excel / CSV Upload** | Drop in any `.xlsx`, `.xls`, or `.csv` file |
| 📋 **Copy-Paste Mode** | Paste a column directly — no file needed |
| 👁 **Live Preview Grid** | See every QR code render before downloading |
| 📦 **ZIP Export** | All PNGs packed and named after each student ID |
| 📊 **Excel Export** | Original sheet + new `QrCode` path column added |
| 📱 **Fully Responsive** | Works on desktop, tablet, and mobile |
| 🔒 **100% Private** | Zero server contact — all processing is local |
| ⚡ **No Installation** | One `.html` file — open and use immediately |

---
## 🚀 Quick Start

### Option A — Use the Live Demo *(Recommended)*

Click the badge at the top ↑ or go to:

```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

Open it in your browser and start generating — no download required.

---

### Option B — Run Locally (Fully Offline)

1. **Download** `QR_Generator.html` from this repository
2. **Right-click** the file → **Open with** → Chrome / Edge / Firefox / Safari
3. That's it. No setup. No npm. No server.

---

## 📖 How to Use

### Step 1 · Load Your Data

**Excel File tab**
- Click the upload zone or drag and drop your `.xlsx` / `.xls` / `.csv`
- Use the **Select Target Column** dropdown to pick any column containing you want genererate the qrcode.

**Copy-Paste tab from your excel**
- Copy one any column you want from your spreadsheet (`Ctrl+C`)
- Paste it into the text area (`Ctrl+V`)
- Tick **Skip first line** if the paste includes the column header

---

### Step 2 · Set Your Local Save Folder

Enter the exact path on your computer where the QR images will be stored:

```
c:\desktop\qrcodes\
```

> ⚠️ Always end the path with a backslash `\` — this is required for Publisher to resolve the paths correctly.

---

### Step 3 · Generate

Click **⚡ Generate QR Codes**.  
The preview panel fills with every QR code live you can visually verify before downloading.

---

### Step 4 · Download Your Files

| Button | What You Get |
|---|---|
| 📦 **Download QR Codes (.ZIP)** | ZIP of all `.png` files, each named after the column name |
| 📊 **Download Updated Excel (.XLSX)** | Your original spreadsheet with a `QrCode` column appended |

Extract the ZIP into the folder path you configured. Use the Excel file as your Mail Merge source in Publisher.

---

## File Output

| File                      | Description                                                         |
| ------------------------- | ------------------------------------------------------------------- |
| `QR_Codes.zip`            | All QR codes as individual `.png` files named after each you select column name |
| `Book1_With_QRCodes.xlsx` | Your original spreadsheet with a new `QrCode` column added          |

---

## 🔒 Privacy

- ✅ No data is ever sent to a server
- ✅ No cookies, no tracking, no analytics
- ✅ All QR generation happens inside your browser tab
- ✅ Closing the tab erases everything

---

## 🛠️ Tech Stack

This project uses no build tools, no frameworks, and no backend.

| Library | Version | Purpose |
|---|---|---|
| [QRCode.js](https://github.com/davidshimjs/qrcodejs) | 1.0.0 | QR generation on HTML5 Canvas |
| [JSZip](https://stuk.github.io/jszip/) | 3.10.1 | Packaging PNGs into a ZIP archive |
| [SheetJS (xlsx)](https://sheetjs.com/) | 0.18.5 | Reading and writing Excel files |

All three libraries are loaded from CDN. The tool works fully offline after the first page load.

---

## Browser Support

Works in any modern browser: Google Chrome, Microsoft Edge, Mozilla Firefox, Safari.

---

## License
 
free to use, modify, and share.

---

<div align="center">

Built with ❤️ for student ID production workflows · [Debre Tabor University](https://dtu.edu.et)

**If this saved you time, give it a ⭐ on GitHub!**

</div>
