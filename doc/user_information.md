## 软件目的

软件旨在为用户推荐**今日饮用咖啡因的适宜量**（随时间变化的余量），从而达到控制用户咖啡因摄入量在适宜范围内的目的。

 

## 需要收集的数据

### Part 1 基本信息

用户进入初始页面需完善基本信息，诸如，**身高、性别、年龄、职业、有无肝脏疾病、是否吸烟、是否饮酒**等等。根据 <mark>WHO健康标准(<font color=red>**Todo: 查文献**</font>)</mark>将其归类，并设定对应的**<font color=red>心率、睡眠质量推荐值</font>**。



### Part 2 与硬件的联动

当用户使用硬件设计的特殊杯具饮用咖啡等饮品时，硬件向软件传输**①已摄入咖啡因量**，同时软件记录**②摄入的时间**，并计算当日咖啡因随时间的**③代谢曲线**。

 

同时，用户需**佩戴手环**从而实时监测心率，夜间睡眠等数据，并将其传入软件。



### Part 3 其他记录

用户还需每日记录当日**吸烟、饮酒情况**（隐私条款等），并记录当日是否出现**心悸、肌肉震颤、惊厥**等现象，若出现，则相应降低当日咖啡因含量在推荐值计算中的权重。

 

## 算法

**长时间观测上述数据**，我们将通过前一天数据的综合不断演化学习（**Markov decision process**？），并给出用户在当前状态下（例如咖啡因耐受度因长期摄入而不断提高）的适宜饮用咖啡因含量。

 

## 相关推送

软件的小程序界面还会进行咖啡因相关报道的推送，以及产品的推广等。