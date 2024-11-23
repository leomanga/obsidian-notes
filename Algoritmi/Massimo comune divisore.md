```python
def gcd(a, b):
    while b:
        a, b = b, a%b
    return a
```

La complessità computazionale è di $O(\log(n))$