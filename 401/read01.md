# Java Basics

## Variables :

* ### The Java programming language defines the following kinds of variables: 

* Instance Variables (Non-Static Fields) 
* Class Variables (Static Fields) 
* Local Variables 
* Parameters .

## Naming :
* ### The rules and conventions for naming your variables can be summarized as follows:

*  always begin your variable names with a letter, not "$" or "_". Additionally, the dollar sign character, by convention, is never used at all. 


* When choosing a name for your variables, use full words instead of cryptic abbreviations. Doing so will make your code easier to read and understand.

* If the name you choose consists of only one word, spell that word in all lowercase letters. If it consists of more than one word, capitalize the first letter of each subsequent word. The names gearRatio and currentGear are prime examples of this convention. If your variable stores a constant value, such as static final int NUM_GEARS = 6, the convention changes slightly, capitalizing every letter and separating subsequent words with the underscore character. By convention, the underscore character is never used elsewhere. 

* Summary :
+  Variables names are case sensitive
+ Must start with a letter
+ Full words is much better than cryptic abbreviations
+  If it consists of more than one word, capitalize the first letter of each subsequent word



## Primitive Data Types

The Java programming language is statically-typed, which means that all variables must first be declared before they can be used.


* ### the Java programming language supports seven 8 primitive data types : 


* byte: The byte data type is an 8-bit signed two's complement integer. It has a minimum value of -128 and a maximum value of 127 (inclusive). The byte data type can be useful for saving memory in large arrays, where the memory savings actually matters. They can also be used in place of int where their limits help to clarify your code; the fact that a variable's range is limited can serve as a form of documentation.

* short: The short data type is a 16-bit signed two's complement integer. It has a minimum value of -32,768 and a maximum value of 32,767 (inclusive). As with byte, the same guidelines apply: you can use a short to save memory in large arrays, in situations where the memory savings actually matters.

* int: By default, the int data type is a 32-bit signed two's complement integer, which has a minimum value of -231 and a maximum value of 231-1. In Java SE 8 and later, you can use the int data type to represent an unsigned 32-bit integer, which has a minimum value of 0 and a maximum value of 232-1. Use the Integer class to use int data type as an unsigned integer. See the section The Number Classes for more information. Static methods like compareUnsigned, divideUnsigned etc have been added to the Integer class to support the arithmetic operations for unsigned integers.
* long: The long data type is a 64-bit two's complement integer. The signed long has a minimum value of -263 and a maximum value of 263-1. In Java SE 8 and later, you can use the long data type to represent an unsigned 64-bit long, which has a minimum value of 0 and a maximum value of 264-1. Use this data type when you need a range of values wider than those provided by int. The Long class also contains methods like compareUnsigned, divideUnsigned etc to support arithmetic operations for unsigned long.
* float: The float data type is a single-precision 32-bit IEEE 754 floating point. Its range of values is beyond the scope of this discussion, but is specified in the Floating-Point Types, Formats, and Values section of the Java Language Specification. As with the recommendations for byte and short, use a float (instead of double) if you need to save memory in large arrays of floating point numbers. This data type should never be used for precise values, such as currency. For that, you will need to use the java.math.BigDecimal class instead. Numbers and Strings covers BigDecimal and other useful classes provided by the Java platform.
* double: The double data type is a double-precision 64-bit IEEE 754 floating point. Its range of values is beyond the scope of this discussion, but is specified in the Floating-Point Types, Formats, and Values section of the Java Language Specification. For decimal values, this data type is generally the default choice. As mentioned above, this data type should never be used for precise values, such as currency.
* boolean: The boolean data type has only two possible values: true and false. Use this data type for simple flags that track true/false conditions. This data type represents one bit of information, but its "size" isn't something that's precisely defined.

* char: The char data type is a single 16-bit Unicode character. It has a minimum value of '\u0000' (or 0) and a maximum value of '\uffff' (or 65,535 inclusive).



* ### Default Values :


| Data Type |	Default Value (for fields)|
| byte |	0 |
| short |	0 |
|int |	0|
|long |	0L|
|float |	0.0f|
|double |	0.0d|
|char 	|'\u0000'|
|String |(or any object)   	null|
|boolean |	false|





* ## Literals :

A literal is the source code representation of a fixed value; literals are represented directly in your code without requiring computation. 

* Integer Literals

An integer literal is of type long if it ends with the letter L or l; otherwise it is of type int. It is recommended that you use the upper case letter L because the lower case letter l is hard to distinguish from the digit 1.
* Floating-Point Literals

A floating-point literal is of type float if it ends with the letter F or f; otherwise its type is double and it can optionally end with the letter D or d.

* Character and String Literals

Literals of types char and String may contain any Unicode (UTF-16) characters. If your editor and file system allow it, you can use such characters directly in your code. If not, you can use a "Unicode escape" such as '\u0108' (capital C with circumflex), or "S\u00ED Se\u00F1or" (Sí Señor in Spanish). 



* ## Arrays :

* An array is a container object that holds a fixed number of values of a single type. The length of an array is established when the array is created. After creation, its length is fixed. You have seen an example of arrays already, in the main method of the "Hello World!" application. This section discusses arrays in greater detail.

* Each item in an array is called an element, and each element is accessed by its numerical index. As shown in the preceding illustration, numbering begins with 0. The 9th element, for example, would therefore be accessed at index 8.



* ## Operators

* ### operators of java programming language:
| -----------            | -----------                              |
| equality               | == !=                                    |
| bitwise AND            | &                                        |
| bitwise exclusive OR   | ^                                        |
| bitwise inclusive OR   | \|                                       |
| logical AND            | &&                                       |
| logical OR             | \| \|                                    |
| ternary                |  ? :                                     |
| assignment             | = += -= *= /= %= &= ^= \|= <<= >>= >>>=  |
| Operator               | Sympol                                   |
| postfix                | expr++ expr--                            |
| multiplicative         | * / %                                    |
| additive               | + -                                      |
| shift                  | << >> >>>                                |
| relational             | < > <= >= instanceof                     |





# [back](../README.md)