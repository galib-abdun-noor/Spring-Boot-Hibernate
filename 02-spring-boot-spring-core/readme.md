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

# @GetMapping Annotation
@GetMapping is an annotation in Spring Framework used to map HTTP GET requests to a specific method in a controller class.

When a user sends a GET request to a specific URL, the @GetMapping annotation can be used to map that request to a method in a Spring MVC controller. The method is then executed and its return value is used to generate the response that is sent back to the user.

# @Component Annotation
The @Component annotation is used to mark a Java class as a Spring bean. When a class is annotated with @Component, Spring will automatically detect and instantiate it as a bean in the application context during runtime.

# @Qualifier Annotation
The @Qualifier annotation is used to disambiguate between beans that have the same type when multiple beans of that type are present in the application context.

# @Primary Annotation
When you have multiple beans of the same type and you want to specify which bean should be given preference for autowiring, you can use the @Primary annotation. By marking a bean with @Primary, you indicate that it is the primary bean to be used when autowiring that type.

# Lazy Initialization
Lazy initialization in Spring Boot refers to the delayed creation and initialization of beans until they are actually needed. By default, Spring beans are eagerly initialized during the application startup process. However, with lazy initialization, beans are created only when they are first requested, potentially improving performance and reducing memory consumption.
- Definition: Lazy initialization is a feature that allows beans to be created and initialized on-demand, rather than during application startup.
- @Lazy Annotation: To enable lazy initialization for a specific bean, you can use the @Lazy annotation on the bean declaration or configuration method. This annotation tells Spring to create a proxy object instead of the actual bean instance.

# Singleton
In Spring Boot, the Singleton pattern refers to the default scope of a bean, which means that only one instance of the bean is created and shared across the entire application context.

When you define a bean in a Spring Boot application without explicitly specifying its scope, it is considered to have the singleton scope by default. This means that Spring creates a single instance of that bean and uses it whenever the bean is requested throughout the application

# Bean Scopes
In Spring Boot, the bean scope refers to the lifecycle and visibility of a bean within the Spring IoC (Inversion of Control) container. The Spring IoC container is responsible for creating and managing instances of beans based on their scopes.

The following are the different bean scopes available in Spring Boot:

1. Singleton (default scope): In this scope, a single instance of the bean is created for the entire application context. The same instance is returned whenever the bean is requested. Singleton beans are shared across multiple requests and threads.
2. Prototype: In this scope, a new instance of the bean is created every time it is requested. Prototype beans are not shared, and each request for the bean results in a new instance being created.
3. Request: This scope is applicable in web-aware Spring applications. In this scope, a new instance of the bean is created for each HTTP request. The bean is available only within the scope of that specific request.
4. Session: This scope is also applicable in web-aware Spring applications. In this scope, a new instance of the bean is created for each HTTP session. The bean is available throughout the duration of the session.
5. Application: This scope is specific to web-aware Spring applications. In this scope, a single instance of the bean is created for the entire web application context. The bean is available to all sessions and requests within the application.
6. WebSocket: This scope is specific to web-aware Spring applications that use WebSocket. In this scope, a single instance of the bean is created for each WebSocket connection. The bean is available only within the scope of that specific WebSocket connection.


