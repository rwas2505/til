In order to access an instance variable outside of a class, a method is required to make it public.

One way to do this is by defining a reader/getter method within the class. Below, the `name` and `gender` methods return the instance variables `@name` and `@gender` and make them available publicly.

```ruby
class Person
  def initialize(name, gender)
    @name = name
    @gender = gender
  end

  def name
    @name
  end

  def gender
    @gender
  end
end

john = Person.new("John", "Male")
puts john.name # => John
puts john.gender # => Male
```

As a cleaner, simpler alternative, ruby lets us use the `attr_reader` method. As shown, you can call it on multiple variables rather than creating a getter method for each variable.

```ruby
class Person
  attr_reader :name, :gender

  def initialize(name, gender)
    @name = name
    @gender = gender
  end
end

john = Person.new("John", "Male")
puts john.name # => John
puts john.gender # => Male
```

This also works for setter methods. First we have a setter method defined for name.
```ruby
class Person
  def initialize(name, gender)
    @name = name
    @gender = gender
  end

  def name
    @name
  end

  def name=(name)
    @name = name
  end
end

john = Person.new("John", "Male")
puts john.name # => John
john.name = "Johnathon"
puts john.name # => Johnathon
```

Now using the `attr_writer` method.

```ruby
class Person
  attr_reader :name
  attr_writer :name

  def initialize(name, gender)
    @name = name
    @gender = gender
  end
end

john = Person.new("John", "Male")
puts john.name # => John
john.name = "Johnathon"
puts john.name # => Johnathon
```

Finally, `attr_accessor` can be used to make the method both a reader and a writer.

```ruby
class Person
  attr_accessor :name, :gender

  def initialize(name, gender)
    @name = name
    @gender = gender
  end
end

john = Person.new("John", "Male")
puts john.name # => John
john.name = "Johnathon"
puts john.name # => John
```

