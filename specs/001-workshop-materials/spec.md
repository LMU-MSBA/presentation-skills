# Feature Specification: Workshop Materials

**Feature Branch**: `001-workshop-materials`
**Created**: 2025-01-27
**Status**: Draft
**Input**: Build 2-hour Zoom lesson with materials for facilitation and take-home assignment

## User Scenarios & Testing *(mandatory)*

### User Story 1 - Facilitate Workshop (Priority: P1)

As an instructor, I can follow the facilitation guide to deliver the 2-hour Data Storytelling Workshop with correct timing, teaching moments, and breakout room coordination.

**Why this priority**: Without facilitation materials, the workshop cannot be delivered. This is the core deliverable.

**Independent Test**: Instructor can read through facilitation guide and understand exactly what to do at each time block without referencing other documents.

**Acceptance Scenarios**:

1. **Given** facilitation guide is open, **When** instructor reads Block 3 (Group Exercise #1), **Then** they know exactly what instructions to give, how long to spend in each breakout room, and what to observe without correcting.
2. **Given** workshop is at 0:50 (gap reveal), **When** instructor follows guide, **Then** they can execute the before/after comparison and teach Knaflic principles.
3. **Given** instructor is selecting groups for presentations, **When** they reference the guide, **Then** they know the three selection criteria (strong, needs coaching, interesting).

---

### User Story 2 - Complete Take-Home Assignment (Priority: P2)

As a student, I can complete the take-home assignment by transforming one of two bad slides into a slide with a Takeaway Title.

**Why this priority**: Individual assessment is required for workshop credit. Students need clear instructions and materials.

**Independent Test**: Student can complete assignment using only the take-home document without needing to ask for clarification.

**Acceptance Scenarios**:

1. **Given** student receives take-home document, **When** they read instructions, **Then** they understand they must choose 1 of 2 options and transform it.
2. **Given** student chooses Option A (Website Traffic), **When** they examine the data, **Then** they can discover the insight about organic search conversions.
3. **Given** student submits transformed slide, **When** evaluated, **Then** the criterion is clear: does the title convey an insight?

---

### User Story 3 - Present Visual Slides (Priority: P3)

As an instructor, I can display professional HTML slide mockups during the workshop that demonstrate principles, show before/after examples, and guide activities.

**Why this priority**: Visual slides enhance teaching but the workshop could technically proceed with just the facilitation guide.

**Independent Test**: Opening any HTML slide file in a browser displays a clean, readable slide suitable for screen sharing.

**Acceptance Scenarios**:

1. **Given** instructor opens DC ACT Framework slide, **When** displayed, **Then** the 5 steps are clearly visible and formatted.
2. **Given** instructor shows before/after slide, **When** students view, **Then** the contrast between descriptive and Takeaway Titles is immediately apparent.
3. **Given** all slides use shared CSS, **When** viewing any slide, **Then** consistent branding and typography is maintained.

---

### Edge Cases

- What happens if a student can't identify an insight from Option A or B data? (Answer: Hidden insight is documented in take-home for instructor reference, not visible to students)
- What if Zoom breakout rooms malfunction? (Answer: Facilitation guide includes emergency adjustments section)
- What if workshop runs long/short? (Answer: Facilitation guide includes timing adjustment guidance)

## Requirements *(mandatory)*

### Functional Requirements

- **FR-001**: Facilitation guide MUST cover all 8 time blocks from PRD with exact timing and script outlines
- **FR-002**: Facilitation guide MUST include breakout room rotation strategy for 6 groups
- **FR-003**: Facilitation guide MUST include "gap reveal" instructions at 0:50 mark
- **FR-004**: Facilitation guide MUST include group selection criteria for presentations
- **FR-005**: Facilitation guide MUST include emergency timing adjustments
- **FR-006**: Take-home assignment MUST include 2 bad slide options with data tables
- **FR-007**: Take-home assignment MUST clearly state the evaluation criterion (Takeaway Title)
- **FR-008**: Take-home assignment MUST provide submission instructions
- **FR-009**: HTML slides MUST render correctly when opened in a browser
- **FR-010**: HTML slides MUST use shared CSS for consistent styling
- **FR-011**: Dataset MUST be available in CSV format for students who want raw data
- **FR-012**: AI prompt template MUST demonstrate how to use AI for title refinement

### Key Entities

- **Facilitation Guide**: Step-by-step instructor manual with timing, scripts, and coaching tips
- **Take-Home Assignment**: Student-facing document with bad slide options and instructions
- **HTML Slides**: Visual mockups for key teaching moments
- **Dataset**: Marketing Channel ROI data in CSV format
- **AI Prompt Template**: Example prompts for title refinement

## Success Criteria *(mandatory)*

### Measurable Outcomes

- **SC-001**: Facilitation guide covers all 8 time blocks from PRD
- **SC-002**: Take-home assignment includes both Option A (Website Traffic) and Option B (Employee Satisfaction)
- **SC-003**: All HTML slides display correctly in Chrome, Firefox, and Safari
- **SC-004**: Materials align with all 5 Constitution principles (insight-driven, discovery learning, DC ACT, practical, measurable)
- **SC-005**: Instructor can deliver workshop using materials without additional preparation beyond reading
- **SC-006**: Students can complete take-home assignment without asking clarifying questions
