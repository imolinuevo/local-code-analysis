# TODO

`docker build -t custom-sonar:latest .`

`
docker run -d --name custom-sonar -p 9000:9000 \
-v sonar_home_conf:/opt/sonarqube/conf \
-v sonar_home_extensions:/opt/sonarqube/extensions \
-v sonar_home_logs:/opt/sonarqube/logs \
-v sonar_home_data:/opt/sonarqube/data \
custom-sonar:latest
`