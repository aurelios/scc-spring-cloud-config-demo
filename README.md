# scc-spring-cloud-config-demo
This repository uses git subtree to centralize multiple microservices projects using Spring Cloud Framework to solve the Challenges of Microservices Achitecture.

# Challenges of Microservices

### Configuration Management
Due to the large number of microservices how to manage multiple configurations from different environments ?

* Spring Cloud Config Server ([scc-config-server](scc-config-server))

### Dynamic Scale Up and Scale Down
How to distribute the loads of the microservice when a instance goes up or down ?
* Naming Server(Eureka)
* Ribbon(Client Side Load Balancing)
* Feign(Easier REST Clients)

### Visibility
* Zipking
* Netflix API Gateway

### Fault Tolerance
* Hystrix

### Zero Downtime Deployments


## Git Subtree commands
How to use Git subtree ?

1 - To Create the subtree project

`git subtree add --prefix scc-config-server https://github.com/aurelios/scc-config-server.git main --squash`

2 - To pull the commits from the main project

`git subtree pull --prefix scc-config-server https://github.com/aurelios/scc-config-server.git main --squash`

3 - To push the commits of the subtree into the main project

`git subtree push --prefix scc-config-server https://github.com/aurelios/scc-config-server.git main`

