# CI/CD Workflow Exercise (Go)

A hands-on exercise practicing CI/CD pipelines with GitHub Actions, done as part of my Cloud Computing coursework.

## 📖 What this is
A GitHub Actions CI workflow (`.github/workflows/go.yml`) that automatically builds a Docker image and pushes it to Docker Hub on every push to the `s4` branch. Configured and iterated on by hand to understand how CI/CD pipelines are built — not a generated template.

## 🧰 Tech used
- **CI/CD:** GitHub Actions
- **Containerization:** Docker (Buildx, QEMU for multi-platform builds)
- **Registry:** Docker Hub
- **Trigger:** Push to `s4` branch

## ⚙️ What the pipeline does
1. Triggers on every push to the `s4` branch
2. Sets up QEMU (for multi-platform emulation) and Docker Buildx
3. Logs in to Docker Hub using stored repository secrets (`DOCKERHUB_USERNAME`, `DOCKERHUB_TOKEN`)
4. Builds the Docker image and pushes it to Docker Hub, tagged `user/app:latest`

## 💡 What I learned
Hands-on practice building a full CI/CD pipeline: setting up Docker Buildx and QEMU for cross-platform image builds, securely handling credentials with GitHub Actions secrets, and automating image builds and registry pushes on every code change.

---
*Coursework exercise — Cloud Computing course.*
