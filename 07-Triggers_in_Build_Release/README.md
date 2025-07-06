# Task 7: Apply Triggers in Build and Release
## Objective:
### Configure automated triggers so that changes to the master branch start a complete pipeline that includes both build and release stages, ensuring consistent and continuous integration and deployment.

## Actions Taken
1.  Created a multi-stage YAML pipeline in azure-pipelines.yml with:

- Build Stage:

  - Runs automatically on commits to master.

  - Simulates building the application with echo steps.

- Release Stage:

  - Configured with dependsOn: Build to start automatically when the Build stage completes successfully.

  - Simulates deployment actions with echo steps.

2. Pipeline YAML configuration:

```bash
trigger:
- master

pool:
  name: Default   # your self-hosted agent pool name

stages:
- stage: Build
  displayName: 'Build Stage'
  jobs:
  - job: BuildJob
    displayName: 'Run Build Job'
    steps:
    - script: echo "Building the application..."
      displayName: 'Build step'
    - script: echo "Simulating artifact creation..."
      displayName: 'Create artifact step'

- stage: Release
  displayName: 'Release Stage'
  dependsOn: Build   # runs after Build stage completes
  jobs:
  - job: ReleaseJob
    displayName: 'Run Release Job'
    steps:
    - script: echo "Deploying the application..."
      displayName: 'Deployment step'
    - script: echo "Release complete!"
      displayName: 'Confirmation step'

```
3.  Configured triggers with:

```bash
trigger:
- master
```
 This ensures the pipeline starts automatically on every commit to master.

4. Tested and verified the pipeline:

- Committed the updated azure-pipelines.yml to a feature branch.

- Created a pull request to merge into master.

- Confirmed that the pipeline ran automatically with both stages (Build and Release) executed sequentially.

## Summary
### By creating a multi-stage pipeline triggered on master, I successfully applied triggers in both build and release processes, fulfilling the assignment’s requirements for Task 7. The pipeline now automatically builds and deploys the application on every commit to the master branch.

<img width="1099" height="831" alt="Image" src="https://github.com/user-attachments/assets/56299b2f-42aa-456c-a86a-10f1b4fff968" />

<img width="1593" height="785" alt="Image" src="https://github.com/user-attachments/assets/977863dd-ed12-46e0-ab69-0d3d9a4bf4da" />