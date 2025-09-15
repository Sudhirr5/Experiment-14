# Experiment-14 : Pytest – Python program for Fibonacci Series
### Name : SUDHIR KUMAR. R
### Reg No. : 212223230221

## Aim:
To write a Python program using **Pytest** for generating the Fibonacci Series and testing it using test cases.

## Algorithm:
1. Start the program.
2. Write a Python function `fibonacci(n)` that returns the Fibonacci sequence up to `n` terms.
3. Create a separate test file named **TEST\_EX14.py**.
4. Inside it, write test functions with `assert` statements for different test cases.
5. Run the tests using the command:
   ```bash
   pytest -s TEST_EX14.py
   ```
6. If all assertions pass, the function is correct.

## Program:
**EX14.py**
```python
def fibonacci(n):
    seq = []
    a, b = 0, 1
    for _ in range(n):
        seq.append(a)
        a, b = b, a + b
    return seq
```

**TEST_EX14.py**
```python
from EX14 import fibonacci
def test_fibonacci():
    print("fibonacci(5) =", fibonacci(5))       
    assert fibonacci(5) == [0,1,1,2,3]
    print("fibonacci(10) =", fibonacci(10))     
    assert fibonacci(10) == [0,1,1,2,3,5,8,13,21,34]
    print("fibonacci(1) =", fibonacci(1))       
    assert fibonacci(1) == [0]
    print("fibonacci(0) =", fibonacci(0))      
    assert fibonacci(0) == []
```

## Output:

<img width="1277" height="270" alt="image" src="https://github.com/user-attachments/assets/2b645743-f9b6-45f8-8829-6593c444aa9c" />

## **Result:**
Thus, the Pytest program for Fibonacci Series (EX14.py & TEST_EX14.py) was successfully written, executed, and tested. 
