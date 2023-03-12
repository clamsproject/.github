# clamsproject/.github

Organization defaults for CLAMS project

## Issue templates

### 📋 Because / Done when

### 🐛 Bug Report

### 💡 Feature Request

## Workflows

### `app-docker.yml`

Workflow action to:

- Build a docker image
- Extract labels and tags
- Login to gchr.io
  - Can override with environment variables
- Publish image

#### Usage

Create a `WORKFLOW_NAME.yml` file in your repository under `.github/workflows/`

```yml
name: 🪂 Continuous Deployment

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main
  release:
    types: [published, edited, prereleased]

jobs:
  build:
    name: 🔨 Build and deploy
    uses: clamsproject/.github/.github/workflows/app-docker.yml@main
```

## Organization Profile

Coming soon!
