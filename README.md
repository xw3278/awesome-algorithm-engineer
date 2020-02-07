# awesome-algorithm-engineer

AI的火热给国内带来一个新职业-算法工程师，在国外一般叫machine learning engineer或者data scientist，从业过程中常常会思考这个岗位带来的价值亦或是泡沫，列出这些已经学习过或是评估过并且准备学习的资源，希望对自己，从业者，以及准备入行的朋友们一些帮助

Table of Contents
---

- [计算机基础](#计算机基础)

- [数学](#数学)

- [机器学习](#机器学习)

- [数据分析与可视化](#数据分析与可视化)

- [编程语言](#编程语言)

- [开发工具](#开发工具)

- [方法论及杂书](#方法论及杂书)



计算机基础
---

算法工程师有许多非科班出身，这也是这个岗位某种意义上门槛较低或者容易被称为调包侠的原因，计算机专业有很多看起来晦涩冗长没什么用的课程，但这只能说这些内容不会经常出现于工作中，但了解他们能够让你更理解你所做的事，其中的1%的精华也能在工作中发挥巨大作用

- 计算机系统

	- [深入理解计算机系统](https://book.douban.com/subject/26912767/)著名的大部头CSAPP，讲述了有关计算机系统的方方面面，如数据的表示和处理，程序的执行等等，这本书对应的课程也十分硬核，作业难度比较大，不过粗读一遍，也能收获不少基本概念，比如以前不知道溢出的原理，不知道虚拟内存，不知道编译原理，在这本书中都找到了初步的答案
  
	- [CMU CS15-213](http://www.cs.cmu.edu/afs/cs/academic/class/15213-f19/www/index.html)
	
	- [课程视频](https://www.bilibili.com/video/av31289365)
	
 	- 计算机网络
	
	- 有些算法岗一般仅承担模型训练和测试相关工作，但也有情况下需要搭建算法服务，来进行线上推理，这时候基本的网络相关知识非常重要
	
	- [图解HTTP](https://book.douban.com/subject/25863515//) HTTP协议作为最通用的应用层协议，实用性非常高。这本书图文并茂，一两天就可以阅读完成
	
- 数据库原理

  - 少数在学校上过的计算机课程之一，工作后发现算法岗一般以离线大数据计算为主，除了索引和SQL之外其他用处不多，现在公司内线上查询一般以MySQL为主，用到的话可以参阅[高性能MySQL](https://book.douban.com/subject/23008813/)。
  
- 算法设计

  - 国内的算法工程师基本上可以翻译成机器学习工程师，传统算法在机器学习中的作用一般是用来优化一些机器学习算法中的子步骤，如w2v里的霍夫曼树，强化学习中的动态规划，不过作为面试必考仍然有必要掌握
  
  - [算法导论](https://book.douban.com/subject/20432061/) 算法的大部头，粗读了解基本思路即可
  
  - [算法第四版](https://book.douban.com/subject/19952400/) 比较友好的一本书，Coursera上有[对应课程](https://www.coursera.org/learn/algorithms-part1)
  
  - [leetcode](https://leetcode-cn.com/) 大家都懂的
- 待评估课程

  - CS61A，MIT6.824



数学
---

很多人都说算法工程师需要强大的数学功底，但个人感觉吧，在应用层面，大学数学基本够用，看不懂的查一下工具书也基本能理解，不太存在从体系上就不理解的情况。

- 线性代数
  
  - [MIT 线性代数](https://www.bilibili.com/video/av15463995) 看完了之后感觉大学老师的教学水平和MIT确实有差距，很清晰很透彻，对很多概念有了新的认识
- 概率论与数理统计

  - [All of Statistics](https://book.douban.com/subject/2285151/) 非常全面的工具书，用于概念速查用

- 其他

  - 很多机器学习教材像MLAPP，花书，统计学习方法的附录或者前几章都有数学基础的回顾，按需阅读即可



机器学习
---

机器学习的理论及应用，是算法工程师的核心技能，而且近年来发展迅速，需要进行持续学习，这里列举一些学习过程中遇到的好资源，很难说看完某几本书或者某几门课就足够，因为各种精华要点都分散在不同的地方，真正理解需要相互参阅

- 传统机器学习

  - [统计学习方法](https://book.douban.com/subject/33437381/) 在以前，彻底搞懂这本书中的理论及全部公式，基本可以对面试中的所有问题应答如流，可以说是最好的中文入门书籍

  - [机器学习](https://book.douban.com/subject/26708119/) 被称为西瓜书的另一本入门书籍，可以和统计学习方法互相对照补充阅读

  - [机器学习基石](https://www.bilibili.com/video/av12463015) 台大林轩田的机器学习入门课，理论程度会比较深，对某些算法的讲解颇为精辟

  - [机器学习技法](https://www.bilibili.com/video/av12469267) 上一门课的进阶课程

  - [Stanford CS294]([http://cs229.stanford.edu/](http://cs229.stanford.edu/)) 大名鼎鼎的Ng的机器学习入门课程，理论应用兼备

- 深度学习

  - [Coursera 深度学习](https://www.coursera.org/specializations/deep-learning) Ng主导的deeplearning.ai提供的深度学习入门课程，可以说是零基础的神经网络教程

  - [李宏毅 深度学习](https://speech.ee.ntu.edu.tw/~tlkagk/courses.html) 台大李宏毅的系列课程，我认为最好的中文深度学习教程，每年随课程更新

  - [Stanford CS231N]([http://cs231n.stanford.edu/](http://cs231n.stanford.edu/)) 以CV，CNN为主的深度学习课程

  - [Stanford CS224N]([http://web.stanford.edu/class/cs224n/](http://web.stanford.edu/class/cs224n/)) 以自然语言处理为主的深度学习课程

  - [Stanford CS285](http://rail.eecs.berkeley.edu/deeprlcourse/) 以前叫CS294，深度强化学习课程

  - [深度学习](https://book.douban.com/subject/27087503/) 花书，个人觉得阅读起来还是有些难度，偏研究向

- Coding

  - [Kaggle](https://www.kaggle.com/) 一个机器学习的竞赛网站，重点不是拿名次，而是学习很多人分享的思路方法以及代码

  - [scikit-learn](https://scikit-learn.org/) 常用python机器学习库，其中的User Guide包含大量示例

  - [Tensorflow](https://www.tensorflow.org/)，[Pytorch](https://pytorch.org/) 两大深度学习框架，同样有大量示例代码

  - [动手学深度学习](https://github.com/d2l-ai/d2l-zh) 李沐的动手学深度学习，手把手实现各种网络结构，有Mxnet，Pytorch，TensorFlow版

- 待评估课程

  - Stanford CS230，CS276



数据分析与可视化
---

机器学习、深度学习的崛起的原因之一就是互联网时代产生的大数据，在模型之外往往还要对数据进行各种各样的处理，模型或者策略上线后，指标的跟踪也需要数据分析与可视化，这部分的技能从目前看来必备且保值。

- SQL

  - 算法工程师经常自嘲为sql boy确实不是开玩笑的，数据分析、特征处理其实占据了工作的主要时间，写一手好SQL能大大提升工作效率

  - [SQL必知必会](https://book.douban.com/subject/24250054/)，入门级别SQL书

  - [hive编程指南](https://book.douban.com/subject/25791255/)，hive是使用SQL进行MapReduce计算的大数据工具，，HQL属于SQL方言，是数据分析师和算法工程师必备技能

- Spark

  - Spark是一个分布式计算引擎，和MapReduce属于同一级别，同时支持scala, java, python接口，灵活性非常高，原生支持SQL和HQL，也可以做机器学习(不支持深度学习)

  - [官方文档](https://spark.apache.org/docs/latest/)，一般的开源框架，最好的学习手册一般都是官方文档，因为版本变化很快

  - [高性能spark ](https://book.douban.com/subject/30166057/)，讲了一些spark原理和调优方案

- 可视化

  - 可视化这块基本感觉是锦上添花，很多时候做了几个自我感觉良好的图，然后往往boss或者pm想看的就是表格而已，可能是因为可视化相比于纯数字很容易造成错觉，引起错误的判断
  
  - [Tableau](https://www.tableau.com/)，付费可视化工具，效果很酷炫，对地图数据的展示很棒
  
  - Excel，看起来low但实际最方便的工具之一
  
  - 各种库，如[Matplotlib](https://matplotlib.org/)，[Seaborn](https://seaborn.pydata.org/)，[Bokeh](https://docs.bokeh.org/en/latest/index.html#)，[D3.js](https://d3js.org/)



编程语言
--

岗位要求方面，一般会写掌握python，java或者C++，从学习曲线的角度以及流行程度，大部分人应该都会选择python，python毋庸置疑是当今机器学习的第一语言，从优先级来讲一定是最需要熟悉的。java主要用在后端服务开发，C++的话目前没有学习，由于其高性能似乎会应用于在线算法服务上。另外个人也比较推荐js的学习，属于前端第一语言，加上python基本可以当个小全栈。

- Python

  - [The Hitchhiker’s Guide to Python](https://docs.python-guide.org/) 安装，配置和使用python的最佳实践指南

  - [Python编程-从入门到实践](https://book.douban.com/subject/26829016/) 很多人推荐的一本书，个人没有看过，不过python的基本语法非常简单，快的话一两天就可以看完，书籍也有很多。学习的重点还是以应用为主，像pandas，scikit-learn, tensorflow这种直接按照文档学习即可

  - [流程的python](https://book.douban.com/subject/27028517/) 进阶级别python书，在魔法方法，协程，元编程方面讲的特别好，看不懂源码的时候看看这本书就对了

  - [python3标准库](https://pymotw.com/3/) 熟练使用标准库可以让代码更加pythonic，一般先了解各个标准库的用途，之后需要的时候再去查询对应api

  - Python项目源码阅读，requests，flask，django这些基本上各种教程都有推荐阅读

- Java

  - [Cornell CS2110](https://www.cs.cornell.edu/courses/cs2110/2018sp/index.html) 当年的java入门课，当时用的课本是 *Data Structures and Abstractions with Java, 3rd edition*

  - [java编程思想](https://book.douban.com/subject/2130190/) 朋友推荐的书，阅读中



开发工具
--

对于能够显著提升工作效率的工具，我总是非常狂热的，即使这件工具的学习成本可能非常高，即便最后发现很多工具对效率提升没有想象那么高，但额外的逼格也足够让人满足:)

- Linux

  - [linux命令行与shell脚本编程大全](https://book.douban.com/subject/26854226/) 不管愿不愿意，在服务器上开发总是不可避免的，基本命令的学习让你可以顺畅完成工作，一些高级命令更是如虎添翼，python当然也可以用于脚本，但在很多任务下相比原生的工具，无论在速度还是代码简洁性方面都有很大差距

  - [Cornell CS2043 Unix Tools & Scripting](https://www.cs.cornell.edu/courses/cs2043/2014sp/) 不错的unix工具入门课

- 编辑器

  - [Vim实用技巧](https://book.douban.com/subject/25869486/) 因为vim很酷，我想变得很酷，所以学习vim，毕竟总是需要在服务器上修改代码的

- Git

  - [ProGit2](https://github.com/progit/progit2-zh) 如果你公司的代码需要版本控制，但你没有系统学习过git，那几乎可以保证总有一天你会搞出问题而不知道如何修复，这本书可以满足你的一切需求

  - [learngitbranching](https://learngitbranching.js.org/) git的动画教学加练习



方法论及杂书
---

很多书可能实用程度看起来较低，或是以编程的方法论为主，讲述的内容较为抽象，但内容相对前文的一些书籍不那么硬核，适合当做闲书阅读，但里面的某些内容，甚至有时候只有一两句话，却能起到画龙点睛之用

- 编程方法论

  - [代码整洁之道](https://book.douban.com/subject/4199741/) 教会你区分好代码与坏代码，有助于培养程序审美

  - [设计模式](https://book.douban.com/subject/1052241/) 很经典的书，阅读起来相对枯燥，研习中

  - [重构-改善既有的代码设计](https://book.douban.com/subject/1229923/) 一段代码很烂很多时候是很容易看出来的，但重构往往吃力不讨好，因为不产生即时的商业价值，而且容易产生bug，但这本书会告诉你为什么需要做重构以及如何避免重构带来的问题

  - [代码大全](https://book.douban.com/subject/1477390/) 名字很霸气的一本书，评分很高，阅读中

- 项目管理

  - [人月神话](https://book.douban.com/subject/1102259/) Brooks法则： 向进度落后的项目中增加人手，只会使进度更加落后，记得最深也有所体验的一句话