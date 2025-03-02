# NURBS笔记

## 一、曲面和曲线

### 基本知识

代码

```python
from geomdl import fitting
from geomdl.visualization import VisMPL as vis

# The NURBS Book Ex9.1
points = ((0, 0), (3, 4), (-1, 4), (-4, 0), (-4, -3))
degree = 3  # cubic curve

# Do global curve interpolation
curve = fitting.interpolate_curve(points, degree)

# Plot the interpolated curve
curve.delta = 0.01
curve.vis = vis.VisCurve2D()
curve.render()
```



## 二、基函数



### 设置

