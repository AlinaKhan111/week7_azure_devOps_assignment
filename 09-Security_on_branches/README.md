# Task 9: Apply Security on Branches so Contributors Can Create Pull Requests but Cannot Directly Merge Code to Master

## Objective:

- ### Enforce a workflow where Contributors must use pull requests to propose changes to master.

- ### Prevent Contributors from pushing or merging code directly to master, ensuring code review and policy enforcement.

## Steps Performed:
1. ### Configured Branch Security
- Went to Repos → Branches → master → Branch security.

- For the Contributors group:

  - Contribute → Deny  — blocks direct pushes and merges into master.

  - Create branch → Allow  — lets them create feature branches from master.

  - Create pull request → Allow  — allows them to submit pull requests targeting master.

  - Read → Allow — ensures read access to the codebase.

- For Project Administrators:

  - Contribute → Allow  — they can push or merge directly if needed.

  - Bypass policies when pushing → Allow (optional)  — grants override capabilities if required.

Saved changes to enforce updated security.

2. ### Tested the Permissions
- As a Contributor:

  -  Successfully created a feature branch from master.

  - Created a pull request from the feature branch targeting master.

  -  Direct push attempts to master failed with the expected error:

```bash
TF402455: Pushes to this branch are not permitted; you must use a pull request to update this branch.
```



## Summary:
Branch security was successfully applied so that Contributors:

- Can create feature branches.

- Can submit pull requests to propose changes to master.

- Cannot push or merge directly to master, enforcing a controlled workflow with code reviews and build validations.


![Image](https://github.com/user-attachments/assets/1d975099-94fc-46f4-9883-53c80843e7e4)
![Image](https://github.com/user-attachments/assets/2497e209-af2e-458e-90b7-38800e8e5266)