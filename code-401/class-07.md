# Python Scope & the LEGB Rule:

The concept of scope rules how variables and names are looked up in your code. It determines the visibility of a variable within the code.

The letters in the acronym LEGB stand for Local, Enclosing, Global, and Built-in scopes. This summarizes not only the Python scope levels but also the sequence of steps that Python follows when resolving names in a program.

# (Links to an external site.)Understanding Scope:

In programming, the scope of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on.

General scopes:
    Global scope: The names that you define in this scope are available to all your code.
    Local scope: The names that you define in this scope are only available or visible to the code within the scope.

# Python Scope vs Namespace:

In Python, the concept of scope is closely related to the concept of the namespace. As you’ve learned so far, a Python scope determines where in your program a name is visible. Python scopes are implemented as dictionaries that map names to objects. These dictionaries are commonly called namespaces. These are the concrete mechanisms that Python uses to store names. They’re stored in a special attribute called .dict.

Using the LEGB Rule for Python Scope:

Python resolves names using the so-called LEGB rule, which is named after the Python scope for names.

Local (or function) scope is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function.

Enclosing (or nonlocal) scope is a special scope that only exists for nested functions.

Global (or module) scope is the top-most scope in a Python program, script, or module.

Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session.

square() is a function that computes the square of a given number, base.

## Discovering Unusual Python Scopes

You’ll find some Python structures where name resolution seems not to fit into the LEGB rule for Python scopes. These structures include:

- Comprehensions
- Exception blocks
- Classes and instances

## Class and Instance Attributes Scope

When you define a class, you’re creating a new local Python scope. The names assigned at the top level of the class live in this local scope. The names that you assigned inside a class statement don’t clash with names elsewhere. You can say that these names follow the LEGB rule, where the class block represents the level.
Using Scope Related Built-In Functions

1- globals(): is a built-in function that returns a reference to the current global scope or namespace dictionary

2- locals(): This function updates and returns a dictionary that holds a copy of the current state of the local Python scope or namespace.

3- dir(): to get the list of names in the current Python scope

4- vars(): vars() is a Python built-in function that returns the .dict attribute of a module, class, instance, or any other object.

# Conclusion

The scope of a variable or name defines its visibility throughout your code. In Python, the scope is implemented as either a Local, Enclosing, Global, or Built-in scope. When you use a variable or name, Python searches these scopes sequentially to resolve it. If the name isn’t found, then you’ll get an error. This is the general mechanism that Python uses for name resolution and is known as the LEGB rule.