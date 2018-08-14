### 傅里叶变换 Fourier Transform

    傅里叶变换：与傅里叶级数不同，傅里叶变换将时域离散（非周期）的连续信号转换为一个频域非周期的连续信号。
    PS1：可以将时域信号理解为周期无限大的函数
    PS2：正是由于频域中的谱变得连续，傅里叶级数中的求和变为了积分
    
<div align=center><img width="310" height="250" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Fourier_unit_pulse.svg/800px-Fourier_unit_pulse.svg.png"/></div>

    如果将函数的观察空间拓展到虚数空间，我们就可以发现正弦波的叠加是e^{it}在实数空间的投影。
    假设有一条是实数轴，乘以-1表示实数轴反向，那么乘以i（i^{2}=-1）则表示实数轴旋转90度成为虚数轴。
    通过欧拉公式：
    
<div align=center><img src="https://latex.codecogs.com/gif.latex?e^{ix}=\cos&space;x&plus;i\sin&space;x" title="e^{ix}=\cos x+i\sin x"/></div>

    我们可以发现e^{it}表示一条在复频域逆时针旋转的螺旋线（类似弹簧），其实部投影为cos(x)，虚部投影为sin(x)。
    
<div align=center><img src="https://pic2.zhimg.com/80/v2-5d7bcbf6454b2612da47e85bdbab99e5_hd.jpg"/></div>
<div align=center><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Euler%27s_Formula_c.png/330px-Euler%27s_Formula_c.png"/></div>

    当e^{it}与e^{-it}相加时，两条旋转方向不同的螺旋线进行了叠加，虚数部分进行了抵消：
    
<div align=center><img src="https://latex.codecogs.com/gif.latex?\cos(x)=\frac{e^{it}&plus;e^{-it}}{2}" title="\cos(x)=\frac{e^{it}+e^{-it}}{2}" /></div>


参考资料
1. [傅里叶分析之掐死教程（完整版）](https://zhuanlan.zhihu.com/p/19763358)
2. [如何理解傅里叶变换公式？](https://www.zhihu.com/question/19714540)
