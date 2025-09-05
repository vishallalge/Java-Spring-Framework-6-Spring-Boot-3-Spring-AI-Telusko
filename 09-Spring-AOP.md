
# Spring AOP (Aspect-Oriented Programming):


## What is spring AOP ? 

- AOP (`Aspect-Oriented Programming`) in Spring is a programming paradigm that helps you separate cross-cutting concerns (common functionality that is used across multiple modules, but is not part of the main business logic).
- Instead of writing the same code (like logging, transactions, security checks) in every class/method, you write it once in an aspect and let Spring apply it automatically where needed.

## AOP Concepts : 
- Join Point (When):

    - Movie Analogy: A scene in the movie where the action happens.
    
    - AOP Definition: The specific point in the program's execution where the action (advice) will be applied. This could be method execution, exception handling, etc.

- Advice (What):
    
    - Movie Analogy: The action that happens at a particular scene; the plot twist.
    
    - AOP Definition: The code that is executed at a join point. It defines the "what" of the AOP implementation. Examples include before advice, after advice, and around advice.
    
- Aspect (Where - Conceptual):
    
    - Movie Analogy: The script of your movie; it defines what plots happen and where.

    - AOP Definition: A module that captures cross-cutting concerns (like logging, security) and applies them to other modules using pointcuts. It defines the "where" of the AOP implementation.

- Pointcut (Where - Operational):
    
    - Movie Analogy: The specific scenes (join points) where the plot twists (advice) occur, like a bookmark in your script.

    - AOP Definition: An expression that defines the join points where the advice should be applied. It's the operational definition of where the advice will be executed.

- Target Object (Whom):
    
    - Movie Analogy: The main character who experiences the plot twists (advice).
    
    - AOP Definition: The object that the advice is applied to. It's the object that the advice will affect.
     
- Weaving (How):
    
    - Movie Analogy: The director's job; how the script (aspect) is turned into a movie.
    
    - AOP Definition: The process of linking the aspect with the target object to create the advised object. This can happen at compile time, load time, or runtime.

- Proxy (The Double):
    
    - Movie Analogy: The stunt double; takes the hits and makes the main character look good.

    - AOP Definition: An object that is created to represent the target object after the advice has been applied. The proxy intercepts method calls to the target object and applies the advice before or after the actual method execution.
- Types of Advice (The Genre):
    
    - Movie Analogy: The genre of your movie; the style of how the plot twists (advice) will unfold.
    
    - AOP Definition: Different types of advice in Spring AOP:
    
    ○ Before: Executed before the method execution.
    
    ○ After: Executed after the method execution, regardless of the outcome.
    
    ○ After-returning: Executed after the method execution if it completes successfully.
    
    ○ After-throwing: Executed after the method execution if it throws an exception.

    ○ Around: Executes both before and after the method execution, giving you control over the entire method invocation.
