
# Microservices :


## What is Microservices ? 

- Microservices is an architectural style for building applications. Instead of creating one big monolithic application, microservices break it down into small, independent services that each handle a specific business function.


## Why Microservices ? 
- In software development, we often start with a monolithic approach - one large application that handles everything. 
- However, as applications grow, we can face challenges with scaling, maintenance, and deployment. This is where microservices come in. 



## Microservices Approach 

- Split the application into smaller, independent services  
- Each service runs independently and has its own responsibility  
- Services communicate with each other when needed


## Challenges in Microservices 
- Scaling: We can now scale services independently based on demand (unlike monoliths where we scale the entire application)  
- Multiple Instances: We might have multiple instances of each service with different IP addresses  
- Service Discovery: How does one service find another?  
- Load Balancing: How do we distribute traffic across multiple instances of the same service?


## Client Access and API Gateway 
- Another challenge is how clients interact with our services: 
    - Clients shouldn't need to know about all the different services and their URLs  
    - Clients shouldn't have to remember multiple endpoints

- Solution: API Gateway 
    - Acts as a single entry point for all client requests  
    - Routes requests to the appropriate service  
    - Simplifies the client experience 


## Service Registry 
- When we have many services (possibly 10 or more: 
    - Services need to locate each other  
    - Remembering IP addresses isn't practical  
    - Services constantly change (new instances added, old ones removed) 

- Solution: Service Registry 
    - Services register themselves when they start up  
    - Services can look up other services by name  
    - No need to hardcode IP addresses


## Fault Tolerance 
- What happens when a service fails?

- Solutions: 

    - Circuit Breakers: Detect failures and prevent cascading failures  
    - Fail Fast: Quickly identify when a service is unavailable  
    - Fallbacks: Provide alternative responses when a service is down  
    - Proper Error Handling: Communicate issues to clients appropriately
