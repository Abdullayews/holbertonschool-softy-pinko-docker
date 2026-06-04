<div align="center">

# 🚪 Softy Pinko — task 5: add the reverse proxy

**Three containers: front-end, back-end, and an nginx proxy in front.**

[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)](https://nginx.org)
[![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Holberton](https://img.shields.io/badge/Holberton-Specialization-E44D26?style=flat-square)](https://www.holbertonschool.com)

</div>

---

## 📖 About this project

A third container joins: an nginx **reverse proxy** that fronts the whole stack. Requests hit the proxy, which routes static traffic to the front-end container and API calls to the back-end — the standard production topology, in miniature.

## 🎯 Concepts covered

- Reverse proxies — why production has one
- nginx proxy_pass routing
- Three-service topology

## 📂 Files

| File | What it does |
|---|---|
| [`back-end/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task5/back-end/Dockerfile) | API image |
| [`back-end/api.py`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task5/back-end/api.py) | Flask back-end |
| [`docker-compose.yml`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task5/docker-compose.yml) | Three services: proxy, back-end, front-end |
| [`front-end/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task5/front-end/Dockerfile) | Front-end image |
| [`front-end/softy-pinko-front-end.conf`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task5/front-end/softy-pinko-front-end.conf) | nginx static site config |
| [`proxy/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task5/proxy/Dockerfile) | The nginx reverse-proxy image |
| [`proxy/proxy.conf`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task5/proxy/proxy.conf) | Routing rules — static → front, /api → back |

## ⚙️ Requirements

- 🐧 Ubuntu 20.04 LTS · Docker Engine + docker-compose
- 📄 Each task folder is self-contained — build from inside it

## 🚀 Try it yourself

```bash
cd task5
docker build -t softy-pinko .
docker run -p 80:80 --rm softy-pinko   # then compose, from task4 on
docker-compose up --build
```

---

✍️ **Muhəmməd Abdullayev** · [![GitHub](https://img.shields.io/badge/@Abdullayews-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Abdullayews) · one of the projects in **[holbertonschool-softy-pinko-docker](../README.md)**
