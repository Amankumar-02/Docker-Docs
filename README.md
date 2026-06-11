# 🐳 Docker Learning Notes

A beginner-friendly guide and hands-on notes for learning **Docker**.  
This repo contains basic concepts, useful commands, and simple examples.

---

## 📌 What is Docker

Docker is a platform that lets you run applications inside isolated environments called **containers**.

It helps developers:
- Run apps consistently on any system  
- Avoid “it works on my machine” issues  
- Package app + dependencies together  

---

## 🧱 Key Concepts

### 📦 Image
A **blueprint** for creating containers.

```bash
docker pull nginx
```

### 🚀 Container
A **running instance** of an image.

```bash
docker run nginx
```

### 💾 Volume
Used to store **persistent data** (data survives container deletion).

```bash
docker volume create mydata
```

### 🌐 Network
Allows containers to **communicate** with each other.

```bash
docker network create mynetwork
```

---

## ⚙️ Common Docker Commands

### 📥 Images

```bash
docker pull <image>
docker images
docker rmi <image-id>
```

### 📦 Containers

```bash
docker run <image>
docker ps
docker ps -a
docker stop <container-id>
docker rm <container-id>
docker rm -f <container-id>
```

### 🧹 Cleanup

```bash
docker container prune
docker image prune
docker system prune
docker system prune -a
```

### 🧪 Example: Run Nginx

```bash
docker run -d -p 8080:80 nginx
```

Then open:

```
http://localhost:8080
```

### 🧪 Example: Interactive Alpine Container
Alpine Linux is a lightweight Linux image used for testing.

```bash
docker run -it alpine sh
```

Inside container:

```
ls
pwd
cat /etc/os-release
```

---

## 📚 Learning Outcome
After this, I learned:

- How containers work
- Difference between images and containers
- How to manage Docker resources
- Basic real-world usage

---

## 🚀 Next Steps

- Learn Dockerfile
- Build custom images
- Learn Docker Compose
- Run full-stack apps (frontend + backend + DB)
