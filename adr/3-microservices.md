# Microservices Architecture

## Status

Accepted

## Context

![image](https://github.com/aimanyusra/roadwarriors/assets/27656498/f243dad2-c64b-44c5-8fa5-f140f55ba2e6)

## Decision Drivers

### Scalability

Various services grow at varying rates, making it challenging to anticipate the extent of their scalability. Microservice architecture allows for a responsive scaling of services.

### Interoperability

One of our system’s feature is to be able to seamlessly integrate with external parties such as travel agencies. Microservices allow us to perform integration and deployment continuously according to the needs of external parties without impacting the other services.

### Availability

Users must be able to access the system at all times. Ensuring high availability is essential to provide a reliable user experience and minimize downtime. Services can be designed to gracefully handle errors, recover from failures, and not propagate failures to other parts of the system.

### Responsiveness

To ensures that users do not experience significant delays or unresponsiveness when interacting with the software, we can scale the service that owns the feature accordingly. This minimizes latency and jobs that can be done asynchronously can be assigned to other service to ensure resources are used according to the prioritization. 

# Consequences

### **Increased Complexity**

Microservices introduce a higher degree of architectural complexity compared to monolithic applications. Managing numerous services, coordinating their interactions, and ensuring data consistency across them can be challenging. Ensuring that services work together seamlessly may require implementing coordination mechanisms such as service discovery, load balancing, and message queues.

### Maintainability

Given the distributed nature and complexity of microservices, maintaining such systems requires careful planning and practices. As more components are introduced in microservices architecture, there are more things to take care of such as versioning, service decoupling, transaction control between services and etc.

### Higher cost

While microservices benefits us with scalability and performance, it also comes with a higher operating cost compared to a monolith architecture.
