程序入口在：**TUM**的二进制，也就是`ros_tum_realtime.cc`文件。
几个参数的意义：
- path_to_prototxt  //模型文件，网络模型
- path_to_caffemodel //训练文件，训练好的权重参数
- path_to_pascal.png // 标签文件,上色的图片

程序的脑图：
![DS-SLAMcode](https://raw.githubusercontent.com/zhuhu00/img/master/DS-SLAMcode.png)

代码解读：
其他部分和ORB-SLAM2的代码一样了。主要解决的还是人的运动。在检测中，当一个特征点在人上，如果是动态，则整个区域都是运动特征点。
1. https://blog.csdn.net/qq_41623632/article/details/112911046
2. https://blog.csdn.net/qq_41623632/article/details/112966024
3. https://blog.csdn.net/qq_41623632/article/details/112972443
4. https://blog.csdn.net/qq_41623632/article/details/113406058
