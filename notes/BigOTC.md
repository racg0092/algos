# Big-O Time Complexity
It helps to identify when you should or shoul not use specific algorithms or data structures. Basically as your
input grows, how fast does computation or memory grow ?

In Big-O notation you always assume it will be the worst case. For example if a loop over an array of characters has a
conditional structure to break once it finds a capital `E` that is still O(N) because in the worst case scenario there 
is no capital `E` in the string and therefore you would loop throuhg the entire string.

**Three importact concepts**
- Growth is with respect to the input
- Constants are dropped
- Worst case is usually the way to measure


**Common Big-O Complexity**
- O(1)
    - No matter how much the input grows it does
 the same set of operations every single time.
- O(logn)
    - 
- O(n)
    - Linear growth
- O(n^2)
    - Quadratic growth
- O(2n)
    - Exponential growth
- O(n!)
    - algorithms that are impractically to solve in a traditional 
 computer


### O(N^2)
Quadratic growth example. For every single character in the array
we will go over every single character in the array

```go
// horrible example find a better one
func findRepetitions(n string) int {
    repetitions := make(map[string]int)
    for i := 0; i < len(n); i++ {
        repetitions[n[i]] = 0
        for j := 0; j < len(n); j++ {
            if n[i] == m[j] {
                repetitions[i] += 1
            }
        }
    }
}
```



