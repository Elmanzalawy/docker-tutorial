## Commands
[CLI Commands Reference](https://docs.docker.com/engine/reference/commandline/cli/)

- ##### Build Image
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