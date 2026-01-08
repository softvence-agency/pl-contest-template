# 📌 CI/CD Deployment Contest – Project Lead Selection

## 🎯 Objective

This contest is designed to evaluate **real-life backend devloyment task**.  
Based on this task, we will **select Project Leads (PL)**.

Each developer must **deploy an application to a VPS using a full CI/CD pipeline**.  
Deployment must be **automatic on every push to the `main` branch**.

📅 **Deadline:**  
**From now to 10/01/2026 at 10:00 AM**

---

## 🧩 Mandatory Conditions (Very Important)

1. **PostgreSQL database is mandatory**
   - Application must use PostgreSQL
   - DB must run using Docker

2. **Cross-technology deployment**
   - **Laravel & Python developers** → must deploy a **Node.js (NestJS)** application
   - **Node.js developers** → must deploy a **Python (FastAPI or Django)** application

3. **CI/CD must be fully automated**
   - Firstly it would be manually deploy then the pipeline would be automated
   - Deployment must trigger on **push to `main` branch**

---

## 🏗️ Technology Stack (Required)

Each project must use:

- GitHub repository
- Docker & Docker Compose
- VPS (Linux Server)
- CI/CD (GitHub Actions)
- PostgreSQL
- Nginx or Caddy (recommended)
- Environment variables (`.env`, and `.env.production`)

---

## 📂 Step-by-Step Tasks (What You Must Complete)

---

## Step 1: Repository Setup

- Cloning our provided template called [PL Contest Template](https://github.com/softvence-agency/pl-contest-template)
- Add proper project structure
- Replace template `README.md` file with:
  - Project description
  - Tech stack
  - Deployment steps
  - Simple CI/CD explanation (optional)

---

## Step 2: Application Setup

- Setup the assigned backend framework:
  - **NestJS**
  - **or FastAPI / Django**
- Create at least:
  - One health check API (`/health`)
  - One database connection API (`/db`)
  - 2 endpoint for storing data and retrieving it

---

## Step 3: PostgreSQL Integration

- Configure PostgreSQL connection
- Use `.env` for credentials
- Ensure DB connection works inside Docker
- Database data must persist using volumes, and maintain network

---

## Step 4: Dockerization

You must provide:

1. `Dockerfile`
2. For prod `docker-compose.yaml` and dev `docker-compose.dev.yaml` Or use profileing system or direact file for `development` and `production`

Docker Compose must include:

- Application service
- PostgreSQL service
- Network configuration
- Volume for DB persistence

---

## Step 5: VPS Preparation

On your VPS:

- Install Docker & Docker Compose
- Configure firewall (open required ports)
- Make sure your application has inside `~/projects` folder
  **Creadentials**
  Host: `User:`
  Password: ``

---

## Step 6: CI/CD Pipeline Setup

This is the **core evaluation part**.

Pipeline must:

- Trigger on `push` to `main`
- Checkout code
- Build Docker images
- Stop old containers
- Run new containers using Docker Compose
- Handle environment variables securely

---

## Step 7: Environment Management

- No secrets inside code
- Use:
  - GitHub Secrets
- Separate:
  - Development
  - Production configuration

---

## Step 8: Deployment Verification

After deployment:

- Application must be accessible via:
  - Public IP or domain
- APIs must return proper response
- PostgreSQL data must persist after container restart

---

## Step 9: Documentation (Mandatory)

Each developer must submit:

- Repository link
- VPS public IP / domain
- CI/CD config file
- Short explanation:
  - Common issues faced and solutions (Mandetory)

---

## 🧪 Bonus Points (Optional but Strongly Recommended)

- HTTPS (SSL) [if you have domain]
- Reverse proxy setup
- Database migration handling
- Health checks in CI/CD
- Logging & monitoring basics (optional)

---

## 🏆 Evaluation Criteria (PL Selection)

We will evaluate based on:

1. CI/CD correctness
2. Automation level
3. Docker & DB understanding
4. Clean documentation
5. Debugging & problem-solving ability
6. Production readiness mindset

---

## 📚 Reference

You **follow and apply concepts** from this course:

🔗 **CI/CD, Docker, AWS EC2 Full Course (3h 10m)**
👉 https://www.youtube.com/watch?v=FRJ_C-sZJB8

---

## 📢 Final Note

This is **not a tutorial task**, this is a **real production-level challenge**.  
Take it seriously and do it properly.

If anyone faces **real blocking issues**, you may reach out to me.

**Best of luck to everyone.**  
This contest will define our **next Project Leads** 🚀
