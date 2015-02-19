## Why variable names cannot have ? or ! in Ruby but method names can

I had this question and found a good discussion on [StackOverflow](http://stackoverflow.com/questions/5448938/in-ruby-a-variable-name-cannot-end-with-such-as-has-completed-but-a-meth)

> There is a difference as a variable holds a specific value whereas one single method could return values of different types.
> However, from a semantic point of view: Methods are messages sent to an object, so you could tell the object do do something or ask it for a value (hence the question mark).
> Variables are just holding a certain value.


