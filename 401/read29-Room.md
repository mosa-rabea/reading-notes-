# Room

Room is an ORM (object relational mapper) for SQLite database in Android.
It is part of the Architecture Components released by Google.
Room allows you to create and manipulate database in Android more quickly.
See it as an abstraction layer on top of inbuilt SQLite database.


### benefits of using Room

* Compile-time verification of SQL queries.
* Convenience annotations that minimize repetitive.
* Streamlined database migration paths.

> the above benefits makes using Room is much better than using the SQL API's directly.



### Primary components

Room has three main components which are :

1. The database class, it has some conditions:

* The class must be annotated with a @Database annotation that includes an entities array that lists all of the data entities associated with the database.
* The class must be an abstract class that extends RoomDatabase.
* For each DAO class that is associated with the database, the database class must define an abstract method that has zero arguments and returns an instance of the DAO class.


2. Data entities.

3. Data access objects (DAOs).

![room](https://media.geeksforgeeks.org/wp-content/uploads/20210506144355/output.png)



#### Defining data using entities

we use the define entities to represent the objects we want to store in the database, and each entity corresponds to a table in the associated Room database, and each instance of an entity represents a row of data in the corresponding table.

* Each Room entity must define a primary key, The most straightforward way of doing this is to annotate a single column with @PrimaryKey.

* to assign automatic IDs to entity instances, set the autoGenerate property of @PrimaryKey to true.

* If an entity has fields that you don't want to persist, you can annotate them using @Ignore.

* if an entity inherits fields from a parent entity, use the ignoredColumns property of the @Entity attribute.

### relationships between objects in database
#### embedded objects:
we use it when we have a class which has a field of type other class.


#### one-to-one relationships
we use it when each instance of the parent entity corresponds to exactly one instance of the child entity.

#### one-to-many relationships
when each instance of the parent entity corresponds to zero or more instances of the child entity, but each instance of the child entity can only correspond to exactly one instance of the parent entity.

#### many-to-many relationships
where each instance of the parent entity corresponds to zero or more instances of the child entity, and vice-versa.

#### nested relationships
when three or more tables are all related to each other.


