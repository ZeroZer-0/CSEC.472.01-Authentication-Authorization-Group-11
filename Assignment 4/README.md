# README.md - CSEC 472 Assignment 4: Authentication & Security Models

## Task 1 Implementation Reference

### Task 1-A-a: Define a set of roles based on official job positions and functions
- Cell 2, Lines 56-66: `ROLE_METADATA`

### Task 1-A-b: Each user should be assigned a unique User ID and mapped to one or more roles
- Cell 2, Lines 115-137: `User.__init__`
- Cell 3, Lines 7-24: `main`

### Task 1-A-c: Implement role hierarchies where higher roles inherit access rights from lower roles
- Cell 2, Lines 43-53: `ROLE_HIERARCHY`

### Task 1-B-a: Implement a mapping of roles to applications and access rights
- Cell 2, Lines 7-40: `ROLE_PERMISSIONS`

### Task 1-B-b: Ensure that a role inherits permissions from roles below it
- Cell 2, Lines 72-93: `get_effective_permissions`

### Task 1-B-c: Implement a function that checks whether a user has access to a given application based on their assigned role
- Cell 2, Lines 96-102: `check_access`

### Task 1-C-a-i: Verify user credentials and role assignments
- Cell 2, Lines 146-147: `start_session`

### Task 1-C-a-ii: Ensure that only authorized users can access applications
- Cell 2, Lines 204-244: `request_access`

### Task 1-C-a-iii: Implement a log of access attempts for auditing purposes
- Cell 2, Lines 173-202: `log_access_attempt`

### Task 1-D-a: Implement a session-based access control where users are authenticated for a fixed session period
- Cell 2, Lines 139-151: `start_session`
- Cell 2, Lines 153-156: `end_session`
- Cell 2, Lines 167-171: `session_expired`
- Cell 2, Lines 229-234: `request_access`

### Task 1-D-b: Ensure users can hold up to 4 roles at a time but must select an active role for each session
- Cell 2, Line 126-129: `User.__init__`
- Cell 2, Lines 146-149: `User.start_session`
- Cell 2, Lines 223-227: `request_access`

### Task 1-D-c: Validate user roles dynamically when accessing an application
- Cell 2, Lines 96-102: `check_access`
- Cell 2, Lines 237-244: `request_access`

### Task 1-D-d: Implement error handling for invalid role selections and unauthorized access attempts
- Cell 2, Lines 124-132: `User.__init__`
- Cell 2, Lines 146-147: `User.start_session`
- Cell 2, Lines 237-244: `request_access`

### Task 1-E-a-i: Different users with varying roles and job functions attempt to access applications
- Cell 3, Lines 36-111: `main`

### Task 1-E: Create a Test Scenario, with detailed output showing User ID, selected role, application, access type, result, error messages
- Cell 3, Lines 36-111: `main`

### Task 1-E-b-iii: Log access attempts for future auditability
- Cell 2, Lines 173-202: `log_access_attempts`
- Cell 2, Line 226: `request_access`
- Cell 2, Line 233: `request_access`
- Cell 2, Line 240: `request_access`
- Cell 2, Line 244: `request_access`