# Loops (for ,for-each,While):

*  looping is a feature which facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to false.

## types of loops in Java: 

* While loop: repeats a statement or a block of statements while its controlling Boolean-expression is true.

* for loop: allows us to repeat certain operations by incrementing and evaluating a loop counter.

* for-each loop

* Do-While loop: works like the while loop but it excute the code at least once.

### like a For Statement :

 The for statement provides a compact way to iterate over a range of values. Programmers often refer to it as the "for loop" because of the way in which it repeatedly loops until a particular condition is satisfied. The general form of the for statement can be expressed as follows:

for (initialization; termination;
     increment) {
    statement(s)
}
When using this version of the for statement, keep in mind that:

 * The initialization expression initializes the loop; it's executed once, as the loop begins.
* When the termination expression evaluates to false, the loop terminates.
* The increment expression is invoked after each iteration through the loop; it is perfectly acceptable for this expression to increment or decrement a value.





# Packages and Import

* in java, packages means directory, so when we say package name its just the same as directory name which contains the .java files .
* we declare packages when we define our java program .
* if you want to use packages from other libraries you have to name the packages in an import statement .


## Package declaration

* in your code after the optional package declaration, you can have an import statement to specify classes from other packages .

* we can use classes from another file by fully qualified class name without import.


* make a single class visible from the imported file.



## most common imports

* import java.awt.*;	Common GUI elements.
* import java.awt.event.*;	The most common GUI event listeners.
* import javax.swing.*;	More common GUI elements. Note "javax".
* import java.util.*;	Data structures (Collections), time, Scanner, etc classes.
* import java.io.*;	Input-output classes.
* import java.text.*;	Some formatting classes.
* import java.util.regex.*;	Regular expression classes.


* there are no different if we imported all classes or imported only one class .







## [BACK](../README.md)