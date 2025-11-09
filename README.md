# Matrix Build CI/CD Demo

This repository demonstrates a GitHub Actions workflow with matrix build strategy and artifact management.

## Contact Information

**Email:** 24f1002781@ds.study.iitm.ac.in

## Workflow Features

- **Matrix Strategy**: Builds across 4 Node.js versions (14, 16, 18, 20)
- **Parallel Execution**: All matrix jobs run simultaneously
- **Artifact Management**: Each build generates and uploads unique artifacts
- **Artifact Naming**: All artifacts use the prefix `build-e86dd6b-node<version>`

## Matrix Configuration

The workflow builds for the following configurations:
- Node.js 14 (legacy)
- Node.js 16 (stable)
- Node.js 18 (current)
- Node.js 20 (latest)

## Artifacts Generated

Each matrix job produces:
- `output.txt` - Build information and metadata
- `metadata.json` - Structured build data in JSON format

## Running the Workflow

The workflow triggers on:
- Push to main/master branch
- Pull requests to main/master branch
- Manual workflow dispatch

## View Results

Check the Actions tab to see:
- Parallel matrix job execution
- Generated artifacts for each Node.js version
- Build logs and timings
