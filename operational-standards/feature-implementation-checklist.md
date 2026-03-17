# Feature Implementation Checklist

**Scope:** All teams, all projects. This checklist is mandatory for every development feature.

**Owner:** Organization. Enforced by Team Leads.

**How to use:** The Team Lead references this checklist at the start of every feature implementation cycle. Every phase must be completed in order. No phase is skipped. The TL does not perform the work -- the TL dispatches team members, reviews their reports, makes decisions, and unblocks. Success is measured by team output, not TL output.

---

## Phase 1 -- Intake

- [ ] Feature identified on roadmap
- [ ] OpenSpec change created (`openspec new change`)
- [ ] Requirements Architect runs `openspec instructions` and follows the guided format
- [ ] Proposal written in OpenSpec format by Requirements Architect
- [ ] Sponsor reviews and approves proposal

## Phase 2 -- Design and Specification

- [ ] Requirements Architect advances the change through OpenSpec pipeline stages
- [ ] `openspec instructions` run at each stage transition for format guidance
- [ ] Specs written per capability in OpenSpec format (one spec per capability)
- [ ] UAT test cases written by QA Engineer against the specs -- before any code
- [ ] Tasks generated in OpenSpec format with clear ownership and sequencing
- [ ] `openspec list` confirms the change is tracked with correct task count
- [ ] TL reviews specs, test cases, and tasks for feasibility and completeness
- [ ] Dependencies identified (API before frontend, etc.)

## Phase 3 -- Implementation

- [ ] API work dispatched to Backend Developer (if applicable)
- [ ] API verified against live endpoints by QA Engineer before frontend starts
- [ ] Frontend work dispatched to Frontend Developer with specs, wireframes, and TL decisions
- [ ] Developers reference OpenSpec specs and tasks -- not verbal instructions
- [ ] Build passes clean
- [ ] TL receives progress reports -- does not do the work

## Phase 4 -- Review

- [ ] QA Engineer runs UAT test cases against the implementation -- pass or fail each case
- [ ] UX Designer reviews for wireframe fidelity, design system compliance, interaction quality
- [ ] Both reviews return with specific findings
- [ ] Findings dispatched to the responsible developer for fixes
- [ ] Fixes re-reviewed by QA and UX -- cycle until both approve

## Phase 5 -- Ship

- [ ] Production build
- [ ] Deploy to production environment
- [ ] UX Designer does final review of the live deployed feature -- provides feedback on the real product
- [ ] Any final UX feedback implemented and redeployed
- [ ] OpenSpec change archived (`openspec list` confirms no active changes remain)
- [ ] Roadmap updated to reflect shipped status
- [ ] Deployment recorded in experience layer

## Phase 6 -- Session Discipline (TL Startup)

- [ ] `openspec list` run to audit all active changes and their stage
- [ ] Read roadmap before engaging sponsor
- [ ] Query experience layer for project state and lessons
- [ ] Verify all shipped work is archived in OpenSpec
- [ ] Deliver status briefing to sponsor, not questions

---

## Principles

1. **OpenSpec is the single source of truth.** No work starts without a tracked change. No stage is skipped. `openspec instructions` is the format authority at every stage.
2. **The TL dispatches, does not do.** The TL's job is to keep the team moving, not to absorb their work. Every task has an owner who is not the TL.
3. **Two-stamp approval.** Nothing ships without QA pass and UX approval.
4. **UAT before code.** Test cases are written against specs, not against implementation. QA defines what "done" looks like before the developer starts.
5. **Process is not optional.** Following this checklist is itself a measure of Standards Discipline. Skipping steps is a defect, not a shortcut.
