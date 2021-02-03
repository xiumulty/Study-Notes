# 第一学期目标 #
- 小甲鱼后面是讲pygame的，所以学到了爬虫就不往下学了，把Python爬虫加强一波
- 把尚硅谷HTML和css的144节课程全部学完
- 前端课程学到了一定程度后开始学习后端PHP语言
- 预计寒假开始学后端
希望在寒假结束前能全部完成。

# 2021年2月2-3日 #
- 刷题中，写了一波杭电的题，太菜了，只写出了一题，唉，菜是原罪
- 写了一些web的基础题，了解了一些之前没注意到的小细节
- 本来是想学一下序列化和反序列化，php对象还没学，基础还不够，准备加强一波基础

# 2021年2月1日 #
- 学了一波sql注入语句，包括information_schema、information_schema.tables、information_schema.columns、group_concat，其实information_schema就是一个库，这个库记录了整个mysql数据库的所有信息，详细理解也记了笔记
- 刷了一波题，做出来好爽的哈哈哈哈

# 2021年1月31日#
- 注册登陆界面开发结束，虽然很简陋，但是还是很有成就感的
- 上午学长培训了一波，对于web方向清晰了一些
- 写了两题web，学了一个是堆叠注入，可以用`;`来执行多条语句，再到结尾加上`#`屏蔽掉后面的语句
- 第二个是`select 1 from 表`这个操作是会创建一个临时列，可以用于子查询是否成功 

# 2021年1月30日 #
- 感冒了，淦，一天都没精力
- 实现对用户提交数据的规范，涉及到一个函数`is_numeric()`，这个函数是判断字符串是否为数字
- 下一步的计划是实现登陆界面

# 2021年1月28-29日 # 
- 注册登入界面html的设计，实现了简单的注册界面，就是使用sql插入语句把记录插入到数据库

# 2021年1月26-27日 #
- sql基础语句过了一遍了，笔记和理解全部记录起来了
- 准备开始学mysql支持的数据类型，争取2月份开始网站的搭建

# 2021年1月24-25日 #
- mysql的语句学习，DDL和DML语句，大概过了一下，具体用起来还是得再复习一遍，先把笔记做在博客里
- 了解了sql的select语句，可以理解简单的sql注入原理

# 2021年1月21-23日 #
- 看博客看到了一个sql注入，了解了一下发现看得懂一些，就了解了一下，但是之前管理员登陆的那题还是写不出，因为有引号屏蔽，我试了宽字节注入也没用，还是先放一下
- 学习php和mysql的联动，先学一点基础的语句


# 2021年1月20日 #
- 把php和web的交互学完了，感觉要记的东西比较多，先记在博客上慢慢记
- 表格是html的内容，但是我没学到，不过看的例子比较多，就是一个`<table>`标签里面加上`<tr>`
然后再往`<tr>`里面加`<td>`或其他表单元素
- 明天去做核酸检测，然后尽量早点结束php基础学习开始mysql的学习 

# 2021年1月19日 #
- 黑马程序员的课程是看完了，准备看书上的了，看php和web的交互和传值这些知识
- 下午到晚上都在外面玩，这波半夜在学一点，早点开始mysql的学习

# 2021年1月18日 #
- 还是php，把数组学完就开始学和web的交互了
- 又尝试了一下管理员后台的那题，还是写不出，估计要mysql的知识了

# 2021年1月17日 #
- 继续肝了php，准备19号结束

# 2021年1月16日 #
- 学了php函数、操作符，看书补漏了一个静态变量，东西写在了博客上
- 晚上再肝了一波循环分支，直接肝完，明天学字符串操作和文件包含。

# 2021年1月15日 #
- PHP学习开始，冲冲冲，今天熬波夜
- 建了一个php的学习笔记博客，笔记都记在那了
- 今天直接听了28节课，虽然前面的东西很水哈哈哈，学的记在了PHP学习笔记里了

# 2021年1月14日 #
- 坐了一天的车，到了广州，准备开始学php了
- 晚上有点累，不知道能不能学下去了，尽量多看一些php的东西吧

# 2021年1月13日 #
- 上午在整理宿舍和行李，啥都没学
- 下午考了思修就玩了好久
- 六点半开始了爬虫学习，实现了有道翻译的解密，拿到成果太爽了，明天博客记录一下思路吧，把学到的写上去，学到挺多的
- 明天回广东，冲冲冲，爬虫先告一段落了，开始开发学习了

# 2021年1月12日 # 
- 考完高数感觉很差劲。。。下午去打了一波球回宿舍就直接去吃饭了
- 回宿舍开始准备学习咯
- 两点半终于是肝完了，主要学了aiohttp的使用，先pip安装，这个东西可以提升爬虫的爬取效率，主要的操作步骤是：1，建立目标（由url组成的列表）。2，用循环对每一个url封装创建任务`asyncio.ensure_future()`。3，创建事件循环`asyncio.get_event_loop()`运行事件循环`.run_until_complete(asyncio.wait(tasks))`。4，里面有个`asyncio.wait(tasks)`是用来把封装的任务单里的协程作为任务加入日志。5，运用aiohttp来定义爬虫协程
- 思修懒得复习，应该不会挂的

# 2021年1月11日 # 
- 上午考完英语，阅读都看不懂。。。
- 下午在自习室看高数，太冷了，冻感冒了，不知道对我明天考试有没有影响
- 晚上在宿舍在整体过一遍知识点，被一波整理的公式就睡觉

# 2021年1月10日 #
- 起床就去了惟义楼呆着，下午五点去跑了一波步，晚上九点半就睡着了
- 期末复习真无聊

# 2021年1月9日 #
- 今天上午在自习室学了两小时，太冷了就出去吃了个饭就直接回宿舍学了
- 宿舍学习效率确实低，明天不能呆在宿舍学了
- 代码一点都没看，都肝高数了，做的很烦
- 下午健身，看了一下二头肌，还是有锻炼效果的，很满意哈哈哈

# 2021年1月8日 #
- 今天上午到下午都在自习室学高数，这天气真冷啊，下午去打了一波篮球，啧手感还行
- 回来就直接看博客了，改善了一下有道翻译的爬虫，弄成了可以循环使用，基本上放电脑上都可以当自己用的翻译软件了哈哈哈
- 准备学异步改善爬虫的，想着重新写一下再复习一遍，搞到了12点，搞出了bug了淦，找了好久发现原来是`xpath()`函数返回的是列表，爬图片的时候要一张一张爬，所以在最后加上[0]才能进行get请求，虽然没学到什么新的东西，但是也算完整的复习了一波，还是可以的
- 准备学高数了，先不肝异步了

# 2021年1月7日 #
- 上午没干到啥事，中午去了自习室学高数，前面的题目都整理完了，开始了积分的学习
- 本来打算0点开始学高数的，学着这个协程就停不下来了
- 协程大概能实现简单的并发运行了，整理一下思路步骤：
  1，创建好协程
  2，创建好任务单（把想执行的协程写在一个列表里）
  3，创建循环时间：`loop = asyncio.get_event_loop()`
  4，运行这个事件循环：`loop.run_until_complete(asyncio.wait(renwu))`
- 今天就到这里了，剩下几天就尽量不学py了，搞一波高数了

# 2021年1月6日 #
- 上午考数逻和py，没啥好说的，考的还可以
- 回来发现群里的都在搞kali，我也试着搞了一下，kali四个g我下的太慢了，后来找乐子哥U盘拷贝的，没有去配置，下次再说这个
- 学了一点python的asyncio模块的使用（异步 IO）：按照博主的解释async是异步，io是等待，可交给 asyncio 执行的任务，称为协程（coroutine）,继续肝，内容比较多就记在博客上了

# 2021年1月5日 #
- 上午起的晚，十点多才醒，中午吃完饭十二点半就去了教室自习，肝了一下午数逻，感觉复习的差不多了
- 健身回来晚上继续肝了数逻，十一点算是过了一遍，准备再全部溜一遍就睡觉了
- 今天一点代码都没学，但是学长发了个题，一开始看到这个登入框就想到了弱口令爆破，加了四个字典两万五千多条密码，解到一半，学长说扫后台，我一开始拿蚁剑来扫的，但是没密码，蚁剑好像也不能爆破，就去网上下了一个御剑来爆破一波，拿到了后台目录，发现学长在群里发了御剑。。。但是由于开发还是太烂，看不懂PHP不然这些php我得好好审计学习一波，明天考试，也不敢花太多时间一个个函数去学。先把考试过了，再学一波开发了，有一说一，自己爆破出后台目录很有爽感哈哈哈。

# 2021年1月4日 #
- 凌晨失眠，想着早点上床，一直睡不着，想一些乱七八糟的
- 上午去了教室学了一波高数，下午整了一波爬虫，然后去了健身
- 晚上也在肝爬虫，实现了豆瓣的动态网页的爬取，记录在了博客上，怕再失眠浪费时间，就直接肝到了一点半困了就上床秒睡了

# 2021年1月3日 #
- 今天早上起得早，八点起来去自习室学数逻复习到了只剩下了最后的选择器和时序电路了，明天或者后天可以完全复习完
- 下午也泡在自习室，肝完了职业规划，过了一遍python笔记
- 下午四点回宿舍，又开始学起了爬虫，其实主要是夯实，至少把之前学的全部都理解了，并把理解详细的写在了博客里
- 晚上健身回来继续肝爬虫，实现了有道翻译功能的动态爬取，学了一下json库和json的相关知识
- 今天学了十几个小时，挺充实的，再接再历

# 2021年1月2日 #
- 早上依旧11点起来的，太咸鱼了
- 下午又开始爬虫的学习，有人说bts4没有lxml好用，我学习的博客也用的lxml
- 回来差不多七点，又开始了爬虫的学习，大概学了xpath的运用，能爬文字和图片了，把理解写和过程到了博客，一直肝到晚上2点，感觉不错

# 2020年1月1日 #
- 元旦时节，早上睡到了11点才起来，发现社团团建，马上赶过去吃了个火锅，贼爽，听学长的描述让我动力满满
- 下午回来开始了爬虫的学习，感觉很有趣
- 晚上去自习室学了两个小时的高数，自习室真冷，下次不去了

# 2020年12月31日 #
- 上午都在写python题，挺有难度的，对于编程没什么太大的收获，但是对于思路有一定的帮助
- 下午啥都没干，晚上去外面吃了个饭
- 明天开始重回轨迹

# 2020年12月30日 #
- python把作业写完了，明天python上机推进度
- 高数只写了两题呀，惭愧惭愧
- 整理了一下博客文件
- 今天太咸鱼了，杜绝这种状况

# 2020年12月29日 #
- 高数只整理了一下错题，没做太多事
- python把字符串的函数都过了一遍，做习题发现有个知识点的遗漏，列表推导式
- 英语口语练习

# 2020年12月28日 #
- 高数大概总结要复习的内容，做了一些错题笔记
- python没学太多，主要复习了一下。
- 网站算是暂时竣工吧，有实力了再搞个服务器备个案
- 数逻结课，感觉还不错，出的题都写得出，准备开始全面复习了

# 2020年12月27日 #
- 又肝了一天的博客，想实现双线部署，实现是实现的了，但是没太大的作用，coding现在给分配的ip是国外的，访问速度还是比较慢
- 现在都搞出问题来了，唉，越搞越错，把问题解决了，博客就先放一段落

# 2020年12月26日 #
- 晚上肝python肝到了2点，差不多把魔法方法过了一下
- 装修了一下博客，应该短时间不会做太大改动
- 下午去自习室学了两个多小时的高数和数逻，学着心情有点不好，很烦躁
- 下午到晚上两点都在实现双线部署博客，买了一个域名，但是访问速度没有什么提升
 
# 2020年12月25日 #
- 学了一点python的魔法方法，大晚上的十一点半才开始学，太怠惰了
- 上午整了一上午高数，下午思修也整了一节半课的高数
- 回来宿舍做了两题ctf，安装了一个蚁剑，感觉使用起来比菜刀体验要好，设计的更舒服吧
- 跑江科后街吃了一顿，有一说一，那里的臭豆腐挺好吃的哈哈哈
- 英语又鸽了，总是提不起学英语的欲望
  
# 2020年12月24日 #
- 学了一些python的魔法方法，试着用类和对象写了一个计时器，
- 记录我第一次旷课哈哈哈，职业生涯规划旷了，在宿舍又折腾我这博客，改了一个butterfly主题，还得是这个主题，看了一些大佬的博客魔改的是真的好看，以后再慢慢优化吧，现在用的简单点
- 圣诞节班里的礼物挺好的，是我收到的最高配的礼物了，甚至还有圣诞老人！
- 高数继续整，希望不挂科

# 2020年12月23日 #
- 体育卷子昨天写到了十二点多，直接肝完了
- python学了一些与类和对象相关的BIF：issubclass,isinstance,hasattr,getatt,setattr,delattr,property,学了第一个魔法方法构造和析构
- 前端放了，没学前端
- 制作了一个错题本，把之前遇到的高数错题好题整理了一下
- 数字逻辑把同步的触发器全部自学完了，发现还有主从触发器和边沿触发器，真的是淦
- 整了一晚上，搞到了十二点五十，把对__new__函数大概弄懂，写了一篇博客加深了印象，累了累了

# 2020年12月22日 #
- python准备学习魔法方法，听说很难
- 前端作业写完了，但是没有继续听课了
- 下午和晚上都在学高数，直接复习到了导数和微分，再接再历，高数有救
- 找到了英语听写的神器，竟然就在我的手机里，有道翻译就可以直接听写，花了一个小时整理了三个单元的单词，没想到这么花时间

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
