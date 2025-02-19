### Creational Patterns

Provides mechanisms for the flexbile creation of objects 

### Factory Patterns

The Factory Pattern isn't actually just one pattern. There are a variety of factories that have different implementation features, but they are all responsible for making new objects in a flexible manner.

So far, most of our patterns have their own unique benefits but one of the main reasons we keep implementing patterns is to overcome obstacles that arise when we change certain aspects of our code. We've use interfaces, composition, and polymorphism to help us write code that is adaptive to change. This goes back to the principles of chapter 1. However, change is ever-present. This chapter focuses on hard coding new objects, and where change might impact us, and more importantly, how we end up repeating ourselves in our object creation, which violates DRY.

#### Simple Factory

Creates a class with a create(string s) method that receives a string for input, and using conditionals, creates and returns an object of a specified type.

**From the book:** 
The Simple Factory isn’t actually a Design Pattern; it’s more of a programming idiom. But it is commonly used, so we’ll give it a Head First Pattern Honorable Mention. Some developers do mistake this idiom for the Factory Pattern, but the next time that happens you can subtly show you know your stuff; just don’t strut as you educate them on the distinction.

### Factory Method

Rather than creating a class dedicated to creation, subclasses instead implement an abstract method, where they handle the creation of their own objects. We're leveraging the same techniques, but rather than 

### Singleton
#### What the singleton is
Singleton pattern allows us to create only one instance of an object. The common approach is the add conditional logic to a constructor or initializer, or to create a private constructor that is invoked through a helper method.

For languages like C++, Java, C#, your go-to strategy will be to

- make a private static member variable (pointers work best in C++) to an instance of the class 

- make a private constructor

- make a public GetInstance() method that's responsible for checking if the reference or pointer is null, and if so, invoke the private constructor and set the static member.

Python is a bit different. It doesn't have standard privacy and its init processes are a bit different. In Python, we have 3 methods at our disposal during the creation of an object. We have \_\_init\_\_, \_\_new\_\_, and \_\_call\_\_ that we can use. When we invoke a python constructor like 
x = some_class(), call, then new, then init are invoked. Since none of these are private, the standard is to 

- make a class variable for your instances (just don't use self.)

- and then check if a class instance exists during call or new.

Python references

https://www.geeksforgeeks.org/singleton-method-python-design-patterns/

Classic Python Singleton
```
class Singleton:
    _instance = None

    def __new__(cls, *args, **kwargs):
        if cls._instance is None:
            cls._instance = super().__new__(cls)
        return cls._instance

# Usage
a = Singleton()
b = Singleton()
assert a is b  # True

```

Metaclass Singleton
```
class SingletonMeta(type):
    _instances = {}

    def __call__(cls, *args, **kwargs):
        if cls not in cls._instances:
            cls._instances[cls] = super().__call__(*args, **kwargs)
        return cls._instances[cls]

class Singleton(metaclass=SingletonMeta):
    pass

# Usage
a = Singleton()
b = Singleton()
assert a is b  # True

```

#### Pros and Cons
Why use the singleton as opposed to static classes?

Typically static classes don't support any kind of inheritance. This makes a static class rigid in some aspects, but what we really want is flexibility.

Singletons are live objects that can hold state and are dynamic. 