# TODO

`docker build -t custom-sonar:latest .`

`docker run -d --name custom-sonar -p 9000:9000 custom-sonar:latest`

`curl "http://admin:admin@localhost:9000/api/webhooks/create" -X POST -d "name=jenkins&url=http://localhost:8080/sonarqube-webhook/"`