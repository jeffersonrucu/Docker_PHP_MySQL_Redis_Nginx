
# Docker with PHP, MySQL, Redis and Nginx

This setup provides a Docker-based environment for running PHP, MySQL, Redis, and Nginx.

## 🚀 Getting Started

### Prerequisites
Ensure you have the following tools installed on your system:

- Docker (20.10 or newer)
- Docker Compose (v2.0 or newer)

## 📄 Instructions

### 1. Configure Environment Variables
Copy the provided .env.example file to .env and adjust the variables as needed:
```bash
cp .env.example .env
```

### 2. Build and Start the Containers
Run the following command to build and start the containers in detached mode:

```bash
docker-compose up --build -d
```

### 3. Access the Application
Web Service (Nginx): http://localhost:9000

## Reference

- [How to implement a Load Balancer Using Nginx & Docker](https://dev.to/mazenr/how-to-implement-a-load-balancer-using-nginx-docker-4g73)

- [Load Balancing with Docker Compose and NGINX](https://medium.com/@aedemirsen/load-balancing-with-docker-compose-and-nginx-b9077696f624)

- [Using Redis with docker and docker-compose for local development a step-by-step tutorial](https://geshan.com.np/blog/2022/01/redis-docker)

- [Deploying a PHP Web App with Docker Compose, Nginx, and MariaDB](https://medium.com/@tech_18484/deploying-a-php-web-app-with-docker-compose-nginx-and-mariadb-d61a84239c0d)

- [Dockerize your PHP application with Nginx and PHP8-FPM](https://marc.it/dockerize-application-with-nginx-and-php8)