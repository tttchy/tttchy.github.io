---
layout:   post
title:    应用城市冠层模式研究建筑物形态对城市边界层的影响
subtitle: 文献阅读  
date:   2018-11-10
author:     tttchy   #写文章的作者是谁
catalog:    ture
tags:    
      ucm
      Numerical-simulation
      Urban-boundary-layer
      Building-morphology    #前面加-会使其再多一个框 ,可添加多个标签,,#号健为注释的作用 模块的开始必须以---开头，不然会出现错误
---

城市冠层是指从建筑物顶部到地表的这一层，讨论一个城市的冠层结构变化应主要从以下几个方面进行:(1)城市区域水平范围的扩张,(2)建筑物高度的增加 ,(3)建筑物分布密度的变化等 。街渠是城市冠层的基本单位 ,通过改变街渠几何形态学参数(如街渠高度、街渠宽度以及建筑物宽度等)来描述城市冠层结构的变化 。街渠是城市冠层的基本单位 ,通过改变街渠几何形态学参数(如街渠高度、街渠宽度以及建筑物宽度等)来描述城市冠层结构的变化 

传统平板模式中处理城市区域地-气间相互作用时 ,并不考虑街渠几何形态的影响,通过加大地表动力学粗糙度以及降低反照率等方法来达到模拟城市气象环境的目的城市冠层对边界层的作用不只体现在动力作用方面，还有热力作用，城市冠层热力效应就是城市热岛现象形成的重要原因，对边界层结构由着重要影响。


城市冠层模式描述的主要是冠层内的辐射过程，根据城市冠层建筑物的几何特征细致地考虑了街渠内的辐射传输过程, 如:街渠中各表面对辐射的吸收、反射 、遮蔽以及多次反射吸收等过程。街渠中存在屋顶、路面和墙面 3 种表面,城市冠层模式的特点就是在这 3 种表面上分别建立能量平衡关系 ,计算表层温度和 3 种不同表面与相连大气间的热通量交换, 再根据不同表面所占比重算出街渠单元与上部大气间总的热通量交换,所以本文主要是从建筑物热力效应的角度来分析建筑物形态变化对城市边界层的影响, 同时通过引入与建筑物形态相关的动力学粗糙度和零平面位移来考虑建筑物对边界层的动力作用。

城市冠层模式在计算时做如下假定:研究区域内所有建筑物高度和宽度相同;沿道路延伸的两排建筑物与道路等长 ,且道路长度远大于建筑物宽度;研究区域内任何走向街渠存在的可能性都相同 。在3 种不同表面分别建立能量平衡关系 , 但是街渠内两面相对墙的物理过程大多是相同的, 比如天空可视因子 、墙面热力结构 、建筑物内部温度和对散射辐射的吸收等 ,因此并不分开考虑 。唯一不同的就是到达两面墙上的直接太阳辐射 , 会造成两面墙的表面温度不同 ,但是这种差异对街渠整体与上部大气间的热通量不会产生明显影响 

城市冠层模式具体计算流程如图 1 所示, 驱动冠层模式的气象要素有:冠层上部大气的风速 、气温以及向下长短波辐射通量 ,冠层的形态学参数包括 :街渠形态(长、宽 、高),各表面整层厚度, 墙面、路面和屋顶表面材料反照率, 以及表面材料的热力系数(热传导系数 、比辐射率、热容量),各表面的热力粗糙度和动力粗糙度等。
？？？？冠层有这么多的参数，如何针对不同的地区进行计算呢？？？？？  对于该篇文章由于其只是考虑从热力效应方面考虑建筑物形态变化对边界层的影响，所以文中也就只是提到了各能量通量的计算方式？？
城市冠层模式中计算各表面与相连大气的热量交换, 冠层整体与上部大气间的热量交换是对各表面热量通量进行权重后的结果,

![icon](https://github.com/tttchy/pictures/blob/master/The%20simulation%20flow%20chart%20of%20UCM.png?raw=true)

在城市中 ,由于垂直存在的墙面无形中增加了城市人为材料的表面积 , 使得权重不能简单应用 3 种面的面积比来计算, 而应使用式(1)来计算:
![icon](https://github.com/tttchy/pictures/blob/master/FLUX-canopy.png?raw=true)

敏感性实验：
城市区域只有建筑物和道路 ,所有建筑物都具有相同的高度和屋顶宽度,街道宽度也完全相同。根据屋顶宽度和街道宽度就可确定单位网格上的建筑物面积密度；当建筑物密度在30 %左右时 ,粗糙度最大,然后粗糙度随建筑物密度增大而降低 ;零平面位移随着建筑物密度的增大与建筑物高度越来越接近。每个试验的城市地区粗糙度 Z 0 和零平面位移高度 Z d 均由建筑物高度和密度值参看原文献的引用。
建筑物密度=屋顶宽度/（屋顶宽度+街渠宽度）

三点讨论：面积大小、高度变化、密度变化对边界层的影响。建筑物分布密度变化对地表热量通量和动量通量造成的影响比城市面积扩张和建筑物高度变化对地表通量的影响都要明显 。

！！！！讨论了不同城市面积对边界层结果和气象环境变化的影响：小城镇尺度，中等城市，大城市 （仅从面积的变化便可代表不同城市规模，怀疑？？？？）,
讨论了动量通量，热量通量，层结稳定度，湍能廓线，湍流扩散系数。:城市面积越大 ,模拟范围内农作物区面积就越小 ,农作物区域对城市区域所能影响的范围和程度都变小，面积扩张对气象环境造成的影响, 主要源于扩张使得周围环境的气象状况发生改变, 从而对城市区域的气象环境影响发生变化

摘 要 文中将城市冠层模式耦合到南京大学城市尺度边界层模式中, 通过模拟对比发现, 耦合模式对城市地区气温模拟结果更接近于观测值, 尤其是对城市地区夜间气温模拟的改进。 运用改进耦合模式通过多个敏感性试验的模拟, 从城市面积扩张、建筑物高度增加、建筑物分布密度变化等角度研究城市建筑物三维几何形态变化对城市边界层及城市气象环境的影响,试验结果表明:(1)城市面积扩张使得城市下垫面的热通量增大, 热力湍流活动增强, 动量通量输送增强, 城市湍能增大, 湍流扩散系数变大, 城市气温升高, 且对不同时刻城市区域大气层结稳定度均有不同程度的影响。(2)建筑物高度增加增大了城市下垫面的粗糙度和零平面位移, 同时也增大了城市街渠高宽比。 城市建筑物越高, 白天城市地区地表热通量越小, 城市上空大气温度越低, 平均风速减小, 湍能减小;夜间由于高大建筑物释放储热比低矮建筑物要多, 其热力湍流相对活跃, 地表热通量增大, 使得城市区域气温较高。(3)建筑物密度增大, 会减小城市下垫面的粗糙度同时增强街渠对辐射的影响。 建筑物密度增大在白天会减小地表热通量和动量通量, 使城市气温降低, 平均风速增大, 城市湍流活动能力减弱;夜间城市释放较多储热使得气温较高