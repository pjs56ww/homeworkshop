# Homework

## 문제1

아래 보기 중, 변경할 수 있는(mutable) 것과 변경 불가능한 것(immutable)을 구분 하시오. 

​                                    String List Tuple Range Set Dictionary



```python
#immutable : String Tuple Range
#muatable : List Dictionary Set
```



## 문제2

range와 slicing을 활용하여 1부터 50까지 숫자 중 홀수로 이루어진 리스트를 만드시오.

```python
# Homework P2

a_list = list(range(1, 51))
b_list = a_list[0:50:2]
print(b_list)

'''
[1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25, 27, 29, 31, 33, 35, 37, 39, 41, 43, 45, 47, 49]
'''
```



## 문제3

반 학생들의 정보를 이용하여 key는 이름, value는 나이인 딕셔너리를 만드시오.

```python
# Homework P3

student_dic = {'마준희': 27, '박재성': 27, '서종식': 26, '임진호': 26}
print(student_dic)

'''
{'마준희': 27, '박재성': 27, '서종식': 26, '임진호': 26}
'''
```

