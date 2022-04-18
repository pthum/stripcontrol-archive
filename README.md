# stripcontrol-archive
This repository contains old and unmaintained implementations of the "stripcontrol" light system.
There's neither a guarantee that the parts will actually work, nor do they get updates. This is just an archive to keep the other repositories clean.


## Contained old implementations
- [Old frontend implementation](stripcontrol-frontend/README.md)
- [Old spring-boot implementation](stripcontrol-springbackend/README.md)
- [Old quarkus HTTP-API implementation](stripcontrol-quarkusbackend/README.md)

### stripcontrol-frontend
Includes the frontend, which is a VueJS application. The backend applications copy the resources from this project and serve them during runtime.

### stripcontrol-springbackend
An implementation of the backend part based on the Spring Boot framework.

### stripcontrol-quarkusbackend
An implementation of the first backend part based on the Quarkus framework. This implementation handles the database interaction and sends MQTT messages (and delivers the frontend).
There's an [alternative implementation](https://github.com/pthum/stripcontrol-golang) available written in golang.
