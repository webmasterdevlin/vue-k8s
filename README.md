#### Dockerizing a Vuejs app

Login to Docker Hub

```zsh
$ docker login
```

create a Vuejs container

```zsh
$ docker build -t {yourDockerUsername}/vuejs-app:1.0.0 .
```

Test the Vuejs container by running it. It should be visible at localhost:8080

```zsh
$ docker run -p 8080:80 {yourDockerUsername}/vuejs-app:1.0.0
```

Push the container to your Docker Hub account repository

```zsh
$ docker push {yourDockerUsername}/vuejs-app:1.0.0
```
