# Container usage description

- How to build `custom-sonar` image:

```
docker build -t custom-sonar:latest .
```

- How to run `custom-sonar` container:

```
docker run -d --name custom-sonar -p 9000:9000 \
-v sonar_home_conf:/opt/sonarqube/conf \
-v sonar_home_extensions:/opt/sonarqube/extensions \
-v sonar_home_logs:/opt/sonarqube/logs \
-v sonar_home_data:/opt/sonarqube/data \
custom-sonar:latest
```