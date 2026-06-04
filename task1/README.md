<div align="center">

# 🧴 Softy Pinko — task 1: the API image

**Flask in a container: an api.py that answers in JSON.**

[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)](https://nginx.org)
[![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Holberton](https://img.shields.io/badge/Holberton-Specialization-E44D26?style=flat-square)](https://www.holbertonschool.com)

</div>

---

## 📖 About this project

The back-end is born: a small Flask `api.py` gets its own Dockerfile — Python base, dependencies, port exposure. Now the app answers HTTP from inside a container, isolated from the host.

## 🎯 Concepts covered

- Python base images & pip installs
- EXPOSE and container ports
- Containerized HTTP services

## 📂 Files

| File | What it does |
|---|---|
| [`Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task1/Dockerfile) | Python base + Flask app baked in |
| [`api.py`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task1/api.py) | The Flask API returning its JSON payload |

## ⚙️ Requirements

- 🐧 Ubuntu 20.04 LTS · Docker Engine + docker-compose
- 📄 Each task folder is self-contained — build from inside it

## 🚀 Try it yourself

```bash
cd task1
docker build -t softy-pinko .
docker run -p 80:80 --rm softy-pinko   # then compose, from task4 on
docker-compose up --build
```

---

✍️ **Muhəmməd Abdullayev** · [![GitHub](https://img.shields.io/badge/@Abdullayews-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Abdullayews) · one of the projects in **[holbertonschool-softy-pinko-docker](../README.md)**
