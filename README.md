# springdemo
Spring integration with docker

Tutorial for Spring
https://spring.io/guides/gs/rest-service/

1.build docker image:

mvn install dockerfile:build

2. Create Container:
docker run -p 8080:8080 -t demo/springdemo:latest
image name : demo/springdemo:latest (this can be replaced in pom file)
Container name : thirsty_poincare (created by default and can be changed)

customized docker Container name :
docker run -d --name springdemo -p 8080:8080 -t demo/springdemo:latest

3. Handling Containers:

to start:
docker start thirsty_poincare
to stop:
docker stop thirsty_poincare

Container name : thirsty_poincare (created by default and can be changed)

4. Check Localhost
http://localhost:8080/
