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
dtype: 指定数据类型
zeros: 创建数据全为0
ones: 创建数据全为1
empty: 创建数据接近0
arrange: 按指定范围创建数据
linspace: 创建线段