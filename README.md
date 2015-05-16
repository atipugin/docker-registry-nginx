# docker-registry-nginx

Nginx image to protect your private Docker registry.

## Requirements

- docker
- docker-compose
- apache2-utils

## How to use

1. Clone the repo:

  ```shell
  git clone https://github.com/atipugin/docker-registry-nginx
  cd docker-registry-nginx
  ```

2. Add authorized users:

  ```shell
  htpasswd -c docker-registry.htpasswd <USER>
  ```

3. Configure registry container using env variables in ```docker-compose.yml``` file.

4. Run it:

  ```shell
  docker-compose up -d
  ```
