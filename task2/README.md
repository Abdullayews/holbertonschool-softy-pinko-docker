<div align="center">

# 🔀 Softy Pinko — task 2: two containers

**Front-end meets back-end — an nginx image and an API image, talking over a Docker network.**

[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)](https://nginx.org)
[![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Holberton](https://img.shields.io/badge/Holberton-Specialization-E44D26?style=flat-square)](https://www.holbertonschool.com)

</div>

---

## 📖 About this project

First multi-container setup: the static front-end is served by its own image (with an nginx config), the Flask API runs in another, and a user-defined Docker network lets them reach each other by name. The moment an 'architecture' appears.

## 🎯 Concepts covered

- User-defined Docker networks
- Container-to-container DNS names
- nginx as a static file server

## 📂 Files

| File | What it does |
|---|---|
| [`back-end/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task2/back-end/Dockerfile) | The API image |
| [`back-end/api.py`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task2/back-end/api.py) | Flask back-end |
| [`front-end/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task2/front-end/Dockerfile) | The static-site image |
| [`front-end/softy-pinko-front-end.conf`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task2/front-end/softy-pinko-front-end.conf) | nginx config serving the static front-end |

## ⚙️ Requirements

- 🐧 Ubuntu 20.04 LTS · Docker Engine + docker-compose
- 📄 Each task folder is self-contained — build from inside it

## 🚀 Try it yourself

```bash
cd task2
docker build -t softy-pinko .
docker run -p 80:80 --rm softy-pinko   # then compose, from task4 on
docker-compose up --build
```

---

✍️ **Muhəmməd Abdullayev** · [![GitHub](https://img.shields.io/badge/@Abdullayews-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Abdullayews) · one of the projects in **[holbertonschool-softy-pinko-docker](../README.md)**
