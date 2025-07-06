# Task 2: Apply Branch Policies so Only Project Administrator Can Access the Master Branch

## Objective:
- ###  Restrict direct access to the master branch to only Project Administrators.

- ### Prevent Contributors from pushing directly to master, enforcing a safer workflow.

## Steps Performed:

### 1. Initialized the repository

   - Cloned the Azure Repos Git repository locally.

   - Added initial files and pushed them to create the master branch.

### 2. Navigated to Branch Security

   - In Azure DevOps, went to Repos → Branches.

   - Hovered over the master branch → clicked the 3 dots (⋮) → selected Branch security.

### 3. Configured permissions

- Selected the Contributors group:

      - Set Contribute → Deny

      - Set Force push (rewrite history, delete) → Deny

- Verified Project Administrators had Contribute → Allow.

### 4. Saved changes

- Saved the updated branch permissions to enforce security on master.

### 5. Tested permissions

- Confirmed Contributors are blocked from pushing directly to master.

- Verified Project Administrators retain full push access.

## Summary:
### Successfully applied branch security so that only Project Administrators can push directly to the master branch. Contributors must now submit pull requests, creating a controlled and auditable workflow that aligns with best practices.