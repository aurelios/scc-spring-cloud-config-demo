# scc-limits-service
This project shows how to connect the microservice **scc-limits-service** with the **Spring Cloud Configuration Server([scc-config-server](scc-config-server))** to fetch the configuration file automaticaly.


## 🚀 How to run ?
1 - Run  [scc-config-server](scc-config-server)

2 - Run the application
```shell script
./mvnw spring-boot:run
```
The endpoint bellow returns the properties `limits-service.minimum` and `limits-service.maximum` configured on application.properties configuration file.

http://localhost:8080/limits

We can notice that the properties returned are from the qa configuration file of the repository loaded by spring cloud configuration server([scc-config-server](scc-config-server)) and not from application.properties of the project.

