# 喜马拉雅极速版  



喜马拉雅**极速版**自动化脚本    
请仔细阅读本说明     
 
 [xmly_speed](xmly_speed.py) 
 cron   */30 * * * *   (30分钟运行一次,不要修改)

### 支持功能
~~1.幸运转盘4次~~  收益过低,且容易报错,故去除  
2.答题(完整)  
3.听书集卡获得抽卡机会、领取万能卡  
4.首页、宝箱奖励及翻倍(完整)  
5.自动刷收听时长(可选项)   
6.每日签到，除了第30天 
7.每日通知 



### 邀请任务
[注册链接直达](https://m.ximalaya.com/xmds-node-spa/apps/speed-growth-activities/web-earn/landing?parentUserId=58434192&channel=1&srcChannel=weixin&srcPicUrl=https://fdfs.xmcdn.com/group63/M06/26/3C/wKgMcl0Z7-bgXtm3AAAP_-xdbjM707.png&srcText=1) (手机号注册)  
如果你的手机以及手机号之前没有注册过喜马拉雅的话，可以帮我完成一个邀请任务，感谢。

### 账号注册以及风控
1、使用**不同的手机设备**进行注册、刚注册的账号**不要退出**和切换账号，以免账号被封禁  
2、刚注册的账号**不要立刻跑脚本**，以免账号被封禁，无法提现  
3、同一手机最好不要切换账号，以免cookie过期 (待测) 



### Note
- **前三天的新手任务接口没有抓到，需要手动完成**  
- **有些游戏 第一次需要手动运行**
- ~~旧脚本会刷收听时长，因此而黑号的，本人概不负责，请知悉（最新代码已经移除）~~ 最新版本修订为可选项
- 似乎并没有出现黑号情况，故默认打开  
- 不要询问 **可以通过简单搜索就可以知道答案** 的问题



### 赞赏码(开发不易,请作者喝杯奶茶)

<p align="center">
  <img src="thanks.jpg" alt="抓包" width='50%' height='50%'/>

### 运行方案

1、GitHub action自动运行，账号信息读取自`Repo-Setting-Secrets`  

- cookie 信息抓包自**手机app(喜马拉雅极速版)**，域名为 `m.ximalaya.com`的可以
- fork 本项目
- Secrets 新增 `XMLY_SPEED_COOKIE`，填入cookie信息 ，多账号换行
- star一下，立即执行，观察运行情况
-  **必须**  修改一次文件（比如自己库中的README.md文件）才能定时运行   (！！！！不要再问为什么不能自动运行;不懂不要修改cron )  
- 需要刷时长的，Secrets 新增 `XMLY_ACCUMULATE_TIME`，填入`zero_s1`；可能会黑号，请知悉
- 需要bark通知服务的(自行搜索)，Secrets 新增 `BARK`；

2、下载到本地运行   
   需要第三方库`requests`  

### 如何抓包cookie
- [手机抓包工具汇总](https://blog.zengrong.net/post/capture-package-on-phone/)
- [Stream -- iPhone上抓包神器](https://blog.csdn.net/heqiang2015/article/details/84023327)

<p align="center">
  <img src="抓包.png" alt="抓包" width='40%' height='40%'/> 

框中信息，不包含开头的`Cookie: `

### 查看action运行情况

点击 Actions -Workflows

### 历史star数  
[![Stargazers over time](https://starchart.cc/Zero-S1/xmly_speed.svg)](https://starchart.cc/Zero-S1/xmly_speed) 