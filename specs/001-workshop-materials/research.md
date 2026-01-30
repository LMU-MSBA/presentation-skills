# Research: Workshop Materials Technical Decisions

**Feature**: 001-workshop-materials
**Date**: 2025-01-27

## Technical Context Resolution

### Decision 1: HTML Slide Format

**Decision**: Use standalone HTML files with inline or linked CSS, no JavaScript

**Rationale**:
- Simple to create and edit
- Opens directly in any browser
- Works offline without build process
- Easy to screenshot for other formats
- No framework dependencies to maintain

**Alternatives Considered**:
- **Reveal.js**: Overkill for static mockups, requires build setup
- **Google Slides export**: Would need external service
- **PDF slides**: Not easily editable, harder to iterate
- **Markdown with Marp**: Requires toolchain installation

### Decision 2: CSS Approach

**Decision**: Single shared `styles.css` file linked by all slide HTML files

**Rationale**:
- Consistent styling across all slides
- Easy to adjust branding/colors in one place
- Small file size, fast loading
- Simple to understand and modify

**Alternatives Considered**:
- **Inline styles**: Harder to maintain consistency
- **Tailwind CSS**: Requires build process
- **CSS-in-HTML**: Duplicated styles across files

### Decision 3: Slide Dimensions

**Decision**: 16:9 aspect ratio (1280x720px viewport), centered content

**Rationale**:
- Standard presentation aspect ratio
- Matches Zoom screen share well
- Large enough for readability
- Works on most monitors

**Implementation**:
```css
.slide {
  width: 1280px;
  height: 720px;
  /* Center in viewport */
  margin: 0 auto;
}
```

### Decision 4: Typography

**Decision**: System fonts with fallbacks, large readable sizes

**Rationale**:
- No font loading required
- Works offline immediately
- Professional appearance
- Consistent across platforms

**Implementation**:
```css
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
}
.slide-title {
  font-size: 48px;
  font-weight: 600;
}
.slide-body {
  font-size: 28px;
}
```

### Decision 5: Color Scheme

**Decision**: Professional blue/gray palette with accent for emphasis

**Rationale**:
- Neutral enough for any branding
- High contrast for readability
- Accent color for highlighting key insights
- Matches typical business presentation style

**Implementation**:
```css
:root {
  --primary: #1a365d;      /* Dark blue for titles */
  --secondary: #4a5568;    /* Gray for body text */
  --accent: #ed8936;       /* Orange for emphasis */
  --background: #ffffff;   /* Clean white background */
  --muted: #e2e8f0;       /* Light gray for borders */
}
```

### Decision 6: Data Table Styling

**Decision**: Clean bordered tables with alternating row colors

**Rationale**:
- Easy to read at presentation distance
- Clear column separation
- Highlight row on hover for teaching
- Match Knaflic's clean data visualization principles

### Decision 7: Markdown for Text Documents

**Decision**: Use Markdown (.md) for facilitation guide, take-home, and support docs

**Rationale**:
- Easy to read in any editor
- Renders nicely on GitHub
- Converts easily to other formats if needed
- Instructor can annotate easily
- No special software required

**Alternatives Considered**:
- **Word docs**: Requires specific software
- **PDF**: Not easily editable
- **HTML**: Overkill for text documents

## Slide Inventory

Based on PRD workshop structure, these slides are needed:

| Slide | Purpose | Key Content |
|-------|---------|-------------|
| 01-title | Workshop opener | Title, subtitle, instructor name |
| 02-dc-act-framework | Framework intro | 5 steps with emphasis on step 4 |
| 03-scenario-intro | Context setting | Marketing analyst scenario |
| 04-dataset | Data display | Channel performance table |
| 05-group-exercise-1 | Instructions | What to do in breakout rooms |
| 06-knaflic-principles | Teaching | 6 principles table |
| 07-before-after | Gap reveal | Descriptive vs insight-driven |
| 08-group-exercise-2 | Revision instructions | How to improve with AI |
| 09-take-home-intro | Assignment intro | What to submit for credit |

## Browser Compatibility

**Target Browsers** (all modern versions):
- Chrome (primary)
- Firefox
- Safari
- Edge

**Testing Approach**:
- Open each HTML file in Chrome, verify layout
- Spot-check in Firefox and Safari
- Ensure text is readable at normal zoom

## File Organization

```
workshops/data-storytelling/
├── slides/
│   ├── styles.css          # Shared styling
│   └── *.html              # Individual slides
├── assets/
│   └── *.csv               # Data files
└── *.md                    # Text documents
```

## Summary

Simple, static HTML/CSS slides with Markdown documents. No build process, no JavaScript, works offline. Professional appearance suitable for Zoom screen sharing.
