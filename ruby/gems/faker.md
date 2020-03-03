*Faker documentation can be found [here](https://github.com/faker-ruby/faker#installing)*

First, run command `gem install faker` in terminal if you don't already have it. This installs the faker gem locally.

Once faker is installed, `require 'faker'` in local file.

The below code creates an employee `Class`, and then generates 100 random employees by assigning a `Faker::Name.first_name` to `@first_name` and `Faker::Name.last_name` to `@last_name`. The code will assign a random first and last name to each employee from the faker gem.

```ruby
require 'faker'

class Employee
  attr_accessor :first_name, :last_name, :salary, :active, :email

  def initialize(input_options)
    @first_name = input_options.fetch(:first_name, Faker::Name.first_name)
    @last_name = input_options.fetch(:last_name, Faker::Name.last_name   )
    @salary = input_options.fetch(:salary, 0)
    @active = input_options.fetch(:active, true)
    @email = input_options.fetch(:email, "#{first_name}#{last_name}@gmail.com")
  end

  def full_name
    if @last_name.end_with?("s")
      "#{first_name} #{last_name}, Esquire"
    else
      "#{first_name} #{last_name}"
    end
  end
end

employees = []
100.times do
  new_employee = Employee.new(active:true)
  employees << new_employee
end

employees.each{|employee| p employee.full_name} # prints each employee's full name on a new line
```

