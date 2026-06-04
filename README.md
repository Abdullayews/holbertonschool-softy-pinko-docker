<div align="center">

# 🐳 Softy Pinko — One App, Seven Steps to a Load-Balanced Cluster

**Containerization from first principles: one Dockerfile → two containers → compose → reverse proxy → load balancing.**

[![Docker](https://img.shields.io/badge/Docker-Engine-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com)
[![docker-compose](https://img.shields.io/badge/docker-compose-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docs.docker.com/compose/)
[![nginx](https://img.shields.io/badge/nginx-proxy%20%20%26%20%20static-009639?style=for-the-badge&logo=nginx&logoColor=white)](https://nginx.org)
[![Flask](https://img.shields.io/badge/Flask-API-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Holberton](https://img.shields.io/badge/Holberton-Specialization-E44D26?style=for-the-badge)](https://www.holbertonschool.com)

</div>

---

## 🧭 About this repository

The Softy Pinko project takes one tiny app — a static front-end and a
Flask API — and containers it **seven times over**, each task adding the
next production concept:

1. **task0** — the first Dockerfile, the build-run-verify loop
2. **task1** — the Flask API gets its own image
3. **task2** — front-end + back-end containers talking over a Docker network
4. **task3** — code baked properly into self-contained images
5. **task4** — `docker-compose` replaces the manual `docker run` choreography
6. **task5** — an nginx **reverse proxy** fronts the whole stack
7. **task6** — the API scales to two servers behind a **load balancer**

By the end, a miniature production topology runs from a single
`docker-compose up` — with redundancy you can test by killing a container.

## 📚 The tasks

| Project | What it covers |
|---|---|
| [`task0/`](task0/README.md) | The first image — FROM, COPY, CMD, run |
| [`task1/`](task1/README.md) | The API image — Flask answering JSON from a container |
| [`task2/`](task2/README.md) | Two containers — nginx static front-end + Flask API, networked |
| [`task3/`](task3/README.md) | Self-contained images — code copied in, portable |
| [`task4/`](task4/README.md) | docker-compose — the whole stack, declared once |
| [`task5/`](task5/README.md) | The reverse proxy — nginx routing static and /api traffic |
| [`task6/`](task6/README.md) | Load balancing — two API servers, one proxy, zero SPOFs |

## 🛠️ Environment

- Ubuntu 20.04 LTS · Docker Engine + docker-compose
- Each task folder is self-contained — `cd` in and build

## 🚀 Run the finale

```bash
git clone https://github.com/Abdullayews/holbertonschool-softy-pinko-docker.git
cd holbertonschool-softy-pinko-docker/task6
docker-compose up --build      # proxy + 2 APIs + front-end
```


## 👤 Author

**Muhəmməd Abdullayev** — Computer Engineering student · Qarabağ University & Holberton School

<p>
<a href="https://github.com/Abdullayews"><img src="https://img.shields.io/badge/GitHub-@Abdullayews-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"></a>
<a href="https://t.me/arasss08"><img src="https://img.shields.io/badge/Telegram-@arasss08-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram"></a>
<a href="mailto:08abdullayevv@gmail.com"><img src="https://img.shields.io/badge/Email-08abdullayevv@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
</p>

> 🇦🇿 Part of my Holberton School journey — Foundations & Specializations, one repo at a time.

