Ruby `methods` can take many types of arguments including 
* No parameters
* Ordinal parameters
* Parameters with defaults
* Hash parameters
* Arguments as arrays
* Keyword arguments

Ordinal parameters require arguments to be passed in the order set in the method.

Parameters with default values can be set by using `method(parm1, param2 = default_value)`. You can then call the `method` without passing in a value for `param2` and the method will return `default_value`, or you can overwrite the default value by calling a new value for `param2`.

You can use a `hash` as an argument to pass an arbitrarty number of arguments to a method. Ruby allows us to leave off the braces when passing in a hash to a method if the parameter is the last or only parameter. 

An arbitrary number of arguments can also be passed as an array with the splat `*` operator. It will take the arbitraty number of arguments and collect them as an array. Since it will collect all values at and after its argument position, it should only be used as the only or the last argument.
