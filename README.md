CI/CD Pipeline for .NET Application

 -Overview

This project demonstrates a basic Continuous Integration (CI) pipeline for a .NET application using GitHub Actions. 
The pipeline automatically validates builds on every code push, ensuring that the application compiles successfully in a clean Windows environment.

The goal of this project is to understand and implement CI fundamentals, including build automation, YAML-based workflows, and Git-based integration checks.

-Tech Stack

* .NET (ASP.NET Core)
* GitHub Actions
* YAML (workflow configuration)
* Windows-based runner
* Git & GitHub

-CI Pipeline Workflow

The CI pipeline is triggered automatically on:

* Every push to the repository
* Every pull request

-Pipeline Steps:

1. Checkout Code – Fetches the latest code from the repository
2. Setup .NET Environment – Installs the required .NET SDK
3. Restore Dependencies – Downloads all required packages
4. Build Application – Compiles the application to validate the build

If any step fails, the pipeline stops and reports an error.

 -Project Structure
.
├── Helloapi/                # .NET application source code
├── .github/workflows/       # GitHub Actions CI workflow
│   └── main.yml
├── .gitignore
└── README.md

-  How to Run Locally

Prerequisites

* .NET SDK installed
-Steps

bash
dotnet restore
dotnet build
dotnet run
What This Project Demonstrates

* Automated build validation using GitHub Actions
* YAML-based CI workflow configuration
* Windows-based CI execution for .NET applications
* Hands-on understanding of Continuous Integration concepts

Future Improvements

* Add automated unit tests*to the pipeline
* Generate and upload build artifacts
* Introduce basic security checks
* Extend pipeline to include a deployment stage



