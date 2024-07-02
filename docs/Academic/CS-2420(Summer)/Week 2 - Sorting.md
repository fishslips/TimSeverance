### Selection Sort

This is one of the "easy" ones. Selection sort works by having two trackers that walk through the array. The left side of the array is sorted, while the right is considered unsorted. The first tracker keeps track of the bounds of the sorted and unsorted space by pointing to the first item in unsorted space. The second tracker looks for the smallest item it can find in the unsorted region. Because the left side of the array is sorted, we know we're comparing the last item in the left/sorted side, against whatever smallest number the second tracker can find. As our second tracker encounters smaller numbers, it tags the smallest one by assigning it to a variable "smallest."

Once we find the smallest item in the right side, we simply swap its place with the first item in the unsorted space, and move our bounds forward. This is easily implemented with double loops with variables i and j for trackers.

The intuition for this sort is the left side increments one at a time, while the right side is scanned multiple times. This will be juxtaposed with insertion sort.

### Insertion Sort

This one is also easy. Conceptually, it works similarly to selection sort. The left side is "sorted," while the right side is not. However, the area that we repeatedly work on is different.

With insertion sort, we once again have trackers, most easily implemented with i and j variables in a double loop scenario (never be afraid to use more robust naming conventions though). Unlike selection sort, we start our i and j at index  rather than zero, and automatically count the left side "sorted." We're effectively partitioning the regions again, and obviously, an array with only one element is sorted in relation to itself. 

Where insertion differs from selection is that the tracker variable, j, doesn't walk through finding the smallest item, rather, it starts at the bounds, and walks through the sorted region trying to put the current number in the right spot.

This is accomplished by checking the current item marked by j, and the item to its left at j-1, seeing if j is smaller, and if so, swapping the two items. J is then decremented, and the same check is performed again, gradually pushing the "current" item down the sorted region until it's in the right spot. Finally, once the item is in place (j is greater than or equal to the item to its left), we increment i, and reset j to be equal to i. 

### Comparisons

These two sorts are fairly similar. Both of them have O(n<sup>2</sup>) time complexity. For selection and insertion sort, we have a time complexity T(n) = (n-1) * n/2. This gives us (n<sup>2</sup>-n)/2. Remember back to the section on O notation however. O notation just describes the overall time complexity, which roughly translates to pick the highest order term, as the largest term grows fastest and affects the shape of the graph the most. 

Now, here's where things get interesting. We talked about how generally in algorithmic analysis we want to analyze the worst case scenario. We want to see, given the worst set of conditions, how long will this thing take to complete. If both algorithms perform about the same, how do we choose one over the other? As the text mentions in 3.4, insertion sort has a runtime of O(n) for nearly sorted lists. This is where insertion sort might be a better option to implement over 

### Links

[15 Sorting Algorithms in 6 Minutes](https://www.youtube.com/watch?v=kPRA0W1kECg)

[Bogosrt](https://en.wikipedia.org/wiki/Bogosort)

[Timsort](https://en.wikipedia.org/wiki/Timsort)

[Powersort](https://www.youtube.com/watch?v=exbuZQpWkQ0)

[BigOCheatSheet](https://www.bigocheatsheet.com)
