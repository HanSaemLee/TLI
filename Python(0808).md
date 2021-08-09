# Python(0808)

## Numerical Python(Numpy) - part 1

```python
# de facto standard(사실상의 표준)
import numpy as np
```



### 1. Numpy Dimensional array

```python
a = np.array([1, 4, 5, 8], float)
------
출력 : array([1., 4., 5., 8.,])
```



### 2. Array shape

```python
# Vector(1차원)
vector = np.array([1, 4, 5, 8])
vectoor.shape
------
출력 : (4,)
```

- 1차원인 vector.shape를 입력하면  열의 개수를 튜플형태로 반환



```python
# Matrix(2차원)
matrix = np.array([1, 2, 3], [4, 5, 6])
print(matrix.shape) # 행이 2개 열이 3개
print(matrix)		# [[1 2 3][4 5 6]] (콤마, 없음주의)
```



```python
tensor = np.arange(1, 25).reshape(2, 3, 4)
print(tensor)
------
출력 : [[[  1  2  3  4]
      	[  5  6  7  8]
      	[  9 10 11 12]]
      [[ 13 14 15 16]
       [ 17 18 19 20]
       [ 21 22 23 24]]
```

- .reshape(2, 3, 4) - 큰 두개의 묶음 2와 3행 4열을 의미

```
vector.size, matrix.size, tensor.size
------
size는 원소의 총 개수를 출력
```

