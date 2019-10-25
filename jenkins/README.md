# Container usage description

- How to build `custom-jenkins` image:

```
docker build -t custom-jenkins:latest .
```

- How to run `custom-jenkins` container:

```
docker run -d --name custom-jenkins -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home custom-jenkins:latest
```