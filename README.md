# Fourier-epicycles-drawer

Fourier Epicycles(Fouricle) 是一个MATLAB APP，它基于傅里叶级数理论，使用一系列周转圆绘制任意2D闭曲线。

我推荐通过[3Blue1Brown的视频](https://www.bilibili.com/video/BV1vt411N7Ti?spm_id_from=333.999.0.0)和[课程](https://www.3blue1brown.com/lessons/fourier-series)来了解关于傅里叶级数以及使用它画圆的方法，同时也推荐我编写的说明文档“原理及实现方法”，其中包含了我对它过程的理解以及使用MATLAB语言实现它的方法。文档中的实现代码只是初步的、便于读者理解其过程的简化版，如果读者感兴趣，可以在mlapp文件中查看源代码。说明文档推荐使用Markdown或HTML打开，因为PDF无法查看动图。

该APP基于MATLAB 2022a实现，并已在2021a以上版本测试，能够正常使用。

# 主要目标特性

| 特性                    | APP实现 | 文档 |
| ----------------------- | ------- | ---- |
| 用户手绘图像            | ✔️       | ✔️    |
| 加载/保存数据、保存动画 | ✔️       | ❌    |
| 绘图速度调节            | ✔️       | ❌    |
| 曲线平滑、采样          | ✔️       | ❌    |
| 线简化算法              | ❌       | ❌    |
| 对曲线关键点进行微调    | ❌       | ❌    |
| 描图画线                | ❌       | ❌    |
| 从图像自动生成曲线      | ❌       | ❌    |
| 绘制多条曲线            | ❌       | ❌    |
| 自动美化曲线            | ❌       | ❌    |

在未来版本中，采样操作将作为线简化算法的一种，其作用是使用尽可能少的点来尽可能还原用户绘制的曲线特性。平滑操作将作为自动美化曲线方法的一种，其作用是使用更平滑的曲线来代替用户手绘的曲线，甚至去猜出用户脑子想画但手画不出来的曲线。

# 致谢

本项目基于Víctor Martínez-Cagigal的 [Drawing with Fourier Epicycles](https://github.com/vicmarcag/Drawing-with-Fourier-Epicycles/releases/tag/1.1.0) 项目改进而成。本项目的动机起自于夕沉向我提出的想法。
