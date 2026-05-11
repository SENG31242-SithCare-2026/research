# Contributing Guidelines

This document outlines the branching strategy, commit conventions, and pull request process for the SithCare `research` repository, adhering to the SENG 31242 System Design Project standards.

## 1. Branch Strategy
All team members must follow this branching strategy:

* **`main`**: This is a protected branch representing the latest approved version of our research artifacts. It only accepts merges via Pull Request with at least 1 approval.It enforces a linear history and dismisses stale PR approvals when new commits are pushed.
* **`draft/<document>`**: Use this prefix for active working branches for a document in progress. 
    * *Example:* `draft/client-interview-notes` 
* **`fix/<issue-number>`**: Use this prefix for corrective changes addressing review feedback. 
    * *Example:* `fix/42` 

## 2. Commit Message Convention
All commits must follow the adapted Conventional Commits specification:

`<type>(<scope>): <short imperative summary>` 
`[Optional body: explain WHY this change was made, not WHAT]` 
`[Optional footer: references to issues]` 

**Allowed Types:**
* `docs`: Adding or updating a document (e.g., meeting notes, transcripts).
* `feat`: Adding a new section or design element.
* `fix`: Correcting an error or incorporating review feedback.
* `refactor`: Restructuring a document without changing its content.
* `chore`: Repository housekeeping (updating `.gitignore`, `README`, etc.).
* `style`: Formatting changes only (font, heading levels, etc).

*Example:* `docs(interviews): add transcript for clinical psychologist interview` 

## 3. Pull Request Process
1.  Create a draft PR as soon as a branch is created to signal work-in-progress.
2.  When ready for review, mark the PR as "Ready for Review" and assign a reviewer from the team.
3.  Ensure your PR description follows the exact template below:

### PR Description Template

```markdown
## Summary

## Changes Made
- [ ] Item 1 
- [ ] Item 2 

## Related Issues
Closes #<issue-number> 

## Review Checklist
- [ ] Content is accurate and consistent with the approved project scope 
- [ ] References are correctly cited
- [ ] No spelling or grammatical errors (proof-read aloud) 
- [ ] Document formatting follows the report specification (Chapter 8) 
