
# Spring Boot Web :


## What is Servlet and Tomcat? 

- A Servlet is basically a Java class that handles web requests and responses. 

- For example, when a client sends a request, the Servlet processes it and sends back the response.

- Tomcat, on the other hand, is a web server and servlet container. It provides the environment where Servlets run. 

- In simple terms: Servlets are the programs, and Tomcat is the container that executes those programs.

- In Spring Boot, we don’t directly work with raw Servlets, but internally it uses a DispatcherServlet, and Tomcat is embedded by default to handle requests.

- Servlet = program that handles requests
- Tomcat = server that runs those programs


## Servlet VS Tomcat :

| **Servlet**                                                    | **Tomcat**                                         |
| -------------------------------------------------------------- | -------------------------------------------------- |
| A **Java class** that handles requests and responses           | A **web server + servlet container**               |
| Part of **Java EE specification**                              | Implementation of **Servlet & JSP specification**  |
| Focus: **Business logic** (process request, generate response) | Focus: **Runtime environment** to execute Servlets |
| Example: `HttpServlet`, `DispatcherServlet`                    | Example: **Apache Tomcat server**                  |


## Need of MVC (Why we use it?) - 

- Separation of concerns → Each layer has a clear responsibility (UI, logic, data).

- Better maintainability → Easier to change UI without affecting business logic.

- Reusability → Same Model can be used with different Views.

- Testability → Business logic (Model) can be tested separately from UI.

- Scalability → Application can grow without becoming messy.



## REST APIs (HTTP Methods) - 
| **HTTP Method** | **Purpose**                             | **Description**                                        |
| --------------- | --------------------------------------- | ------------------------------------------------------ |
| **GET**         | Retrieve data (Read)                    | Fetch all resources or a specific one                  |
| **POST**        | Create new resource                     | Add a new resource (data sent in request body as JSON) |
| **PUT**         | Update existing resource (replace)      | Update full details of an existing resource            |
| **DELETE**      | Remove resource                         | Delete an existing resource                            |


