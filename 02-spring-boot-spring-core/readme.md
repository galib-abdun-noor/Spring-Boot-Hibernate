# Dependency Injection
Spring Dependency Injection is a design pattern and a core feature of the Spring Framework that enables the management of objects and their dependencies.
- DI allows for loose coupling between classes by removing the responsibility of creating and managing dependencies from the classes themselves.
- The core principle of DI is that the dependencies of a class are injected into it from an external source, rather than being created or instantiated within the class.
- Dependency Injection can be achieved in Spring through constructor injection, setter injection, or field injection.

# Constructor Injection
In constructor injection, dependencies are provided to a class through its constructor.

# Setter Injection
In setter injection, dependencies are provided to a class through setter methods.

# Field Injection 
In field injection, dependencies are directly injected into class fields without using constructor or setter methods.

# AutoWiring
Spring autowiring is a feature of the Spring Framework that allows the automatic injection of dependencies into a Spring-managed object. Instead of manually configuring dependencies, Spring autowiring enables developers to simply declare a dependency as a field or constructor parameter of a Spring-managed object and let Spring automatically inject the appropriate dependency at runtime.

# @GetMapping annotation
@GetMapping is an annotation in Spring Framework used to map HTTP GET requests to a specific method in a controller class.

When a user sends a GET request to a specific URL, the @GetMapping annotation can be used to map that request to a method in a Spring MVC controller. The method is then executed and its return value is used to generate the response that is sent back to the user.

# @Component annotation
The @Component annotation is used to mark a Java class as a Spring bean. When a class is annotated with @Component, Spring will automatically detect and instantiate it as a bean in the application context during runtime.


