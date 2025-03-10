# IRS
IRS: A Large Synthetic Indoor Robotics Stereo Dataset for Disparity and Surface Normal Estimation

# Introduction

**IRS** is an open dataset for indoor robotics vision tasks, especially disparity and surface normal estimation. It contains totally 103,316 samples covering a wide range of indoor scenes, such as home, office, store and restaurant. 

|<img src="/imgs/left.png" width="100%" > | <img src="/imgs/right.png" width="100%" > |
|:--:|:--:|
|Left image|Right image|
|<img src="/imgs/disparity.png" width="100%" > | <img src="/imgs/normal.png" width="100%" > | 
|Disparity map|Surface normal map|

*****

# Overview of IRS

Rendering Characteristic|Options
:--|:--:
indoor scene class|home(31145), office(43417), restaurant(22058), store(6696)
object class|desk, chair, sofa, glass, mirror, bed, bedside table, lamp, wardrobe, etc.
brightness|over-exposure(>1300), darkness(>1700)
light behavior|bloom(>1700), lens flare(>1700), glass transmission(>3600), mirror reflection(>3600)

We give some sample of different indoor scene characteristics as follows.

|<img src="/imgs/home.png" width="100%" > | <img src="/imgs/office.png" width="100%">  | <img src="/imgs/restaurant.png" width="100%" >|
|:--:|:--:|:--:|
|Home|Office|Restaurant|
|<img src="/imgs/normal_light.png" width="100%" > | <img src="/imgs/over_exposure.png" width="100%" > | <img src="/imgs/dark.png" width="100%" >|
|Normal light|Over exposure|Darkness|
|<img src="/imgs/glass.png" width="100%" > | <img src="/imgs/mirror.png" width="100%" > | <img src="/imgs/metal.png" width="100%" >|
|Glass|Mirror|Metal|

# Network Structure of DispNormNet

We design a novel network, namely DispNormNet, to estimate the disparity map and surface normal map together of the input stereo images. DispNormNet is comprised of two modules, DispNetC and NormNetDF. **[DispNetC](https://arxiv.org/pdf/1512.02134.pdf)** is identical to that in **[this paper](https://arxiv.org/pdf/1512.02134.pdf)** and produces the disparity map. NormNetDF produces the normal map and is similar to **[DispNetS](https://arxiv.org/pdf/1512.02134.pdf)**. "DF" indicates disparity feature fusion, which we found important to produce accurate surface normal maps.

<div align="center">
<img src="/imgs/DispNormNet.png" width="100%" >
DispNormNet
</div>

# Paper
Q. Wang<sup>*,1</sup>, S. Zheng<sup>*,1</sup>, Q. Yan<sup>*,2</sup>, F. Deng<sup>2</sup>, K. Zhao<sup>&#8224;,1</sup>, X. Chu<sup>&#8224;,1</sup>.

IRS : A Large Synthetic Indoor Robotics Stereo Dataset for Disparity and Surface Normal Estimation. [\[preprint\]](/pdfs/IRS_indoor_robotics_stereo_dataset.pdf)

<font size=2>
* indicates equal contribution. &#8224; indicates corresponding authors.<br>
<sup>1</sup>Department of Computer Science, Hong Kong Baptist University. <sup>2</sup>School of Geodesy and Geomatics, Wuhan University.
</font>

<!--
Q. Wang<sup>*,1</sup>, S. Zheng<sup>*,1</sup>, Q. Yan<sup>*,2</sup>, F. Deng<sup>2</sup>, K. Zhao<sup>&#8224;,1</sup>, X. Chu<sup>&#8224;,1</sup>.[preprint](/pdfs/IRS_indoor_robotics_stereo_dataset.pdf)

[IRS : A Large Synthetic Indoor Robotics Stereo Dataset for Disparity and Surface Normal Estimation](https://www.github.com)

<font size=2>
* indicates equal contribution. &#8224; indicates corresponding authors.<br>
<sup>1</sup>Department of Computer Science, Hong Kong Baptist University. <sup>2</sup>School of Geodesy and Geomatics, Wuhan University.
</font>

-->

# Download 
You can use the following BaiduYun link to download our dataset. More download links, including Google Drive and OneDrive, will be provided soon.

BaiduYun: <a href="https://pan.baidu.com/s/1VKVVdljNdhoyJ8JdQUCwKQ" target="_blank">https://pan.baidu.com/s/1VKVVdljNdhoyJ8JdQUCwKQ</a>

# Video Demonstration

<!--
<iframe width="560" height="315" src="https://www.youtube.com/embed/jThNQFHNU_s" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
-->

[![IRS Dataset and DispNormNet](http://img.youtube.com/vi/jThNQFHNU_s/0.jpg)](http://www.youtube.com/watch?v=jThNQFHNU_s)

# Contact

Please contact us at [qiangwang@comp.hkbu.edu.hk](mailto:qiangwang@comp.hkbu.edu.hk) if you have any question. 
