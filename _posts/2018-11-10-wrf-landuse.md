---
layout:   post
title:    珠三角土地覆被资料优选及在WRF模式中的初步应用
subtitle:   文献阅读
date:   2018-11-10
author:     tttchy   #写文章的作者是谁
catalog:    ture
tags:    
      landcover 
      WRF
      pearl-delta-region    #前面加-会使其再多一个框 ,可添加多个标签,,#号健为注释的作用 模块的开始必须以---开头，不然会出现错误
---



文献发表时间2014-8

![icon](https://github.com/tttchy/pictures/blob/master/landuse.png?raw=true)

模式内置modis资料在东莞、佛山、中山区域对建成区面积高估超过10倍，在而在广州、惠州、江门、珠海对建成区面积高估约1倍，在肇庆和深圳相对合理；glc2010低估，glc2009高估，但偏差小于250km2. （文献同时也探讨了对林业，农业等的讨论）

![icon](https://github.com/tttchy/pictures/blob/master/land%20area%20rate%20.png?raw=true)

结合表 2 可以看出， 在整个珠三角地区内置的MODIS 资料对建成区面积高估超过 3 倍， 在部分城市高估超过 10 倍，这样的高估导致模拟城市化研究时，往往对地表温度等结果有所高估， 收集到的资料中 GLC2009 和 CAS2005 资料对建成区面积虽然也有一定的高估， 但在各城市高估的比例并不大．


模式选取的物理参数化方案包括: Lin 微物理过程参数化方案， Goddard 短波辐射方案， rrtmg 长波辐射方案，MYJ 边界层方案， Noah 陆面过程方案和 BEP 城市方案． 在本研究中， 用于对比土地覆被资料是: 转换为 USGS24 种类型的内置 MODIS 资料和 GLC2009资料。

![icon](https://github.com/tttchy/pictures/blob/master/The%20spatial%20distribution%20of%20MODIS%20and%20GLC2009%20land%20cover%20types%20in%20the%20Pearl%20%EF%BC%B2iver%20Delta%20region.png?raw=true)


![icon](https://github.com/tttchy/pictures/blob/master/Main%20physical%20parameters.png?raw=true)
在陆面方案中，对城市区域和非城市区域地表变量的计算是分开的


结论：1、从整体上看， 土地覆被资料的更新能够改善模式对珠三角区域的温度、风速和水汽压的模拟， 且其中 10 m 风速对于土地覆被格局的改变最为敏感。
     2、土地覆被类型及其比例的改变直接影响地表反照率、粗糙度、植被覆盖率、气孔阻抗、可见光辐射和水汽压差等参数， 而这些参数在陆面过程方案和城市方案中会对地表能量收支平衡和水汽平衡产生影响，而能量和水汽平衡的改变将会对模拟场中空气污染物的扩散和传输造成影响．
