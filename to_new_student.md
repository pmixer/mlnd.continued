欢迎参加优达学城机器学习入门纳米学位项目，各位新同学可以先到[迎新帖](?)留言介绍一下自己。
我是助教?，如果学习当中碰到什么问题可以在论坛相应板块发帖并@? ，也可以把帖子链接发到微信通关群。

## 做好准备

Udacity 的机器学习纳米学位偏重对各个方法的直觉性的认识和实际的编码操作，这是在大部分学校通常是无法获取到的稀缺资源。
这也意味着你需要为一些事情做好准备：

+ 凡是上手编码，无论新手老手，总会碰到各种各样的错误，这很正常，而且从侧面讲，这是学习的绝佳时机，人在不断犯错和纠正的过程中进步。
+ 面对新领域，总有看起来永远学不完的知识在等着你，要学会如何起步懂得取舍才能构建起知识大厦；没有目的性和方向性的学习只会让你收获一盘散沙。
+ 作为一家负责任的公司，Udacity 把学员课程学习情况作为重中之重，平时免不了有人敲敲来进度；鼓励速度快的同学主动分享带节奏，慢也不怕，放宽心，只要每天学一小时，总可以在半年内完成的。
+ 请记住，在学员群、论坛、教室等处，都有工作人员和助教为你服务，个人无法解决的问题尽管提出，有好的资料也别忘分享。

在最初的学习阶段，了解做什么和为什么要比知道具体如何操作来的重要，在一些逐渐清晰之后，不妨从一些示例代码上做修修改改起步，逐渐过渡到独立编码实现，模仿常常是跨过“能”与“不能”之间鸿沟的有效方式，从新手到高手需要不断的练习与总结。

## 蟒蛇&大蟒蛇
不可避免地，工具安装、设置和程序报错是被最常提出的问题，动手编程是纳米学位的重中之重截个图交给别人 debug 很难在编程时学到真东西，希望你能对自己所使用的兵器有足够的了解，不至于在未来面对报错时手足无措。

Python(蟒蛇) 是课程中最常使用的编程语言，对于初学者来讲二者有微妙的不同，在 Py2 中输入 `from __future__ import print_function` 和 `from __future__ import division`
能够弥合大多数新用户对二者差异的顾虑。当然，现在我们更推荐 Py3，它对编码等问题支持更好，不过就上手而言，23均可。在解释器中输入 `import this` 能够快速
带你领略 Python 哲学，作为一门胶水语言，它的数据交换协议给各种模块的集成提供了良好接口，同时语法简洁，便于使用。编程遇到任何问题，先记得 Python 解释环境下通过 `help(函数名/类.方法名)` 等形式调出内嵌帮助文档查看具体工具用法。

如果想在开始之前更多熟悉 Python，可以参加 Udacity 的 CS101: [计算机科学导论Python](https://cn.udacity.com/course/intro-to-computer-science--cs101)，围观谷歌联合创始人布林为主讲 Dave 打 call，同时，官方还准备了付费课程（可选）
[Python 入门](https://cn.udacity.com/course/intro-to-python-nanodegree-foundation--nd000-cn-python)服务 Python 新手。如果你有十足的探索精神，
不妨试试去解 [Python Challenge](http://www.pythonchallenge.com)，蒟蒻编者在第六关等你:cry:

在后期你会接触大蟒蛇(Anaconda)，这是一个数据科学集成工具包，使用它能够方便地管理多个独立的 Python 环境，为你的开发部署活动服务。建立环境，启动环境，安装和删除文件都简单易行，课程到需要使用大蟒蛇的部分会作详细介绍，同时包安装速度过慢可以考虑替换国内的(比如 [THU](https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/)) conda 和 pip 源：

```bash
conda create -n mlnd python=3.5 # 创建环境
[source(on mac/linux)] activate mlnd # 启动环境
conda install jupyter notebook # 安装包
conda install -c https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/ jupyter notebook # 指定 conda 源安装包
pip install -i  https://pypi.tuna.tsinghua.edu.cn/simple numpy # 指定 pip 源安装包
jupyter notebook # 启动 notebook
conda uninstall [package name] # 卸载包
[source(on mac/linux)] deactivate mlnd # 注销环境
```

## 如何提问
好的提问方式能够节约你的时间，提升你的学习质量，说不定还能认识一群志同道合的朋友，我们推荐阅读：[提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/master/README-zh_CN.md)  
，其内容简单来说：
1. 根据报错信息自己判断哪段代码出问题，原因是什么，并尝试修改代码
2. 善用搜索，通过Google和stackoverflow查看类似问题及解决方法
3. 优达学城论坛，先用右上角的搜索看看是否有一样的问题帖子，然后到对应项目的子版块发帖。
 - 使用有意义且描述明确的标题，比如报错关键词
 - 帖子内容先附上课程详细链接
 - 标明运行环境（系统，版本等）
 - 详细报错信息
 - 尝试的解决方案（这个很重要，有利于别人用排除法节省分析时间）

注： **不要直接在群里或论坛贴代码！** 考核内容不能直接贴出来否则会违反[Honor Code](https://cn.udacity.com/legal/)。先自己尝试提炼有效信息和自己的分析，结合 **完整报错**信息来提问。  
提供 **文本**报错信息，尽量不要用截图，绝对不要用曝光不足、失焦的低分辨率手机照片。
**报错信息过长不要发微信群**，影响他人查看其他回复，直接发论坛。

优达学城论坛支持markdown格式编辑，这里有个[教程](http://commonmark.cn/help/tutorial/)，也可以参考这篇[论坛快速指南](https://discussions.youdaxue.com/t/topic/58)。结合论坛的实时预览可以快速熟悉用法。

如果发现翻译或内容有误，可以在[这个版块](https://discussions.youdaxue.com/c/translation)发帖。
标题格式：课程名称-部分-课-节-标题-错误
内容截图圈出错误，或者复制粘贴然后标红错误即可。

## 更多资源
### 讨论组
[中文论坛](https://discussions.youdaxue.com)
[英文论坛](https://discussions.udacity.com)

### 微信通关群
像RPG一样打怪通关，项目审核通过后填写通关申请表（链接见通关群群公告），提交申请表同时麻烦群内截图网站任意有效位置证明项目已通过并 **@** 助教，拉你进入下一个项目的群。记得退掉旧群，方便问题定位和学员管理(各通关群以字母 P 编号，最初以字幕 S 编号的同期学员群不要退出)。
 注：**确保你已经顺利通过项目后再提交通关申请表**，项目提交页面会出现“恭喜! 你已顺利完成此项目”字样，如下图所示：
<img src="//cn-discussions.s3.cn-north-1.amazonaws.com.cn/original/3X/9/0/900f0157dee18a2297a181e9cdc75a8bc347aec1.png" width="451" height="58">
(注:微信昵称填 **群昵称** 而不是微信号)。

### 速查手册
[Python](https://docs.python.org)
[微积分](http://tutorial.math.lamar.edu/pdf/Calculus_Cheat_Sheet_All.pdf)
[线性代数](http://www.souravsengupta.com/cds2016/lectures/Savov_Notes.pdf)
[统计](http://web.mit.edu/~csvoss/Public/usabo/stats_handout.pdf)
Numpy [简洁](http://cs231n.github.io/python-numpy-tutorial)-[详细](https://docs.scipy.org/doc/numpy-dev/user/quickstart.html)

### 打比赛&读论文
如果打算在机器学习领域深挖，希望 Udacity 的课程能成为你熟悉英文材料和上手实际项目的桥梁，同时我们也推荐一些站点作为**课外活动**场所：

+ [Kaggle](https://www.kaggle.com/)
+ [天池](https://tianchi.aliyun.com/)
+ [AI Challenge](https://challenger.ai/)
+ [ICCV&CVPR](http://openaccess.thecvf.com/menu.py)
+ [NIPS](http://papers.nips.cc/)
+ [JMLR](http://www.jmlr.org/)
+ [ICLR](http://www.iclr.cc/)


# FAQ
* 个别扩展资料网页打不开，连接被重置
有两个解决方法：
 1. 使用代理，推荐买个VPS搭SS，方法网上搜。
 2. [改hosts](https://github.com/racaljk/hosts)，免费，但仍然看不了youtube，且需经常更新。

* 部分文件无法下载
可以去官方的[Github地址](https://github.com/udacity)和 Mentor 准备的[Github Issue页](https://github.com/PeterHuang2015/AWESOME-MLND/issues/1)查查是不是有你需要的。

* 项目过期未提交
项目页面显示的时间为建议完成时间，并非deadline。在课程规定的有效期内提交并通过所有项目审核即可。

* 毕业后还能查看课程吗？
有效期内成功毕业则拥有已学内容的永久访问权限。若过期未毕业则需重新报名才能再次获得权限。
