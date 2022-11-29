塔防精灵自动对战脚本
============
备注：
---------
加微信，联系方式在最下面。 

正文：
--------------------
    本程序实现塔防精灵(微信小程序中的游戏)， (在电脑上)自动化对战，挂机刷奖杯.本程序我自己每天也在用，赛季固定1万+奖杯。
    上卡逻辑经过我几个月的细腻优化，强处就是逻辑强灵活多变应付复杂战场环境。
    不像某些自称也是挂机脚本的,看他那界面绿了吧唧的，表面做的很花哨，貌似“功能齐全”，实际无一精通，上卡逻辑不行，就是用某傻逼精灵撺掇出来的。
    本程序每一个代码都是本人亲敲，掌握全部技术细节，界面友好只有一个按钮
    而且很便宜

实际演示：
----------
[![Watch the video](https://i2.hdslb.com/bfs/archive/303a4497cf6b431703f5ff5498ceb5f85a0ad042.jpg@320w_200h)](https://www.bilibili.com/video/BV1zg411p7C3/?vd_source=42cda5a0c779ca6427c28a9c9ebe5c78)


下载链接：
-------------------
    https://github.com/finitebull/-/releases
    或者傻逼百度网盘下载：https://pan.baidu.com/s/131tydqO7H5o-kiWcPO19vQ?pwd=1111   提取码: 1111 
    或者试试这个   ：  https://cia.wang/s/Mg3fO
    
为什么需要挂机脚本：
-------------------
    1.首先因为懒，不想为了每个赛季的奖励每天起早贪黑的刷，爷还有别的事要干，但是游戏里的每个奖励都要拿到
    2.即使你不懒，你也需要一个挂机程序，重复的逻辑已经写在程序里了，不需要每一局游戏集中注意力的想我接下来要出什么英雄
    3.如果你是个勤奋的人，反应速度又是那么的快，那你能有我的程序快么？虽然有人反应能很快， 但是没有人能一直快，尤其在两三个小时下来之后。
    4.拜托，坐下来喝杯茶，一边欣赏着游戏自己玩自己，别被游戏玩了，透支了生命，以后老了还得住院，你是不知道医院多贵，医院上来就是10万级别的

实现方法和原理：
---------
    电脑上利用“腾讯手游助手”这个傻逼软件或者 “微信电脑版”，（建议使用“微信电脑版”），结合我的脚本，自动点击该点击的位置
    因为是模拟点击，不对游戏原程序进行修改和各种方式的hook ， 所以不属于外挂， 不需要担心被封号
    我的卡组的话长期胜率50% ， 但是因为胜利一局给30多分， 输掉一局扣不超过20 分， 所以挂机是有收益的。更别提看广告输了不扣分的

目前已经支持了的功能有：
---------------------
    1.英雄按给定的权重上场
    2.英雄上场秒点，抢占先机
    3.小鹿自动卖
    4.奖励箱子秒点
    5.对手上场的英雄光环识别， 并调整策略
    6.游戏结束后广告自动观看，并开始下一局

关于价格：初步定为
------------------
    65元RMB 享受终生     （2023年即将恢复到原价95元RMB）
    0.01元RMB 或者不给钱也行，免费试用2天


另外参考一下这是游戏里卖英雄的价格
![image](https://user-images.githubusercontent.com/94673579/198992881-fc06928b-0412-40ee-8d1e-ff8d2331b4a5.png)

需要准备和满足的条件：
---------------
    windows 10 及以上 64位 系统的电脑 （以后会增加32位电脑的支持， 目前就是这样）
    “腾讯手游助手”这个傻逼软件或者 “微信电脑版”这个傻逼软件
初次打开的界面如下：
------------
![image](https://user-images.githubusercontent.com/94673579/203703277-de0b8182-4a74-416b-93f9-ec3a5d022981.png)

激活成功界面如下：
-------------------
![image](https://user-images.githubusercontent.com/94673579/204074615-97f51151-6609-42f1-b2e2-5917c799cc49.png)


挂机使用的卡组：
------------------------
![image](https://user-images.githubusercontent.com/94673579/203709095-b61df149-6543-4608-b863-edf92a851a7a.png)
这是一款低保卡组，回想一下炉石的挂机脚本用的是什么？不也是些操作简单的卡组么
如果需要自定义并使用其他的高级卡组，加钱啊，没有什么是加钱解决不了的
![image](https://user-images.githubusercontent.com/94673579/203710844-2a944b9a-ac9b-497e-92fa-bd4519ffe803.png)
每个赛季保证都能上10000以上，获得免费金卡一张，

卡组上场权重逻辑:  (逻辑是写死在程序里的，虽然不建议换挂机卡组，但是想换卡组的参考我的逻辑自己替换截图也是可行的，自定义更高级的卡组逻辑欢迎打赏)
------------------------
    上场顺序是
    gugong的权重是 20 ， shenv的权重是 15 ， binggong的权重是 9 ， songshu的权重是 10 ， xiaolu的权重是 8 ， lvgong的权重是 7 ， haiyao的权重是 5 ， huoqiang的权重是 4 ， dashu的权重是 2 ， dijing的权重是 1
    另外
    如果 binggong 在场上则  songshu 的权重变成 6
    如果 songshu 在场上则 binggong的权重变成 6 ， dijing的权重变成 0
    如果 haiyao 在场上 dashu的权重变成 0
    如果 dashu 在场上 haiyao的权重变成 0
    如果 对面三法被动
     haiyao的权重变成 5 ， dashu的权重变成 0
    如果 对面三弓被动
     haiyao的权重变成 0 ， dashuy的权重变成 5
    另外小鹿会被卖
    场上有的先上，然后数大的先上，然后根据逻辑。
如果想换阵容
------------------------
    代码你改不了，你能改的只有截图，比如我这套卡组c位是骨弓和蛇女，你把这两个的截图替换成你的英雄，文件名字不变，以此类推，这样就实现了简单的换阵容，汉语拼音 binggong 就是冰弓，以此类推。因为逻辑是写死的，所以在一定程度上可以换卡组，但是如果想要更高级的卡组逻辑需要 我给你定制代码才行 ，然后我得吃饭吧，你懂的，拿起手机打赏吧。
    另外英雄的截图是游戏界面下面那个，扩建和刷新中间那些个。
    另外每个英雄有两张截图，带下划线的是动画播放完稳定的时候的，没下划线单透明感觉的是刷新后0.2秒后的，用来快速出牌的。目前你自己截图就没法使用快速出牌功能了，两个截图成一样的就行

游戏机制分析：
-------------
    你想赢？你想赢就得有人输。这些玩家在游戏开发商眼中都是一样的，凭什么就让你赢让别人输？可能那位说我充钱了，那还有比你充的多的呢；那位说我技术好，那还有比你手速快的呢；那位说我运气好， 我说兄弟别骗自己了。所以说做好长期胜率50%的心理准备吧，如果你是个新手，系统会给你匹配机器人让你的胜率80%，渐渐的系统会减少机器人的比率，慢慢降低你的胜率鼓励你充钱，充钱就给你提高胜率，过两天你给他的钱他花完了就降低你的胜率让你再充。所以充钱不是让你赢的必要条件，一直冲钱才是。如果想白嫖各种金卡就能够要承受住每天2个小时胜率不过50%的心理压力，所以白嫖的人往往弃游，这也是游戏开发商想要看到的，开发商不想把白白的服务器资源浪费在白嫖玩家的身上，人人都充钱对他来讲才好呢。可是现在不一样了，我有挂机脚本了，每天就是点两下鼠标，游戏自己玩自己我根本不看，到时候拿奖励就好了，输了总会赢回来，也不会有心理压力。
    每天挂到输保护的十个广告看完就行了，因为每天不管挂多长时间你都不可能杯数超过氪金大佬，而氪金大佬的杯数增长每天是固定的
![image](https://user-images.githubusercontent.com/94673579/203771805-f89accf7-680a-4188-abfd-b50415c43316.png)
    
    定义1：氪金大佬，氪金大佬是那些充了很多钱，不会输，胜率100%的人
    定义2：氪金大佬理想曲线。是指每个赛季15天，氪金大佬的奖杯数随着时间天数的变化曲线
    所以说氪金大佬理想曲线是一个什么样的曲线呢？anyone？ anyone？
    没有错，氪金大佬理想曲线是关于时间的一次函数。这是因为，氪金大佬的杯数增长只与氪金大佬每天的游戏局数有关， 与对手无关，而一个人每天的平均游戏局数可以看成是常数，也就是氪金大佬的杯数增长率是常数，所以是关于时间的一次函数
    至于大部分的其他人，你的曲线是贴在氪金大佬理想曲线下方时而接近时而远离的弧线，
    看图，这就带来一个问题，就是可能有一半的时间，你打了一天游戏杯数也没增长，可能反而下降了；另外一半的时间，可能就是下一天，好像李刚附体，杯数增长比氪了金的人还要快
    但是很快奥，又回到打了一天游戏杯数也没增长的状态了
    这会导致大量“勤奋”自己打的玩家弃游，该得的奖励他没得到
    所以说别被游戏给玩了，你需要一个挂机脚本
    
    
联系方式：（都写得明明白白的了你不看，那些加微信就知道问问题的，以后一条问题一块钱，发红包，问题写在红包里， 不然老子没那闲工夫一条一条回你）
--------------
   
    作者微信号：  old_favorite
     
    作者的邮箱 (基本不看)： aa15478aa@163.com
    
