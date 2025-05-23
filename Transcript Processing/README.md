# chatgpt
Custom GPT's need instructions.  This repository should hold a variety of ChatGPT instructions.  One GPT is one set of instructions, so they all go in this folder.  

# 📄 Transcript Formatter

A simple, rules-driven assistant for cleaning and formatting raw transcript files (.vtt or .txt) into clean, speaker-organized documents. Built to support consistent formatting, version control, and issue tracking for quality assurance.

---

## 🚀 Features
- Removes timestamps and numeric markers
- Normalizes speaker names using alias maps
- Groups speech by canonical speaker
- Supports Markdown (.md), Word (.docx), and Plain Text (.txt) output
- Clean, readable formatting with one paragraph per speaker turn

---

## 🛠️ How It Works
1. Upload a raw transcript (Zoom VTT or plain text).
2. System removes metadata (timestamps, numeric lines).
3. Speaker names are normalized based on alias map.
4. Consecutive speech is grouped and formatted.
5. Output is exported in user-selected format.

---

## 🧱 File Structure

```
/transcript-formatter
├── README.md                # This file
├── transcript_formatter_guide.md  # Detailed instructions & changelog
├── example_transcripts/     # (Optional) Sample input and output
└── issues/                  # GitHub Issues linked to version changes
```

---

## 📦 Output Formats
- **Markdown (.md)**: `**Speaker Name:**`
- **Word (.docx)**: Bold speaker name (no asterisks)
- **Plain Text (.txt)**: Unformatted speaker name

---

## 🧩 Contributing & Issues

If you find bugs or formatting inconsistencies:
1. Open an issue with:
   - Sample input transcript (or excerpt)
   - Description of the issue
   - Expected vs. actual result
2. Reference the issue number in future commits

We track changes in `transcript_formatter_guide.md`, including version numbers and resolved issue links.

---

## 📅 Versioning
See [Transcript Formatter Guide](./transcript_formatter_guide.md) for version history and changelog.

---

## ✅ TODOs
- [ ] Support external alias maps (CSV/JSON)
- [ ] Add template for academic/legal formats
- [ ] Regression test suite using gold-standard transcripts

---

## 🧠 Maintainers
Built and maintained by[ Matt Coblentz].
