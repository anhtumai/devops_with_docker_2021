# Part 3

## Exercises

### 3.1

Deploy a blog-list-backend to Heroku using Github Actions: [Heroku link](https://blog-list-backend.herokuapp.com/api/users)

[Github Action workflow yml file](https://github.com/anhtumai/blog-list-backend/blob/containerize/.github/workflows/github-actions-demo.yml)

### 3.2

Bash script to clone, build and push Docker image to Docker Hub: [main.sh](./ex3/main.sh)

Docker file: [Dockerfile](./ex3/Dockerfile)

Inventory file format: [inventory](./ex3/inventory)

Usage:

```shell
$> sudo docker build . -t clone_push
$> sudo docker run -it -v /var/run/docker.sock:/var/run/docker.sock -v $PWD/inventory:/usr/src/inventory clone_push
```

__Notes__: git_url option only supports https link, not SSH link.

### 3.3

Frontend Dockerfile: [Dockerfile](./ex3/Dockerfile.front)

Backend Dockerfile: [Dockerfile](./ex3/Dockerfile.back)

```shell
# Working directory: ./ex3
$> docker-compose build
$> docker-compose up
```

![Screenshot](screenshots/ex3.png)

### 3.4

Frontend Dockerfile: [Dockerfile](./ex4/Dockerfile.front)

Backend Dockerfile: [Dockerfile](./ex4/Dockerfile.back)

```shell
# Working directory: ./ex4
$> docker-compose build
$> docker-compose up
```

![Screenshot](screenshots/ex4.png)

### 3.5

Frontend Dockerfile: [Dockerfile](./ex5/Dockerfile.front)

Backend Dockerfile: [Dockerfile](./ex5/Dockerfile.back)

```shell
# Working directory: ./ex5
$> docker-compose build
$> docker-compose up
```

![Screenshot](screenshots/ex5.png)

### 3.6

Frontend Dockerfile: [Dockerfile](./ex6/Dockerfile.front)

Backend Dockerfile: [Dockerfile](./ex6/Dockerfile.back)

```shell
# Working directory: ./ex6
$> docker-compose build
$> docker-compose up
```

![Screenshot](screenshots/ex6.png)

### Size check from 3.3 to 3.6

![Backend size check](screenshots/backendsizecheck.png)
![Frontend size check](screenshots/frontendsizecheck.png)

### 3.7

In this exercise, I optimize Dockerfiles for [app used in ex 2.11](../Part2/ex11).
Check [app description](../Part2/ReadMe.md#2.11)

Frontend Dockerfile: [Dockerfile](./ex7/Dockerfile.optimize.front)

Backend Dockerfile: [Dockerfile](./ex7/Dockerfile.optimize.back)

```shell
# Working directory: ./ex7
$> docker-compose build
$> docker-compose up
```

![Size comparison](screenshots/ex7-size-comparison.png)

As you can see, the sizes of of images used in ex 3.7 have dropped significantly
compared to ex 2.11.

