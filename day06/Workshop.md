# Workshop

아래와 같은 클래스 Circle이 있을 때, 반지름이 3이고 x, y 좌표가 (2, 4)인 원을 만들어 넓이와 둘레를 출력하시오.

```python
class Circle:
    pi = 3.14 # instance
    x = 0
    y = 0
    r = 0

    def __init__(self, r, x, y): # 생성자
        self.r = r
        self.x = x
        self.y = y

    def area(self): # area method
        return self.pi * self.r * self.r
    
    def circumference(self): # circumference method
        return 2 * self.pi * self.r

    def center(self): # center method
        return (self.x, self.y)

ex_circle = Circle(3, 2, 4) # 생성자 호출
print(f'해당 원의 넓이는 {round(ex_circle.area(), 2)}입니다.') #area method 호출
print(f'해당 원의 둘레는 {ex_circle.circumference()}입니다.') # circumference method 호출
print(f'해당 원 중심의 좌표는 {ex_circle.center()}입니다.') # center method 호출
```

