---
layout: default
title: 机器学习CR-EP01：机器学习的动机与应用【存疑】
---
开始看斯坦福的公开课《机器学习》，Andrew Ng教的，看起来很年轻，像是个中国人，传说中也是很牛逼闪闪的人物（注：刚看到[未来的大学](http://blog.renren.com/share/250444366/16554017245?from=0101010202&ref=hotnewsfeed&sfet=102&fin=0&fid=24043898897&ff_id=250444366&platform=0&expose_time=1383196480)里说“而在2013年，Andrew Ng入选财富杂志全球40岁以下最富有的40人。”）。

CR是Class Report，课堂笔记。《机器学习》第一集。

一、应用举例

机器学习可以用于各个学科，每个领域都有人来找他谈合作，天天谈。举了个例子，是邮局寄信的时候后，手写的邮编是由机器识别出来的，这个手写字体的识别就是机器学习的应用。（国内的邮局应该还是人工识别吧？邮递员大学该好好努力了！）

二、机器学习定义

给了两个机器学习的定义。

一是1959年Arthur Samuel的定义（好早！同样是Arthur，可我还没出生呢！）：Field of study that gives computers the ability to learn without explicitly programed. 意思是说：无需显式的事先编程定义，就可以使计算机具有学习能力的研究领域。感觉有一点点人工智能的意思。这里举了一个Arthur做的西洋棋的例子，说最后Arthur写出来的西洋棋程序超过了Arthur本身的下棋能力。让人想起了很久之前IBM的“深蓝”电脑与棋王的对决。

二是1998年Tom Mitchell的定义（貌似经典的机器学习书就是他的那本吧）：A computer program is said to learn from experience E with respect to some task T and performance mesure P, if its performance on T, as measured by P, can improve with experience E. 这个定义看起来严格了一点，像是数学定义似的，关键是听起来还押韵！很好玩的样子。

根据这两个定义，我自己对机器学习的理解就是：无需显式的事先编程，就可以使计算机根据某种已经确定的测量方法，从既往的经验结果中学习，并且提高在未来对数据的预测和判断能力。说白了，跟一个小孩在认识世界的步骤一样，根据个人以往的经历形成自己的对世界的观念（其实也可以叫做“偏见”），从而对未来未知的数据或事件可以进行更加准确的判断和识别。

三、机器学习的主要范围

主要有四个。

1. Supervised learning（有监督学习）

是指从已知训练集分类/答案的数据集中进行学习。比如：房价预测（回归问题）、良性/恶性肿瘤分类（离散数据的分类问题）。

不过这里提到了一个有意思的问题：数据一般是用高维度向量表示，维度越多，信息量越大。很多时候会用到无限维的东西，那么，在计算机中，如何使用有限的内存表示无限维的点呢？Andrew说讲到了SVM再来说。【存疑】

2. Learn Theory（学习理论/策略）

讲到这里，Andrew讲了个笑话，说是他去硅谷的时候，很多人都会拉着给他讲他们在做的机器学习的东西，展示他们六个月以来的研究成果，他看了之后，觉得they are waste of time from the start of six months ago！Andrew说他的课堂的目标是希望学生不止对机器学习开始感兴趣，而且是Quilified in machine learing research!希望我的学习不会是浪费时间吧！

3. Unsupervised Learning（无监督学习）

是指没有标注过的数据集，由机器自己去寻找something interesting. 比如：聚类。Andrew举了之前学生做的例子，使用聚类分离噪杂的鸡尾酒会中两个人的说话声音。效果很好，能够很清晰的将两个人的声音分离开来（这个代码可以用一行matlab代码实现，所以Andrew力推要学习Matlab。当然他也说了，这一行代码是研究了好久之后的结果，所以这个task也没那么简单）。还有比如，将照片中的像素聚类，从而得到照片中物体的轮廓。

4. Reinforcement Learning（强化学习）

是指通过对学习结果的鼓励和惩罚（惩罚函数），来得到更优的学习结果。就像是家里训练小狗，做得好了说"good dog"， 不好了说"bad dog"，这样，以后狗的表现就越来越好（我怎么感觉人在这个社会里也是这样被社会训练的呢？跟“乖孩子”、“坏孩子”一样。那样“你看看别人家的孩子”这种是不是可以看做一种新的机器学习类型？可以叫做榜样学习(Example Learning)，哈哈）。课堂上展示了之前学生做的一个电脑控制飞机倒立悬空的视频，可以看出飞机可以很稳定的在空中悬停，很牛逼的技术。还有个机器狗学习走路，这样的技术跟月球行走一样。国外的孩子学的NB，玩的也高端大气。

最后，Andrew强调可以组成3人以内的学习小组，可以互相讨论，但不能互相抄袭作业！所以，如果你看到了这里，求小伙伴加入！

参考资料：

* 斯坦福大学公开课-《机器学习》Andrew Ng