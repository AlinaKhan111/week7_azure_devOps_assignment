# Task 1: Create Project with User Groups and Implement Group Policies

## Objective:
- ### Set up an Azure DevOps project with distinct user groups.

- ### Assign appropriate permissions to ensure controlled access for different roles.

##  Steps Performed:
### 1. Created a new Azure DevOps project
   - Navigated to the Azure DevOps organization.

   - Clicked New Project, provided project details, and created it.

### 2. Accessed Project Settings

   - Clicked Project settings in the lower-left corner of the project page.

### 3. Configured user groups

   - Opened Permissions → Project-level groups.

   - Verified built-in groups:

      - Project Administrators

      - Contributors

      - Readers

- (Optional) Created a custom group if needed.

### 4. Assigned users to groups

- Added users to appropriate groups using Add → Users, assigning them to Project Administrators, Contributors, or Readers as needed.

### 5. Applied example group policies

- Project Administrators: Full permissions.

- Contributors: Granted contribute permission; restricted admin-level permissions like editing policies or deleting repos.

- Readers: Granted read-only permissions; prevented from contributing or changing settings.

### 6. Tested group access (optional)

- Logged in with a test user assigned to each group to verify effective permissions:

      - Readers could only view content.

      - Contributors could push code but not modify settings.

      - Project Administrators could perform all actions.

## Summary:
### Successfully set up an Azure DevOps project with clearly defined user groups and permissions to ensure secure, role-based access control. This foundational setup allows effective team collaboration while enforcing least-privilege security.