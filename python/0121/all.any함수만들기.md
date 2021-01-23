#  # all(),any() 직접 구현하기

## `all()` 직접 구현하기

```python
def my_all(elements):
    for i in elements:
        if not i:
            return False
    return True

print(my_all([]))
print(my_all([1, 2, 5, '6']))
print(my_all([[], 2, 5, '6']))
print(all([]), all([1, 2, 5, '6']), all([[], 2, 5, '6']))
```

## `any()` 직접 구현하기

```python
def my_any(elements):
    for i in elements:
        if i:
            return True
    return False

print(my_any([1, 2, 5, '6']))
print(my_any([[], 2, 5, '6']))
print(my_any([0]))
print(any([1, 2, 5, '6']), any([[], 2, 5, '6']), any([0]))
```

