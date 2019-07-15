# Homework

## 1번문제

```python
'''
False, None, True, and, as, assert, break, class, continue, def, del, elif, else, except, finally, for, from, global, if, import, in, is, lambda, nonlocal, not, or, pass, raise, return, try, while, with, yield
'''
```



## 2번 문제

```python
# 문제 상황
a = 0.1 * 3
b = 0.3

print(a==b)
'''
결과 : False
'''

# 기본적인 처리방법
a = 0.1 * 3
b = 0.3
c = abs(a - b) <= 1e-10
print(c)

'''
결과 : True
'''

# sys 모듈을 통해 처리하는 방법
a = 0.1 * 3
b = 0.3
import sys
c = abs(a - b) <= sys.float_info.epsilon
print(c)

'''
결과 : False
'''

# math 모듈을 통해 처리하는 법
a = 0.1 * 3
b = 0.3
import math
c = math.isclose(a, b)
print(c)

```



## 3번 문제

```python
# 1) \n
print('안녕하세요.\n저는 박재성입니다.')

'''
안녕하세요.
저는 박재성입니다.
'''

# 2) \t
print('안녕하세요.\t저는 박재성입니다.')
'''
안녕하세요.	저는 박재성입니다.
'''

# 3) \\
print('안녕하세요.\\저는 박재성입니다.')
'''
안녕하세요.\저는 박재성입니다.
'''

```



## 4번 문제

```python
# 1) %-formatting을 활용
name = '철수'
print('안녕, %s' % name)

'''
안녕, 철수
'''

# 2) str.format()을 활용
print('안녕, {}', .format(name))
'''
안녕, 철수
'''

# 3) f-string을 활용
name = '철수'
print(f'안녕, {name}')
'''
안녕, 철수
'''
```



## 5번 문제

```python
# 답: int('3.5')
'''
float형 값이 str 내부에 있으면 int형으로 변환할 수 없다.
'''
```

