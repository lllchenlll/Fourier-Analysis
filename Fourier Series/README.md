### 傅里叶级数 Fourier series

    什么是傅里叶级数（三角级数）： 任何 *周期函数* 均可用正弦及余弦函数构成的无穷级数来表示。
    PS1：基函数为sin\cos是因为其相互正交，且是二阶偏微分方程的的本征解。
    PS2：泰勒函数同样是对函数的展开（指数展开），其可以观察函数不同阶的导数来判断函数的变化程度。

    对一个周期函数来说，其还有包含频率等在内在因素。
    频率表示了周期性变化的快慢。
    	
    傅里叶级数的公式：
    
<div align=center><img src="https://latex.codecogs.com/gif.latex?f(x)=a_{0}&plus;\sum_{n=0}^{\infty}(a_{n}\cos\frac{n\pi&space;x}{l}&plus;b_{n}\sin\frac{n\pi&space;x}{l})" title="f(x)=a_{0}+\sum_{n=0}^{\infty}(a_{n}\cos\frac{n\pi x}{l}+b_{n}\sin\frac{n\pi x}{l})" /></div>

    l是周期的一半，意味着上面的公式可以表示任一周期为2l的周期函数。
    简单来说，傅里叶级数将周期函数拆分为 常量（直流分量） + 1倍频分量 + 2倍频分量 + ... +
    
    公式中的正弦与余弦函数系数可由函数投影进行计算，类比于向量投影（即向量内积），两个函数的内积为二者相乘后在全区间的积分。
    
<div align=center><img src="https://latex.codecogs.com/gif.latex?\left&space;\langle&space;u,v&space;\right&space;\rangle:=\int_{a}^{b}u(x)\bar{v}(x)dx" title="\left \langle u,v \right \rangle:=\int_{a}^{b}u(x)\bar{v}(x)dx" /></div>

参考网址：
1. [到底神马是傅里叶级数！](https://blog.csdn.net/Edin_BlackPoint/article/details/53581902)
