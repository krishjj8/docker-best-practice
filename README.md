# 🐳 Docker Best Practice Project

This project demonstrates a minimal Node.js application containerized using **Docker best practices**, and integrated with **GitHub Actions CI/CD workflows**.

---

## 📦 Project Overview

This project teaches:

* ✅ Building lightweight and secure Docker images using `node:alpine`
* ✅ Using `.dockerignore` to reduce build context
* ✅ Creating a non-root user inside the container for security
* ✅ Layering Dockerfile instructions for better caching
* ✅ Automating Docker image builds with **GitHub Actions**

---

## 🛠 Tech Stack

* **Node.js** v20
* **Docker**
* **GitHub Actions** for CI
* Linux: Fedora (local development)

---

## 🚀 Run Locally

Clone the project:

```bash
git clone https://github.com/krishjj8/docker-best-practice.git
cd docker-best-practice
```

Build and run the Docker container:

```bash
docker build -t docker-best-practice .
docker run --rm docker-best-practice
```

---

## 📁 Project Structure

```
.
├── Dockerfile                  # Docker image instructions
├── .dockerignore               # Ignored files for smaller image
├── index.js                    # Sample Node.js app
├── package.json                # App metadata and dependencies
└── .github/workflows/
    └── docker.yml              # GitHub Actions CI workflow
```

---

## 🔄 GitHub Actions Workflow

This repo uses **GitHub Actions** to automatically:

* Build the Docker image on every push to `main`
* Use `ubuntu-latest` GitHub runner

### Sample Workflow Trigger:

```yaml
on:
  push:
    branches: [ "main" ]
```

---

## 📦 Latest Release

**Version:** `v1.0.0`

Tag it locally if needed:

```bash
git tag v1.0.0
git push origin v1.0.0
```

---

## 🙋‍♂️ Author

**Krish Kumar J**
Fedora Linux | B.Tech ECE | DevOps & Cloud Enthusiast

---

## 🌐 Repository

GitHub: [https://github.com/krishjj8/docker-best-practice](https://github.com/krishjj8/docker-best-practice)
git add README.md
fatal: not a git repository (or any parent up to mount point /)
Stopping at filesystem boundary (GIT_DISCOVERY_ACROSS_FILESYSTEM not set).
