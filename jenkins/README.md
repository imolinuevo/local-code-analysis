# TODO

`docker build -t custom-jenkins:latest .`

`docker run -d --name custom-jenkins -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home custom-jenkins:latest`