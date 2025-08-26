# 🚀 DevOps CI/CD Pipeline with Jenkins, Docker & GitHub

## 📌 Overview
This project demonstrates a **CI/CD pipeline** built using **Jenkins, Docker, GitHub, and Linux**.  
The pipeline automatically builds and deploys a **containerized Python Flask web application** whenever changes are pushed to the GitHub repository.  

To enable GitHub webhooks, **ngrok** was used for exposing the local Jenkins server to the internet.

---

## 🔹 Project Workflow
1. **Developer pushes code** to the GitHub repository.  
2. **GitHub Webhook (via ngrok)** triggers Jenkins.  
3. **Jenkins Pipeline** executes:  
   - Clones the repository  
   - Builds a new Docker image  
   - Runs placeholder tests  
   - Deploys the containerized app  
4. **Flask App** becomes available at `http://<server-ip>:5000` with updated changes.

---

## 🔹 Tools & Technologies Used
- **Linux (Ubuntu)** → Environment & automation scripts  
- **Git & GitHub** → Source code management & webhook integration  
- **Jenkins** → CI/CD automation  
- **Docker** → Containerization & deployment  
- **Python Flask** → Sample web application  
- **ngrok** → Tunnel for GitHub webhooks  

---

## 🔹 Project Structure

my-devops-project/
├── app.py # Flask web application
├── requirements.txt # Python dependencies
├── Dockerfile # Docker image build instructions
└── Jenkinsfile # Jenkins pipeline definition


## 🔹 Pipeline Stages
1. **Clone** → Pulls latest code from GitHub  
2. **Build** → Builds a Docker image for the app  
3. **Test** → Placeholder stage for running unit tests  
4. **Deploy** → Deploys the container with the new version  

---

## 🔹 Demo App Output
When deployed successfully, the Flask app displays:


---

## 📢 About This Project
This is a **portfolio project** designed as a **showpiece** to demonstrate how DevOps engineers can integrate **GitHub, Jenkins, Docker, and CI/CD best practices** in a real-world workflow.  

---
