

## What the function does

The function `find_max(numbers)` returns the largest number in a list.

## Manual trace

Input:

```text
[3, 1, 9]
```

Initial value:

```
biggest = 3
```

Loop:

- i = 0 → numbers[0] = 3 → 3 > 3 is False → biggest = 3
- i = 1 → numbers[1] = 1 → 1 > 3 is False → biggest = 3

The loop ends and the function returns:

```
3
```

Expected result:

```
9
```

## bug

There is an off-by-one bug in the loop.

The loop uses:

```python
range(len(numbers) - 1)
```

This skips the last element of the list, so the value `9` is never checked.

The loop should iterate over all elements after the first on
