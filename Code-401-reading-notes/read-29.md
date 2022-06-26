## Read 29

- The Room persistence library provides an abstraction layer over SQLite to allow fluent database access while harnessing the full power of SQLite. In particular, Room provides the following benefits:

1) Compile-time verification of SQL queries.

2) Convenience annotations that minimize repetitive and error-prone boilerplate code.

3) Streamlined database migration paths.

- The database class provides your app with instances of the DAOs associated with that database. In turn, the app can use the DAOs to retrieve data from the database as instances of the associated data entity objects. The app can also use the defined data entities to update rows from the corresponding tables, or to create new rows for insertion.

- You define each Room entity as a class that is annotated with @Entity. A Room entity includes fields for each column in the corresponding table in the database, including one or more columns that comprise the primary key.

- By default, Room uses the class name as the database table name. If you want the table to have a different name, set the tableName property of the @Entity annotation. Similarly, Room uses the field names as column names in the database by default. If you want a column to have a different name, add the @ColumnInfo annotation to the field and set the name property. 

- Sometimes, certain fields or groups of fields in a database must be unique. You can enforce this uniqueness property by setting the unique property of an @Index annotation to true

- In the intermediate data class approach, you define a data class that models the relationship between your Room entities. This data class holds the pairings between instances of one entity and instances of another entity as embedded objects. Your query methods can then return instances of this data class for use in your app.

- Room supports both of the approaches described above, and you should use whichever approach works best for your app. This section discusses some of the reasons why you might prefer one or the other.

- The intermediate data class approach allows you to avoid writing complex SQL queries, but it can also result in increased code complexity due to the additional data classes that it requires. In short, the multimap return type approach requires your SQL queries to do more work; and the intermediate data class approach requires your code to do more work.

- A many-to-many relationship between two entities is a relationship where each instance of the parent entity corresponds to zero or more instances of the child entity, and vice-versa.

- In the music streaming app example, consider again the user-defined playlists. Each playlist can include many songs, and each song can be a part of many different playlists. Therefore, there should be a many-to-many relationship between the Playlist entity and the Song entity.

- When you use the Room persistence library to store your app's data, you interact with the stored data by defining data access objects, or DAOs. Each DAO includes methods that offer abstract access to your app's database. At compile time, Room automatically generates implementations of the DAOs that you define.

- You can define each DAO as either an interface or an abstract class. For basic use cases, you should usually use an interface. In either case, you must always annotate your DAOs with @Dao. DAOs don't have properties, but they do define one or more methods for interacting with the data in your app's database.

