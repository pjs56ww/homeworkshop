# Workshop

## 문제

- Palindrome은 앞에서부터 읽었을 때와 뒤에서부터 읽었을 때 같은 단어를 뜻한다.
  따라서, ‘a’ ‘nan’ ’토마토’ 모두 palindrome에 해당합니다.

- 단어를 입력받아 Palindrome을 검증하고 True나 False를 리턴하는
  함수 palindrome(word)를 만들어보세요.



```python
# Workshop ex1

def palindrome(word):
    word_list = []
    count = 0
    count2 = 0
    pal = True
    for i in word:
        word_list.append(i)
        count += 1
    
    for j in word:
        if count2 <= count / 2:
            if word_list[count2] != word_list[count - count2 - 1]:
                pal = False
                break
        count2 += 1
    return pal  

print(palindrome('토마토'))
'''
True
'''

print(palindrome('nan'))
'''
True
'''

print(palindrome('abba'))
'''
True
'''

print(palindrome('ssafy'))
'''
False
'''

# Workshop ex2

def palindrome(word):
    compare = word[::-1]
    if compare == word:
        return True
    else:
        return False
    

print(palindrome('토마토'))
'''
True
'''

print(palindrome('abbbba'))
'''
True
'''

print(palindrome('ssafy'))
'''
False
'''
```

