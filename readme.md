## Docker Commands

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

- ##### Run all docker-compose containers
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

- ##### Create swarm

  ```bash
  docker swarm init
  ```

- ##### Add worker to swarm

  **NOTE** - This command requires to SSH into the machine that we want to add to the swarm.

  ```bash
  docker swarm join --token <token> 192.168.65.3:2377
  ```

- ##### Add a service to the sawrm

  ```bash
  docker service create --replicas <number of replicas> --name nodeserver1 <image> ping docker.com
  ```

---

## Kubernetes Cluster

[minikube commands reference](https://minikube.sigs.k8s.io/docs/start/)

- ##### Start cluster

  ```bash
  minikube start
  ```

- ##### Deploy service to kubernetes cluster
  ```bash
  kubectl create deployment nodeapplication --image=node
  ```
