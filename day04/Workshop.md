# Workshop

## 문제

- 양의 정수 x를 입력 받아 제곱근의 근사값을 반환하는 함수를 작성하세요.
- v sqrt() 사용 금지

```python
def sqt(x):
    max = float(x)
    min = 1
    result = (float(x) - 1) / 2
    
    while True:
        if float(x) - (result ** 2) > 0.0001:
            min = result
            result = (max + min) / 2
            
        elif float(x) - (result ** 2) < -0.0001:
            max = result
            result = (max + min) / 2
            
        else:
            break
    return result

num = input()
print(sqt(num))
print(sqt(num) ** 2)
          
'''
input : 6
output : 2.4495086669921875
output ** 2 : 6.000092709669843

input : 3
output : 1.7320556640625
output ** 2 : 3.000016823410988

input : 13
output : 3.6055526733398438
output ** 2 : 13.000010080228094
'''
```



