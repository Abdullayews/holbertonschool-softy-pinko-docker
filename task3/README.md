<div align="center">

# 🔁 Softy Pinko — task 3: copying code in

**Same two containers — now with the code baked in properly.**

[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)](https://nginx.org)
[![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Holberton](https://img.shields.io/badge/Holberton-Specialization-E44D26?style=flat-square)](https://www.holbertonschool.com)

</div>

---

## 📖 About this project

Task 3 refines the multi-container pattern: `COPY`ing application code into the images and running it on start, so containers are self-contained rather than depending on host files. The front-end config and the API finally ship as real, portable images.

## 🎯 Concepts covered

- COPY vs volumes — baking code into images
- Self-contained, portable images
- Container start commands

## 📂 Files

| File | What it does |
|---|---|
| [`back-end/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task3/back-end/Dockerfile) | API image with code copied in |
| [`back-end/api.py`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task3/back-end/api.py) | Flask back-end |
| [`front-end/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task3/front-end/Dockerfile) | Front-end image, self-contained |
| [`front-end/softy-pinko-front-end.conf`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task3/front-end/softy-pinko-front-end.conf) | nginx static site config |

## ⚙️ Requirements

- 🐧 Ubuntu 20.04 LTS · Docker Engine + docker-compose
- 📄 Each task folder is self-contained — build from inside it

## 🚀 Try it yourself

```bash
cd task3
docker build -t softy-pinko .
docker run -p 80:80 --rm softy-pinko   # then compose, from task4 on
docker-compose up --build
```

---

✍️ **Muhəmməd Abdullayev** · [![GitHub](https://img.shields.io/badge/@Abdullayews-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Abdullayews) · one of the projects in **[holbertonschool-softy-pinko-docker](../README.md)**
