<div align="center">

# ⚖️ Softy Pinko — task 6: load balancing

**Scale the back-end to two servers and let the proxy balance them.**

[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)](https://nginx.org)
[![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Holberton](https://img.shields.io/badge/Holberton-Specialization-E44D26?style=flat-square)](https://www.holbertonschool.com)

</div>

---

## 📖 About this project

The finale: two identical API servers behind the reverse proxy, with nginx distributing requests between them. One server dies? The other answers. Add `2-api-servers.txt` — the notes on running both back-ends — and the mini stack is now redundant.

## 🎯 Concepts covered

- Load balancing with nginx upstream
- Horizontal scaling of a service
- Redundancy — killing one server, surviving

## 📂 Files

| File | What it does |
|---|---|
| [`2-api-servers.txt`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task6/2-api-servers.txt) | Notes on running the second API server |
| [`back-end/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task6/back-end/Dockerfile) | API image (runs twice) |
| [`back-end/api.py`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task6/back-end/api.py) | Flask back-end |
| [`docker-compose.yml`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task6/docker-compose.yml) | Two back-ends + proxy + front-end |
| [`front-end/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task6/front-end/Dockerfile) | Front-end image |
| [`front-end/softy-pinko-front-end.conf`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task6/front-end/softy-pinko-front-end.conf) | nginx static site config |
| [`proxy/Dockerfile`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task6/proxy/Dockerfile) | The load-balancing proxy image |
| [`proxy/proxy.conf`](https://github.com/Abdullayews/holbertonschool-softy-pinko-docker/tree/main/task6/proxy/proxy.conf) | upstream block balancing the two APIs |

## ⚙️ Requirements

- 🐧 Ubuntu 20.04 LTS · Docker Engine + docker-compose
- 📄 Each task folder is self-contained — build from inside it

## 🚀 Try it yourself

```bash
cd task6
docker build -t softy-pinko .
docker run -p 80:80 --rm softy-pinko   # then compose, from task4 on
docker-compose up --build
```

---

✍️ **Muhəmməd Abdullayev** · [![GitHub](https://img.shields.io/badge/@Abdullayews-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Abdullayews) · one of the projects in **[holbertonschool-softy-pinko-docker](../README.md)**
