# -Desktop-Organizer-for-macOS
A lightweight bash script that cleans up your Desktop in seconds. It scans all loose files and automatically sorts them into clearly named folders — Images, Videos, Documents, Code, Archives, and more — based on file extension.

# Desktop Organizer for macOS

A lightweight bash script that cleans up your Desktop in seconds. It scans all loose files and automatically sorts them into clearly named folders — Images, Videos, Documents, Code, Archives, and more — based on file extension.

---

## Features

- Sorts files into 12 categories automatically
- **Dry-run mode** — preview every move before anything changes
- Never deletes files or overwrites duplicates
- Leaves existing folders untouched
- No dependencies — uses only built-in macOS tools

---

## Usage

```bash
# Preview changes without moving anything
bash organize_desktop.sh --dry-run

# Sort your Desktop
bash organize_desktop.sh
```

---

## Folder structure

After running, your Desktop will be organized like this:

```
~/Desktop/
├── Images/          # jpg, png, gif, webp, heic, svg, raw, cr2…
├── Videos/          # mp4, mov, avi, mkv, m4v…
├── Audio/           # mp3, wav, aac, flac, m4a…
├── Documents/       # pdf, doc, docx, txt, md, pages…
├── Spreadsheets/    # xls, xlsx, csv, numbers…
├── Presentations/   # ppt, pptx, key…
├── Archives/        # zip, dmg, pkg, tar, gz, 7z…
├── Code/            # py, js, ts, html, css, json, sh…
├── Design/          # psd, ai, sketch, figma, xd…
├── Applications/    # app, exe
├── eBooks/          # epub, mobi, azw3…
└── Other/           # anything not recognized
```

---

## Safety

- **No deletions** — files are only moved, never removed
- **No overwrites** — if a filename already exists in the target folder, the script auto-renames it (e.g. `report_1.pdf`)
- **Dry-run first** — always recommended before running for real
- **Folders are skipped** — only loose files on the Desktop are touched

---

## Requirements

- macOS
- Bash (pre-installed on all Macs)

---

## License

MIT
