## Read 17

### OAuth

-simple: a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties (if you visit the home page, you will be automatically redirected to GitHub).

- click: adds an explicit link that the user has to click to login.

- logout: adds a logout link as well for authenticated users.

- two-providers: adds a second login provider so the user can choose on the home page which one to use.

- custom-error: adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API.

- First, you need to create a Spring Boot application, which can be done in a number of ways. The easiest is to go to https://start.spring.io and generate an empty project (choosing the "Web" dependency as a starting point).

- In your new project, create index.html in the src/main/resources/static folder. You should add some stylesheets and JavaScript links so the result looks like this

- Spring Boot attaches special meaning to a WebSecurityConfigurerAdapter on the class annotated with @SpringBootApplication: It uses it to configure the security filter chain that carries the OAuth 2.0 authentication processor.

- Many JavaScript frameworks have built in support for CSRF (e.g. in Angular they call it XSRF), but it is often implemented in a slightly different way than the out-of-the box behaviour of Spring Security. For instance, in Angular, the front end would like the server to send it a cookie called "XSRF-TOKEN" and if it sees that, it will send the value back as a header named "X-XSRF-TOKEN"

- Remember that now the logout endpoint is working with the browser client, then all other HTTP requests (POST, PUT, DELETE, etc.) will also work just as well. So this should be a good platform for an application with some more realistic features.

