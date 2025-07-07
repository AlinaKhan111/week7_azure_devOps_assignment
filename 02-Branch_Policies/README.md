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

#02
<img width="1273" height="359" alt="Image" src="https://github.com/user-attachments/assets/b2088013-4b6a-4981-82e5-90346f014653" />
<img width="1491" height="959" alt="Image" src="https://github.com/user-attachments/assets/913a8bed-e399-4f16-8252-5a08fb2add2b" />
<img width="1919" height="897" alt="Image" src="https://github.com/user-attachments/assets/e4849a76-f20e-4ccc-999a-fcf3be5b46ae" />
<img width="1919" height="916" alt="Image" src="https://github.com/user-attachments/assets/01f1b531-e346-4c35-a7e0-08930006892c" />
![Image](https://github.com/user-attachments/assets/c8d493f0-8eb6-4a20-8aaa-3fb467d4a635)