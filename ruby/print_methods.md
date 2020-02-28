In Ruby, `puts` is actually short for `put.to_s` and so Ruby is calling `.to_s` on an object. It also adds a new line at the end of each statement so you can read it more easily.

Next, `p` calls `.inspect` ([explanation here](https://www.rubyguides.com/2018/12/ruby-inspect-method/)) on an object and also adds a line at the end of each statement.

In addition to `puts` and `p`, we can use `pp` (pretty print). Per Ruby [documentation](https://ruby-doc.org/stdlib-2.5.3/libdoc/prettyprint/rdoc/PrettyPrint.html),this class implements a pretty printing algorithm. It finds line breaks and nice indentations for grouped structure.

You can also use awesome print (`ap`). It needs to be installed with `gem install awesome_print` and then in your `.rb` file you must `require "awesome_print"`. This organizes the data even more than `pp`.