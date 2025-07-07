# Task 10: Use Work Items in Pipelines
## Objective:
### ntegrate Azure Boards work items with Azure Pipelines to automatically associate tasks, bugs, or user stories with builds for better traceability and project management.

## Steps 
1. Create a Work Item

   - In Azure DevOps, go to Boards → Work Items.

   - Create a new Task, Bug, or User Story (e.g., “Fix login redirect”).

   - Note the work item ID (e.g., #12).

2. Reference the Work Item in Commit Messages

   - When committing code locally, include the work item ID in your commit message:

   `git commit -m "Fix login redirect (Fixes #12)"`
   - Push your changes to the repository.

3. Pipeline Association

   - When the pipeline runs (automatically or manually), Azure DevOps will detect the work item ID in your commit.

   - The build will automatically link to the referenced work item.

4. Verify the Link

   - In Azure DevOps, go to Pipelines → Builds → select the relevant build → Summary tab.

   - In the Related Work Items section, confirm the work item ID appears, showing successful association.

## Summary:
Although this task was documented conceptually, it describes the industry-standard process of linking Azure Boards work items with pipeline builds by referencing work item IDs in commit messages. This workflow ensures full traceability from requirement to deployment, aligning with best practices in agile software development.