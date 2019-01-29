---
layout:     post
title:      matplotlib
subtitle:   matplotlib usage
date:       2018-06-05
author:     YGW
header-img: img/post-bg-universe.jpg
catalog: true
tags:
    - python
---

## 三维图像
    ```python
    # f1 score curve
    import matplotlib.pyplot as plt
    from mpl_toolkits.mplot3d import Axes3D
    import numpy as np
    x = np.linspace(0.01, 1, 20)
    y = np.linspace(0.01, 1, 20)
    X, Y = np.meshgrid(x, y)
    print(X)
    print(Y)
    Z = 2*X*Y/(X+Y)
    fig = plt.figure()
    ax = fig.gca(projection='3d')
    ax.plot_surface(X, Y, Z, rstride=1, cstride=1, cmap='rainbow')
    plt.show()
    ```

## 


