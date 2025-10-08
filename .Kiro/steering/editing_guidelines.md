# Hugo Worklog Editing Guidelines

## CRITICAL: User Information Gathering Requirement

**MANDATORY STEP BEFORE ANY WORKLOG UPDATE:**

Before updating any week's worklog content, the AI MUST ask the user for the following specific information:

### Required Information to Collect:

1. **Week Title**: What is a descriptive title that summarizes the main activities of this week? (e.g., "Development Environment Setup and AWS Cloud Day 2025")

2. **Week Date Range**: What are the start and end dates for this week? (e.g., "Week X is from DD-DD/MMM/YYYY")

3. **Daily Activities**: For each day of the week, what activities were performed?
   - Day 1: [activities]
   - Day 2: [activities]
   - Day 3: [activities]
   - etc.

4. **Learning Outcomes**: What did you learn this week?
   - Technical skills acquired
   - AWS services explored
   - Tools and technologies used

5. **Challenges**: What challenges or difficulties did you face?

6. **Achievements**: What did you accomplish or complete?

7. **Additional Context**:
   - Any GitHub repos created?
   - Any specific AWS services used? (EC2, S3, Lambda, etc.)
   - Any workshops attended?
   - Any blog translations completed?

8. **Images**: Do you have any screenshots or images to include? If yes, what should they show?

### AI Behavior Rules:

- ❌ **NEVER** proceed with updating worklog content without first collecting this information from the user
- ❌ **NEVER** assume or fabricate worklog activities
- ❌ **NEVER** use generic placeholder content without user confirmation
- ✅ **ALWAYS** ask the user for specific details before writing content
- ✅ **ALWAYS** confirm the information with the user before finalizing the update
- ✅ **ALWAYS** allow the user to modify or add to the content during the process

### Example User Interaction:

```
AI: "I'm ready to update Week X worklog. Please provide the following information:

**Week Date Range:** When did Week X start and end?

**Daily Activities:** What did you do each day of the week?
- Day 1 (Date):
- Day 2 (Date):
- Day 3 (Date):
[etc.]

**Learning Outcomes:** What did you learn this week?

**Challenges:** What difficulties did you encounter?

**Achievements:** What did you accomplish?

**AWS Services Used:** Which AWS services did you work with?

**Images:** Do you have any screenshots to include? If yes, please describe what they should show.

**Blog Translations:** Did you translate any blogs this week?

**Workshops:** Did you attend any workshops this week?"
```

## General Documentation Principles

- Create placeholder for images when documenting worklog entries
- Document based ONLY on information provided by the user
- Add necessary details to fulfill the worklog requirements, but do not exaggerate
- Maintain professional tone throughout all documentation
- Ensure consistency between English and Vietnamese versions
- Never fabricate or assume activities without user confirmation, however if necessary add a few more details to fulfill the worklog, but do not exaggerate it.

## Hugo Front Matter Format

All worklog pages MUST follow this exact front matter format:

```yaml
---
title: "Week X Worklog"  # or "Worklog Tuần X" for Vietnamese
date: "YYYY-MM-DD"       # Actual date of the week
weight: X                # MUST match week number (1-12)
chapter: false
pre: " <b> 1.X. </b> "   # Section numbering
---
```

### Critical Weight Configuration Rules

**IMPORTANT:** The `weight` parameter controls the ordering in Hugo navigation.

- Week 1 MUST have `weight: 1`
- Week 2 MUST have `weight: 2`
- Week 3 MUST have `weight: 3`
- ... and so on through Week 12 with `weight: 12`

**Never use the same weight value for multiple weeks** - this causes incorrect alphabetical sorting where Week 1.1 appears after Week 1.9.

### Front Matter Examples

**English Version (_index.md):**

```yaml
---
title: "Week 1 Worklog"
date: "2025-09-08"
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---
```

**Vietnamese Version (_index.vi.md):**

```yaml
---
title: "Worklog Tuần 1"
date: "2025-09-08"
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---
```

## Worklog Content Structure

Each week's worklog should include:

### 1. Week Objectives

- Clear, concise bullet points
- Focus on learning goals and deliverables

### 2. Tasks Table

Format:

```markdown
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
```

- Use actual dates in DD/MM/YYYY format
- Include reference links where applicable
- Break down tasks with sub-bullets using `<br>` and `&emsp;` for indentation

### 3. Week Achievements

- Detailed bullet points of what was accomplished
- Include technical details and specific AWS services used
- Use sub-bullets for detailed breakdowns
- Add image placeholders with descriptive captions

### 4. Challenges Faced (Optional)

- Brief description of difficulties encountered
- Keep it honest but professional

### 5. Key Learnings (Optional)

- Important takeaways from the week
- Lessons learned

### 6. Next Week Goals (Optional)

- Forward-looking objectives
- Planning for upcoming work

## Image Handling

### Image Placement

- Store images in `static/images/weekX/` directory
- Create README.md in each week's image folder with instructions

### Image Reference Format

```markdown
![Descriptive Alt Text](/images/weekX/filename.png)
*Caption describing the image*
```

### Image Guidelines

- Use PNG or JPG format
- Remove sensitive information (account IDs, keys, etc.)
- Use descriptive filenames
- Keep file sizes reasonable
- Recommended resolution: 1920x1080 or similar

## Bilingual Content Requirements

### Consistency Rules

- Both English and Vietnamese versions must have identical structure
- Information scope should match across languages
- Dates and technical terms should be consistent
- Both versions must have the same `weight` value

### Translation Guidelines

- Maintain professional tone in both languages
- Adapt cultural context where appropriate
- Keep technical terms in English when commonly used (e.g., AWS, EC2, S3)
- Translate descriptions and explanations fully

## File Naming Conventions

- English files: `_index.md`
- Vietnamese files: `_index.vi.md`
- Maintain existing numerical prefixes in folder names (1.1-, 1.2-, etc.)
- Image folders: `weekX` (lowercase, no hyphens)

## Hugo Build Validation

After making changes, always verify:

1. Hugo builds without errors: `hugo --quiet`
2. Navigation order is correct (Week 1 → Week 2 → ... → Week 12)
3. Both language versions are accessible
4. Images load correctly (or placeholders are documented)

## Common Mistakes to Avoid

1. ❌ Using same weight for multiple weeks
2. ❌ Inconsistent date formats
3. ❌ Missing bilingual versions
4. ❌ Broken image links
5. ❌ Exaggerated or fictional content
6. ❌ Inconsistent front matter formatting
7. ❌ Missing or incorrect `pre` values

## Quality Checklist

Before completing a week's documentation:

- [ ] Front matter weight matches week number
- [ ] Both English and Vietnamese versions updated
- [ ] Dates are accurate and consistent
- [ ] Image placeholders created with README
- [ ] Content is professional and accurate
- [ ] Hugo builds successfully
- [ ] Navigation order is correct
