

```python
import numpy as np
```


```python
# row * col
a = np.array([[10, 20, 30],[1, 2, 3]])
```


```python
a
```




    array([[10, 20, 30],
           [ 1,  2,  3]])




```python
a.shape
```




    (2, 3)




```python
np.sum(a,axis=0)
```




    array([11, 22, 33])




```python
# Always remeber to reshape, Don't work with rank #1 matrices
np.sum(a,axis=0).shape
```




    (3,)




```python
# Output is row vector
np.sum(a,axis=0).reshape(1,3)
```




    array([[11, 22, 33]])




```python
np.sum(a,axis=1)
```




    array([60,  6])




```python
np.sum(a,axis=1).shape
```




    (2,)




```python
# Output is col vector
np.sum(a,axis=1).reshape(2,1)
```




    array([[60],
           [ 6]])




```python
a = np.random.rand(3,1)
```


```python
# Coloum Vector
a
```




    array([[ 0.98228564],
           [ 0.46773212],
           [ 0.17529722]])




```python
a = a.reshape(1,3)
```


```python
# Row Vector
a
```




    array([[ 0.98228564,  0.46773212,  0.17529722]])


