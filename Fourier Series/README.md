### 傅里叶级数 Fourier series

    什么是傅里叶级数（三角级数）： 任何 '周期函数' 均可用正弦及余弦函数构成的无穷级数来表示。
    PS1：基函数为sin\cos是因为其相互正交，且是二阶偏微分方程的的本征解。
    PS2：泰勒函数(需要满足n阶导数必须存在)同样是对函数的展开（指数展开），其可以观察函数不同阶的导数来判断函数的变化程度。
    PS3：三角函数具有微积分不变性（形状不变，只改变幅值和相位） 

![fourier](https://upload.wikimedia.org/wikipedia/commons/2/2b/Fourier_series_and_transform.gif)

    对一个周期函数来说，其还有包含频率等在内在因素。
    频率表示了周期性变化的快慢。
    	
    傅里叶级数的公式：
    
<div align=center><img src="https://latex.codecogs.com/gif.latex?f(x)=a_{0}&plus;\sum_{n=0}^{\infty}(a_{n}\cos\frac{n\pi&space;x}{l}&plus;b_{n}\sin\frac{n\pi&space;x}{l})" title="f(x)=a_{0}+\sum_{n=0}^{\infty}(a_{n}\cos\frac{n\pi x}{l}+b_{n}\sin\frac{n\pi x}{l})" /></div>

    l是周期的一半，意味着上面的公式可以表示任一周期为2l的周期函数。
    简单来说，傅里叶级数将周期函数拆分为 常量（直流分量） + 1倍频分量 + 2倍频分量 + ... +
    
    公式中的正弦与余弦函数系数可由函数投影进行计算，类比于向量投影（即向量内积），两个函数的内积为二者相乘后在全区间的积分。
    
<div align=center><img src="https://latex.codecogs.com/gif.latex?\left&space;\langle&space;u,v&space;\right&space;\rangle:=\int_{a}^{b}u(x)\bar{v}(x)dx" title="\left \langle u,v \right \rangle:=\int_{a}^{b}u(x)\bar{v}(x)dx" /></div>

    每个分量的系数计算来源于f(x)在各个分量下做投影的结果，即相乘做积分
    PS: 各个分量需用完备正交基表示，即两两相乘积分(一个周期内)为0，自身乘方积分为1
    
<div align=center><img src="https://latex.codecogs.com/gif.latex?a_{0}=\frac{\left&space;\langle&space;f,1&space;\right&space;\rangle}{\left&space;\langle&space;1,1&space;\right&space;\rangle}=\frac{\int_{-l}^{l}f(x)dx}{\int_{-l}^{l}dx}=\frac{\int_{-l}^{l}f(x)dx}{2l}" title="a_{0}=\frac{\left \langle f,1 \right \rangle}{\left \langle 1,1 \right \rangle}=\frac{\int_{-l}^{l}f(x)dx}{\int_{-l}^{l}dx}=\frac{\int_{-l}^{l}f(x)dx}{2l}" /></div>
<div align=center><img src="https://latex.codecogs.com/gif.latex?a_{n}=\frac{\left&space;\langle&space;f,\cos\frac{n\pi&space;x}{l}&space;\right&space;\rangle}{\left&space;\langle&space;\cos\frac{n\pi&space;x}{l},\cos\frac{n\pi&space;x}{l}&space;\right&space;\rangle}=\frac{\int_{-l}^{l}f(x)\cos\frac{n\pi&space;x}{l}dx}{\int_{-l}^{l}\cos^{2}\frac{n\pi&space;x}{l}dx}=\frac{\int_{-l}^{l}f(x)\cos\frac{n\pi&space;x}{l}dx}{l}" title="a_{n}=\frac{\left \langle f,\cos\frac{n\pi x}{l} \right \rangle}{\left \langle \cos\frac{n\pi x}{l},\cos\frac{n\pi x}{l} \right \rangle}=\frac{\int_{-l}^{l}f(x)\cos\frac{n\pi x}{l}dx}{\int_{-l}^{l}\cos^{2}\frac{n\pi x}{l}dx}=\frac{\int_{-l}^{l}f(x)\cos\frac{n\pi x}{l}dx}{l}" /></div>
<div align=center><img src="https://latex.codecogs.com/gif.latex?b_{n}=\frac{\left&space;\langle&space;f,\sin\frac{n\pi&space;x}{l}&space;\right&space;\rangle}{\left&space;\langle&space;\sin\frac{n\pi&space;x}{l},\sin\frac{n\pi&space;x}{l}&space;\right&space;\rangle}=\frac{\int_{-l}^{l}f(x)\sin\frac{n\pi&space;x}{l}dx}{\int_{-l}^{l}\sin^{2}\frac{n\pi&space;x}{l}dx}=\frac{\int_{-l}^{l}f(x)\sin\frac{n\pi&space;x}{l}dx}{l}" title="b_{n}=\frac{\left \langle f,\sin\frac{n\pi x}{l} \right \rangle}{\left \langle \sin\frac{n\pi x}{l},\sin\frac{n\pi x}{l} \right \rangle}=\frac{\int_{-l}^{l}f(x)\sin\frac{n\pi x}{l}dx}{\int_{-l}^{l}\sin^{2}\frac{n\pi x}{l}dx}=\frac{\int_{-l}^{l}f(x)\sin\frac{n\pi x}{l}dx}{l}" /></div>

参考网址：
1. [到底神马是傅里叶级数！](https://blog.csdn.net/Edin_BlackPoint/article/details/53581902)
2. [傅里叶级数的理解与简单推导](https://blog.csdn.net/constantin_ouc/article/details/78881709)
3. [傅里叶分析之掐死教程（完整版）](https://zhuanlan.zhihu.com/p/19763358)
