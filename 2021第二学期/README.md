本学期目标

- 完成javaweb的基本学习
- javascript，xml快速入门级学习
- 独立写完一个大项目，用javaweb实现的后端的动态网站开发
- nodejs尽量能开始学习
- 继续完善web的技能数和自己的方法论



# 2021年8月17-24日

- 打了两天的祥云杯，大佬云集啊，web这次只写出了两题，其他的都是java和nodejs的题了，感觉现在的题都向java和nodejs偏移了，可能这个就是以后的趋势了，那么开发就更加的重要了，开发搞起来才有出路了

- 这次的web一题是yii的一个公开的poc打的，是一个签到题，还有一题是ssrf，这个ssrf倒是挺有意思的，想了很久终于还是打出来了，本来是想session_upload打的，但是无意间注意到直接提交就能有session的回显，那么久用这个特点去进行包含，这题属实是运气比较好，但是在众多大佬眼前，这个也是个签到题。。。还是自己太菜了
- 看了剩下web题目的wp，真是看不懂了，太菜了太菜了，层层穿透那题涉及的fastjson是真没做过，还有frp代理也从来没打过，唉，太难搞了
- misc这边做了一个内存取证的题倒是比较有成就感的，之前遇到的一个工具FTK真是神器，好多镜像都能直接打开浏览了，思路变的特别清晰，一开始找到hint，叫我们仿真登陆镜像，这是没接触过的，百度和谷歌搜了好久，终于找到一个比较好的方法，先把镜像挂载起来，然后开vm的虚拟机，仿真登陆win7系统，但是登陆是要一个密码，在mem文件中volatility找到系统密码hash，拿去md5出密码，再登陆了系统，找到流量包和一个新的提示，给了一个word的密码，在流量包里面找到了一个rar压缩包，里面是word文件，打开就是flag

# 2021年8月16日

- arm的mac安装ctfd平台出了问题，有些库装不上，去自己的vps上搭了一个ctfd，vps上倒是特别顺利
- 搞了一波docker，基础的操作以及没什么问题了，部署了两个题到vps的ctfd上，上传了一个去dockerhub
- vps上跑ctfd的时候，外网无法访问，我看网上的教程都是利用python的一个库去转发端口，但是我自己的vps上跑不起来这个东西，没作用，后来看里面的serve.py的源码，里面的127.0.0.1换掉就可以跑了。。真无语，在本地的kali搭的ctfd用这个库去转发，网址访问速度还慢的一批，真不知道为啥要用这个来转发
- 在本地搭了一个乌云的镜像库，一个peiqi的文库，docker真香

# 2021年8月15日

- 一个朋友给了一个反序列化的题，没事干就看了一下，是一个国外比赛的题，难度倒是挺低的，刚好想起学校ctf平台缺题目，所以几打算搞一个题上去，然后就想着先自己本地看看怎么玩转这个ctfd平台，在kali搭建了一个，然后就是docker的学习，搞了一天，也算有点收获

# 2021年8月14日

- 在buu刷了一波题，第一次做了python的题，之前一直没有搞python开发，一直没去下手搞python题，最近发现好像很多题都是python和java和nodejs的，所以就想着去做一做，这次感觉还行，其实也就是那些步骤，看开发的路由，代码审计，这次做的题是SSRF me，这里学到了一些新的东西，hash长度拓展攻击，他可以在一个字符串后面拼接另一个字符串，而md5值不变，那题有一个解法就是利用这个去伪造token去进行ssrf
- 这次还做了一个javaweb的题，不过这次的没有什么代码审计方面的知识，主要就是对javaweb项目结构的了解，最近也在搞javaweb的开发，这题是有一个任意文件下载的点，但是javaweb的结构很复杂，不知道flag会在哪里，这里就考察对javaweb项目结构的了解了，我直接打开最近在搞的javaweb项目，访问/WEB-INF/we b.xml看servlet的位置，再去classes目录找到class文件直接看源码，找到flag

# 2021年8月13日

- 遇到一个杂项的题题目描述是说捡到一个硬盘，下载下来是一个E01后缀，是encase的一个镜像，但是在百度和谷歌都没找到能用的encase，能下的全tm在csdn，下载要会员，真恶习，后来找到一个内存分析的软件，也可以打开E01后缀的镜像，里面有一个文件夹，里面有四百多个子文件夹，文件夹的名字是一串串的base64，我用python把整个base64跑出来，但是在decode这里出了问题，直接去decode出来的和一条条decode出来的不一样，最后一个decode出来有一个PK在后面，但是整体去decode却不是，估计是哪里漏了什么东西，懒得管这个题了就放掉了
- ctfshow继续刷题，这次刷的sql注入的题，前面几十题简单的就当作复习了，后面遇到没见过的再总结起来
- jsp的学习，继上次的jsp内置对象继续学习，相关内容已记录在博客

# 2021年8月12日

- 有个海南大学的内部赛，混进去玩了一下，主要是这次的杂项，学到了一个usb流量分析，跑网上的脚本，是一个键盘流量，试了两个密码学的题，感觉还行
- web方面差一个题，这个题只能晚上12点做。。。时间是在服务区设置的，只能等。。。是一个flask题，要求提交一个参数，这个参数会进一个函数，但是这个函数是不知道的，唯一能操作的就是这个提交的参数，题目描述说写下出题者的姓名，但是都试过都没有，就没管这种傻批题了

# 2021年8月11日

- jsp的学习，jsp的九大内置对象的学习

# 2021年8月10日

- javaweb的学习，已经过完了servlet，重看了一遍新视频的servlet实战开发，就开始了jsp的学习了
- 主要学习了jsp的本质，他的本质还是servlet程序，我们访问jsp的时候，Tomcat会帮我们把jsp页面翻译成一个java源文件，然后编译成.class字节码程序
- 然后是jsp的语法，有这几种种标签`<%@ xxx %>`是头部page指令标签，`<%! xxx%>`是声明脚本的标签，`<%= xxx %>`是表达式脚本标签，在页面输出数据用的， `<% xxx %> `是代码脚本标签，这个就是用来编写自己需要的功能的标签，写java语句

- 在Github上找了几个javaweb的小型项目，下载到了本地准备看看别人是怎么写的

# 2021年8月8-9日

- 捣鼓了一天的mac，装了好多东西，感觉mac是越来越好用了hhh
- 熬了一个通宵，强行调整一下我的生物钟😂
- 上周开发一直没搞，这周继续开发的学习了，已经偏离太多了，开发要搞起来
- 之前在mac上调这个javaweb一直操作数据库失败了，也没找到原因，后来在用这个mamp的时候发现这个东西竟然自动关闭了mysql外部的接入，搞得我一直失败，后来打开后再去测试，又错了。。寻思是哪里搞错了，打开windows里面的数据库一看，tmd字段名写错了，passwd写成了password，难怪连不上，改完就成功的操作到数据库了

# 2021年8月5-7日

- 捣鼓了一下m1的虚拟机，现在已经可以装win10了
- 挖洞中，人生第一个高危终于过了！！
- 挖了一个站，好多站点，感觉很有可能打进去，找到了一个通达OA的洞，可以得到在线人的cookie，但是扫了2000下，一个人都没有。。。等开学了再看看这个洞，进后台再看看能不能getshell
- 因为用冰蝎一直失败了，所以在自己的vps上测试了一下，自己传了一个冰蝎马上去，后来成功的连上去了，这个冰蝎是不能连自己写的一句话，只能连他自己的冰蝎马，还有一个比较有意思的发现，自己的vps被钟马了，腾讯云会发短信和微信来通知，并把文件都标出来

# 2021年8月3-4日

- 刷了一些文件上传的题，这次的刷的题主要是配合这文件包含来使用的
  - 第一是php伪协议配合.user.ini的结合，先传一个.user.ini`auto_prepend_file=shell.png`，然后再传图片，里面的内容就是php伪协议读取flag.php，这里有一个waf就是不能出现php，这里就是用`.`来拼接绕过的
  - 然后就是一些二次渲染，分了两种，一个是png的二次渲染，一个是jpg的二次渲染，由于题目会识别图片内容，所以加上了二次渲染，传上去再进行文件包含执行命令
  - .htaccess的使用，这个是老朋友了，不多说，不过这个文件可以有很多的用法，我现在暂时只会一种`SetHandler application/x-httpd-php` 
  - 免杀马的使用，这里我去网上收集了七八个免杀的小马，就是用各种方法去拼接出命令的执行语句
  - 日志包含，之前没接触过过，一直不理解日志包含，这次就遇到了，其实原理也很简单，就是让一句话的木马出现在log.txt，再去包含这个日志文件，php遇到这个一句话木马就会解析从而实现攻击，这里遇到的通常就是改UA头

# 2021年8月2日

- 挖到了第一个高危getshell，激动，看了一晚上的信息收集，在收集浙江万里学院的资产的时候，找到了一个CVE-2019-0604，goby直接打了一个马进去，我去github上找了一个脚本去打，没打进去，然后在里面找到了一个管理员的账号密码，进后台去看看能不能找第二个getshell，找到了一个文件上传点，可惜是白名单，绕不过去，他这个waf首先是不允许php，但是这个过滤在发送的数据包里面，是可以修改的，过了这一层过滤，他还会检查文件内容，删除掉里面的木马，我想着能不能再过滤了第一层的时候就马上去访问这个暂存的文件，但是发现他发现不是图片后会上传不上去，后来我打算先传一个图片，找到他们的返回包，然后再传马上去，伪造一下返回包，但是他还有一层，他要裁剪图片，他发现文件内容不是图片，也会直接删掉文件，搞到半夜四点还是搞不进，就放弃了。。

# 2021年8月1日

- 鼓捣了一天的cobalt strike，在自己的vps跑了一个服务，打了本地的windows一下，这个东西还真挺牛，但是本地win提权没成功，键盘记录无法获取
- 继续挖洞，找到一个进了后台的，但是上传shell这里有点问题了，这个站首先上传是白名单的，能改的我都试过，后缀换了是传不上，其次是他的后缀是portal，这个后缀我百度了一下，一脸懵逼，就算能传都不知道传什么马，再次他的上传路径没有漏出来，只能暂时放弃了



# 2021年7月31日

- 巅峰极客ctf打了一波，但是很遗憾，考的python和nodejs我都不会写，只能再慢慢学了，晚上挖了一下src，只有一个信息泄露，我太难了

# 2021年7月30日

- 看了一个regexp的正则注入题，正则注入的思路就是先闭合，有waf绕waf，如果字符有的过滤了就要用hex来绕过，像之前的红明谷sql题，这里用的`admin'||pass/**/regexp/**/'.*'#`，这个pass是字段，因为过滤了select，没想到还可以这样的绕，学到了，然后就是用户名和密码去跑，跑出来三个用户名三个密码，有一个md5可以解出来，登入就拿到了flag
- 挖洞中，可惜的是今天一天都没产出，好烦

# 2021年7月28-29日

- 开发的学习，response的学习
- 29号还停电了，去工作室配置了一下mac的环境
- 写了一个php特性的题，自己是没琢磨出，学长给弄出来了，回头总结一下

# 2021年7月26-27日

- 实现servlet的注册，之前的小项目只有登录竟然忘记了注册，这次正好就当重温，再搞了几个servlet实现注册功能
- 实现的时候，除了之前的JDBCUtils没涉及，这次剩下的都过了一遍，理解的也差不多，就是这里的BeanUtils有点忘记是干啥来的了，翻笔记好像也忘记记载了

# 2021年7月25日

- javaweb的学习
- 看了一下这次XCTF的比赛，NAN战队做出了14道题，真牛，可惜我没参赛，看赛后能不能看看wp学到一点东西

# 2021年7月21-24日

- 回学校了，一切都要开始步入正轨了

# 2021年7月17-20日

- 生病的太难受了，去医院打了一天针休息了两天
- 网课这边还是继续看的jQuery，回学校后开始猛肝

# 2021年7月15-16日

- 下乡了一天，一回老家就生病。。。好烦
- js的学习，jQuery的学习开始

# 2021年7月15-17日

- js学习
- 感冒了，没啥精神

# 2021年7月14日

- 坐一天车回老家了，晚上开始开发学习，准备先补一下之前漏学的js
- js中记录一些小知识点：
  - arguments可以让无参函数传参，arguments[2]这样表示传入的第三个参数
  - 对象定义：`var 变量名 = new Object();`
    - 属性定义：`变量名.xxx = xxx;`
    - 方法定义：`变量名.xxx = function(){}`
  - 另一种定义方式 ：`var 变量名 = { 属性名:值, 方法名:function(){}};`注意要用逗号
- Document对象及其方法的学习，意在把标签属性等用对象来管理，Document.getElementById()这类的来获取Dom对象

# 2021年7月13日

- 坐飞机回广州，还是第一次坐飞机

# 2021年7月12日

- 上午抽时间搞了一波javaee，写了一点基础编程题
- 下午在配vscode环境，搞了好久md，这个晚上十一点才成功debug
- 晚上再看看http协议

# 2021年7月9日

- 四点睡觉，六点起床，再坐十多个小时的车，实在是没力气学了，困死
- 路上看了一波HTTP协议

# 2021年7月8日

- 重温java基础，类的定义，数组的定义这类的基础内容
- 微信读书在看HTTP协议图解，看完就准备看看java编程实例，再然后是计算机网络，希望暑假能看完



# 2021年7月8-12日

- 草原之旅，学习倒是怠慢了，回去加倍补回来

# 2021年7月7日

- 做了半天车，晚上做了一下小目标，重新复习一下java基础和javaweb基础

# 2021年6月20-7月6日

- 漫长且痛苦的期末复习，考完咯
- 明天开溜，假期学习开始，冲冲冲

# 2021年6月17-19日

- 国赛
- 第一天被打的很惨，一开始啥都不会，很慌，利用密钥来连接远程主机，id_rsa文件，一开始连不上，后来发现是用户名打错了，xctf打成了xcft。。。环境全被别人搅屎搞坏了
- 下午才开始有点点输出，写了一点自动化脚本跑
- 第二天就比较有经验了，一开局就去连xftp了，然后再kali用命令连接一波来执行命令，把www目录给备份下载下来，然后做代码分析，然后就是看流量包了，找到攻击途径，马上写出自动化脚本，然后就去代码审计，找出漏洞出现的位置，不知道为啥选宽会觉得代码审计是很简单，但是他觉得简单我也不多和他说了哈哈哈
- 调整好心态，别管别人怎么说，好好做好自己的事情，渗透冲冲冲

# 2021年6月14日

- 端午节休息了一下，下午去打了一场篮球，晚上肝高数
- 希望期末不挂！！！

# 2021年6月13日

- 上午一上午停电，挺无语的，下午三点才开电脑
- 继续肝强网杯，搞了一个杂项，还可以哈哈哈

# 2021年6月12日

- 今天上午考四级，过不了，下次吧。。。
- 下午打强网杯，好难，被别人打击到了，要好好反思，暑假冲爆他

# 2021年6月11日

- 学了一波线代，脑袋疼，，，
- 数据结构里搞得图出了bug，不过解决了，明天准备打个ctf了，强网杯
- 

# 2021年6月10日

- 肝了一波数据结构，实现了一下图，明天准备实现广度优先遍历，加油，争取都过
- 好想买MacBook啊。。。

# 2021年6月8-9日

- 挖了几个洞，交了src，不知道能不能拿分，护网后对于资产收集有了更明确的概念，不像以前那样拿扫描器去通扫了，希望早日挖到可以getshell的站吧

# 2021年6月6日

- 上午来了个学长，绿盟的，来学习讲了一下课，也就四个人听。。。不过还是学到了一点点，关于以后工作的事情
- 中午在外面吃了个饭，下午就去八一纪念馆拍了几个视频，准备交作业，下午回来睡了一下，就去打了一场球，这周就当休息了一下吧

# 2021年6月5日

- 校赛结束了，提权还是没有成功，后来找中南大学的师傅交流了一下，说是redis-cli提权，害，还是别人厉害啊，加油冲冲冲，至少成绩在本校还是可以的哈哈哈
- 上了一天的形势政治，晚上又去外面和室友去玩了，休息了一波，明天还要去外面排短片，这个双修是没啥时间学
- 最近的任务主要是加强学习课程的跟进吧，可别挂机了

# 2021年6月1-4日

- 赶课程进度，太多没学的了，已经开始慌了。。。。
- 又a了两个校赛题，一个是cookie里面有一个编码用来验证身份，找了一波规律，是这样的，绕过ascii是奇数就ascii+2如果是偶数，那就ascii-2，所以注册一个adminadmin，截取一半的cookie就成了
- 还有一个是mssql的，好像也叫作sql server，的确是差异备份getshell，之前过滤的()在前加上一些特殊的符号就可以绕过了，比如%1e，这样就可以执行sql语句了，之前查询不到库名，现在也可以通过master..sysdatabases来查询库名了，然后就是备份了，他把backup database这类的语句都过滤了，你过滤一个就算了，全部过滤就有点此地无银三百两了，应该就是用一个方法把他们全部过滤掉，发现在语句中间加上%1e就可以绕过了，然后接上蚁剑或者菜刀就可以去c盘找flag了
- 提权题给了hint和没给一样，了解过提权的谁不知道要去提权才能进root啊。。。

# 2021年5月30日

- 打了一波校赛，没啥输出了，那个backup，是mssql不是mysql，利用他的报错，注入到了字段，但是就止步于此了，过滤的太严了，好多操作都做不了，名字是backup，但是却和mssql的典型题型备份差异写webshell拉不上关系，把log备份和库名备份都过滤了。。还不能用括号，那么查询语句也用不了，很多函数也用不了
- backup这题实在打不进了，就去看google那题了，想到登录框可以sql注入，为什么不读取一下信息呢，而且有报错，可以使用报错注入快速的获取到信息，一打，果然是这样，成功得到admin和他的密码，然后还有一个是一个key，拿着这个key，base64解码一下，得到一个secret，估计就是google的密钥了，看网上说是base32加密的，拿去加密，果然是，里面还写了一些话，然后拿这个密钥去网站找php的谷歌验证码生成的脚本，拿到验证码，去提交就得到了一个php文件，里面已经写好了一句话，开蚁剑连上去，在根目录有一个run.sh，会把flag写进/root/flag.txt，但还是没有root权限，吐了，提权不会，只有之前打了两个vulnhub学到一个find提权一个git提权，其他的在网上找了一下方法，时间任务好像也不行没有写的权限，脏牛的好像也不行，没有gcc命令，然后就是无头苍蝇了，差最后一步提权了，好气啊

# 2021年5月28-29日

- 护网结束，很累，最后一天还是被我们getshell到了，一个学校的站，我中午准备睡觉的时候，测出了一个弱口令，里面有上传文件的功能，检验方法竟然是前端发送一个数据到后端，那就抓包直接改了，成功上传后，猜测到了上传路径是uploads/1.jsp，用蚁剑，加上cookie成功连接进去，然后学长就拿着提权了一下，探测了一下内网的ip，我找数据库的初始化文件，找到系统管理员的账号密码，又加了一波分

# 2021年5月27日

- 护网第四天，发了第二批目标，但是两个都是gov。。。还有一个站一扫就ban掉了
- 分了一个萍江学院过来，资产收集的倒是挺齐全，但是后来爆破多了，也被ban了，后面就真没得打了
- 整理了一下方法论，PHP_SESSION_UPLOAD最近遇到两次了，整理了一下

# 2021年5月26日

- 护网第三天，实在没什么挖的了，明天再看看吧
- 找到高中母校的弱口令，但是也没打到什么，云存储的，不解析jsp。。。。

# 2021年5月25日

- 护网第二天，找到其他的弱口令，但是没什么用，权限太低了，然后挖了两个存储xss，写了个报告交上去了，留了一个搞cookie

# 2021年5月24日

- 护网的第一天，搞出了几个弱口令
- 好累一天

# 2021年5月21-23日

- 这几天打了三个比赛，neepuctf，宁波市赛，美团ctf。
- 宁波是险进，压轴进的hhh，好多题目是有别人的环境写的，还有原题，密码学一题flag没交上。。
- 美团的是只出了一题，思路总是局限于闭合sql语句，学长说很多题目不闭合，而是用反斜杠转义
- neepu的web最后一个，是session_upload配合session反序列化，但是我打到了22号晚上三点都没打成，等复现打一波
- 明天护网了，冲冲冲

# 2021年5月19-20日

- 20号凌晨找到了一个getshell，peiqi师傅牛逼！！但是没有利用上，连不上蚁剑，不过文件确实是传上去了，把漏洞交给学长了，到时候护网打一波hhh
- 搞了一波数据结构，学了一下二叉堆实现优先队列，小看数据结构了，还是有点难度的
- 打了一波新冠疫苗，一天都困的。。。今天就早睡一点了，明天继续搞
- javaweb的开发准备在护网结束或者护网晚上回来看看

# 2021年5月17-18日

- 又打了一台vulnhub，感觉还可以，学到了挺多ctf里面学不到的操作，比如git提权，很多工具的使用，kali里面集合了很多工具，有一个可以用爬虫查网站敏感信息来爆破的工具
- 重新建了一个gitbook来记录渗透的知识，工具使用，小技巧之类的，慢慢积累
- 18号倒没打vulnhub了，打了一下ISCC，出来两个杂项，这个CRC32爆破的CRC值竟然不唯一，跑脚本出来的可以跑出很多来。。。
- 马上去护网了，收集了一波江西高校的子域名，搞了1600+条，到时候慢慢扫，希望我能有点输出

# 2021年5月15-16日
- 最近比赛多，真是类，还得考期中，就刚好对到了国赛。。
- 国赛打了一波，自己还是比较满意的，进线下应该稳了
- 希望西安的线下不会和护网重掉
- 国赛搞了一波通宵，生平第一次通宵，下午团建一起去外面吃了顿饭
- 很多渗透大佬说想提升可以搞个vulnhub去做渗透，晚上搞了一波vulnhub，打通了一个DC-1，感觉很不错，以后继续打


# 2021年5月13-14日
- 打了一波宁波的杂项题，jpg解密总结了一波，第一次遇到了文件内容反向读取的题，方法也总结了一波
- 初识openssl加密，写了一下aes和des加密的题目，ISCC的那个web搞出来了，写了个脚本，比18年原题的wp要简单哈哈

# 2021年5月10-12日

- 漏了很多天，忘记了。。。
- 打了一波ISCC的web和杂项，貌似都遇到了AES加密和DES加密，去学一波
- 最近两天都在搞宁波的比赛，两个sql注入，一个User-Agent注入，一个过滤了很多，用regexp来替换了等号做的，在win10上跑了个寂寞，每次都出问题，今天放到linux里面跑，贼舒服，又快又对
- 杂项遇到的都是不熟悉的知识点，学到了很多操作和工具，BWM盲水印，CRC32爆破宽高，进一步了解了一下LSB隐写，对于图片隐写理解更深了

# 2021年5月9日

-  今天打了两场比赛，红帽和津门，web题第一次涉及到了disable_function函数的绕过，我是传马直接用蚁剑的插件绕过的
- 还是那题，涉及到了一个assert，可以执行php代码
- 还是那题，第一次找cve复现成功，还是独立完成的，也大概看了一下，理解起来也算比较简单的一个链子，算是今天唯一欣慰的吧
- RGB的杂项题，这题着实把我给难倒了，看学长的提示都复现的很吃力
- 布尔盲注跑密码真是我的一生之敌，每次都跑不对。。。
- 听说红帽的最后一个是0day，希望能看到wp哈哈哈
- 半夜睡不着，学了一波phar反序列化，实现的原理就是phar里的Meta-data的信息会序列化后存入phar文件里面，当这个phar文件被phar://伪协议读取到的时候，就会触发反序列化，从而达到攻击效果

# 2021年5月8日

- 计组把我搞自闭了。。没想到每科都要期中考试，吐了，本来就没时间学了。。。
- 重新搞了一下goby，换了一个老版本的，新版本的感觉好多问题

# 2021年5月7日

- 总结方法论，把杂项和src的方法总结了一下

- 今天摸了好久的鱼，好烦。。。

# 2021年5月6日

- 看到NU1L战队的预备战队要招新了，学长说让我试试，试着投了个简历，没想到还真进了，希望后面能好好发展吧
- 学了一波区块链的智能合约的知识，试着写了一下ISCC的区块链的题目

# 2021年5月5日

- 打了一天比赛，累死掉，wp已提交到csdn，还挺多人看的。。。

# 2021年5月4日

- 坐了一天车，累死了，下午打了一波篮球，回来困得又睡了一觉。。
- 晚上继续javaweb的学习，把response类学完，想实现博客系统的开发，还是差了比较多，准备看看动态博客那里的数据库是怎么设计的

# 2021年5月3日

- 打了一下ctfshow的大牛杯，写了一题出来，质量感觉还行，做着挺舒服的

# 2021年5月1-2日

- 通宵坐火车回老家，睡到中午就去吃酒席了，下午去下乡看了一下
- 回来下午在弄菜，休息了一下午，吃了晚饭就去打球了，晚上回来就写了一下iscc的比赛
- 有点上头，打到快四点钟才去睡觉
- 2号白天继续打比赛，搞出几题web，还是比较开心的，学到了一些东西，差一题ak哈哈
- 准备半夜和好兄弟去聚一波，吃波夜宵



# 2021年4月30日

- 水了一天的课，下午去打了一波球，晚上准备了一下准备回老家了，很想老家的吃的哈哈哈
- 在家里的三天希望自己能保证web的学习，也要兼顾学校课程的学习

# 2021年4月29日

- 蓝帽杯打了一波，有一说一，题目质量很差，我只写出了一题来，杂项有一个emoji解密的差最后一步。。。web题出的很烂，第一题五百多解，第二题才一个解，不过学到是也学到了一些，比如foremost的使用、MP3解密、wengdings符号解密，还有一个github的cve



# 2021年4月28日

- 继续javaweb的学习，学习了一波response对象的知识，学了一下重定向并实现了一下，还区分了一下重定向和转发的区别

# 2021年4月27日
- 本来想早点睡觉的，肝上了一道题，在php版本大于7.4的时候可以定义__unserialize方法，反序列化方法，当执行反序列化的时候会执行这个方法，那题用这点来使wakeup函数失效，从而造成干扰
- 继续写题，写到了一题反序列化的字符逃逸，之前写过一题，现在算是巩固了一下知识
- 写到了一题session的反序列化，肝出来就睡觉
- 算是大概了解这个session的反序列化了，当开启session的时候，会在服务器的/tmp里面生成一个session，而php对于这个东西内置了三个引擎，分别对应这三种不同的存储格式
  - 漏洞出现的原因就是**使用了不同的引擎**，1.php使用了php引擎，2.php使用了php_serialize引擎，这样就可以通过修改session的值来进行攻击
  - 页面需要使用某个session的时候就会去调用，调用到就回去反序列化，这时候如果反序列化到了我们构造的恶意session就会出问题

# 2021年4月26日
- 刷了一波ctfshow的反序列化，学到了一个soupcilent原生类，用于发送post请求，常用SSRF和CRLF
- 说到CRLF，我也是第一次遇到，在http请求体里面，可以使用`\r\n`来表示换行，这样就可以自己伪造一个http报文，传递攻击信息
- 这段时间偶尔刷刷题，维持一下手感

# 2021年4月24-25日
- 肝了两天的页面算是成功了，前端搞了一个晚上，后端搞了一整天，熬夜熬的颈椎都有问题了。。
- 实现了java后端的登陆，还有response要学，这次先涉及到了但是还没正式开始学
- 国赛报名了，希望能有好成绩
- 发现javaweb的开发真的是很麻烦，php里简简单单的一个操作，java偏要搞出一大堆类来东跑西跑。。。
- 发现自己的java基础很薄弱，虽然成功完成了案例，但是很多知识点都还是去网上查了，明明是跟着视屏学的为啥我的很多知识点就没学呢
- javaweb的登陆案例的大概思路是这样：
  1. 前端开发，把username和passwd给发送到后台
  2. 创建一个javaBean，User类，用来封装前段传进来的信息，实现setter、getter、tostring方法
  3. 这里要提取JDBCUtils（有个小坑，druid.properties要放到resource里面，不然加载不出），JDBCUtils要实现：预定义连接池对象、在静态代码块中（加载配置文件、初始化连接池对象）、获取连接池对象的方法、获取连接的方法
  4. 创建UserDao类，用来操作数据库，里面设置一个login方法，该方法传入User对象，执行查询语句查询User对象的数据是否存在数据库，在login方法里使用JDBCTemplate来操作数据库，获取执行sql语句的方法要使用queryForObject()，返回一个User对象
  5. Servlet的实现，获取到前端的输入后，把参数用BeanUtils封装成User对象，再交由UserDao的login方法来判断是否查询成功，得到结果转发到successServlet或failServlet

# 2021年4月22-23日
- javaweb开发，感觉最近效率有点低。。
- 24号开始登陆注册页面的开发吧

# 2021年4月21日
- javaweb继续推进，感觉不需要多久就可以开始网站开发了
- 最近学校课程学的很累，尤其是计组，前段时间没听就跟不上了。。。

# 2021年4月20日
- 肝到凌晨两点半，扛不住了，上午上了两节课套了个高数继续回来肝，在中午终于肝出来了，写了一个wp，成就感满满
- 继续javaweb的开发，学完了servlet的基础，学完请求就可以开始登陆注册的开发了
- javaweb快成熟的时候就开始做大项目了，搞一个动态聊天网站，看下这个学期能不能完成

# 2021年4月19日
- MRCTF的wp终于出来了，好家伙，这个web是真难啊，最简单的一题poc都有一百八十行。。。
- 复现了一下那题CVE-2019-9081，最开始就要构造一个原生类来读取key，读取到key后再利用cve漏洞poc结合这题的修改重新找一条路来执行命令，是真的折磨，这个CVE-2019-9081太复杂了，以我现在的实力还不能完全的复现，就只能用用poc

# 2021年4月18日
- 被计组折磨的一天
- 漏洞方面，对于挖洞的思路更进一步了，fofa的使用，poc的利用，资产的收集
- 找到了一个Kyan密码泄露的漏洞，扫到了好多出来，但是很可惜不知道去哪交这种，学长推荐不要去挖这种洞，我就先放弃了
- 写了几个爬虫来爬取大学的域名，复习了一下爬虫的使用和文件操作


# 2021年4月17日
- 开始servlet的学习，大概学了一下，今天肝完
- 买了一个FOFA高级会员，希望他值这个价吧
- 挖了几个信息泄露，就是不知道能不能过，感觉大概率过不了
- 准备收集一波江西高校的资产

# 2021年4月16日
- 挖到了一个严重的漏洞，未授权rce，但是我拿不到poc，大概学了一下反弹shell，在自己虚拟机是反弹成功了，但是不知道为什么在vds上弹不上，估计是防火墙的原因，一直说无法连接

# 2021年4月14-15日

- 14号接触了一下渗透，看了一点文章，学了一点思路
- 子域名扫描、nmap、Google hacking、goby等软件的认识
- 15号终于挖到了第一个漏洞，是江西外语外贸的存储xss，还是一下子爆出两个哈哈哈

# 2021年4月13日

- Tomcat搭建完成，已经可以访问了，相关内容也学完了，接下来就是servlet的学习了
- 装了一个Postman，原来之前看赵总的抓包工具就是这个呀，界面挺好看的，功能还是没有burp多


# 2021年4月12日
- javaweb继续推进，学完了Template，其他的倒确实很简便，但是感觉query方法好鸡肋啊，还说经常使用，这也太麻烦了，还要自己编写一个类来封装数据
- 明天开始Tomcat的学习

# 2021年4月11日

- 上午尝试复现一个weblogic的cve，目前的实力只能复现第一层，不过巩固了一下docker的操作
- 下午去参加活动了，晚上在宏毅培训，尴尬的很。。。他们的后端成员已经建了一个群
- 晚上回来搞了一下xdebug，配合phpstorm可以用来一步步的看，之前看一些大佬复现都用phpstorm来调试复现的，php的调试是真麻烦，搞了我快两个小时才搞好
- 肝完了连接池，抽取工具类这里出了一点问题，用一个很难看的方式解决了，明天继续

# 2021年4月10日
- 打MRCTF，打自闭了，唯一写出的是一个re。。
- 有一题web是cve，感觉最近老是做出cve的题，就想尝试去搞一下cve，太难了，几十个文件跳来跳去
- 班级说要搞一个oj，我试着用了一下docker，成功搭建了青岛大学oj系统，感觉还不错，后来一直在搞这个docker
- 想着复现MRCTF的cve，就去准备搭建的环境，安装了composer，这个可以直接搭建好一个框架，有时候需要老版本的就可以使用这个
`composer create-project --prefer-dist laravel/laravel=5.7.0 test`来指定版本


# 2021年4月9日
- 实现java的jdbc的工具类提取并成功测试

# 2021年4月8日

- 今天学的比较少，太累了，学并实现完了java的增删改查的操作

# 2021年4月7日

- 尴尬的发现flask的模板叫jinja2，我一直以为是jianjia2，全部写错了。。。
- 开始javaweb的学习，今天学了jdbc，jdbc就是用java实现对数据库的连接和操作，简单实现了mysql的连接和sql语句的执行，就是不知道为什么，getInt()得到的数据不知道变成了个啥数字，用getString()就得到了正确的值
- 把jdbc基础肝完了，明天再继续

# 2021年4月6日

- 第一次写到了xxe的题目，还是没有接触的一种领域，有时间去学习一波
- 转专业是提交了，希望能有预想的结果吧
- 花了180加了一个知识星球，感觉还是停止的，投资自己哈哈哈，发现先知社区真是web手的宝藏，好多干货
- 写了一万年的jianjia2模板注入，今天终于写到了一次其他的模板Twig


# 2021年4月5日
- 论文写了大半天，晚上才开始刷题，写了几题ctfshow的文件上传
- 想去复现一下之前比赛的题目，发现都是啥javaweb，感觉这就是web手前期的烦恼吧，没有前置知识，连碰这类题的资格都没有。。。
- 跑去打了一个国外的比赛，有一个题目会检测你xff的ip，给了一篇文章，知道了xff的ip可以有很多，一般的网站就是读取最后一个，因为大多框架都会把真实的加在最后，但是如果挂了代理，最后的ip就会变成代理的ip，网站识别的是与他们最后应用的ip，那个题就是检查第一个ip和最后一个ip是不是1.3.3.7，我不知道怎么去让最后一个ip为1.3.3.7，就卡死了。。。

# 2021年4月4日

- 今天凌晨肝到4点才睡，身体要垮
- buu刷了十题，准备开始总结我的方法论了，总结完成后打包发到网站里面

# 2021年4月3日

- 早上起来就开始打比赛，一直打了打到打不出了就刷buu去了，从上午10点一直肝到晚上19点，早饭午饭都没吃![img](file:///C:\Users\asus\AppData\Roaming\Tencent\QQTempSys\JSYTP{[X$W]SQL5MPZQMCKQ.png)，硬肝了八九个小时，江西省第三，还行吧，队友也给力哈哈哈，向学长学习

- 这次虎符比赛感觉web题很多是很接近真实环境的渗透的，第一次搜cve做题，复现漏洞

- 刷buu又一次遇到了无参数rce，ctfshow的web40就是这种，里面的正则有个`\((?R)?\)`这个的意思就是括号里面不能有参数，但是可以嵌套括号,例如这样（a())不能这样(abc)

- 复现昨天红明谷的那题正则sql，弄懂了那个查询语句，这个binary是参数的数据类型，不是啥函数。。这样可以直接用hex匹配字符串

  ```
  select(select/**/*from/**/f1ag)regexp/**/binary/**/0x{}
  ```

# 2021年4月2日

- 红明谷杯开打，差点打出那题命令执行，还是被学长抢先了哈哈哈，学长太强了
- 红明谷的sql注入是正则注入，第一次听说，晚上学习了一波，复现了一下

# 2021年4月1日

- 写了一点ctfshow的文件上传，涉及到了php的短标签<?=
- ctfshow的渔人杯wp出了，复现了一波，把web的给复现了，顺便写了几题杂项的题目

# 2021年3月31日

- 把报错注入大概弄懂，常见的有xpath和主键重复两种，xpath比较好理解，主键重复我看了比较久，主要是group-concat的时候，查询到虚拟表没有是数据的时候就会插入数据，而`floor((rand(0)*2)`在插入的时候还会执行一次，只要提到了rand就会进行一次计算，而rand获取的随机数是稳定的，\*2后加工floor就是011011，这样遍历随机数数据到第四条的时候就会出现主键重复错误
- 反序列化写了一题，发现个知识点，php7.1后对于类的权限修饰符不敏感了，所以protected和private里面的特殊字符如果过滤就可以直接改public，private的是`\x00类名`，`\x00变量名`同时处理类名和变量名，protected就只要处理变量名`\x00*\x00变量名`
- ctfshow的渔人杯打了一次，一题都没写出来啊。。

# 2021年3月30日

- 写了一个数字型布尔盲注，第一次写，感觉还不错

- 利用这个方式，结合二分法来去匹配flag的字符，写脚本跑出flag

  ```
  ascii(substr((select(flag)from(flag)),%d,1))<%d
  ```

- 写了一题报错注入，打算把报错注入都学一下，慢慢理解



# 2021年3月29日

# 2021年3月29日

- java基础学的有一点点了，接下来就是数据库操作，不知道宏毅用的是什么数据库
- 写了一题python开发的题

# 2021年3月28日

- java学习，社团教的也太潦草了，回来自己查资料肝了一波

# 2021年3月25-27日

- 继续java学习，明天准备跟社团参加一波培训
- 27号的一波比赛，第一次用到大马，实现的方法是改后缀为图片后缀，里面会有一个预览功能，包含了里面的代码，实现木马的运用，用了一个蚁剑的大马，很爽

# 2021年3月24日

- 又没来得及打卡。。淦
- 学了一波java
- 复现vnCTF2020的题，有一个需要反弹shell，了解了一波，但是没有成功，下次找个难度低的反弹shell来试一试
- 复现nepCTF的杂项，真的是难呀，签到题都这么难的，总的来说还是太菜



# 2021年3月23日

- 划水的一天，晚上吃了饭就看了一波nepctf的wp，linux的很多命令小技巧还是需要积累沉淀
- 看wp对于linux的>理解更清晰了一点，之前就是潦草的看了一下，今天学到这个叫重定向，所以`ls>1`的意思就是把ls的内容写入1，`>cat`就是创建一个文件叫cat，有一个命令`*>1`就通配符*，Linux会把第⼀个列出的⽂件名当作命令，剩下的⽂件名当作参数。这个操作还是有点迷
- 写了一波php特性，又遇到了变量覆盖`$$`，之前写还有敏感度，现在都忘了，真操蛋，还得多复习复习

# 2021年3月22日

- 远子哥熬夜进医院了，卷出问题了，不能再卷下去了，今天开始做出改变
- 学了一波java，整理笔记

# 2021年3月21日

- 剩下的题是真写不出了，只能等wp复现了

- 下午自习室一波，任务太多了，压力有点大

- 宏毅培训鸽了，类和对象自己差不多学完了

- 晚上写了一波bugku，学到了这个正则表达式，php的正则如果要过滤\\的话，就要写\\\\\\\，四个反斜杠

  其中两个是字符串里面转义反斜杠，转义成两个反斜杠后再到正则里面转义成一个反斜杠，有点绕，但是不知道为什么在菜鸟教程里面测试的两个反斜杠就可以了，题目里却要四个

- 第一次使用php://input协议，之前学到了，就是get这个协议，再post想要的内容，这样传值可以绕过一点一些过滤

# 2021年3月20日

- 中午起来就开始打nepctf了，第一题卡了我好久，就先放弃了，去看gamejs，每次做的js的游戏类都很简单，但是这题却实难，一天下来就三个解，后来就去写第二题，换ip就能做出来，比第一简单多了，不知道为什么第一题解出那么多，第二题这么少，后来写反序列化，是我迄今写过的最难的反序列化，学到并用到了一波pop链，就是初始化的时候去实例化一个别的类的对象，后面还有php原生类，用来删除文件，后来就是命令执行，也是我写的最难的一个命令执行，只允许10个字符，就用拼接的方法创建大量的文件来拼出命令执行

- 第一题解法，intval函数可以传2aaaa，识别到字母就停止，所以2aaaa就被认作2，后面的字符就可以逃过去

  这样就可以再数字后面接一个分号，后再接系统命令，再引用变量来执行命令

- 解了三题，个人感觉还不错，web区的题目不简单

# 2021年3月19日

- 早上突然来了一个人加我，问我关与yilia主题配置的相关问题，他好像23岁，知道我在读大一后吓一跳哈哈哈，说听完说像个老油条了，感觉还是不错了

- 刷了一波buu的题，写了三个难题，刚好复习到了一波.user.ini，但是出现了一个疑问，图片的文件头复制过去好像会变，只有GIF89a可以用
- 写了两个都是ssrf加反序列化的，用了一波post的sqlmap，说实话，sqlmap确实挺慢的，爆破了好久才得到表的信息
- 装修了一波桌面，简练了很多，看起来很舒服

# 2021年3月18日

- 刷了一波php特性的题，学到了几个函数的漏洞，in_array()函数，第三个参数没设置的时候1.php会被转换成1来识别，反射类：echo new ReflectionClass()获取类的很多信息，in_numeric()函数，在php5的环境下可以识别16进制，hex2bin()把16进制换成字符，bin2hex()把字符串换成16进制
- 有个小技巧，“<?=\`cat *`; ”base64编码后再转16进制，只有数字和字母e，会被认作科学计数法
- 写了几个文件上传的题目，学到了.user.ini的用法，除了.htaccess的解析，还可以用这个来让同目录下的php包含我们带木马的图片

# 2021年3月17日

- 晚自习看了一波sql注入的学习，还学了一点sqlmap的用法，还有更多用法有待探究
- 回来本来想整理java笔记的，又被src给诱惑了，跑去挖漏洞还是一无所获，但是找到了几个工具，还不错，虽然还不会用，但是至少了解了一些
- 学长准备带我打一波比赛了，起飞！
- java笔记明天再整理了
- 看了一下远海的博客，挖漏洞是真的牛，看到他进入了后台我都激动了。。。这玩意会上瘾。。感觉走对了路，是确实喜欢这些东西，不然也不能支持我天天晚上肝到一两点，兴趣和事业结合在一起让我觉得人生有点美妙了

# 2021年3月16日

- 下午自习室整理三个小时的笔记
- 回来准备复现一波V&NCTF，太难了，笛卡尔积注入，从来没有接触过，后面的路由问了学长说是开发的知识，以后慢慢学
- 写了一个cve的漏洞题，shopxo1.8，有默认密码直接登录admin.php，进去后再主题这里上传木马，但是要让木马被插入到已知的目录，就要下载一个主题，再插入到主题里面并运用，这个时候蚁剑就连接上了，本来以为直接就能拿到flag了，发现flag在root里面，我们没有权限，但是里面有一个py文件，可以进行读写文件的操作，就直接open("/root/flag","r").read()来读取，再write写出来就拿到了flag
- 写了八九杂项的题目，又用到了一波binwalk，发现stegsolved有更多的用法，例如LSB隐写的破解
- 压缩包爆破工具，发现一个png文件直接改后缀zip是不能直接爆破的，用了binwalk分离出zip才能爆破

# 2021年3月15日

- 比赛是没打了，继续java的学习

# 2021年3月14日

- 半夜肝起来了，把vishwaCTF给ak了！！！记录第一次ak
- 早上起来就接着打V&NCTF2021了，好难，写了一个web的签到题，js小游戏，改参数通关就行
- 晚上去了宏毅培训，学了一波template模板，学姐讲的比较快，我又没有学js，刚开始有点迷糊，后面差不多懂了意思，ajax这个东西没了解过，是用来前后端交接的东西，只能有机会再自学了
- 看到vishwaCTF又更新了两个web，马上跑去写，第一个看到了flask就知道是模板注入，怎么cat flag都没有，就用ls找了一波目录，还是没有flag的身影，后来在main.py里面找到了，可能阿三不喜欢直接给一个flag在目录里吧，第二题是一个逻辑判读，如果正确，那么就会usleep 1秒钟，解题的思路就是用python先集合所有字符，再拼接起来去访问，通过反应的时间来判断是否正确，但是由于外网的原因，访问时间很不准确，所以就跑下去了，思路应该是对的，虽然没拿到flag，但是还是很开心
- 准备睡觉了，还是觉得template的心得要趁热打铁写一波，就爬下床整理一波笔记，重新过了一遍，整个过程算是搞懂了，后面再学这些js和ajax之类的了

# 2021年3月13日

- 一天打了三场比赛，都是国外的，成绩还不错，vishwaCTF差一题ak，uctf干了三题web，nahamconctf比较难，只写了一题出来，再接再厉吧，希望能进线下比赛
- 学到了一个流量分析，用wireshark，就是费眼睛。。

# 2021年3月12日
- 一波java学习，整理了第二篇的笔记，做笔记真的挺麻烦的，但是怕记不住，还是写比较好
- php特性写了一点，用到了一次三元操作符，里面有个操作是这样的`$_GET?$_GET=&$_POST:'flag';`意思是只要get提交了东西就会被转成POST方式
- 明天三场外国的比赛，试着写写吧，如果网络不流畅就算了

# 2021年3月11日
- 中午注册了几场比赛，马上就可以打了，不过是国外的，不够流畅我就不打了
- 写了几个ctfhub的文件上传题，学了一波文件头的操作，之前就是照着套，现在知道前面的东西是怎么来的了，就是某个图片格式的开头标识，也没必要记，随便打开一个图片文件复制黏贴就好了
- 了解了一下00截断，ctfhub有一个00截断的题，上传shell.php的时候会被识别，所以再加一个后缀jpg来欺骗服务器，shell.php%00.jpg即可绕过，但是那题没有给出上传的路径，所以需要主动给他加个路径，抓到的包里面有一个get请求就是路径，但是只到了upload，我们就在后面再加上/shell.php%00就可以去蚁剑连接/upload/shell.php了

# 2021年3月10日
- java学习，下一阶段类和对象
- 笔记整理

# 2021年3月8-9日
- 白天上课，晚上两天在外面恰饭，晚上才开始学
- ctf刷题先停了，准备先把java搞一波
- java笔记整理第一期结束

# 2021年3月7日

- 中午请学长吃了个饭，大佬就要去腾讯实习了，实名羡慕
- 回来刷了一波buuctf，学到了一个.htaccess文件，这个文件叫分布式配置文件，用于文件上传的时候，过滤的很严，只能穿图片格式的时候，就可以再上传一个这个来把图片文件解析成php文件从而实现一句话木马的执行
- 写了一个sql注入的题目，和平常写的那种组合拳就能写出来的不一样，这题没有回显，只有true和flase来判断账号密码是否匹配，判断逻辑是：网站接收密码后，会先进行md5加密后再插入数据库，当输入密码进行登入的时候，就会把后来输入的密码md5加密后再匹配数据库的密码，所以用联合注入的时候，密码的位置就要自己md5加密一下再登入
- 后来写了几题xss，打破了对xss思想的局限，之前没想到过滤了字符也能xss，双引号可以用单引号来代替，浏览器会自己换成匹配的引号，当尖括号被过滤时其实也没必要闭合标签，可以使用onclick和onmouseover事件

# 2021年3月6日

- 继续写命令执行的题目，学到了一波新的操作，可以用`glob协议`进行目录扫描

- 遇到了一个uaf漏洞，问了一下说是一个堆的漏洞，有一个关于这个漏洞的脚本，就是利用了这个漏洞去返回对已破坏的变量的引用，很迷，以后有实力在来深究
- php的对象里有个魔法方法__toString()，它是在直接输出对象引用时自动调用的方法
- 开始文件包含刷题之旅，一开始就是php和data协议，后来是日志文件getshell，访问日志文件(/var/log/nginx/access.log)的时候看内容，一般会显示User-Agent的值，所以我们可以插入木马执行system命令到User-Agent里面，这样实现日志文件的getshell
- 学了一波PHP_SESSION_UPLOAD_PROGRESS加条件竞争的漏洞，具体原理就是我们可以设置一个session，id可以自己定，PHP_SESSION_UPLOAD_PROGRESS的内容可以插入一段木马，会生成一个临时文件sess_xxx，我们赶在临时文件被删除之前访问到就可以执行里面的system命令
- 用到了一波php协议的write，可以理解为当需要把信息写入某个文件的时候，使用这个协议进行加工，再写入进去，而read就是先加工再返回到客户端读取
- base64编码后，如果题目过滤了=，可以再加空格，可以把=给换掉
- 看了一下，刷题数今天超过100了，加上其他平台可能有150吧，继续加油

# 2021年3月5日

- antctf开赛，好家伙，贼难，0解。。。
- 下午上课只学了一点点的java，很失败啊，回来打ctf也没去整理笔记

- 刷命令执行的题刷到半夜，还是有几题没写出来，看wp都写不出，技术还需要沉淀

# 2021年3月4日

- 数据结构课在老师那里复习python，真的是没意思，掏手机看java的课程，一口气加速又快进，直接听了快有60节课，因为有一点c和python的基础，学这个快的一批，前期完全没阻碍
- 还是满课。。。晚自习回来才打开电脑，安装了一个idea，破解了一波，直接搞到2099年的使用期限
- 开始打ctf了，了解到/bin目录和/usr/bin的一些必备执行档，可以直接用命令调用，比如bin/base64 flag.php这样可以把文件已base64读取出来
- 写了两题无字母数字webshell的命令执行题目，这些大佬真的是对linux了解的超级透彻，第一个是用post包传一个shell上去，里面写了我们需要执行的代码命令到临时文件夹tmp里面，再用glob通配符[@[]]精准定位文件，让这个文件为我们所用，去执行一些命令
- 第二个无字母数字的是$(())这种操作，按位取反（~）的操作这些大佬也想的出来，用$(())来堆出一个数字，绕过正则，$(())这个操作[这里](https://blog.csdn.net/u013402321/article/details/80333272)写的也很详细
- 明天有时间把java笔记一起整理上去吧，尽量能把基础的对象的知识学完，早点开启javaweb

# 2021年3月3日

- 学校课程安排的太满。。。一直到下了晚自习才有自己的时间打打ctf
- 听了一点远海的src课程，干货挺多的，就是这些干货大多数我都自学到了。。。对我帮助还是不太大
- 第一次尝试到了xss，不过是self-xss，卵用都没有，而且不小心挖的是超星的。。。学长说不要用alert，要用console.log(1)这样文明一点

# 2021年3月2日

- 下午刷了一波命令执行，学到挺多小知识点的，`>/dev/null 2>&1`这个东西会让输出没有回显，绕过方法是分隔符，`|.*f.*l.*a.*g.*|`这种类型的过滤除了变量的拼接，还可以用?匹配`fl??`，然后学了一个grep指令，是用于在某一文件中查询带有特点字符的句子，并把整行输出，有时候cat和rac和nl这类的指令被ban了后可以使用这个来输出

- jdk8不能直接run burp，我的vscode又是只能用jdk11以上的，找了一下解决方法，安装更老版本的java拓展可以运行，但是打开的时候还是有报错，虽然不影响结果，就是不咋美观，不过也管他咯
- 今天晚上在肝高数的微分方程，唉，真的是烦躁高数啊

# 2021年3月1日

- 晚上写了比较多的命令执行的题目，写的这些说是命令执行漏洞，其实更偏向于文件包含的漏洞，这次就直接把php协议data协议都用上了，具体的常用命令都记下来了，data命令有个通配符绕过data://text/plain,\<?php system('cat fl*')?>可以绕过过滤了flag的题目
- 后来接触到了无参数RCE，一个很骚的操作，具体涉及到了很多的函数，收藏了一篇文章写的比较全
- 准备开始学java冲冲冲，争取快点解决掉基础，开始javaweb的学习

# 2021年2月27-28日

- 到学校了，感冒加坐车很累。。。
- 听了几节前端的课程
- 刷了一波攻防世界，涉及到了文件包含，就跑去复习了一下文件包含的笔记，把php的伪协议记了一下，主要涉及filter和input，data协议没怎么看，下次一定
- 刷到了之前写过的题目，随便注，涉及到堆叠注入和表名修改

- 之前看都看不懂的题目也写出来了，warmup，php的代码审计，审计到是不难，就是这个url二次编码的操作学到了一些东西，服务器获取你的get提交会把url解码一次，如果还有urldecode就可以二次编码

# 2021年2月26日

- 元宵节给自己放了一天的假，买的白帽子讲web安全到了，看了一点，感觉很强，慢慢看吧，很多知识点还是没听说过的



# 2021年2月25日

- tplmap一直还没搞好，所以决定今天要把它给解决掉，一开始总搞都说缺少什么ssl，我就直接重装了kali，发信kali自带的python就是2.7的版本，我就直接安装pip了，先安装的setuptool，再安装pip，一开始安装的9.0.1的版本还安装不上，我就下载了更老的8.0.1的版本，就安装成功了，后来去安装tplmap的必要模块，又出现了问题，一查说是由翻墙的原因不能访问，所以就加了一大串意思是转到国内源，tplmap算是可以运行了，就是这个国内源的这个不知道有没有一劳永逸的办法
- 下午刷了几题buuctf的题目，有写了两个文件上传的题目，发现php后缀还有一个绕过是phtml，而且上传文件时如果题目的上传目录有同名的文件会直接覆盖掉，所以不用担心重名的问题，写了一个sql注入，算是写的题里比较难的一题了，首先就过滤了很多关键的字符，绕过的方法就是双写，被过滤的字符在错误提示里会消失，第二点就是这题和那些简单题不一样，flag在的库不是题目的默认的库，需要查询一下所有的库名，换一个库查询才能拿到flag
- 了解了一下src漏洞提交平台，学长说漏洞先不急，先搞开发，我就重新捡起了之前没学完的html准备把剩下的给刷完，学长叫我去宏毅学一下，其实我觉得挺为难的，从来没去过，突然跑过去怪尴尬的，也不知道宏毅的学的咋样了，走一步看一步吧

# 2021年2月24日

- xss的学习开始，把网课听完了，了解了三张类型：存储型，反射型，dom型，写了相关的笔记
- 开始刷了一波ctfshow的xss题，一口气全部刷完了，收集了几条xss的常用代码，一个是获取cookie的一个是获取整个html代码的，如果是有那种登录框，可以把用户名设置成js的代码，跳转到自己的服务器里面，在服务器里面配置好脚本，到时候可以直接去服务器日志里读取相关信息，一般的xss跳转可以使用body标签，有个onload属性，意思是网页加载完成后去执行后面的js

# 2021年2月24日

- 感冒睡到中午才醒来，随便吃了一点就开始了php面向对象的学习，写好了笔记，基本结束PHP基础的学习
- 写了之前留下的buuctf的SSRF的题目，又写了一题命令执行，命令执行还挺难的
- 由于经常涉及到正则匹配，所以去菜鸟了解了一下，主要今天学了一个比较特殊的`.*f.*l.*a.*g.*`意思是匹配到有按照flag四个字母顺序的字符串

# 2021年2月22日

- 下了一波乡，回来就睡了一觉睡到晚上了
- 感冒了，很难受，写了三题ctfshow的命令执行

# 2021年2月21日

- 写出了剩下的题，就在我以为快ak的时候，又给我上了一题，裂开。。。
- 发现学着越来越需要linux的命令了，所以准备把遇到的指令都记下来
- 把web的九题写好了wp

# 2021年2月20日
- 刷题，写了一题模板注入，一题命令盲注，都不是太懂，前置知识差的太多了，打完这个比赛会开始基础开发学习，不然写的太吃力 

# 2021年2月19日 #
- 刷题，web写出了四题，对于这个结果其实不太满意
- md5加密前和加密后一样的是这个：0e215962017可以记下来

# 2021年2月18日 #
- 网站备案成功了，顺便拿到了学长自己开发的typecho主题，配置了一波，感觉很nice
- 那题抽卡题看了一下学长的wp，是git泄露加上反序列化，反序列化没学，但是git泄露了解过，之前写的题直接访问/.git/index.php就拿到了代码，但是这次就不一样了，试不出目录，后来就了解到有个脚本叫GitHack，可以爆破出git的目录并保存，但是在官方找到的需要python2才能运行，所以我就找到了一个别的博主自己改装的python3的脚本，文件是扫下来了，但是还写不出，慢慢来吧
- 开始了xss的学习，和sql有点像，挺有意思的，搭建了一个xss-libs靶场，写了一点最基础的反射型xss
- 明天有比赛打，中南大学寒假CTF新人赛，冲冲冲，不知道能写出多少哈哈哈，希望不零蛋就行

# 2021年2月17日 #
- 上午没咋学，陪我妈包饺子包了一上午，喉咙剧痛
- 下午整了一下杭电的题，有个题不小心碰进了一个已注册的号，直接拿了现成的flag，问了一下学长说是模板注入，还没学过，也不急，慢慢来
- 写了一下杭电的杂项的题目，学到一个新的东西就是已知明文攻击，这个东西就是在一个压缩包里套了一个子压缩包，都加了密，但是父与子之间有一个相同的文件(CR32值)，把这个相同的文件提取出来再通过储存的方式压缩一下，就可以拿去明文爆破了
- 晚上又开始了php的学习，冲冲冲

# 2021年2月16日 #
- 继续复现week2的题，发现我的burp有点问题，经常改了端口没反应，偶然发现是证书没配置好，之前的不知道是哪里搞的来的，没效果，所以重新绑定了一个证书，问题就解决了，很是舒服
- 通过burp写了一个sql注入的题目，复习了一下那些sql的语句，难度倒不大，就是有过滤的字符串，官方没给还真不好怎么整
- 写了一下week3的题目，写不出。。。发现自己的基础有些差，所以又捡起了php来学习，听了四十节课，觉得有必要的笔记也做好了，这种学着学着就慢慢理解之前留下的疑惑的感觉很nice，这可能就是融会贯通，很爽

# 2021年2月15日 #
- 复现杭电的week2的题目，改天会专门去了解一下xss再来干这类的题目
- 学习了一下ctf的一类典型的题目——条件竞争，原理就是多个线程同时向服务器发起请求，服务器反应不过来就会发生错误，有两类解法，一是使用burp开启多线程来进行，二是通过python的threading模块来写
- 尝试写了一下多线程的脚本后，开始了多线程threading库的学习，大概的了解了最基础的使用方法，有个小技巧就是可以通过for循环来开启很多的线程，准备写一个基础的多线程的博客给自己看的

# 2021年2月14日 #
- 复现了一下杭电week1的web题，写了一个python脚本，复习了一波爬虫和json库的dumps和loads这样的函数
- 学习了一下sympy库，这个是用来解数学的库，今天用它解了定积分的题目，wp也写在了博客里
- 想去弄懂http走私，太菜了看不懂。。。
- 想去弄懂week2的变量覆盖，发现php知识还是有所欠缺，一定要找个时间补一补
- 听完了涅普计划的文件上传和文件包含，并结合视频做好了详细的笔记，内容还是很多的，发现里面有我之前一直疑惑的PHP伪协议，也就是php的封装协议，解决了一些疑惑还是很舒服的

# 2021年2月13日 #
- 买了一个服务器，顺带搭建了一个typecho动态博客，访问速度贼快，把自己的hexo的静态博客也搭在自己的服务器里面了
- 装了一个linux的虚拟机，配合这个服务器的搭建，对于linux有个模糊的认识

# 2021年2月12日 #
- 解出了那道难题，成就感满满
- 文件上传的网课听了一波，准备把笔记补充完整