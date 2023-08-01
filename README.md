This is a [Laravel](https://laravel.com).

# Penggunaan

- build

      docker compose build

- create

      docker compose create

- start

      docker compose start

- one line => Builds, (re)creates, starts, and attaches to containers for a service.

      docker compose up
      docker compose up -d => --detach , -d		Detached mode: Run containers in the background

- cek image

      docker image ls
      atau menggunakan group
      docker image ls | grep nama => docker image ls | grep express-js

- cek container

      docker container ls -a
      atau
      docker compose ps

- stop

      docker compose down

- hapus image

      docker image rm IMAGE ID

- masuk ke dalam container

      docker exec -i -t laravel-docker /bin/bash

- list file

      ls -al

- create a new Laravel project

      composer create-project laravel/laravel .
      cd ..
      chown -R www-data:www-data .

- ganti permissions folder laravel-docker (optional)

      chown -R username:groupname . or chown -R username:groupname *
      example
      sudo chown -R san:san .

- copy file .htaccess to folder laravel-docker

      laravel is ready to use

- run VS Code with the root privileges

      sudo code . --user-data-dir='.' --no-sandbox

# Referensi

- laravel-docker : [click here](https://github.com/pitocms/laravel-docker)
