[API GATEWAY Youtube Video](https://youtu.be/MAlEaDL6P5A?si=vxnfylopodHY-OW0)
```
 Spring Web ---> Spring Reactive Web
 Gateway ------> Reactive Gateway
 Use **Spring Reactive Web** instead of the **Spring Web** dependency.
 Use **Reactive Gateway** instead of the **Gateway** dependency.
```

# Steps👇👇👇

## 1.Dependencies
- Spring Reactive Web
- Reactive Gateway
- Eureka Discovery Client
- Spring Boot DevTools 

## 2.main application
```
@SpringBootApplication
@EnableDiscoveryClient
public class ApiGatewayApplication {

	public static void main(String[] args) {
		SpringApplication.run(ApiGatewayApplication.class, args);
	}

}

```
## 3.application.properties  file
```
spring.application.name=API_GATEWAY
server.port=8765
spring.cloud.gateway.discovery.locator.enabled=true
```
