---
name: Teacher Account Management
about: Request changes to teacher accounts or permissions
title: "Teacher Account: [ADD/MODIFY/REMOVE] - [TEACHER NAME]"
labels: ["user-management", "teacher-account", "admin-request"]
assignees: ["@copilot"]

---

## Account Action Required

**Type of Request:** (Select one)
- [ ] Add new teacher account
- [ ] Modify existing teacher account
- [ ] Remove teacher account
- [ ] Reset teacher password

## Teacher Information

**Full Name:** [Teacher's full name for display]

**Username:** [Desired username (for new accounts) or existing username]

**Display Name:** [How the name should appear in the system (e.g., "Ms. Rodriguez", "Mr. Chen")]

**Role:**
- [ ] Teacher
- [ ] Administrator
- [ ] Principal

## Account Details

**For New Accounts:**
- **Initial Password:** [Temporary password - teacher should change on first login]
- **Activities to Supervise:** [List any activities this teacher will manage]

**For Modifications:**
- **Current Username:** 
- **New Display Name:** (if changing)
- **New Role:** (if changing)

**For Password Reset:**
- **New Temporary Password:** 
- **Reason for Reset:** 

## Authorization

**Requesting Administrator:** [Your name and role]

**Authorization Level:**
- [ ] I have administrative privileges to make this change
- [ ] This request has been approved by the principal
- [ ] This is an emergency access request

**Reason for Request:** [Brief explanation of why this change is needed]

**Timeline:** [When does this need to be completed]

---

**For Copilot Agent:** This request requires updating the `initial_teachers` array in `src/backend/database.py`. For new accounts, follow the existing format with username, display_name, hashed password using `hash_password()` function, and role. Ensure usernames are unique and passwords are properly hashed.