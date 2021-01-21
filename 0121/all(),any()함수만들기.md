#  # abs() 직접 구현하기

## `abs()` 직접 구현하기

```python
def my_abs(x):
    if type(x) == complex:
        real = x.real
        imag = x.imag
        abs_value = (real**2 + imag**2)**0.5
        return abs_value

    else:
        if x == 0:
            return x ** 2
        if x < 0:
            return x*(-1)
        else:
            return x
    
print(my_abs(3+4j))
print(my_abs(-0.0))
print(my_abs(-5))
print(abs(3+4j), abs(-0.0), abs(-5))
```

## 
