# spring-cloud-eureka-hystrix

## Projects

* Spring cloud config - provides server and client support for external configuration. It is a centralized configuration that can be used in distributed systems. 

![image](https://user-images.githubusercontent.com/15162574/113487137-2c192d80-94ae-11eb-9c32-390a47556979.png)


* Spring Cloud Netflix - 

    **Eureka Server** is the service discovery pattern implementation. Microservices instances can register and be discovered by other microservices. Is also provides a way to add multiple Eureka Servers that can register between them to provide the necessary redundancy. It provides the @EnableEurekaServer that enables an embedded service discovery.
    
    ![image](https://user-images.githubusercontent.com/15162574/113487260-050f2b80-94af-11eb-9498-c5a96dcd9718.png)


    **Eureka Client provides** a discoverable pattern that registers Eureka Server and offers useful information, such as URL and ports. It provides the @EnableDiscoveryClient annotation that registers the microservice.

    **Circuit Breaker** is a pattern that offers a fault-tolerant scenario to your applications. It provides the @EnableCircuitBreaker and @HistirixCommand annotations, which are simple decorators with the functionality to create fault-tolerant microservices.
    
    ![image](https://user-images.githubusercontent.com/15162574/113487284-2112cd00-94af-11eb-80a4-da3b9af94ec9.png)


    **Eureka Ribbon** is an implementation of the client-side load-balancing patterns. It provides the @LoadBalanced annotation that normally goes in the RestTemplate instance; this creates the client load-balancing required for multiple microservices registered in Eureka Server.

    **Netflix Zuul** is an implementation of routing and filter patterns for creating proxies.

    **External Configuration** provides a way to communicate directly with Netflix Archaius to provide a Spring environment similar to Spring Cloud Config Server.

## Endpoints:

### Hystrix:

http://localhost:8083/hystrix

http://localhost:8083/actuator/hystrix.stream


### Eureka: 

http://localhost:8761/


### H2-console:

http://localhost:8181/h2-console



## Properties:

### Movie:

http://localhost:8888/movies/default


### Movie-Web:

http://localhost:8888/movies-web/default
