# Tasks: Workshop Materials

**Input**: Design documents from `/specs/001-workshop-materials/`
**Prerequisites**: plan.md (required), spec.md (required), research.md, quickstart.md

**Tests**: Not requested - manual browser testing only

**Organization**: Tasks are grouped by user story to enable independent implementation and testing of each story.

## Format: `[ID] [P?] [Story] Description`

- **[P]**: Can run in parallel (different files, no dependencies)
- **[Story]**: Which user story this task belongs to (e.g., US1, US2, US3)
- Include exact file paths in descriptions

## Path Conventions

- **Project root**: `workshops/data-storytelling/`
- **Slides**: `workshops/data-storytelling/slides/`
- **Assets**: `workshops/data-storytelling/assets/`

---

## Phase 1: Setup (Shared Infrastructure)

**Purpose**: Create directory structure and shared styling

- [x] T001 Create slides directory at workshops/data-storytelling/slides/
- [x] T002 Create assets directory at workshops/data-storytelling/assets/
- [x] T003 Create shared CSS stylesheet at workshops/data-storytelling/slides/styles.css with slide dimensions (1280x720), typography, and color scheme

**Checkpoint**: Directory structure ready, shared CSS available for slides

---

## Phase 2: Foundational (Blocking Prerequisites)

**Purpose**: None required - all user stories can proceed independently after Setup

**⚠️ Note**: For this static content project, there are no blocking foundational dependencies. User stories can begin immediately after Setup.

**Checkpoint**: Foundation ready - user story implementation can begin

---

## Phase 3: User Story 1 - Facilitate Workshop (Priority: P1) 🎯 MVP

**Goal**: Instructor can deliver the 2-hour workshop using the facilitation guide

**Independent Test**: Instructor can read through facilitation guide and understand exactly what to do at each time block without referencing other documents

### Implementation for User Story 1

- [x] T004 [US1] Create facilitation guide at workshops/data-storytelling/facilitation-guide.md with all 8 time blocks from PRD
- [x] T005 [US1] Add Block 1 (Opening + Framework) content with script outline and DC ACT framework introduction
- [x] T006 [US1] Add Block 2 (Scenario Introduction) content with Marketing Channel ROI context
- [x] T007 [US1] Add Block 3 (Group Exercise #1) content with breakout room rotation strategy and observation notes
- [x] T008 [US1] Add Block 4 (Gap Reveal + Knaflic Principles) content with before/after comparison script
- [x] T009 [US1] Add Block 5 (Group Exercise #2) content with coaching guidance and AI usage instructions
- [x] T010 [US1] Add Block 6 (Presentation Setup) content with group selection criteria
- [x] T011 [US1] Add Block 7 (Group Presentations) content with feedback framework
- [x] T012 [US1] Add Block 8 (Wrap-up + Assignment) content with summary and assignment introduction
- [x] T013 [US1] Add emergency timing adjustments section to facilitation guide
- [x] T014 [US1] Add timing cheat sheet table to facilitation guide

**Checkpoint**: User Story 1 complete - instructor can deliver workshop using facilitation guide alone

---

## Phase 4: User Story 2 - Complete Take-Home Assignment (Priority: P2)

**Goal**: Student can complete take-home assignment using only the provided document

**Independent Test**: Student can complete assignment without asking clarifying questions

### Implementation for User Story 2

- [x] T015 [US2] Create take-home assignment document at workshops/data-storytelling/take-home-assignment.md with instructions
- [x] T016 [US2] Add Option A (Website Traffic) bad slide with data table and hidden insight reference
- [x] T017 [US2] Add Option B (Employee Satisfaction) bad slide with data table and hidden insight reference
- [x] T018 [US2] Add evaluation criterion section (insight-driven title = pass)
- [x] T019 [US2] Add submission instructions section
- [x] T020 [P] [US2] Create CSV dataset at workshops/data-storytelling/assets/marketing-channel-roi.csv

**Checkpoint**: User Story 2 complete - students can complete take-home assignment independently

---

## Phase 5: User Story 3 - Present Visual Slides (Priority: P3)

**Goal**: Instructor can display professional HTML slides during workshop

**Independent Test**: Opening any HTML slide in browser displays clean, readable slide suitable for screen sharing

### Implementation for User Story 3

- [x] T021 [P] [US3] Create title slide at workshops/data-storytelling/slides/01-title.html
- [x] T022 [P] [US3] Create DC ACT Framework slide at workshops/data-storytelling/slides/02-dc-act-framework.html
- [x] T023 [P] [US3] Create scenario introduction slide at workshops/data-storytelling/slides/03-scenario-intro.html
- [x] T024 [P] [US3] Create dataset display slide at workshops/data-storytelling/slides/04-dataset.html
- [x] T025 [P] [US3] Create Group Exercise 1 instructions slide at workshops/data-storytelling/slides/05-group-exercise-1.html
- [x] T026 [P] [US3] Create Knaflic principles slide at workshops/data-storytelling/slides/06-knaflic-principles.html
- [x] T027 [P] [US3] Create before/after transformation slide at workshops/data-storytelling/slides/07-before-after.html
- [x] T028 [P] [US3] Create Group Exercise 2 instructions slide at workshops/data-storytelling/slides/08-group-exercise-2.html
- [x] T029 [P] [US3] Create take-home intro slide at workshops/data-storytelling/slides/09-take-home-intro.html

**Checkpoint**: User Story 3 complete - all slides render correctly in browser

---

## Phase 6: Polish & Cross-Cutting Concerns

**Purpose**: Support materials and final validation

- [x] T030 [P] Create Zoom setup guide at workshops/data-storytelling/zoom-setup.md
- [x] T031 [P] Create AI prompt template at workshops/data-storytelling/ai-prompt-template.md
- [x] T032 Validate all HTML slides open correctly in Chrome browser
- [x] T033 Validate facilitation guide covers all 8 PRD time blocks
- [x] T034 Validate take-home assignment includes both Option A and Option B
- [x] T035 Run quickstart.md verification checklist

---

## Dependencies & Execution Order

### Phase Dependencies

- **Setup (Phase 1)**: No dependencies - can start immediately
- **Foundational (Phase 2)**: N/A for this project
- **User Story 1 (Phase 3)**: Depends on T003 (styles.css) only if creating slides inline
- **User Story 2 (Phase 4)**: No dependencies - can run in parallel with US1
- **User Story 3 (Phase 5)**: Depends on T003 (styles.css)
- **Polish (Phase 6)**: Depends on all user stories being complete

### User Story Dependencies

- **User Story 1 (P1)**: Can start immediately after Setup
- **User Story 2 (P2)**: Can start immediately after Setup - independent of US1
- **User Story 3 (P3)**: Requires T003 (styles.css) - can run in parallel with US1/US2

### Parallel Opportunities

- T001, T002, T003 in Setup can run in parallel
- T020 (CSV) can run in parallel with other US2 tasks
- All slide tasks (T021-T029) can run in parallel after T003

---

## Parallel Example: User Story 3

```bash
# After styles.css is complete, launch all slides in parallel:
Task: "Create title slide at workshops/data-storytelling/slides/01-title.html"
Task: "Create DC ACT Framework slide at workshops/data-storytelling/slides/02-dc-act-framework.html"
Task: "Create scenario introduction slide at workshops/data-storytelling/slides/03-scenario-intro.html"
# ... all 9 slides can be created simultaneously
```

---

## Implementation Strategy

### MVP First (User Story 1 Only)

1. Complete Phase 1: Setup (T001-T003)
2. Complete Phase 3: User Story 1 (T004-T014)
3. **STOP and VALIDATE**: Instructor can deliver workshop with facilitation guide alone
4. Deploy/demo if ready

### Incremental Delivery

1. Complete Setup → Styles ready
2. Add User Story 1 → Facilitation guide complete → **MVP!**
3. Add User Story 2 → Take-home assignment complete
4. Add User Story 3 → Visual slides complete
5. Each story adds value without breaking previous stories

### Full Parallel Strategy

1. Complete Setup (T001-T003)
2. In parallel:
   - Track A: User Story 1 (facilitation guide)
   - Track B: User Story 2 (take-home + CSV)
   - Track C: User Story 3 (9 HTML slides)
3. Polish phase after all tracks complete

---

## Notes

- [P] tasks = different files, no dependencies
- [Story] label maps task to specific user story for traceability
- Each user story should be independently completable and testable
- Commit after each task or logical group
- Stop at any checkpoint to validate story independently
- All HTML slides share styles.css - complete T003 before starting US3
