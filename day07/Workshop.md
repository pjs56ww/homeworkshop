# Workshop

## 문제

아래와 같은 Animal 클래스가 있을 때, 해당 클래스를 상속 받아 아래 보기와 같이 동작하는 Dog 클래스와 Bird 클래스를 작성하시오.

```python
class Animal:
    def __init__(self, name):
        self.name = name

    def walk(self):
        print(f'{self.name}! 걷는다!')

    def eat(self):
        print(f'{self.name}! 먹는다!')
```



### Dog 클래스

```python
class Dog(Animal):
    def __init__(self, name): # Animal 클래스의 생성자를 상속
        super().__init__(name)

    def walk(self): # Animal 클래스의 walk 함수를 상속
        super().walk()

    def run(self): # Dog 클래스만의 run 함수 생성
        print(f'{self.name}! 달린다!')
```



### Bird 클래스

```python
class Bird(Animal):
    def __init__(self, name): # Animal 클래스의 생성자를 상속
        super().__init__(name)

    def walk(self): # Animal 클래스의 walk 함수를 상속
        super().walk()

    def eat(self): # Animal 클래스의 eat 함수를 상속
        super().eat()

    def fly(self): # Bird 클래스만의 fly 함수 생성
        print(f'{self.name}! 푸드덕!')
```



### main문

```python
dog = Dog('멍멍이') # Dog 클래스의 dog 인스턴스 생성
dog.walk()
dog.run()

bird = Bird('구구') # Bird 클래스의 bird 인스턴스 생성
bird.walk()
bird.eat()
bird.fly()
```



### 결과

```python
'''
멍멍이! 걷는다!
멍멍이! 달린다!
구구! 걷는다!
구구! 먹는다!
구구! 푸드덕!
'''
```

