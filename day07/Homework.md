# Homework

다음은 더하기 기능만이 구현된 간단한 Calculator 클래스이다.

```python
class Calculator:
    count = 0

    def info(self):
        print('나는 계산기 입니다.')

    @staticmethod
    def add(a, b):
        Calculator.count += 1
        print(f'{a} + {b} 는 {a + b}입니다.')

    @classmethod
    def history(cls):
        print(f'총 {cls.count}번 계산 했습니다.')
```



## 문제1

인스턴스 메서드, 스태틱 메서드, 클래스 메서드에 해당 하는 함수가 무엇인지 작성하시오.

```python
# 인스턴스 메서드
	def info(self):
        print('나는 계산기 입니다.')
        
# 스태틱 메서드
	@staticmethod
    def add(a, b):
        Calculator.count += 1
        print(f'{a} + {b} 는 {a + b}입니다.')
        
# 클래스 메서드
	@classmethod
    def history(cls):
        print(f'총 {cls.count}번 계산 했습니다.')
```





## 문제2

각각의 함수(메서드)를 실행하는 코드를 작성하시오.

```python
cal = Calculator() # 인스턴스 생성

cal.info() # 인스턴스를 통해 인스턴스 메서드 실행
Calculator.info() # 클래스를 통해 인스턴스 메서드 실행 => 오류발생
Calculator.info(cal) # 클래스를 통해 인스턴스 메서드 실행
'''
결과:
1. 나는 계산기 입니다.
2. TypeError: info() missing 1 required positional argument: 'self'
3. 나는 계산기 입니다.
'''
'''
인스턴스 메서드를 실행시키는 2번 코드를 통해 클래스를 통하면 self가 지정이 되지 않음을 알 수 있다. 인스턴스를 생성하게 되면 self가 지정이 되는 것을 확인할 수 있다.
'''

cal.add(1, 2) # 인스턴스를 통해 스태틱 메서드 실행
Calculator.add(1, 2) # 클래스를 통해 스태틱 메서드 실행
'''
결과:
1. 1 + 2 는 3입니다.
2. 1 + 2 는 3입니다.
'''
'''
인스턴스, 클래스 둘 다 스태틱 메서드에 접근이 가능함을 알 수 있다.
'''

Calculator.history() # 클래스를 통해 클래스 메서드 실행
cal.history() # 인스턴스를 통해 스태틱 메서드 실행
'''
결과:
1. 총 2번 계산 했습니다.
2. 총 2번 계산 했습니다.
'''
'''
인스턴스, 클래스 둘 다 클래스 메서드에 접근이 가능함을 알 수 있다.
'''

```





## 문제3

파라미터 self와 cls에는 어떤 값이 할당 되는지 작성하시오.

```python
cal = Calculator() # 인스턴스 생성

Calculator.info() # 클래스를 통해 인스턴스 메서드 실행 => 오류발생
Calculator.info(cal) # 클래스를 통해 인스턴스 메서드 실행
'''
위의 코드를 통해 인스턴스를 생성했을 때 self에 cal이라는 인스턴스가 들어감을 알 수 있다.
'''

	@classmethod
    def history(cls):
        print(f'총 {cls.count}번 계산 했습니다.')
'''
위 코드에서 cls는 클래스 객체로 Calculator가 들어가게 된다.
확인하는 법?
'''
```



