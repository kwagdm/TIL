### 코딩0708_한수



------





어떤 양의 정수 X의 각 자리가 등차수열을 이룬다면, 그 수를 한수라고 한다. 등차수열은 연속된 두 개의 수의 차이가 일정한 수열을 말한다. N이 주어졌을 때, 1보다 크거나 같고, N보다 작거나 같은 한수의 개수를 출력하는 프로그램을 작성하시오.

첫째 줄에 1,000보다 작거나 같은 자연수 N이 주어진다.

첫째 줄에 1보다 크거나 같고, N보다 작거나 같은 한수의 개수를 출력한다.



```python
N = input('put any natural number below 1001')


B = []
C = []

if len(N) <= 2:
  A = N

else:
  for i in range(100, int(N) + 1):
    B.append(str(i))

  for i in B:
    if int(i[0]) - int(i[1]) == int(i[1]) - int(i[2]):
      C.append(i)
  
  A = 99 + len(C)

print(A)

```



