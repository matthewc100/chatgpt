# 📝 Transcript Formatting Assistant Guide

## 📌 Purpose
This document defines the rules and procedures for formatting transcripts, ensuring consistent, readable output regardless of input variation. It supports maintenance, issue tracking, and iterative improvement.

---

## ✅ Current Version: v1.1 — May 21, 2025

### Summary of Changes:
- Introduced speaker alias normalization
- Improved grouping logic for mid-paragraph speaker changes
- Clarified format-specific styling rules
- Added best practices for clean formatting and maintenance

### Reason for Update:
Corrected misformatting where alias names (e.g., "Matthew Loebman") were not grouped under the correct speaker ("Matt Loebman"). Resolved issue where multiple speakers were combined into a single paragraph.

---

## 📋 Formatting Instructions

### 1. Remove Metadata
- ❌ Timestamps (e.g., `00:00:01.000 --> 00:00:03.000`)
- ❌ Numeric markers (e.g., `1`, `2`)

### 2. Normalize Speaker Names
- Map all alias forms to canonical names using a predefined dictionary

| Alias           | Canonical Name     |
| --------------- | ------------------ |
| Matthew Loebman | Matt Loebman       |
| vservant        | Veronica Servantez |
| Matt Coblentz   | Matt Coblentz      |
| Evan Woollacott | Evan Woollacott    |

### 3. Group Speech by Speaker
- ✅ Only one bolded speaker label per paragraph
- ✅ Combine consecutive speech from the same speaker
- ⛔ Never include multiple speakers in one paragraph
- ✅ Break paragraphs at any speaker change — even if mid-sentence

### 4. Format Output Appropriately
- **Markdown (.md):** `**Speaker Name:**`
- **Word (.docx):** Bold font (no asterisks)
- **Plain Text (.txt):** Just the speaker name, followed by colon

### 5. Ensure Clarity
- ✅ Add a line break between each speaker paragraph
- ✅ Preserve natural conversation flow
- ✅ Keep paragraphs readable — break long ones if necessary

---

## 🔄 Workflow
1. User uploads transcript file (.vtt or .txt)
2. System removes timestamps and numbers
3. Speaker names normalized using alias map
4. Text grouped and formatted by canonical speaker
5. User selects output format
6. Formatted transcript returned for download

---

## 🧩 Issues Tracker
_Reference GitHub issue numbers or summaries linked to formatting bugs and fixes._

- #1: Initial implementation
- #2: Misattribution of aliases (fixed in v1.1)
- #3: Multiple speakers in one paragraph (addressed in v1.1)

---

## 📎 Next Steps / To Do
- [ ] Add support for uploading external alias maps (CSV/JSON)
- [ ] Implement formatting presets (e.g., for legal, academic transcripts)
- [ ] Integrate gold-standard test cases for regression testing