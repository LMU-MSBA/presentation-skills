# Quickstart: Using Workshop Materials

## Overview

This guide explains how to use the Data Storytelling Workshop materials for facilitation and student assessment.

## Materials Inventory

After implementation, you'll have:

```
workshops/data-storytelling/
├── PRD.md                      # Reference document (already exists)
├── facilitation-guide.md       # Your step-by-step script
├── take-home-assignment.md     # Share with students after workshop
├── zoom-setup.md               # Pre-workshop technical setup
├── ai-prompt-template.md       # Share with students during Exercise 2
├── assets/
│   └── marketing-channel-roi.csv  # Raw data for students
└── slides/
    ├── styles.css              # Don't edit unless rebranding
    └── *.html                  # Open in browser to present
```

## Before the Workshop

### 1. Technical Setup (30 min before)

1. Read `zoom-setup.md` for breakout room configuration
2. Test Zoom screen sharing
3. Open all HTML slides in browser tabs (in order)
4. Have `facilitation-guide.md` open for reference

### 2. Verify Materials

- [ ] Can open each slide in browser
- [ ] Facilitation guide is printed or on second screen
- [ ] Take-home assignment ready to share
- [ ] CSV file ready to share if requested

## During the Workshop

### Presenting Slides

1. Open slide HTML file in Chrome
2. Press `F11` for fullscreen (or `Cmd+Shift+F` on Mac)
3. Share browser window in Zoom
4. Navigate between slides by switching browser tabs

### Following the Script

Keep `facilitation-guide.md` visible on a second monitor or printed. Key sections:

- **Block 3 (0:25-0:50)**: Exercise 1 instructions and breakout rotation
- **Block 4 (0:50-1:05)**: Gap reveal script (the key teaching moment)
- **Block 7 (1:30-1:51)**: Presentation feedback framework

### Breakout Room Rotation

During 25-minute Exercise 1:
- ~4 minutes per room
- Observe without correcting (discovery learning)
- Note candidates for presentations

During 20-minute Exercise 2:
- Now you CAN coach and give feedback
- Confirm your 3 presentation selections

## After the Workshop

### Sharing Take-Home Assignment

1. Share `take-home-assignment.md` via course LMS or email
2. Optionally share `marketing-channel-roi.csv` for students who want raw data
3. Set submission deadline

### Grading

Evaluation is binary: **Does the slide have a Takeaway Title?**

Pass examples:
- "Organic Search Drives 59% of Conversions—Increase SEO Investment"
- "Sales Department Turnover Urgent—Satisfaction Scores Signal Crisis"

Fail examples:
- "Website Traffic Analysis"
- "Q3 Employee Survey Results"

## Customization

### Changing Colors/Branding

Edit `slides/styles.css`:
```css
:root {
  --primary: #1a365d;      /* Change for title color */
  --accent: #ed8936;       /* Change for emphasis color */
}
```

### Updating Data

1. Edit the HTML file directly
2. Update table rows in the `<table>` element
3. Refresh browser to see changes

### Adding Slides

1. Copy any existing HTML file as template
2. Update content between `<div class="slide">` tags
3. Keep link to `styles.css` intact

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Slides look wrong | Clear browser cache, refresh |
| Text too small | Increase browser zoom (Cmd/Ctrl +) |
| Colors don't match | Check styles.css is in same folder |
| Breakout rooms not working | See zoom-setup.md troubleshooting section |

## Verification Checklist

Before first delivery:

- [ ] Opened each slide in browser successfully
- [ ] Read through facilitation guide completely
- [ ] Tested Zoom screen share with slides
- [ ] Have take-home assignment ready to share
- [ ] Reviewed grading criteria (Takeaway Title = pass)
