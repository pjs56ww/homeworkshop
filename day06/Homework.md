# Homework

## 문제1

Python은 객체 지향 프로그래밍 언어입니다. Python에서 기본적으로 정의되어 있는 클래스 5가지만 작성하시오.

```python
'''
list: []로 instantce를 받는다. attribute는 없으며, .append(), .pop()과 같은 method가 있다.
dict: {}로 instantce를 받는다. attribute는 없으며, .keys(), .values()와 같은 method가 있다.
str: ''로 instantce를 받는다. attribute는 없으며, .split(), .join()과 같은 method가 있다.
int: 0, 1과 같은 정수로 instance를 받는다. .real(), .imag()와 같은 attribute가 있으며, method는 없다.
그 외로
float
bool
complex
... 등이 있다.
'''
```



## 문제2

다음 매직 메서드의 역할을 간단하게 작성하시오.
• __init__
• __del__
• __str__
• __repr__

```python
# __init__은 생성자로 instance object가 생성될 때 자동으로 호출되는 함수이다.
# __del__은 소멸자로 instance object가 소멸될 때 자동으로 호출되는 함수이다.
# __str__은 객체의 문자열 버전을 반환한다.
# __repr__은 객체의 '출력될 수 있는 표현'을 문자열 형태로 반환한다.
```



## 문제3

아래 코드의 ‘.sort()’와 같이 문자열, 리스트, 딕셔너리 등을 조작할 때 사용하였던 것들은 클래스에 정의된 메서드들이었다. 이처럼 문자열, 리스트, 딕셔너리 등을 조작하는 메서드 3가지를 그 역할과 함께 작성하시오.

```python
numbers = [5, 1, 2]
numbers.sort()
print(numbers) #[1, 2, 5]
'''
1. str
1-1) str.split(): 문자열을 특정 구분자로 나눔
1-2) str.join(): 리스트를 특정 구분자를 포함해 문자열로 변환
2. list
2-1) list.index(value): 값을 이용하여 위치를 찾기
2-2) list.extend([value1, value2]): 리스트 뒤에 값을 추가 
2-3) list.insert(index, value): 원하는 위치에 값 추가
3. dict
3-1) dict.get(key, default): 키의 value를 리턴
3-2) dict.pop(key): 특정 키의 value를 리턴하고 삭제
3-3) dict.clear(): dictionary의 모든 요소를 삭제 
'''
```



