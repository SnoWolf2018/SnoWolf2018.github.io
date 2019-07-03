---
title: PythonPlotDemo
date: 2019/07/03 周三
categories:
- Python
tags:
- Python
---

```python
import matplotlib.pyplot as plt
import numpy as np
#测试用示例
t = np.arange(0.0, 2.0, 0.01)
s = 1 + np.sin(2*np.pi*t)
plt.close('all')#不加这一行，在jupyter notebook中无法显示曲线
plt.plot(t, s)
#设置坐标轴及标题
plt.xlabel('time (s)')
plt.ylabel('voltage (mV)')
plt.title('About as simple as it gets, folks')
plt.grid(True)
#输出图片
plt.savefig("test.png")
plt.show() #必须加括号！！
```