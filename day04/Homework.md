# Homework

## 문제1

Python에서 변수를 찾을 때 접근하는 이름 공간을 순서대로 작성하시오.

```python
'''
Local namespace => Enclosed namespace => Global namespace => Built-in namespace
'''
```



## 문제2

다음 중 옳지 않은 것을 고르시오.
(1) 함수는 오직 하나의 객체만 반환할 수 있어서, ‘return a, b’처럼 쓸 수 없다.
(2) 함수에서 return을 작성하지 않으면 None 값을 반환한다.
(3) 함수의 인자(parameter)는 함수를 선언할 때 설정한 값이며,
인수(argument)는 함수를 호출할 때 넘겨주는 값이다.
(4) 가변 인자를 설정할 때는 인자 앞에 *을 붙이고, 이 때는 함수 내에서 tuple로 처리된다.

```python
'''
답 : 1
'''

# (1) 함수는 오직 하나의 객체만 반환할 수 있어서, ‘return a, b’처럼 쓸 수 없다.(x)
def func():
    a = 0
    b = 0
    return a, b

print(func())
'''
결과)
(0, 0)
'''

# (2) 함수에서 return을 작성하지 않으면 None 값을 반환한다.(o)
def func():
    a = 0
    b = 0
    
print(func())
'''
결과
None
'''

# (3) 함수의 인자(parameter)는 함수를 선언할 때 설정한 값이며, 인수(argument)는 함수를 호출할 때 넘겨주는 값이다.(o)
# parameter (매개변수)
# 함수의 정의 부분에 나열되어 있는 변수, 여기서는 plus 함수 정의시에 사용되는 a, b를 parameter(매개변수) 라고 한다.
def plus(a, b):
  return a + b

# argument (전달인자)
# 함수를 호출할때 전달 되는 실제 값, 여기서는 plus 라는 함수에 넣어주는 값 1, 2를 argument(전달인자)라고 한다.
result = plus(1, 2)

# 참고 : https://wayhome25.github.io/etc/2017/12/31/parameter-argument/

# (4) 가변 인자를 설정할 때는 인자 앞에 *을 붙이고, 이 때는 함수 내에서 tuple로 처리된다.(o)
def my_func(*args, second_arg = 'second'):
    print(type(args))

my_func('a', 'b', 'c', 'd')
'''
<class 'tuple'>
'''

```



## 문제3

재귀 함수를 쓰는 장점과 단점을 작성하시오.

``` python
'''
# 장점
 - 재귀를 썼을 때 직관적인 로직들이 존재하기 때문에 알고리즘 자체가 재귀적인 표현이 자연스러울 수 있다.
 - 재귀 호출은 '변수 사용'을 줄여줄 수 있다.
 
 # 단점
  - 많은 함수를 생성하기 때문에 반복에 비해 많이 느리다.
'''
```



