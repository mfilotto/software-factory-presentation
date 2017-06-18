# software-factory-presentation demo clipboard

## Demo dockerize Github Project

- Import project : https://github.com/dockersamples/docker-swarm-visualizer.git to speed-test/docker-swarm-visualizer
- Create `.gitlab-ci.yml` file
```
dockerize:
  script: dockerize
  tags:
  - sln
```
  
- Run docker
```
docker login 
docker run -it -d -p 8080:8080 -v /var/run/docker.sock:/var/run/docker.sock speed-test/docker-swarm-visualizer
```
