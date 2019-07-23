# Workshop

## 문제1

2개의 숫자를 인자로 받아 더하기, 빼기, 곱하기, 나누기 연산의 결과를 반환하는 4개의 함수를 calc.py에 작성하시오. 단, 나누기 연산에서는 try except 구문을 사용하여 ‘0’으로 나누려고 하는 경우에는 문자열 ’0으로는 나눌 수 없습니다.’을 반환하시오.

```python
def calc_add(x, y):
    return x + y
def calc_sub(x, y):
    return x - y
def calc_mul(x, y):
    return x * y
def calc_div(x, y):
    try:
        result x / y
    except ZeroDivisionError:
        print('0으로는 나눌 수 없습니다.')
    else:
        return result

```



## 문제2

1번에서 작성한 calc.py 모듈을 import하여, 각 연산을 수행하는 함수들을 실행하는 코드를 작성하시오.

```python
from calc import calc_add as add
from calc import calc_sub as sub
from calc import calc_mul as mul
from calc import calc_div as div

print(add(5, 5))
print(sub(5, 5))
print(mul(5, 5))
print(div(5, 5))
div(5, 0)

'''
결과: 
10
0
25
1.0
0으로는 나눌 수 없습니다.
'''
```

