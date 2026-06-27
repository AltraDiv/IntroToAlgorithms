
> ==**Insertion Sort**==
```python
def insertionSort(A):
for i in range(1,len(A)):
	key = A[i]
	j = i - 1
	while j >= 0 and A[j] > key:
		A[j+1] = A[j]
		j = j - 1
	A[j+1] = key
```

> ==**Loop Invariant**==
> 	 ===Definition:== Elements are sorted / final place relative to each other
> 	Need to show 3 things:
> 	**1) Initialization**: It is true prior to the first iteration of the loop
> 	**2) Maintenance**: If it is true before the iteration of the loop, it remains true before the next iteration
> 	**3) Termination**: The loop terminates and when it terminates the invariant - usually along with the reason that the loop terminated - gives us a useful property that helps show that the algorithms is correct

> ==**Order of Growth**==
> 	Represented by $\Theta$  for Order Of Growth
> 	Order of Growth ignores constants, etc
> 	~ Roughly proportional
> 	
> Ex. 2n + 3 $\propto$ 10000n + 10 = $\theta$(n)

### 2.3 Designing Algorithms 

> Insertion Sort $\rightarrow$ incremental method

> ==**Divide and Conquer**== 
- Recursive
- Break the problems into similar sub-problems smaller in size
- Solve and then combine

**Divide**: Break problem into one or more smaller instances of same problem
**Conquer:** Solve recursively
**Combine**: Combine the problems to form solution

Merge Sort $\rightarrow$ DnC Method

> Merge Sort
> 	Sorts sub array A[p:r] Starting with A[1:n]
> 	
**Divide**: 
- Divide the subarray A[p:r] to be sorted into 2 adjacent subarrays, each half size.
- Compute midpoint q of A[p:r] then divide A[p:r] to A[p:q] and A[q+1:r]
**Conquer:** Sort each 2 sub arrays A[p:r] and A[q+1:r] recursively using merge sort
**Combine**: Merge A[p:q] and A[q+1:r] into A[p:r]

