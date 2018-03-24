# docker-lamp
Basic LAMP development environment with Docker


## how to use it
1. Clone this repo
2. Set correct UID in `Dockerfile`. Bash command `id -u $USER` will show you your user ID on host. Set it for __www-data__ user in container and your container will be able to manage files owned by you.
3. `docker-compose up -d`
4. Copy your PHP application files to `app/` directory.
5. Develop. Your application is accessable through http://localhost:8080/ , And you can access your MYSQL database on port 8081
