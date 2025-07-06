# Task 3: Apply Branch Security and Locks

## Objective:

- ### Add an extra layer of protection on the master branch by applying locks.

- ### Strengthen branch security to control changes during critical phases.

## Steps Performed:
1. ### Navigated to Branches

   - Opened Repos → Branches in Azure DevOps.

2. ### Applied a lock on the master branch

   - Hovered over the master branch → clicked the 3 dots (⋮) → selected Lock.

   - This locked the branch, making it read-only for most contributors.

3. ### Verified lock behavior

   - Attempted to push to the locked branch as a Contributor: push was blocked.

   - Observed that Project Administrators could still push due to their ability to bypass policies.

4. ### Reviewed permissions

   - Confirmed that branch security from Task 2 remains enforced after locking and unlocking the branch.

## Summary:
### Successfully applied a lock on the master branch to prevent unwanted changes during key development or release phases. Combined with branch security settings, this helps maintain strict control over code changes.

#03
<img width="1582" height="295" alt="Image" src="https://github.com/user-attachments/assets/91d88417-22d2-448d-ba01-7337a8ada2fa" />