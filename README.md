# Direct Modification of Instance Variables in Ruby

This example showcases a potential issue in Ruby related to directly modifying instance variables using `instance_variable_set` and `instance_variable_get`. While this approach might seem convenient, it can bypass accessor methods and lead to unexpected behavior or maintenance difficulties.

**Problem:**
Directly altering instance variables can violate encapsulation and make code harder to maintain.  Changes to the internal state are not tracked through the accessor methods, making it challenging to debug and potentially introducing inconsistencies.

**Solution:**
Always use accessor methods (`attr_accessor`, `attr_reader`, `attr_writer`) to interact with instance variables. This promotes better encapsulation and maintainability.