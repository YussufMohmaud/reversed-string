# Reverse String

## 6 ways and the best one

### How to reverse a string from the worst to the best

1. Using `for loop` and appending individual characters in verse order
2. Using `while loop` to iterate individual characters in reverse order and append those individual characters
3. Using string's `join()` built-in function with reversed()
4. Using `recursion`
5. Creating a `list` from string's built-in function and then reverse()
6. Using `slicing` to create a reverse copy of the string in reverse

## Best Way to Reverse a String in Python

We can model reverse a string through multiple algorithms. We have already seen six of them. But which of them you should choose to reverse a string. We can use timeit module to run multiple iterations of these functions and get the average time required to run them. All the algorithms are stored in a jupyter notebook named reverse_string. I executed all these algorithms one by one for 100,000 times using the timeit module and got the average of the best.

```txt
%timeit -n 100000 'reverse_for_loop("abcd"*10)'
153 ns ± 79.1 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)

%timeit -n 100000 'reverse_while_loop("abcd"*10)'
128 ns ± 61.4 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)

%timeit -n 100000 'reverse_join_reversed_iter("abcd"*10)'
112 ns ± 51.8 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)

%timeit -n 100000 'reverse_recursion("abcd"*10)'
124 ns ± 55.3 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)

%timeit -n 100000 'reverse_list("abcd"*10)'
116 ns ± 55 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)

%timeit -n 100000 'reverse_slicing("abcd"*10)'
122 ns ± 55 ns per loop (mean ± std. dev. of 7 runs, 100000 loops each)
```