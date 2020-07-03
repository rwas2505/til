* ***public:*** is an **access modifier** and it allows for all the other code to access this class. If you do not explicitly apply the *public* keyword, then it would only be accessible within the assembly that defined it. This is because the implicit access modifier for a class is *internal*. 
    * *example:* *public class Person {}* *(Price 146)*

* ***new:*** allocates memory for the objct and initializes any internal data. We could use *Person* in place of the *var* keyword, but the use of *var* involves less typing and is still just as clear.
    * *example:* *var bob = new Person();* *(Price 148)*

* ***object*** is a C# alias keyword for *System.Object*
    * *public class Person: System.Object* is the same as
      *public class Person: object*
    * Both of the examples above state that the *Person* class is a derived or subclass of *System.Object* type. This is not necessary to tell the complier since all types ulitmately inherit directly or indirectly from *System.Object*

    