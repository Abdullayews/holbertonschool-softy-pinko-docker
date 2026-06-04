<div align="center">

# 📦 Softy Pinko — task 0: the first image

**A Dockerfile, an Ubuntu base, and the hello-world of containerization.**

[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)](https://nginx.org)
[![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Holberton](https://img.shields.io/badge/Holberton-Specialization-E44D26?style=flat-square)](https://www.holbertonschool.com)

</div>

---

## 📖 About this project

The opening move of the Softy Pinko Docker series: write a `Dockerfile` that pulls a base image, copies a tiny app in, and runs it. Nothing fancy — just the build → run → verify loop that everything else in this repo builds on.

## 🎯 Concepts covered

- Dockerfile basics: FROM, COPY, CMD
- docker build / docker run / docker exec
- Images vs containers

## 📂 Files

| File | What it does |
|---|---|
| [`Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task0/Dockerfile) | The first Dockerfile — base image, app copy, run |

## ⚙️ Requirements

- 🐧 Ubuntu 20.04 LTS · Docker Engine + docker-compose
- 📄 Each task folder is self-contained — build from inside it

## 🚀 Try it yourself

```bash
cd task0
docker build -t softy-pinko .
docker run -p 80:80 --rm softy-pinko   # then compose, from task4 on
docker-compose up --build
```

---

✍️ **Muhəmməd Abdullayev** · [![GitHub](https://img.shields.io/badge/@Abdullayews-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Abdullayews) · one of the projects in **[holbertonschool-softy-pinko-docker](../README.md)**
