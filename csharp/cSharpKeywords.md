* ***public:*** is an **access modifier** and it allows for all the other code to access this class. If you do not explicitly apply the *public* keyword, then it would only be accessible within the assembly that defined it. This is because the implicit access modifier for a class is *internal*. 
    * *example:* *public class Person {}* *(Price 146)*

* ***Access Modifier***
    * *private:* Member is accessible inside the type only. **This is the default**
    * *internal:* Member is accessible inside the type and any type in the same assembly.
    * *protected:* Member is accessible inside the type and any type that inherits from the type.
    * *public:* Member is accessible everywhere.
    * *internal protected:* Member is accessible inside the type, any type in the same assembly, and any type taht inherits from the type. Equivalent to a fictional access modifier named *internal_or_protected*.
    * *private protected:* Member is accessible inside the type, or any type that inherits from the type and is in the same assembly. Equivalent to a fictional access modifier named *internal_and_protected*. This combination is only available with C# 7.2 or later.

* ***new:*** allocates memory for the objct and initializes any internal data. We could use *Person* in place of the *var* keyword, but the use of *var* involves less typing and is still just as clear.
    * *example:* *var bob = new Person();* *(Price 148)*

* ***object*** is a C# alias keyword for *System.Object*
    * *public class Person: System.Object* is the same as
      *public class Person: object*
    * Both of the examples above state that the *Person* class is a derived or subclass of *System.Object* type. This is not necessary to tell the complier since all types ulitmately inherit directly or indirectly from *System.Object* *(Price 149)

* ***params*** is a C# keyword taht allows you to pass a comma-separated list of parameters of any length as an array. (*p.168*) (*also: https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/params*)

    
* ***properties:*** a property is simply a method (or a pair of methods) that acts and looks like a field when you want to get or set a value, thereby simplifying the syntax.
    * a *readonly* property only has a *get* implementation