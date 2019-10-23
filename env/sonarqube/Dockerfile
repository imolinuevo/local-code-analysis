FROM sonarqube:latest

RUN curl "http://admin:admin@sonarqube:9000/api/webhooks/create" -X POST -d "name=jenkins&url=http://jenkins:8080/sonarqube-webhook/"