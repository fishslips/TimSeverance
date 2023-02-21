### Singleton

#### What the singleton is
Singleton pattern allows us to create only one instance of an object. The common approach is the add conditional logic to a constructor or initializer, or to create a private contructor that is invoked through a helper method.

#### Pros and Cons
Why use the singleton as opposed to static classes?

Typically static classes don't support any kind of inheritence. This makes a static class rigid in some aspects, but what we really want is flexibility.

Singletons are live objects that can hold state and are dynamic. 