## Read 13

- We define a one-to-many relationship using the @OneToMany and @ManyToOne annotations. We can also add the optional @RestResource annotation to customize the association resource.

- In the response body, we can see that the association endpoint, /books/{bookId}/library, has been created.

- Now let's associate the book with the library we created in the previous section by sending a PUT request to the association resource that contains the URI of the library resource

- We can verify the books in the library by using the GET method on the library's /books association resource:

- To remove an association, we can use the DELETE method on the association resource:

-JUnit 5 defines an extension interface through which classes can integrate with the JUnit test.

- We can enable this extension by adding the @ExtendWith annotation to our test classes and specifying the extension class to load. To run the Spring test, we use SpringExtension.class.

- We'll also need the @ContextConfiguration annotation to load the context configuration and bootstrap the context that our test will use.

- WebApplicationContext provides a web application configuration. It loads all the application beans and controllers into the context.

- MockMvc provides support for Spring MVC testing. It encapsulates all web application beans and makes them available for testing.

