# Implementation Plan: Workshop Materials

**Branch**: `001-workshop-materials` | **Date**: 2025-01-27 | **Spec**: [spec.md](spec.md)
**Input**: Feature specification from `/specs/001-workshop-materials/spec.md`

## Summary

Create all materials needed to facilitate the 2-hour Data Storytelling Workshop: facilitation guide (Markdown), HTML slide mockups, take-home assignment, and supporting files. Materials follow constitution principles and enable instructor-led delivery via Zoom.

## Technical Context

**Language/Version**: HTML5, CSS3, Markdown
**Primary Dependencies**: None (static files only)
**Storage**: File-based (Git repository)
**Testing**: Manual browser testing for HTML slides
**Target Platform**: Web browsers (Chrome, Firefox, Safari) + Markdown viewers
**Project Type**: Static content (educational materials)
**Performance Goals**: N/A (static files)
**Constraints**: Must work offline, no JavaScript dependencies
**Scale/Scope**: Single workshop, ~10 HTML files, ~5 Markdown files

## Constitution Check

*GATE: Must pass before Phase 0 research. Re-check after Phase 1 design.*

| Principle | Requirement | Status |
|-----------|-------------|--------|
| I. Insight-Driven Communication | All example slides demonstrate Takeaway Titles | ✅ Pass |
| II. Discovery Learning Pedagogy | Facilitation guide follows attempt → gap reveal → instruction | ✅ Pass |
| III. Framework Alignment | DC ACT framework explicitly referenced throughout | ✅ Pass |
| IV. Practical Application | Marketing Channel ROI scenario uses realistic data | ✅ Pass |
| V. Measurable Outcomes | Take-home has binary criterion (insight-driven title) | ✅ Pass |

**Quality Gates from Constitution**:
- [ ] All content follows Takeaway Title principles
- [ ] Discovery learning sequence is explicit in facilitation guide
- [ ] Assessment criteria are binary and objective
- [ ] Scenario data produces non-obvious but discoverable insights
- [ ] Content directly applicable to job interview or capstone scenarios

## Project Structure

### Documentation (this feature)

```text
specs/001-workshop-materials/
├── plan.md              # This file
├── research.md          # Phase 0: HTML slide patterns research
├── quickstart.md        # Phase 1: How to use materials
└── spec.md              # Feature specification
```

### Source Code (repository root)

```text
workshops/data-storytelling/
├── PRD.md                      # Product requirements (exists)
├── facilitation-guide.md       # P1: Step-by-step instructor manual
├── take-home-assignment.md     # P2: Student assignment document
├── zoom-setup.md               # P3: Technical setup guide
├── ai-prompt-template.md       # P3: AI usage examples
├── assets/
│   └── marketing-channel-roi.csv  # Dataset for students
└── slides/
    ├── styles.css              # Shared slide styling
    ├── 01-title.html           # Workshop title slide
    ├── 02-dc-act-framework.html # Framework introduction
    ├── 03-scenario-intro.html  # Marketing scenario setup
    ├── 04-dataset.html         # Data table display
    ├── 05-group-exercise-1.html # First attempt instructions
    ├── 06-knaflic-principles.html # Gap reveal teaching
    ├── 07-before-after.html    # Transformation example
    ├── 08-group-exercise-2.html # Revision instructions
    └── 09-take-home-intro.html # Assignment introduction
```

**Structure Decision**: Static content project using Markdown for text documents and HTML/CSS for visual slides. No build process required—files are used directly.

## Complexity Tracking

No constitution violations requiring justification. Project uses simple static files with no frameworks or complex dependencies.

## Implementation Phases

### Phase 1: Core Facilitation (P1)
- Create facilitation-guide.md with all 8 time blocks
- Create shared styles.css for slides
- Create HTML slides 01-09

### Phase 2: Student Materials (P2)
- Create take-home-assignment.md with both options
- Create marketing-channel-roi.csv dataset

### Phase 3: Support Materials (P3)
- Create zoom-setup.md
- Create ai-prompt-template.md

## Verification

1. Open each HTML slide in browser - verify renders correctly
2. Read facilitation guide - verify covers all PRD time blocks
3. Check take-home assignment - verify both options present with data
4. Validate against constitution quality gates
