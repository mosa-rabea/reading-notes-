## The Relationships in Spring Data REST

* ### One-to-One Relationship :

* refers to the relationship between two database tables A and B ,
in which only one element of A may only be linked to one element/row of B.


* ### One-to-Many Relationship :

* when a parent record in one table can potentially 
reference several child records in another table

* ### Many-to-Many Relationship :

* a relationship between tables in a database when a parent row 
in one table contains several child rows in the second table



## Integration Testing in Spring :


Integration testing is a very important role in the application development cycle, to start testing in spring there are some configurations which you should do first, which are:

* Enable Spring in Tests with JUnit 5: enabled by adding the @ExtendWith(SpringExtension.class) annotation to the test classes and specifying the extension class to load.


* The WebApplicationContext Object: loads all the application beans and controllers into the context.

* Mocking Web Context Beans: encapsulates all web application beans and makes them available for testing.

* Verify Test Configuration: check that the right servletContext is being attached.

