## Topics to hit

### 09/12/22

pytest
for loops
difficulties with the project
how can I help
selection sort
insertion sort

### 09/14/22

#### Quick Sort
Splits the sort space with a pivot point and recursively sorts.  

Pivot point can be any value in the list.

Zybooks chooses the pivot to be the value at the midpoint of the array. Partions are left and right halves.

We have to move all values smaller than the pivot point value into one partition, and all greater or equal values to the other partition.

The trick is that the values in the low and high partition aren't sorted, it's just that they are less than or equal to or greater than or equal to the value that is selected as partition value

Quicksort uses a helper function, called Partition to create the low



#### Merge Sort

Split down the middle recursively until you get lists of size 1

Lists of size 1 are already sorted

We use index i for low point of left side, j for high point of left side, j+1 for low point of right side, k for high point of right side

We then compare least values from left and right lists, and add smallest value to new index in our master array. 

