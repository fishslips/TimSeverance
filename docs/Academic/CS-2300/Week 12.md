### Counting

#### Product Rule

If we're determining the number of ways that a sequence of choices can be made, we can use the product rule to figure it out.

If we have some choice to make m, and then some other choice to make n, and these choices are independent of eachother, then we can view this as the cardinality, or number of choices that can be made for m, multiplied by the cardinality or number of choices that can be made for n.

In zybooks we're given an example of a menu where you pick a drink, an entree, and a side.

D = {Coffee, OJ}
M = {Pancakes, Eggs}
S = {Bacon, Sausage, Hash Browns}

We can represent the number of choices in a similar fashion to a truth table.

| D      | M       | S          |
| ------ | ------- | ---------- |
| Coffee | Pancake | Bacon      |
| Coffee | Pancake | Sausage    |
| Coffee | Pancake | Hash Brown |
| Coffee | Eggs    | Bacon      |
| Coffee | Eggs    | Sausage    |
| Coffee | Eggs    | Hash Brown |
| OJ     | Pancake | Bacon      |
| OJ     | Pancake | Sausage    |
| OJ     | Pancake | Hash Brown |
| OJ     | Eggs    | Bacon      |
| OJ     | Eggs    | Sausage    |
| OJ     | Eggs    | Hash Brown |

The number of rows is the number of combinations possible.

Alternatively, we can view this as nested for loops

for i in D:
	for j in M:
		for k in S:

This gives us three twice, twice.

The simple form is |D| * |M| * |S| = 12

#### Sum Rule

If all choices are available to use for a given selection like before, we can use the product rule. However, if our choices are partitioned, or exclusive, then we can use the sum rule.

In the book it gives an example of if we want to select a drink, but there are cold drinks and hot drinks. 

It kind of makes sense in the previous example, that our drink option was one out of the sum of drinks. If we want to though, we can nest, or encapsulate our options into categories which can numerically represent a different number of options. If we have hot and cold drinks, for a total of 5 drinks, the overall number of choices is still 2 * 2 * 5, but we can also encapsulate those 5 drinks into 2 distinct choices of either cold or hot drink and make it 2 * 2 * 2.

So, in the passwords example, if we want to make a password that can be 6-8 digits long, with various options for characters, we can view this as chars^6 + chars^7 + chars^8. This works out because we're essentially saying that there are 6 digit options, plus 7 digit options, plus 8 digit options.

Expanded further we can see this as (36x36x36x36x36x36) + (36x36x36x36x36x36x36) + (36x36x36x36x36x36x36x36)

### Bijection Rule

Remember that a function is a bijection if it is one-to-one and onto. We also know that a bijection has an inverse, and the inverse is obtained by mapping the targets to the elements of the domain.

So the bijection rule is that if there are two sets, that are a bijection, they have the same cardinality. Duh.

### Permutation and Combinations

Permutation without parameter contains each element of a finite set exactly once. The number of permutations is n!

r-permutation P(n, r) has closed form n!/(n-r)! and is used when we select a limited number of items from the set.

Combination C(n,r), n choose r, closed form !n/r(n-r)! is used when order doesn't matter