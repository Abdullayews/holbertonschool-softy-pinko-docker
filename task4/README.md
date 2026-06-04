<div align="center">

# 🎼 Softy Pinko — task 4: docker-compose

**Two `docker run` commands become one `docker-compose up`.**

[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)](https://nginx.org)
[![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Holberton](https://img.shields.io/badge/Holberton-Specialization-E44D26?style=flat-square)](https://www.holbertonschool.com)

</div>

---

## 📖 About this project

Multi-container apps deserve a single source of truth. This task introduces `docker-compose.yml` — services, build contexts, networks and ports declared once, started together, torn down together. The dev loop suddenly feels professional.

## 🎯 Concepts covered

- docker-compose: services, networks, build
- One command up, one command down
- Declarative over imperative

## 📂 Files

| File | What it does |
|---|---|
| [`back-end/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task4/back-end/Dockerfile) | API image |
| [`back-end/api.py`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task4/back-end/api.py) | Flask back-end |
| [`docker-compose.yml`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task4/docker-compose.yml) | Both services, declared once |
| [`front-end/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task4/front-end/Dockerfile) | Front-end image |
| [`front-end/softy-pinko-front-end.conf`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task4/front-end/softy-pinko-front-end.conf) | nginx static site config |

## ⚙️ Requirements

- 🐧 Ubuntu 20.04 LTS · Docker Engine + docker-compose
- 📄 Each task folder is self-contained — build from inside it

## 🚀 Try it yourself

```bash
cd task4
docker build -t softy-pinko .
docker run -p 80:80 --rm softy-pinko   # then compose, from task4 on
docker-compose up --build
```

---

✍️ **Muhəmməd Abdullayev** · [![GitHub](https://img.shields.io/badge/@Abdullayews-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Abdullayews) · one of the projects in **[holbertonschool-softy-pinko-docker](../README.md)**
