## 指南针源码说明
## 指南针电路板说明
以下版本，在打板过后，都需要再购买屏幕模块和磁传感器模块，以及电池。

屏幕模块：8Pin插槽

磁传感器模块：QMC5883L电子罗盘模块（5Pin）

电池：3.7V或3.8V锂电池，1.25红黑插头

 ### 简化屏幕模块 1.0
 无法持续为时钟模块供电，开关断电后时钟模块停止工作。因此，时钟模块名存实亡，时钟模块整体可以去除，不影响其他模块工作。
 
 ### 简化屏幕模块 1.5
 可以持续为时钟模块供电，开关断电后时钟模块依旧可以工作。
 
 新增4个按钮，用来调整时间：
 
 - CHANGE按钮用来进入时间编辑模式
 - SWITCH按钮用来切换编辑位置（小时：分钟：秒）
 - HIGH和LOW分别是增加和减少数字。
 
 ### 简化屏幕模块 2.0
 仅去除冗余的稳压模块

 **注意**：磁传感器模块下方尽量不要铺铜，防止干扰。电池不要和磁传感器放置在板子同一侧，也会干扰。晶振要尽最大可能离单片机近，且附近不要铺铜。

 > 后续我们计划使用arm架构的芯片优化指南针。因此如果使用其他芯片想要优化现有程序，需要更换电路图。
