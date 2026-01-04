# Ronaldo2026

Repo for Docker automatic build & publish.

## Setup
1. **GitHub Secrets**: Go to Repo Settings -> Secrets and variables -> Actions. Add:
   - `DOCKERHUB_USERNAME`
   - `DOCKERHUB_TOKEN`

## Usage
- **Push to main**: triggers automatic build & push to Docker Hub.
- **Manual**: Go to Actions tab -> Docker Publish -> Run workflow.

## RunPod / Vast.ai
Use the following image path in your template configuration:
`ginopasticcino2/ronaldo2026:latest` 
*(Replace `ginopasticcino2` with your actual Docker Hub username if different)*

## Local Build (Optional)
```bash
docker build -t ronaldo2026:local .
docker run --gpus all ronaldo2026:local
```
