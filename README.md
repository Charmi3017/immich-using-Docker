# Immich - Self-Hosted Photo and Video Backup with Docker

## 🚀 Overview
[Immich](https://github.com/immich-app/immich) is a high-performance, self-hosted photo and video backup solution that utilizes AI-powered image tagging, facial recognition, and powerful search capabilities.

This guide will help you **deploy Immich using Docker**.

## 🛠 Prerequisites
Ensure you have the following installed on your system:
- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## 📦 Installation
### 1️⃣ Clone the Immich Repository
```sh
git clone https://github.com/immich-app/immich.git
cd immich
```

### 2️⃣ Create a `.env` File (Optional)
Modify environment variables if needed:
```sh
cp .env.example .env
```

### 3️⃣ Run Immich with Docker Compose
```sh
docker-compose up -d
```
This command will:
- Pull the latest Immich Docker images
- Start all necessary services (database, Redis, etc.)

## 🖥 Accessing Immich
Once the containers are running, access Immich via:
```
http://localhost:2283
```
(Default credentials can be set in `.env` or during the first-time setup.)

## 🔄 Updating Immich
To update to the latest version:
```sh
docker-compose pull

docker-compose up -d --force-recreate
```

## 🛑 Stopping Immich
To stop and remove all running containers:
```sh
docker-compose down
```

## 📚 Documentation
For more details, visit the official [Immich GitHub Repository](https://github.com/immich-app/immich).

---
Enjoy seamless and secure self-hosted photo and video backups with **Immich**! 🚀
