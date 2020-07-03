* ***public:*** is an **access modifier** and it allows for all the other code to access this class. If you do not explicitly apply the *public* keyword, then it would only be accessible within the assembly that defined it. This is because the implicit access modifier for a class is *internal*. 
    * *example:* *public class Person {}* *(Price 146)*

* ***new:*** allocates memory for the objct and initializes any internal data. We could use *Person* in place of the *var* keyword, but the use of *var* involves less typing and is still just as clear.
    * *example:* *var bob = new Person();* *(Price 148)*