<!--
================================================================================
SYNC IMPACT REPORT
================================================================================
Version Change: 1.1.0 → 1.1.1 (PATCH - corrected framework wording to match DC ACT mnemonic)

Modified Principles:
- IV. Practical Application: expanded rationale to reference job interviews and capstones

Added Sections:
- Purpose (new section after title establishing strategic context)
- Quality Gates: added job/capstone relevance checkpoint

Removed Sections: N/A

Templates Requiring Updates:
- .specify/templates/plan-template.md: ⚠ pending (software-focused, may need educational variant)
- .specify/templates/spec-template.md: ⚠ pending (software-focused, may need educational variant)
- .specify/templates/tasks-template.md: ⚠ pending (software-focused, may need educational variant)

Follow-up TODOs:
- Consider creating education-specific template variants for workshop development
================================================================================
-->

# Presentation Skills Workshop Constitution

## Purpose

This workshop series prepares analytics students for two critical milestones:

1. **Job Interviews**: Communicating analytical work to hiring managers and stakeholders in a way that demonstrates business impact and decision-making capability
2. **Capstone Project Presentations**: Presenting culminating academic work with the clarity and professionalism expected in industry settings

All content decisions MUST be evaluated against this question: **Will this skill help a student succeed in a job interview or capstone presentation?**

## Core Principles

### I. Insight-Driven Communication

All workshop content, exercises, and deliverables MUST demonstrate insight-driven communication rather than descriptive labeling.

- Slide titles MUST convey actionable insights, not categories
- Every data visualization MUST support a specific insight, not just display data
- Recommendations MUST flow logically from presented insights
- Participants MUST be evaluated on their ability to transform descriptive content into insight-driven content

**Rationale**: This is the core skill being taught, derived from Cole Nussbaumer Knaflic's "Storytelling with Data" methodology. Descriptive titles like "Q3 Sales Data" fail to drive decisions; insight titles like "Q3 Sales Dropped 15%—Supply Chain Action Required" create clarity and urgency. Hiring managers and capstone evaluators judge candidates on their ability to synthesize data into actionable insights.

### II. Discovery Learning Pedagogy

Workshop design MUST follow a discovery learning approach where participants attempt exercises before receiving instruction.

- Participants MUST attempt tasks before being shown "the right way"
- Instruction MUST follow participant attempts to reveal skill gaps
- Feedback MUST highlight the delta between current and desired performance
- Examples MUST include both "before" (common mistakes) and "after" (proper execution)

**Rationale**: Adults learn more effectively when they experience the gap in their skills firsthand. Showing the correct approach after an attempt creates memorable contrast and motivation to improve.

### III. Framework Alignment

All workshop content MUST align with the 5-Step Analytics Framework (DC ACT):

1. **Define** the business problem
2. **Collect** and prepare the data
3. **Analyze** the data and generate insights
4. **Communicate** the insights, recommendations, and predictions
5. **Act** and track the change

- Workshop scenarios MUST include all five steps, even when focusing on step 4 (communication)
- Participants MUST be able to articulate: problem → data → insight → recommendation
- Assessment criteria MUST evaluate framework adherence, not just presentation aesthetics

**Rationale**: Communication skills exist within the broader analytics workflow. Job interviewers expect candidates to demonstrate end-to-end thinking. Capstone evaluators assess whether students understand the full analytical process, not just the final deliverable.

### IV. Practical Application

All learning activities MUST use realistic scenarios with actual (or realistic synthetic) data.

- Datasets MUST be believable and domain-relevant to analytics professionals
- Scenarios MUST have clear business problems with non-obvious insights
- Exercises MUST produce tangible deliverables (slides, presentations)
- Individual assessments MUST demonstrate skill transfer to new contexts

**Rationale**: Abstract exercises don't build transferable skills. Students will face real data in job interviews (case studies, take-home assignments) and capstone projects. Practicing with authentic scenarios builds confidence and pattern recognition for high-stakes situations.

### V. Measurable Outcomes

All workshop objectives MUST have clear, binary assessment criteria.

- Learning outcomes MUST be observable and verifiable
- Assessment criteria MUST be objective, not subjective ("has insight-driven title" vs "looks professional")
- Success metrics MUST be defined before workshop delivery
- Participant work MUST be evaluated against pre-defined rubrics

**Rationale**: Vague outcomes like "improve presentation skills" are unmeasurable. Specific criteria like "slide title conveys actionable insight" can be objectively verified—and mirror the clear pass/fail nature of job interviews and capstone evaluations.

## Content Standards

Based on Cole Nussbaumer Knaflic's "Storytelling with Data" principles:

| Standard | Description | Verification |
|----------|-------------|--------------|
| **Action Titles** | Titles state the insight, not the category | Does the title tell the viewer what to conclude? |
| **Sentence Case** | Titles use sentence capitalization | First letter capitalized, rest lowercase (except proper nouns) |
| **Single-Line Concision** | Titles fit on one line | No line breaks in slide titles |
| **Visual Hierarchy** | Key data points are visually emphasized | Can the viewer find the critical number in 3 seconds? |
| **Chart-Message Alignment** | Visualization type supports the insight | Does the chart make the insight obvious? |
| **Clutter Reduction** | Remove non-essential elements | Every element earns its place |

## Workshop Development Process

### Creation Workflow

1. **Define Outcome**: State the specific, measurable skill participants will demonstrate
2. **Design Assessment**: Create the evaluation criteria and rubric first
3. **Build Scenario**: Develop realistic data and business context
4. **Create "Bad" Examples**: Design common-mistake examples for transformation exercises
5. **Structure Flow**: Apply discovery learning sequence (attempt → gap reveal → instruction → revision)
6. **Validate Timing**: Test all activities fit within allocated time with buffer

### Quality Gates

- [ ] All content follows insight-driven communication principles
- [ ] Discovery learning sequence is explicit in facilitation guide
- [ ] Assessment criteria are binary and objective
- [ ] Scenario data produces non-obvious but discoverable insights
- [ ] Time allocations tested with pilot participants
- [ ] Content directly applicable to job interview or capstone presentation scenarios

## Governance

This constitution establishes the non-negotiable principles for all presentation skills workshop content in this repository.

**Amendment Process**:
1. Propose change with rationale in writing
2. Evaluate impact on existing workshop materials
3. Update all affected materials before ratification
4. Increment version according to semantic versioning

**Versioning Policy**:
- MAJOR: Principle removal, redefinition, or fundamental pedagogical change
- MINOR: New principle added, section expanded, new content standard
- PATCH: Clarification, typo fix, wording refinement

**Compliance Review**:
- All new workshop content MUST be reviewed against constitution principles
- Existing content SHOULD be audited annually for constitution alignment
- Violations MUST be documented with justification or corrected

**Version**: 1.1.1 | **Ratified**: 2025-01-27 | **Last Amended**: 2025-01-27
