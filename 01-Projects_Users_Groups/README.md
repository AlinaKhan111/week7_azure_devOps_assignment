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

<img width="801" height="897" alt="Image" src="https://github.com/user-attachments/assets/4c873df5-bcf6-416c-b188-0a0e1eb6f5b3" />
<img width="710" height="889" alt="Image" src="https://github.com/user-attachments/assets/c82451ff-2d2a-4126-90e1-b7240e0d26cc" />
<img width="1918" height="905" alt="Image" src="https://github.com/user-attachments/assets/3c86979e-2582-4a02-bc74-b2bfd2c8b145" />
<img width="1861" height="912" alt="Image" src="https://github.com/user-attachments/assets/34cd504d-2f89-4b2e-8ba4-19f4a38c9873" />
<img width="1390" height="908" alt="Image" src="https://github.com/user-attachments/assets/d9ccb5c5-1ccf-4a3d-bfce-4f1036da76f0" />
<img width="1562" height="623" alt="Image" src="https://github.com/user-attachments/assets/a5265795-0d78-4ae5-bd83-d2f8447ad6eb" />
<img width="1504" height="876" alt="Image" src="https://github.com/user-attachments/assets/1f016aca-b5a1-4dd7-8ab5-72e71095af99" />
<img width="1717" height="539" alt="Image" src="https://github.com/user-attachments/assets/cf0d4849-472f-46bd-9042-97d1ebb46922" />