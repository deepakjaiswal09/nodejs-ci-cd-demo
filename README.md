# 🚀 Node.js CI/CD Task

A simple **Node.js web application** integrated with a **CI/CD pipeline** using **GitHub Actions**.  
This pipeline automatically **tests, builds, and pushes** a Docker image to **DockerHub** whenever changes are pushed to the `main` branch.

---

## 🛠 Tools & Technologies Used
- **Node.js** – Backend runtime
- **Express.js** – Minimal web framework
- **Jest + Supertest** – Testing framework
- **Docker** – Containerization
- **DockerHub** – Image registry
- **GitHub Actions** – CI/CD automation
- **Postman** – API testing tool

---

## 📸 Screenshots of Workflow

### 1️⃣ Initializing Node.js server and Docker in VS Code
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/52768eb8-d411-45ac-8dba-ff5d8ee310e5" />

---

### 2️⃣ Running the Docker image locally
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c3fec9d5-24ae-4b1f-8018-1fc0a61e3fb5" />

---

### 3️⃣ Docker image pushed to DockerHub
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/58cbbfae-dc50-4b02-90c2-fbc413677359" />

---

### 4️⃣ Testing the localhost server with Postman
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/712e88a2-2477-480e-9665-1841543d7ad9" />

---

### 5️⃣ GitHub Actions CI/CD pipeline run
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/442e4bb6-3160-4ac7-8ad4-c7a8e090cd9e" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/840a0353-4228-434f-8545-50a47225b53e" />

---

## ⚙️ How the CI/CD Workflow Works
1. Code is pushed to the `main` branch.
2. GitHub Actions pipeline runs:
   - **Install dependencies** → `npm ci`
   - **Run tests** → `npm test`
   - **Build Docker image**
   - **Push image to DockerHub**
3. DockerHub hosts the image, ready for deployment anywhere.

---

## How it works
- Push to `main` triggers GitHub Actions.
- Actions run `npm ci`, `npm test`, build Docker image, and push to DockerHub.

## Files
- `.github/workflows/main.yml` - CI pipeline
- `Dockerfile` - multi-stage Dockerfile
- `index.js` - sample Express app
- `tests/` - jest/supertest tests

## How to run locally
1. `npm install`
2. `npm test`
3. `docker build -t <your-image> .`
4. `docker run -p 3000:3000 <your-image>`

## Submission
GitHub repo: https://github.com/deepakjaiswal09/nodejs-ci-cd-demo




