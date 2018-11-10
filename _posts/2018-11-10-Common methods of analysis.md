---
layout:   post
title:    simulation results and analysis
subtitle:   资料查阅
date:   2018-11-10
author:     tttchy   #写文章的作者是谁
catalog:    ture
tags:    
      landcover 
      WRF-MODEL
      pearl-delta-region    #前面加-会使其再多一个框 ,可添加多个标签,,#号健为注释的作用 模块的开始必须以---开头，不然会出现错误
---

常用的一些分析方法：Bias(偏差)：模拟值-观测值；均方根误差（RMSE）：持有疑问，在文献《珠三角土地覆盖资料优选及在wrf模式中的初步应用》常鸣中如图所示方法，用到的数据只有sim（图2，认为此公式有问题，明显和标准差一模一样），而网上均方根误差是模拟值与观测者偏差的平方与观测次数n比值的平方根(图3)，另外，对图3的疑惑，如果，多个模拟值，只有一个观测值怎么算（像标准差那样子？？），以及多个模拟值和多个观测值一一对应怎么算（如图3所示公式？？？）。

图1
![icon](https://github.com/tttchy/pictures/blob/master/R&NV.png?raw=true) 
图2
![icon](https://github.com/tttchy/pictures/blob/master/RMSE&Bias.png?raw=true)
图3
![icon](https://github.com/tttchy/pictures/blob/master/MSE%25RMSE.png?raw=true)
