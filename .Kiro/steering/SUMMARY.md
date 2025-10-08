# Steering Documents Summary

This directory contains guidelines and reference documents for maintaining the Hugo worklog website.

## Available Documents

### 0. AI_WORKFLOW_CHECKLIST.md (START HERE)
**Purpose:** Step-by-step mandatory checklist for AI when updating worklog content

**Key Topics:**
- Mandatory pre-update checklist
- Information gathering template
- Validation steps
- Confirmation process
- Implementation steps
- Critical rules (what to never do / always do)
- Example user interaction flow

**Use When:** 
- **EVERY TIME** before updating any week's worklog
- This is the PRIMARY document to follow for all worklog updates

---

### 1. editing_guidelines.md
**Purpose:** Comprehensive guide for editing and documenting worklog content

**Key Topics:**
- **CRITICAL: User Information Gathering Requirement** (MUST READ FIRST)
- General documentation principles
- Hugo front matter format
- Worklog content structure
- Image handling
- Bilingual content requirements
- Quality checklist

**Use When:** Creating or updating any worklog content

**IMPORTANT:** This document contains MANDATORY requirements for AI to ask users for specific worklog information before proceeding with any updates.

---

### 2. hugo_frontmatter_format.md
**Purpose:** Detailed reference for Hugo front matter configuration

**Key Topics:**
- Standard front matter templates
- Weight parameter rules and importance
- Complete examples for all 12 weeks
- Field descriptions
- Validation checklist

**Use When:** 
- Fixing navigation ordering issues
- Creating new week entries
- Troubleshooting Hugo build problems

---

## Quick Reference

### Correct Front Matter Format
```yaml
---
title: "Week X Worklog"  # or "Worklog Tuần X"
date: "YYYY-MM-DD"
weight: X                # MUST match week number!
chapter: false
pre: " <b> 1.X. </b> "
---
```

### Critical Rule
**The `weight` parameter MUST match the week number (1-12) to ensure correct ordering in navigation.**

### Common Tasks

| Task | Document to Reference |
|------|----------------------|
| Update week content | editing_guidelines.md |
| Fix navigation order | hugo_frontmatter_format.md |
| Add images | editing_guidelines.md (Image Handling section) |
| Create bilingual content | editing_guidelines.md (Bilingual Content section) |
| Troubleshoot Hugo build | Both documents |

## Document Maintenance

These steering documents should be updated when:
- New formatting patterns are established
- Common issues are identified and resolved
- Best practices evolve
- New sections or features are added to the website

## Getting Help

If you encounter issues not covered in these documents:
1. Check Hugo documentation: https://gohugo.io/documentation/
2. Review hugo-theme-learn documentation
3. Examine existing working examples in the content directory
4. Update these steering documents with solutions found
