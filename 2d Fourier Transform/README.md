### 二位离散傅里叶变换（图像傅里叶变换）

    定义：二维离散傅里叶变换是将图像从空域（space domain）转换至频域（frequency domain）的变换。
    应用：图像增强、图像去噪、图像边缘检测、图像特诊提取、图像压缩等。
    
    理论依据：传统的傅里叶变换
    
    二维傅里叶变换及逆变换公式如下：

<div align=center><img src="https://upload-images.jianshu.io/upload_images/4305587-b722ae259c0016cc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700"/></div>
<div align=center><img src="https://upload-images.jianshu.io/upload_images/4305587-9ab77de5b3d6da71.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700"/></div>
    
    公式中的x,y代表输入矩阵中的横纵坐标（0<=x<n,0<=y<m），其中f(x,y)代表m*n大小的矩阵，F(u,v)表示f(x,y)的傅里叶变换后的结果。
    u,v表示正余弦的频率，f(x,y)所在的坐标系为空域，F(u,v)所在坐标系为频域。
    频率矩阵中的每个点代表了一个频率为u,v的函数，当u=v=0时，代表了直流分量。
    如要将变换结果进行可视化，需要计算其频谱（F(u,v)的幅度），计算方法为：
    
<div align=center><img src="https://upload-images.jianshu.io/upload_images/4305587-39ec10307f4625c6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700"/></div>

    其中的R(u,v)表示F(u,v)的实部，I(u,c)表示F(u,v)的虚部。
    换一个思路来说，二维离散傅里叶变换具有可分离性，即其可分离为两次一维的离散傅里叶变换。
    其计算过程如下图所示

<div align=center><img src="https://img-blog.csdn.net/20180615210208158?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3RoZWNlbnRyeQ==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70"/></div>

    一个m*n的二维图像f(x,y)，先按行队列变量y做一次长度为n的一维离散傅里叶变换。
    再将计算结果按列向对变量x做一次长度为m的傅里叶变换就可以得到该图像的傅里叶变换结果。
    
    2维傅里叶变换一般会调整输出的xci
