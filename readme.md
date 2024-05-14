## Commands

[CLI Commands Reference](https://docs.docker.com/engine/reference/commandline/cli/)

- ##### Build image

  ```bash
  docker build -t algofields/frontend .
  ```

- ##### List images

  ```bash
  docker images
  ```

- ##### Create container
    ```bash
    docker run -p 3000:3000 algofields/frontend
    ```

- ##### List active containers
    ```bash
    docker ps
    ```

- ##### Build docker-compose containers

  ```bash
  docker-compose build
  ```

- ##### Run docker-compose containers
  ```bash
  docker-compose up
  ```
  Or use the `-d` parameter to specify specific containers to run
  ```bash
  docker-compose up -d mongo
  ```
- ##### Stop all containers

  ```bash
  docker-compose stop
  ```

- ##### View container logs
  ```bash
  docker-compose logs <container-id>
  ```
