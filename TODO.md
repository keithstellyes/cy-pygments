There are still some problematic lexers to fix, see the lexers in 
`porting-scripts/`

In general, taking better advantage of Cython's capabilities for opimization, for example:

```python
for i in range(10):
    pass
```

to:

```python
int i
for i in range(10):
    pass
```
