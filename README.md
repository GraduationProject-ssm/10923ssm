# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# 10923ssm大学生兼职信息系统

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1Sh44eDEx6?p=24)


# 系统概述
进过系统的分析后，就开始记性系统的设计，系统设计包含总体设计和详细设计。总体设计只是一个大体的设计，经过了总体设计，我们能够划分出系统的一些东西，例如文件、文档、数据等。而且我们通过总体设计，大致可以划分出了程序的模块，以及功能。但是只是一个初步的分类，并没有真正的实现。

整体设计，只是一个初步设计，而且，对于一个项目，我们可以进行多个整体设计，通过对比，包括性能的对比、成本的对比、效益的对比，来最终确定一个最优的设计方案，选择优秀的整体设计可以降低开发成本，增加公司效益，从这一点来讲，整体设计还是非常重要的。

大学生兼职信息系统工作原理图如图4-1所示：

![](/md/blog.013.png)

图4-1 系统工作原理图
## 4.2 系统结构设计
系统架构图属于系统设计阶段，系统架构图只是这个阶段一个产物，系统的总体架构决定了整个系统的模式，是系统的基础。大学生兼职信息系统的整体结构设计如图4-2所示。

![](/md/blog.014.png)

图4-2 系统结构图
## 4.3数据库设计
数据库是计算机信息系统的基础。目前，电脑系统的关键与核心部分就是数据库。数据库开发的优劣对整个系统的质量和速度有着直接影响。
### 4.3.1 数据库设计原则
数据库的概念结构设计采用实体—联系（E-R）模型设计方法。E-R模型法的组成元素有：实体、属性、联系，E-R模型用E-R图表示，是提示用户工作环境中所涉及的事物，属性则是对实体特性的描述。在系统设计当中数据库起着决定性的因素。下面设计出这几个关键实体的实体—关系图。
### 4.3.2 数据库实体
数据模型中的实体（Entity），也称为实例，对应现实世界中可区别于其他对象的“事件”或“事物”。例如，公司中的每个员工，家里中的每个家具。

本系统的E-R图如下图所示：

1、学生信息实体图如图4-3所示：

![](/md/blog.015.png)

` `图4-3学生信息实体图

2、企业信息实体图如图4-4所示：

![](/md/blog.016.png)

`       `图4-4企业信息实体图

3、兼职评价信息实体图如图4-5所示：

![](/md/blog.017.png)

`     `图4-5兼职评价信息实体图
#########

### 4.3.3 数据库表设计
数据库的表信息属于设计的一部分，下面介绍数据库中的各个表的详细信息。

表4-1 allusers表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|username|varchar|50|` `default NULL|
|pwd|varchar|50|` `default NULL|
|cx|varchar|50|` `default NULL|

表4-2：jianzhipingjia表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|` `int|11|NOT NULL |
|addtime|varchar|50|default NULL|
|qiyezhanghao|varchar|50|default NULL|
|qiyemingcheng|varchar|50|default NULL|
|gangweimingcheng|varchar|50|default NULL|
|qiyepingfen|varchar|50|default NULL|
|pingjianeirong|varchar|50|default NULL|
|pingjiariqi|varchar|50|default NULL|
|xuehao|varchar|50|default NULL|
|xueshengxingming|varchar|50|default NULL|
|shouji|varchar|50|default NULL|
|sfsh|varchar|50|default NULL|
|shhf|varchar|50|default NULL|

表4-3：qiye表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|qiyezhanghao|varchar|50|default NULL|
|mima|varchar|50|default NULL|
|qiyemingcheng|varchar|50|default NULL|
|touxiang|varchar|50|default NULL|
|lianxiren|varchar|50|default NULL|
|lianxidianhua|varchar|50|default NULL|
|qiyeyouxiang|varchar|50|default NULL|
|qiyedizhi|varchar|50|default NULL|

表4-4：qiyexinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|` `int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|qiyezhanghao|varchar|50|default NULL|
|qiyemingcheng|varchar|50|default NULL|
|qiyeleixing|varchar|50|default NULL|
|tupian|varchar|50|default NULL|
|yuangongrenshu|varchar|50|default NULL|
|lianxiren|varchar|50|default NULL|
|lianxidianhua|varchar|50|default NULL|
|qiyeyouxiang|varchar|50|default NULL|
|qiyejieshao|varchar|50|default NULL|

表4-5：xuesheng表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|` `int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|xuehao|varchar|50|default NULL|
|mima|varchar|50|default NULL|
|xueshengxingming|varchar|50|default NULL|
|xingbie|varchar|50|default NULL|
|touxiang|varchar|50|default NULL|
|xuexiao|varchar|50|default NULL|
|zhuanye|varchar|50|default NULL|
|shouji|varchar|50|default NULL|
|youxiang|varchar|50|default NULL|
#########



# 5系统界面实现
## 5.1 管理员登录
管理员输入个人的用户名、密码和角色登录系统，这时候系统的数据库就会在进行查找相关的信息，如果我们输入的用户名、密码和角色不正确，数据库就会提示出错误的信息提示，同时会提示管理员重新输入自己的用户名、密码、角色，直到账号密码输入成功后，会提登录成功的信息。网站管理员登录效果图如图5-1所示：

![](/md/blog.018.png)     
图5-1管理员登录界面

## 5.2  管理员功能模块     
管理员对大学生兼职信息系统进行查看首页、个人中心、学生管理、学生简历管理、企业管理、企业信息管理、招聘信息管理、学生应聘管理、兼职评价管理、留言板管理、系统管理并进行详情、删除、修改等操作。程序成效图如下图5-2所示:

![](/md/blog.019.png)

图5-2管理员功能界面图
### 5.2.1轮播图管理
轮播图；该页面为轮播图管理界面。管理员可以在此页面进行首页轮播图的管理，通过新建操作可在轮播图中加入新的图片，还可以对以上传的图片进行修改操作，以及图片的删除操作。程序效果图如下图5-3所示：

![](/md/blog.020.png)

图5-3轮播图管理界面
### 5.2.2 招聘信息管理
管理员对招聘信息管理进行查看企业账号、企业名称、联系人、联系电话、企业邮箱、岗位名称、图片、招聘人数、工作内容、工作地点、工作时间、岗位工资、结算方式等信息并可以进行详情、删除、修改操作。程序效果图如下图5-4所示：

![](/md/blog.021.png) 

图5-4招聘信息管理界面

### 5.2.3企业信息管理
管理员对企业信息管理获取查看企业账号、企业名称、企业类型、图片、员工人数、联系人、联系电话、企业邮箱等信息进行详情、删除、修改操作。程序效果图如下图5-5所示：

![](/md/blog.022.png)

图5-5企业信息管理界面
### 5.2.4学生应聘管理
管理员对学生应聘管理进行查看企业账号、企业名称、岗位名称、工作内容、工作地点、工作时间、岗位工资、申请日期、个人简历、学号、学生姓名、手机、审核回复、审核状态等信息并可以进行详情、删除、修改操作。程序效果图如下图5-6所示：

![](/md/blog.023.png) 

图5-6学生应聘管理界面
### 5.2.5兼职评价管理
管理员对兼职评价管理进行查看企业账号、企业名称、岗位名称、企业评分、评价内容、评价日期、学号、学生姓名、手机、审核回复、审核状态等信息并可以进行详情、删除、修改操作。程序效果图如下图5-7所示：

![](/md/blog.024.png) 

图5-7兼职评价管理界面


## 5.3 前台首页功能模块
前台首页详情页面查看首页、企业信息、招聘信息、兼职资讯、留言反馈、个人中心、后台管理等功能操作。程序效果图如下图5-8所示：

![](/md/blog.025.png)

图5-8前台首页功能界面
## 5.3.1 学生登录、学生注册
学生在线填写学号、密码、学生姓名、学校、专业、手机、邮箱等信息进行注册、登录操作。程序效果图如下图5-9所示：

![](/md/blog.026.png)

![](/md/blog.027.png)

图5-9学生登录、学生注册界面
## 5.3.2招聘信息
学生进入招聘信息可以查看企业账号、企业名称、联系人、联系电话、企业邮箱、岗位名称、图片、招聘人数、工作内容、工作地点、工作时间、岗位工资、结算方式等信息，并可以进行应聘操作。程序效果图如下图5-10所示：

![](/md/blog.028.png)


图5-10招聘信息界面
## 5.3.3个人中心
学生进入个人中心可以填写学号、密码、学生姓名、性别、头像、学校、专业、手机、邮箱进行更新信息、退出登录操作。程序效果图如下图5-11所示：

![](/md/blog.029.png)

图5-11个人中心界面

## 5.4 学生功能模块

学生进入大学生兼职信息系统可以查看首页、个人中心、学生简历管理、学生应聘管理、兼职评价管理、我的收藏管理等信息进行详情、修改、删除操作。程序效果图如下图5-12所示：

![](/md/blog.030.png)

图5-12学生功能界面

### 5.4.1我的收藏管理
学生对我的收藏管理进行查看收藏名称、收藏图片等信息并可以进行详情、删除、操作。程序效果图如下图5-13所示：

![](/md/blog.031.png) 

图5-13我的收藏管理界面



## 5.5企业功能模块

企业进入大学生兼职信息系统可以查看首页、个人中心、学生简历管理、企业信息管理、招聘信息管理、学生应聘管理、兼职评价管理等信息进行详情、修改、删除操作。程序效果图如下图5-14所示：

![](/md/blog.032.png)

图5-14企业功能界面
## 5.5.1学生应聘管理
企业进入学生应聘管理可以查看企业账号、企业名称、岗位名称、工作内容、工作地点、工作时间、岗位工资、申请日期、个人简历、学号、学生姓名、手机、审核回复、审核状态等信息进行详情操作。程序效果图如下图5-15所示：

![](/md/blog.033.png)

图5-15学生应聘管理界面

## 5.5.2兼职评价管理
企业进入兼职评价管理可以查看企业账号、企业名称、岗位名称、企业评分、评价内容、评价日期、学号、学生姓名、手机、审核回复、审核状态等信息进行详情操作。程序效果图如下图5-16所示：

![](/md/blog.034.png)

图5-16兼职评价管理界面
















