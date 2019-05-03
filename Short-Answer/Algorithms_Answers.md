Add your answers to the Algorithms exercises here.
```
a)  a = 0
    while (a < n * n * n): = 0(n^3)
      a = a + n * n = O(n^2)
```     
The answer is O(n).  The while loop requires a to be >= n^3 to exit.
Variable a increases inside the loop at a rate of n^2.  Because of the
way it is set up, the 2nd would be subtracted from the first, leaving O(n)

```
b)  sum = 0
    for i in range(n): = O(n)
      i += 1
      for j in range(i + 1, n): O(n-1)
        j += 1
        for k in range(j + 1, n): O(n-2)
          k += 1
          for l in range(k + 1, 10 + k): O(9)
            l += 1
            sum += 1
```            
            
O(n) * O(n-1) * O(n-2) * O(9) = O(9(n*(n-1)*(n-2)))

I honestly don't know the answer, but I will guess perhaps O(n^3) since 
each loop would a power of n (minus a constant I think) and the last loop
only adds a factor of 9 (Which would be dropped when calculating time
complexity.

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0
        
   return 2 + bunnyEars(bunnies-1)
```

This would be O(n)).  The recursion only occurs n times.