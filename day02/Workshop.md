# Workshop

## 문제1

두 개의 정수 n과 m이 주어질 때, 반복문을 사용하여 별(*) 문자를 이용해 가로의 길이가 n, 세로의 길이가 m인 사각형을 출력하시오.

```python
# Workshop P1

n = 5
m = 9

for i in range(m):
    for j in range(n):
        print('*', end = '')
    print('\n', end = '')
    
'''
*****
*****
*****
*****
*****
*****
*****
*****
*****
'''
```



## 문제2

과목명과 점수가 담긴 딕셔너리가 있을 때, 평균 점수를 출력하시오.

```python
# Workshop P2

students = {'python': 80, 'algorithm': 99, 'django': 89, 'flask': 83}
sum_score = 0
avg_score = 0
for score in students.values():
    sum_score += score

avg_score = sum_score/4
print(f'학생들의 평균점수는 : {avg_score}')

'''
학생들의 평균점수는 : 87.75
'''
```

## 문제3

다음은 여러 사람의 혈액형(A, B, AB, O)에 대한 데이터이다. 반복문을 사용하여 key는 혈액형의 종류, value는 인원 수인 딕셔너리를 만들고 출력하시오.

```python
# Workshop P3

blood_types = ['A', 'B', 'A', 'O', 'AB', 'AB', 'O', 'A', 'B', 'O', 'B', 'AB']
num_of_blood = {}
count_A = 0
count_AB = 0
count_B = 0
count_O = 0

for blood_type in blood_types:
    if(blood_type == 'A'):
        count_A += 1
    elif(blood_type == 'B'):
        count_B += 1
    elif(blood_type == 'AB'):
        count_AB += 1
    else:
        count_O += 1

print(count_A)

num_of_blood['A'] = count_A
num_of_blood['B'] = count_B
num_of_blood['AB'] = count_AB
num_of_blood['O'] = count_O

print(num_of_blood)

'''
{'A': 3, 'B': 3, 'AB': 3, 'O': 3}
'''
```

