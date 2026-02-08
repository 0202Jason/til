## 비트 연산으로 부분집합 생성

```python
arr = [3, 6, 7, 1, 5, 4]

n = len(arr)

for i in range(1<<n):
    for j in range(n):
        if i & (1<<j):
            print(arr[j], end = ", ")
    print()
print()
```
