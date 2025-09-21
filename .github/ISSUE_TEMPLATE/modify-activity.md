---
name: Modify Existing Activity
about: Request changes to an existing extracurricular activity
title: "Modify Activity: [ACTIVITY NAME] - [BRIEF DESCRIPTION OF CHANGE]"
labels: ["enhancement", "activity-modification", "teacher-request"]
assignees: ["@copilot"]

---

## Activity to Modify

**Current Activity Name:** [Enter the exact name as it appears in the system]

## Requested Changes

**What needs to be changed:** (Check all that apply)
- [ ] Activity name
- [ ] Description
- [ ] Schedule (days/times)
- [ ] Maximum capacity
- [ ] Add/remove specific students

### New Information (fill out only the sections that need changes)

**New Activity Name:** [Only if changing the name]

**New Description:** [Only if changing the description]

**New Schedule:** [Only if changing schedule]
- **Days:** (e.g., Monday, Wednesday, Friday)
- **Start Time:** (e.g., 3:30 PM or 07:15 AM)
- **End Time:** (e.g., 5:00 PM or 08:00 AM)

**New Maximum Capacity:** [Only if changing capacity]

**Students to Add:** [List email addresses, one per line]

**Students to Remove:** [List email addresses, one per line]

## Reason for Change

**Why is this change needed:** [Explain the reason for the modification]

**Teacher/Supervisor:** [Your name and contact]

**Urgency:** [High/Medium/Low]

---

**For Copilot Agent:** This request requires updating the specific activity entry in the `initial_activities` dictionary in `src/backend/database.py`. Be careful to maintain the existing data structure format, especially for schedule_details which needs both human-readable schedule string and structured schedule_details object with days array and 24-hour format times.