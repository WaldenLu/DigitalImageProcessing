# DigitalImageProcessing
高级图像处理课程实验
### 实验内容
* 利用 OpenCV 读取图像。
    > 具体内容：用打开 OpenCV 打开图像，并在窗口中显示
* 灰度图像二值化处理
    > 具体内容：设置并调整阈值对图像进行二值化处理。
* 灰度图像的对数变换
    > 具体内容：设置并调整 r 值对图像进行对数变换。
* 灰度图像的伽马变换
    > 具体内容：设置并调整γ值对图像进行伽马变换。
* 彩色图像的补色变换
    > 具体内容：对彩色图像进行补色变换。

### 实验方法
######  对灰度图像的处理：
首先使用imread()读取目标图像为灰度图。    

**二值化**：对每个像素遍历，判断其灰度值，当灰度值大于某一参数时，置灰度值为255，小于时置0。  

**对数变换**：对数变换主要用于将图像的低灰度值部分扩展，将其高灰度值部分压缩，以达到强调图像低灰度部分的目的。  

**伽马变换** ：主要用于图像的校正，将漂白的图片或者是过黑的图片，进行修正。伽马变换也常常用于显示屏的校正，这是一个非常常用的变换。
其输入为[0,1]，其输出也为[0,1]。   

######  对彩色图像的处理
**补色变换**：对RGB颜色取补色，即取色盘上180°角对应的颜色。
例如：R55,G255,B0对应的补色为R200，G0，B255。
