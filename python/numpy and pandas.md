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