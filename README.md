# eagle-eye
Eagle Eye license managing application.

### Microservices
- [licesing-service](https://github.com/cyberalexander/ea-licensing-service)
- [configuration-service](https://github.com/cyberalexander/ea-config-service)


### Useful links
- [GitHub readme basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

### Useful commands
- If you want to compile the source code and build the Docker image, you need to run the following at the root of project directory:
```bash
mvn clean package docker:build
```
- If you want to look at the output for a Docker-based service, start your docker-compose command in detached mode with the '–d' option.
```bash
docker-compose -f docker/common/docker-compose.yml up –d
```
- Then you can look at the specific logs for that container by issuing the docker-compose command with the logs option
```bash
docker-compose -f docker/common/docker-compose.yml logs -f ea-licensing-service
```

