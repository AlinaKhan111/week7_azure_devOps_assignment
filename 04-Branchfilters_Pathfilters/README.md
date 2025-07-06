# Task 4: Apply Branch Filters and Path Filters

## Objective:

- ### Configure branch and path filters so that branch policies (like build validation) apply only to specific branches or folders.

- ### Limit policy triggers to relevant changes, improving efficiency.

## Steps to set branch and path filters
### 1. Go to Branch Policies
- Azure DevOps portal → Repos → Branches → hover over master → 3 dots (⋮) → Branch policies.

### 2. Add or edit a build validation policy
- Under Build validation, click your existing build policy or Add build policy if none exists.

### 3. Set Path filters
- In the build policy dialog:

      - Scroll to Path filters (optional).

      - Set:

          - Include → files or directories that must change to trigger the policy.

              - Example: /src/** → only trigger the build if something under src/ is modified.

          - Exclude → files or directories to ignore.

              - Example: /docs/** → skip build if only documentation changes.

### 4.  Set Branch filters (in YAML pipeline triggers, if needed)
- If you want your pipeline to build only for specific branches:

   - Open your local azure-pipelines.yml.

   - Modify the trigger section:

``` bash
trigger:
  branches:
    include:
      - master
      - release/*
    exclude:
      - experimental/*
```

  - Commit and push your updated YAML.

This ensures your pipeline runs only on master and release/* branches, skipping others like experimental/*.

### 5.  Save changes

- In Azure DevOps web UI, click Save changes after editing build policy path filters.

## Important notes:
 - Path filters in branch policies allow fine-grained control: only meaningful code changes can trigger builds.
-  Branch filters in pipeline YAML control which branches automatically start builds.

## Summary:
### Successfully applied branch and path filters to your build validation policy and pipeline configuration. Now, builds trigger only on specified branches and when relevant files change, optimizing your CI/CD workflow.