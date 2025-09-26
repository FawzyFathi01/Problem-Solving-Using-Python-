## **Link Problem** : https://codeforces.com/problemset/problem/1985/C

## **Code**

```python
test = int(input())

for t in range(test):
    n = int(input())
    arr = list(map(int,input().split()))
    mx = 0
    s = 0
    arr_sum = []
    arr_mx = []

    for item in arr:
        s += item
        arr_sum.append(s)

    for item in arr:
        if item > mx:
            mx = item
        arr_mx.append(mx)

    cnt = 0
    for i in range(n):
        if (arr_mx[i] == (arr_sum[i]- arr_mx[i])):
            cnt+=1
    print(cnt)
```

## **Explain**
- 

## **Notes**
- 