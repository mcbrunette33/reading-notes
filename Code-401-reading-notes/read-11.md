## Read 11

- A common feature of developing web applications is coding a change, restarting your application, and refreshing the browser to view the change. This entire process can eat up a lot of time. To speed up this refresh cycle, Spring Boot offers with a handy module known as spring-boot-devtools. Spring Boot Devtools:

- Enables hot swapping.

- Switches template engines to disable caching.

- Enables LiveReload to automatically refresh the browser.

- Other reasonable defaults based on development instead of production

- You can run the application from the command line with Gradle or Maven. You can also build a single executable JAR file that contains all the necessary dependencies, classes, and resources and run that. Building an executable jar makes it easy to ship, version, and deploy the service as an application throughout the development lifecycle, across different environments, and so forth.

- Static resources, including HTML and JavaScript and CSS, can be served from your Spring Boot application by dropping them into the right place in the source code. By default, Spring Boot serves static content from resources in the classpath at /static (or /public). The index.html resource is special because, if it exists, it is used as a "`welcome page,


- In a typical Spring MVC application, @Controller classes are responsible for preparing a model map with data and selecting a view to be rendered. This model map allows for the complete abstraction of the view technology and, in the case of Thymeleaf, it is transformed into a Thymeleaf context object (part of the Thymeleaf template execution context) that makes all the defined variables available to expressions executed in templates.

- In Thymeleaf, these model attributes (or context variables in Thymeleaf jargon) can be accessed with the following syntax: ${attributeName}, where attributeName in our case is messages. This is a Spring EL expression. In short, Spring EL (Spring Expression Language) is a language that supports querying and manipulating an object graph at runtime.

- In order to access the q parameter you can use the param. prefix:

- Similarly to the request parameters, session attributes can be accessed by using the session. prefix:

