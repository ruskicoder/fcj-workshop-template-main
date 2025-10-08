# AI Workflow Checklist for Worklog Updates

## MANDATORY PRE-UPDATE CHECKLIST

Before updating ANY week's worklog content, the AI MUST complete this checklist:

### Step 1: Information Gathering (REQUIRED)

Ask the user for the following information:

```
I'm ready to update Week X worklog. Please provide the following information:

**Week Title:**
- What is a descriptive title for this week that summarizes the main activities? (e.g., "Development Environment Setup and AWS Cloud Day 2025")

**Week Date Range:** 
- When did Week X start and end? (e.g., "Week X is from DD-DD/MMM/YYYY")

**Daily Activities:** 
What did you do each day of the week?
- Day 1 (Date): 
- Day 2 (Date): 
- Day 3 (Date): 
- Day 4 (Date): 
- Day 5 (Date): 
- Day 6 (Date): 

**IMPORTANT:** Each day must be listed separately in the worklog table. Do not group days together (e.g., "Day 1-2"). If activities span multiple days, distribute them across individual day entries or fill in reasonable details for each day.

**Learning Outcomes:** 
- What did you learn this week?
- What technical skills did you acquire?

**Challenges:** 
- What difficulties or challenges did you encounter?

**Achievements:** 
- What did you accomplish or complete this week?

**AWS Services Used:** 
- Which AWS services did you work with? (e.g., EC2, S3, Lambda, RDS, VPC, etc.)

**Additional Context:**
- Did you create any GitHub repositories?
- Did you use any specific tools or technologies?

**Blog Translations:** 
- Did you translate any blogs this week? If yes, please provide:
  - Blog title
  - Blog topic/summary
  - Original source link
  - Key points from the blog

**Workshops:** 
- Did you attend any workshops this week? If yes, please provide:
  - Workshop name/topic
  - What you learned
  - Relevant workshop sections (5.1-5.6)

**Images:** 
- Do you have any screenshots or images to include?
- If yes, what should they show? (e.g., AWS console, configurations, etc.)
```

### Step 2: Validation (REQUIRED)

- [ ] User has provided week date range
- [ ] User has provided daily activities
- [ ] User has confirmed learning outcomes
- [ ] User has specified AWS services used
- [ ] User has clarified blog translation status
- [ ] User has clarified workshop attendance
- [ ] User has specified image requirements

### Step 3: Confirmation (REQUIRED)

Before proceeding with the update, confirm with the user:

```
Based on your information, I will update Week X with:
- Date range: [dates]
- Activities: [summary]
- AWS services: [list]
- Blog translations: [yes/no - details]
- Workshops: [yes/no - details]
- Images: [list of placeholders]

Does this look correct? Would you like to add or modify anything?
```

### Step 4: Implementation (ONLY AFTER CONFIRMATION)

Once user confirms, proceed with:

1. Update main Worklog index files with week title
   - Update `content/1-Worklog/_index.md` with descriptive week title in English
   - Update `content/1-Worklog/_index.vi.md` with descriptive week title in Vietnamese
   - Format: `**Week X:** [Descriptive Title](1.X-weekX/)`

2. Update English worklog file (`_index.md`)
   - Set correct `weight` parameter (must match week number)
   - Set correct date in front matter
   - Update all content sections based on user input

3. Update Vietnamese worklog file (`_index.vi.md`)
   - Ensure identical `weight` parameter
   - Ensure identical date
   - Translate content appropriately

4. Update blog translation files (if applicable)
   - English version
   - Vietnamese version

5. Update workshop files (if applicable)
   - Relevant workshop sections

6. Create image placeholders
   - Create `static/images/weekX/` directory
   - Add README.md with image instructions
   - Reference images in worklog content

7. Validate Hugo build
   - Run `hugo --quiet` to check for errors
   - Verify navigation order is correct

### Step 5: Completion

- [ ] Mark task as complete in tasks.md
- [ ] Inform user of completion
- [ ] Provide summary of what was updated
- [ ] Remind user to add actual images if placeholders were created

## CRITICAL RULES

### ❌ NEVER DO THIS:

- Proceed without asking user for information
- Assume or fabricate worklog activities
- Use generic placeholder content without user approval
- Skip the information gathering step
- Update content based on assumptions

### ✅ ALWAYS DO THIS:

- Ask user for specific details first
- Confirm information before proceeding
- Use only user-provided information
- Allow user to modify content during process
- Maintain professional tone
- Ensure bilingual consistency
- Set correct `weight` parameter (must match week number)
- Validate Hugo build after updates

## Quick Reference: Week Weight Values

| Week | Weight | Week | Weight | Week | Weight |
|------|--------|------|--------|------|--------|
| 1    | 1      | 5    | 5      | 9    | 9      |
| 2    | 2      | 6    | 6      | 10   | 10     |
| 3    | 3      | 7    | 7      | 11   | 11     |
| 4    | 4      | 8    | 8      | 12   | 12     |

## Example User Interaction Flow

```
User: "Start task 3" (Week 2)

AI: "I'm ready to update Week 2 worklog. Please provide the following information:
     [Full information gathering template]"

User: [Provides information]

AI: "Based on your information, I will update Week 2 with:
     [Summary of what will be updated]
     Does this look correct?"

User: "Yes" or [provides modifications]

AI: [Proceeds with updates]
     [Updates files]
     [Validates build]
     "Week 2 worklog has been updated successfully. 
      Please add screenshots to static/images/week2/ as described in the README."
```

## Troubleshooting

If user provides incomplete information:
- Ask specific follow-up questions
- Clarify ambiguous details
- Suggest reasonable defaults but always confirm

If user wants to skip certain sections:
- Confirm explicitly (e.g., "Should I skip blog translations for this week?")
- Document the skip in the task notes
- Proceed with remaining sections

If user wants to add more details later:
- Remind them that tasks can be revisited
- Explain how to request updates to existing content
- Ensure current update is complete before moving on
