# fibonacci-memoization

Python project for
* (i) [Fibonacci Memoization](#fibonacci-memoization) - example of implementation of the concepts of Memoization in the context of the Fibonacci sequence ([usages](#all-usages))

## Dependencies

The dependencies `argparse` and `time` are native to Python platform.

## Contact / License

Feel free to contact me by mail: guilherme.farto@gmail.com

---

<a name="fibonacci-memoization"></a>
## Fibonacci Memoization (fibonacci-memoization.py)
> Based on the concepts of Fibonacci sequence and Memoization approach - an optimization technique based on storing the results of expensive function calls and returning the cached result when the same inputs occur again

Usage (simulation of Fibonacci sequence **without memoization**):
```python
python fibonacci-memoization.py [-h] -i INDEX [-m]
```

The arguments shoud be:

`-i INDEX, --index INDEX` *(required)*
* index of fibonacci sequence number to be calculated

`-m, --memoization` *(optional)*
* use memoization

<a name="fibonacci-memoization"></a>
## Usages

### Usage (simulation of Fibonacci sequence without memoization):
```python
python fibonacci-memoization.py -i 30
```

Output:

```
  Fibonacci Memoization
  The result for fibonacci(30) is 832040 - calculated in 1.25 seconds
```

### Usage (simulation of Fibonacci sequence with memoization):
```python
python fibonacci-memoization.py -i 30 -m
```

Output:

```
  Fibonacci Memoization
  using memoization for 2 = 1
  using memoization for 3 = 2
  using memoization for 4 = 3
  using memoization for 5 = 5
  using memoization for 6 = 8
  using memoization for 7 = 13
  using memoization for 8 = 21
  using memoization for 9 = 34
  using memoization for 10 = 55
  using memoization for 11 = 89
  using memoization for 12 = 144
  using memoization for 13 = 233
  using memoization for 14 = 377
  using memoization for 15 = 610
  using memoization for 16 = 987
  using memoization for 17 = 1597
  using memoization for 18 = 2584
  using memoization for 19 = 4181
  using memoization for 20 = 6765
  using memoization for 21 = 10946
  using memoization for 22 = 17711
  using memoization for 23 = 28657
  using memoization for 24 = 46368
  using memoization for 25 = 75025
  using memoization for 26 = 121393
  using memoization for 27 = 196418
  using memoization for 28 = 317811
  The result for fibonacci(30) is 832040 - calculated in 0.00811 seconds
```

It is important to highlight the relevant reduction of time when compared to the process of calculating the n-th Fibonacci number (e.g., 30) `without memoization (1.25 seconds)` and `with memoization (0.00811 seconds)`.

The same concept of memoization can be used in numerous other projects that use recursion-based approaches.
