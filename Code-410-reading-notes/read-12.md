## Read 12

- CrudRepository provides CRUD functions

- PagingAndSortingRepository provides methods to do pagination and sort records

- JpaRepository provides JPA related methods such as flushing the persistence context and delete records in a batch

- The Spring Data Repository will auto-generate the implementation based on the name we provided it.

 - Crud funcation ality below:

 - save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch

- findOne(…) – get a single entity based on passed primary key value

- findAll() – get an Iterable of all available entities in database

- count() – return the count of total entities in a table

- delete(…) – delete an entity based on the passed object

- exists(…) – verify if an entity exists based on the passed primary key value

- Passing the pageable object to the Spring data query will return the results in question (the first parameter of PageRequest is zero-based).

- Downside to spring data repo : we couple our code to the library and to its specific abstractions, such as `Page` or `Pageable`; that's of course not unique to this library – but we do have to be careful not to expose these internal implementation details
by extending e.g. CrudRepository, we expose a complete set of persistence method at once. This is probably fine in most circumstances as well but we might run into situations where we'd like to gain more fine-grained control over the methods exposed, e.g. to create a ReadOnlyRepository that doesn't include the save(…) and delete(…) methods of CrudRepository

- https://spring.io/guides/gs/accessing-data-jpa/ 