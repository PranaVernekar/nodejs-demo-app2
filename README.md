# Create a Simple Jenkins Pipeline for CI/CD

## 🎯 Objective
Set up a basic Jenkins pipeline to automate the process of building and deploying a Node.js application.

## 🛠 Tools
- Jenkins
- Docker
- Node.js

## 📦 Deliverables
- A **Jenkinsfile** to build and deploy the app.

## 💡 Steps Followed
1. Installed Jenkins (locally or cloud instance).  
2. Created a **Jenkinsfile** in the repository with the following stages:
   - **Build** → Install dependencies and build the Node.js app.  
   - **Test** → Run automated tests (if available).  
   - **Deploy** → Build a Docker image and run the container.  
3. Configured Jenkins to trigger the pipeline on each **code commit**.  
4. Tested the pipeline by pushing changes and verifying the Jenkins dashboard.  

## ✅ Outcome
Successfully automated the build and deployment process for the `nodejs-demo-app2`.  
Each code change now triggers the Jenkins pipeline automatically.

---

## 📹 Pipeline Build Video
The **14th build** was triggered by the output video's upload.

https://github.com/user-attachments/assets/96abc4cf-1c11-4fc7-90fe-275ed6d9ae46  

---

## 🖼 Screenshot
<img width="1914" height="965" alt="Screenshot 2025-09-23 174917" src="https://github.com/user-attachments/assets/41484086-1898-4fe0-811e-fb50050f7114" />

