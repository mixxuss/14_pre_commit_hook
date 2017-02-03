# Quadratic Equations Solver

This program calculate roots of quadratic equation and have a protect from commits that can broken a program (using tests.py, executed before any commit)

# Example of broken code detection
```
git commit -a
.E..
======================================================================
ERROR: test_returns_none_for_complex_solution (__main__.QuadraticEquationTestCase)
----------------------------------------------------------------------
Traceback (most recent call last):
  File "tests.py", line 22, in test_returns_none_for_complex_solution
    root1, root2 = get_roots(1, 2, 3)
  File "/home/mixus/PyCharmProjects/14_pre_commit_hook/quadratic_equation.py", line 14, in get_roots
    return root1, root2
UnboundLocalError: local variable 'root1' referenced before assignment

----------------------------------------------------------------------
Ran 4 tests in 0.001s

FAILED (errors=1)
No stash found.

```

# Project Goals

The code is written for educational purposes. Training course for web-developers - [DEVMAN.org](https://devman.org)
