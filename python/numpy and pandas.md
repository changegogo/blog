## 数学计算

numpy and pandas

安装

windows:
pip install numpy
pip install pandas

OSX：
pip3 install numpy
pip3 install pandas

```python
# 将一个python二维数组转化为numpy数组
import numpy as np

array = np.array([[1,2,3],[2,3,4]])
print(array) #输出数组
print('number of dim:', array.ndim) #数组的维度
print('shape:', array.shape) #数组的行列数
print('size:', array.size) #数组的元素值
```

创建array有很多形式
关键字

array: 创建数组 <br>
dtype: 指定数据类型<br>
zeros: 创建数据全为0<br>
ones: 创建数据全为1<br>
empty: 创建数据接近0<br>
arrange: 按指定范围创建数据<br>
linspace: 创建线段<br><br>

创建数组<br>
```python
a=np.array([1,2,3])
print(a)
# [1,2,3]
```python

指定数据 dtype
```python
a=np.array([1,2,3], dtype=np.int)
print(a.dtype)
# int32
```

dtype包括
```python
int int64 float float32
```

创建特定数据
```python
a = np.array([[1,2,3],[2,3,4]]) # 2d举证 2行3列
print(a)
```

```python
[[1 2 3]
[2 3 4]]
```
创建全零数组<>br
```python
a = np.zeros((3,4)) # 数据全为0， 3行4列
```
创建全1数组，同时也能指定这些特定的数据的dtype:
```python
a = np.ones((3,4), dtype=np.float)
```
创建全空数组，其实每个字值都是接近于0的数：
```python
a=np.empty((3,4),dtype=float)
```
创建连续数组：
```python
a=np.arange(10,20,2)# 10-20的数据，2为步长
array([10,12,14,16,18])
```
使用reshape改变数据的形状
```python
a = np.arange(12).reshape((3,4)) # 3行4列， 0-11
```
用linespace创建线段型数据：
```python
a=np.linspace(1,10,20) # 开始1，结束10，分割成20个数据，生成线段
```
同样也能进行reshape工作：
```python
a=np.linspace(1,10,20).reshape((4,5)) 
```