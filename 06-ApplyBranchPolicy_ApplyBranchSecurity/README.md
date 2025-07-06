# Task 6: Apply Branch Policy and Branch Security
## Objective:
### Secure the master branch by:
 - ### Applying branch policies to enforce checks (e.g., required builds).
 - ### Setting branch security to restrict direct pushes and enforce PR-based workflow.

## Steps Performed:

### Apply Branch Policies
1.  Went to Repos → Branches → master → Branch policies.
2.  Added a build validation policy requiring the pipeline to succeed before merging PRs.
3. Configured optional path filters to control when the build triggers.
4. Set the policy to Required, blocking PR completion on build failure.
5. Saved the policy.

### Apply Branch Security
1. Went to Repos → Branches → master → Branch security.
2. Configured permissions for Contributors:

  - Contribute → Deny (prevents direct pushes).

  - Create branch → Allow (they can create feature branches).

  - Create pull request → Allow (they can submit PRs).

  - Read → Allow.
3. Configured permissions for Project Administrators:

  - Contribute → Allow (admins can push directly if necessary).

  - Bypass policies when pushing → Allow (optional, gives admins override power).

  - Read → Allow.
4. Saved all security changes.

## Summary:
Branch policies and security were successfully applied on master, ensuring:
- Contributors must use pull requests for changes.
- Builds validate code before merging.
- Only project administrators can push directly, maintaining a secure, controlled workflow.

