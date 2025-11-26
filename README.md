---

# Git & Docker Practice

This repository documents the work completed for practicing Git workflows and Docker basics, including branching, pull requests, merge conflict resolution, containerization, and publishing Docker images.

---

## ✅ Git Tasks Completed

### 1. Create GitHub Repository

* Create a new GitHub repository named **git-practice**
* Initialize it with a `README.md`

---

### 2. Clone the Repository

```bash
git clone https://github.com/<your-username>/git-practice.git
cd git-practice
```

---

### 3. Create and Work on Branches

#### Create a feature branch:

```bash
git checkout -b feature1
```

#### Make changes, commit, and push:

```bash
git add .
git commit -m "Add feature 1"
git push -u origin feature1
```

---

### 4. Create Pull Request and Merge

* Open a Pull Request (PR) on GitHub
* Review the changes
* Merge the PR into the `main` branch

---

### 5. Practice Merge Conflict

#### Steps followed:

1. Create another branch:

   ```bash
   git checkout -b feature2
   ```

2. Modify the same line in `README.md`.

3. Push the branch and create a PR.

4. GitHub detects a merge conflict.

5. Resolve conflict using GitHub’s conflict editor:

   * Choose the final combined text
   * Mark as resolved
   * Merge successfully

---

### 6. Sync Local Repository

```bash
git checkout main
git pull
```

---

## ✅ Docker Tasks Completed

### 1. Learned Docker Basics

Understood the following concepts:

* **Images vs Containers**
* Common Docker commands:

  * `docker build`
  * `docker run`
  * `docker ps`
  * `docker images`
  * `docker push`

---

### 2. Dockerized a Python Application

Created the following files:

* `app.py` (Flask web app)
* `requirements.txt`
* `Dockerfile`

#### Build Docker image:

```bash
docker build -t chinnmayk/python-docker-demo:v1 .
```

#### Run the container:

```bash
docker run -p 5000:5000 chinnmayk/python-docker-demo:v1
```

---

### 3. Push Docker Image to Docker Hub

#### Login:

```bash
docker login
```

#### Tag image (if required):

```bash
docker tag python-docker-demo:v1 chinnmayk/python-docker-demo:v1
```

#### Push to Docker Hub:

```bash
docker push chinnmayk/python-docker-demo:v1
```

---

## ✅ Tools Used

* Git
* GitHub
* Docker Desktop
* Docker Hub
* Git Bash

---

## ✅ Summary

In this practice, the following skills were demonstrated:

✔ Creating and managing Git repositories
✔ Working with branches and pull requests
✔ Handling and resolving merge conflicts
✔ Containerizing a Python application using Docker
✔ Building and running Docker images locally
✔ Publishing Docker images to Docker Hub

---
