**Pipeline Overview**

The workflow is triggered automatically on every push and pull request to the main branch.

**Continuous Integration (CI)**

Source code checkout

Dependency restoration using .NET CLI

Build validation

Automated unit test execution

Basic security scanning of source code

Release build publishing

Build artifact generation and upload

**Continuous Delivery (CD)**

Automatic creation of a versioned GitHub Release

Attachment of published build artifacts

Execution only after successful CI completion

** Technologies Used**

.NET 9

GitHub Actions

YAML

PowerShell

Windows-based GitHub runners

**Security Check**

A basic security scan is included in the pipeline to detect potential hardcoded secrets in source files.
The check is implemented using PowerShell, ensuring compatibility with Windows runners and preventing false positives.

** Artifacts & Releases**

Published application files are packaged as build artifacts.

Artifacts are automatically attached to GitHub Releases as part of the CD stage.

Each release is versioned using the workflow run number.

** Workflow Structure**
.github/
 └── workflows/
     └── main.yml

**Key Learnings**

Designing CI/CD pipelines for Windows-based environments

Writing and debugging GitHub Actions workflows using YAML

Handling real-world CI failures (permissions, shell behavior, deprecated actions)

Implementing secure and reliable automation practices

Understanding the separation of CI and CD in enterprise systems

** Status**

✔ CI pipeline fully functional
✔ CD pipeline successfully creating GitHub Releases
✔ Resume and interview ready

**Note**

This project focuses on pipeline design and automation.
Deployment to runtime environments (e.g., cloud services or servers) is intentionally excluded, as it is typically handled by separate deployment pipelines in enterprise setups.
