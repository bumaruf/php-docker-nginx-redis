<h1 align="center">Docker-compose Php8, Nginx, Redis, MySQL and PHPMyAdmin</h1>

<!-- Tags -->

<p align="center">
  <img alt="License" src="https://img.shields.io/static/v1?label=license&message=MIT&color=ffffff&labelColor=000000">
  <img alt="Nginx" src="https://img.shields.io/static/v1?label=Nginx&message=latest&color=ffffff&labelColor=000000">
  <img alt="PHP" src="https://img.shields.io/static/v1?label=PHP&message=8.X&color=ffffff&labelColor=000000">
  <img alt="Redis" src="https://img.shields.io/static/v1?label=Redis&message=latest&color=ffffff&labelColor=000000">
  <img alt="MySQL" src="https://img.shields.io/static/v1?label=MySQL&message=5.7.24&color=ffffff&labelColor=000000">
  <img alt="PHPMyAdmin" src="https://img.shields.io/static/v1?label=PHPMyAdmin&message=latest&color=ffffff&labelColor=000000">
</p>
<!-- Body -->

## 🚀 How to run

Clone the repository in your computer.

```bash
$ git clone https://github.com/bumaruf/php-docker-nginx-redis
$ cd php-docker-nginx-redis
```

Run docker-compose file

```bash
$ docker-compose up -d
```

## ⚙️ Configuration

Don't forget to configure the environment variables file so that the project works correctly.

Duplicate the file `.env.example` changing name to `.env` and then fill the variables.

```bash
$ cp .env.example .env
```

Example config
```py
# Redis configuration
REDIS_PORT=6379
REDIS_PASSWORD=difficultpassword

# PostgreSQL configuration
POSTGRESQL_USER=root
POSTGRESQL_PASSWORD=difficultpassword
POSTGRESQL_DATABASE=default_db

# Mysql configuration
MYSQL_USER=test
MYSQL_DATABASE=database
MYSQL_PASSWORD=difficultpassword
```

## 📄 License

This project is under an MIT license. See [LICENSE](LICENSE.md) for more details.

---

<!-- Footer -->
Developed by [Otávio Bumaruf](https://github.com/bumaruf).
