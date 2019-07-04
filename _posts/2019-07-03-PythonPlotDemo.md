---
title: PythonPlotDemo
date: 2019/07/03 周三
description: PythonPlotDemo is a simple demo for python .
categories:
- Python
tags:
- Python
---
<!-- more -->

## 运行备注
&ensp;&ensp;&ensp;&ensp;以下代码可在jupyter notebook中运行，也可在命令行中运行，无论在哪运行，最后一行的代码一定要有，否则曲线图无法正确显示。

```
plt.show()
```

```
Tips：Markdown关于首行缩进的运用
一个空格大小的表示：&ensp;或&#8194;，此时只要在相应需要缩进的段落前加上 4个 如上的标记即可，注意要带上分号。
两个空格的大小表示：&emsp;或&#8195;，同理，使用2个即可缩进2个汉字，推荐使用该方式。
```

## 代码示例
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

