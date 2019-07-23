# Homework

## 문제1

```python
def fibo_recursion(n):
    if n < 2:
        return n
    else:
        return fibo_recursion(n-1) + fibo_recursion(n-2)
```

위와 같은 코드가 fibo.py 파일에 작성되어 있을 때, 아래와 같이 함수를 실행할 수 있도록 하는 import 구문을 (A), (B), (C)를 채워 넣어 완성하시오.

```python
from fibo import fibo_recursion as recursion

print(recursion(4))

'''
결과 : 3
'''
```



## 문제2

다음 에러들이 어떠한 경우에 발생하는지 간단하게 작성하시오.
• ZeroDivisionError
• NameError
• TypeError
• IndexError
• KeyError
• ModuleNotFoundError
• ImportError

```python
# ZeroDivisionError
5 / 0
'''
Traceback (most recent call last):
  File "practice.py", line 1, in <module>
    5 / 0
ZeroDivisionError: division by zero
 => 0으로 나누기를 하게 되면 위와 같은 에러가 발생하게 된다.
'''
# NameError
sum(a, b)
'''
Traceback (most recent call last):
  File "practice.py", line 2, in <module>
    sum(a, b)
NameError: name 'a' is not defined
 => 정의되지 않은 변수를 사용하게 되면 위와 같은 에러가 발생한다.
'''
# TypeError
sum('abc', 3)
'''
Traceback (most recent call last):
  File "practice.py", line 2, in <module>
    sum('abc', 3)
TypeError: unsupported operand type(s) for +: 'int' and 'str'
 => 사용되는 변수의 자료형이 잘못되었을 경우 위와 같은 에러가 발생하게 된다.
'''
# IndexError
a_list = [1, 2, 3]
print(a_list[5])
'''
Traceback (most recent call last):
  File "practice.py", line 3, in <module>
    print(a_list[5])
IndexError: list index out of range
 => 정의된 list 내 범위에 없는 index를 사용하였을 때 위와 같은 에러가 발생하게 된다.
'''
# KeyError
a_dict = {'a' : 1, 'b' : 2, 'c' : 3}
print(a_dict['f'])
'''
Traceback (most recent call last):
  File "practice.py", line 3, in <module>
    print(a_dict['f'])
KeyError: 'f'
 => 정의된 dictionary 내에 있지 않은 key를 사용하였을 때 위와 같은 에러가 발생하게 된다.
'''
# ModuleNotFoundError
import Hi
'''
Traceback (most recent call last):
  File "practice.py", line 2, in <module>
    import Hi
ModuleNotFoundError: No module named 'Hi'
 => 정의되어 있지 않은 모듈을 불러왔을 때 위와 같은 에러가 발생하게 된다.
'''
# ImportError
from pprint import abc
'''
Traceback (most recent call last):
  File "practice.py", line 2, in <module>
    from pprint import abc
ImportError: cannot import name 'abc' from 'pprint' (C:\Users\student\AppData\Local\Programs\Python\Python37\lib\pprint.py)
 => 모듈 내에 존재하지 않은 것(?)을 불러 왔을 때 위와 같은 에러가 발생하게 된다.
'''
```



