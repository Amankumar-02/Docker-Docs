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
