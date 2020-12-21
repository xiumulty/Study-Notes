
# 第一学期目标 #
- 把Python小甲鱼的97节课全部学完
- 把尚硅谷HTML和css的144节课程全部学完
- 前端课程学到了一定程度后开始学习后端PHP语言
希望在寒假结束前能全部完成，如果完成了给自己一定的奖励。
# 明日计划 #
- 明天没啥课，得多学一点
- python学到魔法方法
- 前端作业写完争取多听几课
- 以上任务争取在上午做完
- 下午和晚上专攻高数和数逻，还有英语，一个星期没背过单词了，真的有点慌，但是就是不想去背
# 2020年12月21日 #
- 今天的数逻算是听懂了，老师讲的太快了，思维有点跟不上。。。
- python学了类的私有和公有与类的继承
- 前端没学新课，写了一下课程老师布置的作业
- 高数没怎么搞懂的东西，昨天问了下朋友教了一下，高数课看着看着就弄懂了，顺便刷了几面题，贼爽。
# 2020年12月20日 #
- 前端学了三节课，主要是开始了练习，练习慢慢做吧，不急，先复习期末。
- python听了两课，感觉类和对象有点难啊，好抽象，在b站，慕课，参考书的共同帮助下算是大概理解了类和对象，self，__init__的意思，开了一篇博客记录这个
- 关于类和对象，首先要拿class创建一个类，这个类就相当于一个图纸，创建对象就是类的实例化，就相当于那图纸造屋子，对象名=类名()就算是给这个类创建了一个对象，这个对象就是在这个类里面了
- 关于self，一个类可以生成无数个对象，当对象的方法被调用时，对象会将自身作为第一个参数传给这个方法，这个时候python才知道到底这个方法是给哪个对象用的，所以这个self就像是一把钥匙，对应着这个对象对应的门。比如下面的代码
```
class Person: # 创建了一个名为Person的类 
    def setname (self,itname): # 创建一个名为setname的方法，第一个参数为self
        self.itname = itname  # 因为itname是外部变量，要在类中使用要加工
    def printname (self):
        print("我是%s" % self.itname)
a = Person()  # 实例化a
a.setname("小明") # a作为self参数传入，"小明"作为itname参数传入
a.printname()
```
对于self.itname的理解：itname是全局变量，要在类中使用还得加工一下，使用`self.变量名`将外部的变量引入类中使用，不加self.会被当做普通变量。
- 关于__init__，这是一个构造函数（构造方法），实例化对象时，该方法会在对象被创建的时候自动调用，实例化对象的时候是可以传入参数的，这些参数会自动传入该方法中，通过重写该方法可以自定义对象的初始化操作，不重写就默认调用__init__(self)。，类名就作为self，看如下代码。
```
class Person:
    def __init__ (self,itname):  # 额外添加一个参数，实例化对象时输入的内容就作为itname的参数
        self.itname = itname
    def printname (self):
        print("我是%s" % self.itname)
a = Person("小明") # 创建类的时候就可以直接传入参数，类名作为self，"小明"作为itname
a.printname()
```
# 2020年12月19日 #
- 前几天熬夜熬的太凶了，今天早上睡到了十二点
- 前端学了五节课，笔记也整理了
- python只学了一课，类和对象有点没听懂，跑去MOOC上听了一下，差不多弄懂了准备睡觉
# 2020年12月18日 #
- 配置这个next主题花了我好多精力啊，整了一天也不尽人意，个人能力不足，好多配置没有全部弄懂，剩下的以后有能力再搞吧
- 高数没看。。。
- 前端没学。。。
- python没学。。。
- 失败的一天。。。

# 2020年12月17日 #
- 前端课程只听了四节课，做好了笔记
- python直接钢了五节课，明天争取把类和对象全部学完
- 班里算法周赛打了两个小时，一点高数没看
- 换了一个主题，搞了一晚上到十二点四十

# 2020年12月16日 #
- 前端课程听了六节课，并把笔记整理到了两个博客，还整理到了笔记本上
- Python只听了一节课
- 把codeblocks和dev-c++全部卸载了，重新下载了MinGW配置环境，以后就到vscode上打c语言代码了，把配置过程写到了博客里
- 晚自习写了一个多小时的高数，开始准备期末考试了，争取能提高点排名，甚至冲击奖学金哈哈哈

# 2020年12月15日 #
- HTML选择器大概过了一遍并把笔记详细记录在了我的博客
- python文件的学习，买的资料书和小甲鱼的课说的很模糊，又去慕课上找了课，还在CSDN找了资料整理好了笔记
- 因为日记不想让太多人看到所以把之前删掉的库重新创建了一下用来专门写学习记录，顺带又学习了一下git的使用方法。
