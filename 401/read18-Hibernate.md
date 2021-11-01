# Hibernate Many to Many 
simple Entity relationship for many to many:

![img](https://cdn.journaldev.com/wp-content/uploads/2014/05/Many-To-Many-Mapping-Tables.png)

In this example, any given item can be assigned to multiple carts and a cart may have multiple items in it,
 leading to a many-to-many association between the two.

* in the model classes there is some additional code we have to write in order to make a many to many relation, example:

```
@Entity
@Table(name = "Model1")
public class Model1 { 
    // ...
 
    @ManyToMany(cascade = { CascadeType.ALL })
    @JoinTable(
        name = "Model1_Model2", 
        joinColumns = { @JoinColumn(name = "model1_id") }, 
        inverseJoinColumns = { @JoinColumn(name = "model2_id") }
    )
    Set<Model2> model2 = new HashSet<>();
   
    // standard constructor/getters/setters
}
```

```
@Entity
@Table(name = "Model2")
public class Model2 {    
    // ...  
 
    @ManyToMany(mappedBy = "model2")
    private Set<Model1> model1 = new HashSet<>();
    
    // standard constructors/getters/setters   
}
```

*  the Model1 class and Model2 classes refer to one another, which means that the association between them is bidirectional.

* The @ManyToMany annotation is used in both classes to create the many-to-many relationship between the entities.

* This association has two sides i.e. the owning side and the inverse side. In our example, the owning side is Model1 so the join table is specified on the owning side by using the @JoinTable annotation in Model1 class. The @JoinTable is used to define the join/link table. In this case, it is Model1_Model2.

* The @JoinColumn annotation is used to specify the join/linking column with the main table. Here, the join column is Model1_id and Model2_id is the inverse join column since Model2 is on the inverse side of the relationship.

* In the Model2 class, the mappedBy attribute is used in the @ManyToMany annotation to indicate that the Model1s collection is mapped by the Model2s collection of the owner side.






