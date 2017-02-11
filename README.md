# MCM2017
Something about MCM 2017 with Miao Yu and Zibu Liu.

## Preparation

### TO-DO
- [x] UMAP杂志
  - [x] ~~找到能看的地方~~(见Google Drive)，注意看**评委评价**
  - [x] 每个人按年份阅读O奖摘要(完赛注：2011~2013为比赛前一天口头交流)
    - 骆::2011、[2014](preparation/summary-of-outstandings/2014.md)
    - 刘::2012、[2015](preparation/summary-of-outstandings/2015.md)
    - 于::2013、2016
  - [x] 总结出需要准备的模型
- [x] LaTex模板
  - [x] 看一下今年的格式要求：**有页数限制了**
  - [x] 提前整理一套出来::[mcmthesis](https://github.com/Liam0205/mcmthesis), LaTeX2e Template designed for MCM/ICM
- [x] 文献查找准备
  - 试用一下Google Scholar(最后没怎么用上)
- [x] 学习一些算法~~(TBC)~~
  - 评价
    - 层次分析
  - 优化
    - 模拟退火
    - 蚁群
  - 仿真
    - 蒙特卡罗
    - 元胞自动机
- [x] 物资采购::全体，19日晚逛超市
  - 水、食物
  - 草稿纸
- [x] 软件
  - [x] Matlab
  - [x] LaTex开发环境
    - [LaTeXTools](https://github.com/SublimeText/LaTeXTools), LaTeX plugin for Sublime Text 2 and 3
    - [LaTeX-cwl](https://github.com/LaTeXing/LaTeX-cwl), LaTeX cwl files for Sublime Text 2/3

## Contest

### Day-1

第一天蛋淼吵吵说要早起，我跟咧不都是睡到9点多才醒。醒来的时候各题的中文翻译都有了，不过看着还是挺头疼的于是还是滚去看原文了。躺在床上把AB两题看了一遍感觉都可做，个人倾向于B题，毕竟好好的研究了2014的UMAP和那篇O奖，对这个题目背景熟悉的不能再熟悉。不过到了场地之后几个人还是好好的查文献找背景资料，上午就过去了。午饭去南门吃了潮汕粥，几个人敲定就是做B了。回来把2005的UMAP也找出来好好研究了一下。三个人一块想元胞自动机的转换方程，我的话再自己头脑里构思整个模拟用到的数据结构。没有用朴素的二维数组，Plaza用了B个链表，Toll用了B个队列，这样效率会比二维数组高不少，处理长度不止一格的车也很方便(这个功能从一开始就支持了不过论文里一直没有提算是个大失误)。

当晚咧不把论文提纲列好，我多熬了会儿夜把所有开发环境配置完，数据结构搭好，最开始这些基础设施就都完善了，给明天开始的算法编写部分打好基础。

### Day-2

第二天的时间全天都在撸代码，平淡无奇，整体难度并不大，加上前一天数据结构写的很完善，虽然整体的代码是偏面向过程的，但是命名规范、扩展原则等等都严格遵守，这为之后模型的不断调优打下了重要的基础。蛋淼先是写了一套卡方验证把我先行跑出来的出Toll序列验证了一下，确实是符合泊松过程的。然后就是参考了下2014B题的两个评价模型最后决定用FSE(这个选型导致感觉最后我们的paper跟2014A很多地方很像)

### Day-3

### Day-4