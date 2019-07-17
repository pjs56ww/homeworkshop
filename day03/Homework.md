# Homework

## 문제1

Python에서 기본으로 사용할 수 있는 Built in function 5개를 찾아서 작성하세요.

```python
'''
print()
str()
sum()
max()
len()
'''
```



## 문제2

다음과 같이 함수가 정의되어 있다. 보기 중, 오류가 발생하는 코드를 고르시오.

```python
'''
답 : 3
'''
# Homework p1

def ssafy(name, location = '서울'):
    print(f'{name}의 지역은 {location}입니다.')

#1
ssafy(location = '대전', name = '철수')
'''
결과: 
철수의 지역은 대전입니다.
'''

#2
ssafy('길동', location = '광주')
'''
결과: 
길동의 지역은 광주입니다.
'''

#3
ssafy(name = '허준', '구미')
'''
결과: 
SyntaxError: positional argument follows keyword argument
 => 키워드 인자는 반드시 위치 인자보다 뒤에 있어야함을 알 수 있다.
'''
```



## 문제3

다음과 같이 코드가 작성되어 있을 때, 변수 result에 저장된 값을 작성하시오.

```python
'''
답: None
'''

# Homework p2

def my_func(a, b):
    c = a + b
    print(c)

result = my_func(4, 7)
print(result)

'''
11
None
 => 함수 내에서 return으로 반환한 값이 없기 때문이다.
'''
```

