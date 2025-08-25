
# Spring Boot :


## What is Spring? 

- Spring is a Java framework that helps you build applications by managing objects for you and making it easier to connect different parts of your code without writing a lot of setup code.


## What is IoC and DI? 

### IoC (Inversion of Control) - 
- The control of creating and managing objects is handed over to the Spring framework, instead of you manually creating them with new.
- Why? : It decouples the code so you can easily swap implementations, test, and manage lifecycle automatically.

### DI (Dependency Injection) - 
- A way to implement IoC — instead of you creating dependencies, they are injected into your class by Spring.

- IoC is the principle.

- DI is one way Spring achieves IoC.


## Difference between Spring and Spring boot :
| Feature                   | **Spring**                                                         | **Spring Boot**                                        |
| ------------------------- | ------------------------------------------------------------------ | ------------------------------------------------------ |
| **Setup**                 | Needs manual XML or Java configuration for beans, DataSource, etc. | Auto-configuration — minimal setup                     |
| **Dependency Management** | You add multiple dependencies manually                             | Starter dependencies (e.g., `spring-boot-starter-web`) |
| **Application Startup**   | No embedded server by default                                      | Embedded Tomcat/Jetty — run as a standalone Java app   |
| **Real-world effect**     | Slower project setup, more boilerplate                             | Faster development, production-ready defaults          |
| **Example analogy**       | Buying raw materials and building a car from scratch               | Getting a pre-built car, just add your luggage and go  |





## What is Component Container?
- A component container is basically the “brain” that creates, stores, and manages all the objects (beans) your application needs.

- You mark classes with `@Component` 
- Spring scans your project, finds these classes, creates their objects, and keeps them inside the container.

- Whenever you need one, Spring gives it to you — you don’t `new` it yourself.


## How Spring decide which class object we have to create or not ?
- When your app starts, Spring scans specific packages for classes annotated with :

`@Component`
`@Service`
`@Repository`
`@Controller`

- Only these marked classes are considered for bean creation (unless you define beans manually).

## `@Component`
- Role : Tells Spring “Hey, this class is a bean, manage it for me."
- Marks a class as a Spring-managed component.

- Spring’s component scanning will detect it and create an object (bean) at startup.

- The bean is stored in the Spring IoC container for later use.




## `@Autowired`
- Role : Tells Spring “Inject the required dependency here.”

- Looks for a bean in the container that matches the required type.

- Injects it into the variable, constructor, or setter method.

- If multiple beans match, you must specify which one (`@Qualifier` or `@Primary`).




## What is Java based configuration? 

- Java-based configuration in Spring means defining beans and wiring dependencies using Java classes + annotations instead of XML.


## Different Layers in Spring Boot?
- In Spring Boot, the common layers are - 

Controller → Service → Repository → Model
- where each has a separate responsibility -

API handling → business logic → database → data objects 








### Work and How to use ? 
| **Layer**                                  | **Function / Responsibility**                                                   | **How we use it in Spring Boot**                                                                                |
| ------------------------------------------ | ------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| **Controller (Presentation Layer)**        | Handles **HTTP requests & responses**, exposes REST APIs                        | Annotate class with `@RestController` or `@Controller`; define methods with `@GetMapping`, `@PostMapping`, etc. |
| **Service (Business Logic Layer)**         | Contains **business logic**; acts as a bridge between Controller and Repository | Annotate class with `@Service`; call repository methods here and apply logic                                    |
| **Repository (Data Access Layer / DAO)**   | Manages **database operations** (CRUD)                                          | Create an interface, extend `JpaRepository` or `CrudRepository`, annotate with `@Repository`                    |
| **Model / Entity (Domain Layer)**          | Represents **data objects / DB tables**                                         | Annotate class with `@Entity`, `@Table`, and fields with `@Id`, `@Column`                                       |

