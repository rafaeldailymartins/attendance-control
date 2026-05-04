# Attendance Control
![Static Badge](https://img.shields.io/badge/docker-28.3-blue?logo=docker)

[🇺🇸 English](README.md) | [🇧🇷 Português](README.pt-br.md)

**Attendance Control** is a clock in and out system for organizational environments.

The system was initially designed as a college project to serve companies from [**Junior Enterprises Movement**](https://www.juniorenterprises.org/), which had specific attendance control needs. However, it is now being completely refactored to support any type of organization.

## 📋 Dependencies

- [Docker](https://www.docker.com/)

## 📦 Deployment
For production, first change the `ENV` environment variable in your `.env` file to:
```env
ENV=production
```

Then start the Docker container using only the `docker-compose.yml` file:

```console
$ docker compose -f docker-compose.yml up --build
```

## 👨‍💻 Author

Created and maintained by:

| [<img src="https://avatars.githubusercontent.com/u/162728324?v=4" width="60px;"/><br /><sub><b>Rafael Daily</b></sub>](https://github.com/rafaeldailymartins)
| :---: |