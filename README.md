# Custom local environment for static code analysis

A self communicated cluster for local code analysis using dockerized jenkins and sonarqube.
In order to run this project you only need to have installed `docker` and `docker-compose`.
Just run the following command and wait for the containers to be ready (first time with `--build` flag):

```
docker-compose up -d
```

> This project uses the default ports for *jenkins* (`8080`) and *sonarqube* (`9000`) so make sure they are available in your `localhost`