# Data-enhancement
**2022/10/22 修改了github代码导致xmax<xmin的情况。（由于上传疏忽，正确的代码修改了后上传的错误的版本）**

Support data enhancement when there are few data sets（支持数据集较少的情况进行数据增强，包含随机的多种变化）
这是数据集扩增的一个小工具，在您想使用yolo等目标检测算法时数据集较少的情况下能够进行变化增强图片，丰富您的数据集。
(支持LabelIMg和LabelMe标注的文件)
包括3个python文件

（rename_file.py、DataAugmentforLabelImg.py和DataAugmentforLabelMe.py）
原文链接：https://blog.csdn.net/qq_39740357/article/details/123258697

1. rename_file.py能实现文件的重命名,注意修改文件的路径
2. DataAugmentforLabelImg.py能实现LabelImg标注后的图片的增强（包括模糊，亮度，裁剪，旋转，平移，镜像等变化）
3. DataAugmentforLabelMe.py能实现LabelMe标注后的图片的增强（包括模糊、亮度、平移、镜像等变化）

**注意：一些包的安装是必要的，比如Opencv_python等**
<br>
##*将您需要增强的图片放在对应的文件夹即可，具体可参考demo给出的图片和xml文件存放路径，您放入即可*
<br>
**保存结果：**<br>

1. 目标检测增强后的图片默认会保存在./data/Images2中，xml文件会保存在./data/Annotations2中（包括新的图片和xml文件）<br>
2. 目标分割增强后的图片默认会保存在./data2中（包括新的图片和json文件）
   <br>

**实现这个工具参考了：**<br>
https://github.com/maozezhong/CV_ToolBox/blob/master/DataAugForObjectDetection/
