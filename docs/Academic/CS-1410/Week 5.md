### Polymorphism

#### Overriding

#### Overloading
Python doesn't support overloading. 

In strictly typed languages, we can use the types of parameters to affect our method signature. For instance:

public void func(int x, int y):
	return

public void func(int x, string y):
	return

have the same name, but different acceptable parameters. Note that

public void func(int x, int z):
	return 

would not work because the two parameters are ints and so this method signature conflicts with the original func that we defined.

However, in python, we cannot do this. The last defined function with the same name will be the preferred function. 

We can however, circumvent this problem with single dispatch decorators in python.

