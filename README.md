# 🚀 Docker Node.js App

A simple Node.js application containerized using Docker. This project demonstrates how to create a Docker image, run a container, and expose a web application.

---

## 📌 Project Overview

This is a basic Node.js HTTP server that returns:

```
Hello from your Docker App 🚀
```

The app is containerized using Docker and runs on port **3000**.

---

## 🛠️ Tech Stack

* Node.js
* Docker

---

## 📁 Project Structure

```
docker-node-app/
│── app.js
│── package.json
│── Dockerfile
│── README.md
```

---

## ⚙️ Setup & Run Locally

### 1️⃣ Clone Repository

```
git clone https://github.com/pranitdhekane/docker-node-app.git
cd docker-node-app
```

---

### 2️⃣ Build Docker Image

```
docker build -t node-app .
```

---

### 3️⃣ Run Docker Container

```
docker run -p 3000:3000 node-app
```

---

### 4️⃣ Access Application

Open your browser:

```
http://localhost:3000
```

---

## 🐳 Dockerfile Explanation

* `FROM node:18` → Base image
* `WORKDIR /app` → Working directory
* `COPY package*.json ./` → Copy dependencies
* `RUN npm install` → Install dependencies
* `COPY . .` → Copy app files
* `EXPOSE 3000` → Expose port
* `CMD ["node", "app.js"]` → Start application

---

## 📦 Useful Docker Commands

```
docker ps          # Running containers
docker ps -a       # All containers
docker images      # List images
docker stop <id>   # Stop container
docker rm <id>     # Remove container
```

---

## 🎯 Learning Outcome

* Understanding Docker basics
* Writing a Dockerfile
* Building Docker images
* Running containers

---

## 🙌 Author

**Pranit Dhekane**

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!

