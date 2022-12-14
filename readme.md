프로그래머스 연습문제 > 귤 고르기

> https://school.programmers.co.kr/learn/courses/30/lessons/138476

```
import collections

def solution(k, tangerine):
    dict = collections.Counter(tangerine)
    list = dict.most_common()
    print(dict)
    print(list)
    index = 0
    sum = 0
    for (key,value) in list:
        print(key,":",value)
        sum = sum + value
        # print("sum : ",sum)
        index = index+1
        if sum >= k:
            break
    return index
```
