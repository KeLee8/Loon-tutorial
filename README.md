# 前言
嘿 我是MengRain

本篇是Loon的教学旨在方便大家上手（有帮助的话点个关注吧）

我的TG频道：[点击一键关注](https://t.me/mengyulianmian)

我的TG交流群：[点击一键加入](https://t.me/mengdelaochao)


首先强调本教程是完全免费且公开的，请看完免责声明后进行学习，感谢采用本教学

# 免责声明 
MengRain 本仓库中涉及的任何解锁和解密分析脚本仅用于资源共享和学习研究，不能保证其合法性，准确性，完整性和有效性，请根据情况自行判断。

间接使用脚本的任何用户，包括但不限于建立VPS或在某些行为违反国家/地区法律或相关法规的情况下进行传播, MengRain 对于由此引起的任何隐私泄漏或其他后果概不负责。

请勿将本仓库内的任何内容用于商业或非法目的，否则后果自负。

如果任何单位或个人认为该项目的脚本可能涉嫌侵犯其权利，则应及时通知并提供身份证明，所有权证明，我将在收到认证文件后删除相关脚本。

MengRain 对任何本仓库中包含的脚本在使用中可能出现的问题概不负责，包括但不限于由任何脚本错误导致的任何损失或损害．

您必须在下载后的24小时内从计算机或手机中完全删除以上内容。

任何以任何方式查看此项目的人或直接或间接使用该项目的任何脚本的使用者都应仔细阅读此声明。MengRain 保留随时更改或补充此免责声明的权利。一旦使用并复制了任何本仓库相关脚本或其他内容，则视为您已接受此免责声明。

# 教学开始前的吟唱
本片教学使用的是Loon TF版本【3.0.0(485)】以后更新新的版本我也会对本教学继续更新

Loon俗称热气球，气球，小气球 是一款网路代理软件，但是上手最近更新了商店版的3.0新玩家骤然增加 所以应群友要求我编写了本教程

PS.本配置写于2022.11.21

# 注意
本教程基于 [MengRain的配置](https://github.com/MengYuLianMian/Loon-configuration-file-MengRain) 展开


# 一 代理的导入

QR：

Q：什么是代理？

R：通俗来说就是你在机场购买的订阅链接

Q:订阅链接是什么？

R:就是一堆节点

Q:节点是什么？

R:一个节点代表一个代理服务器，代理服务器可以实现流量的中转。

PS.则订阅节点  是许多节点的集合，是一个配置在远端的节点集合，Loon通过url下载下来后解析成一个节点列表。

使用：打开软件于 [仪表]——[所有节点]——[右上角+]——[添加节点]


# A 订阅导入

第一步：点击所有节点

PS.若没有请点击右上角的编辑按钮 将不可见的图标拖出来

![image](https://user-images.githubusercontent.com/89105781/203020981-5e59b9b5-6994-4aa2-b11f-d368d63e788f.png)

第二步：点击右上角的加号【+】打开这个界面 并按照图片填写

PS 1.若无法成功导入请打开资源解析器（最底下那个）我的配置中已经写好了资源解析器（下面会教导入配置文件）

PS 2.UDP，Fast Open，Vmess Aead按需打开

PS 3.若机场为提供Loon一键导入，请复制 原 订阅链接至Loon（若依旧无法使用请打开资源解析器并更新节点的订阅）

![image](https://user-images.githubusercontent.com/89105781/202912573-2240dca9-1360-45c4-aea0-23ac1f546b20.png)

第三步：选择右上角的勾保存

此时回到所有节点界面即可看到你的订阅 点击可查看所有节点

# B 本地导入

第一步：重复A的过程至第二部点击 + 后于最顶部选择[本地节点]填写一个你喜欢的别名

第二步：选择二维码扫描QR码导入 或 点击协议使用其中一个协议使用

PS.如：Shadowsocks是对小火箭的兼容则小火箭能用的使用这个格式在Loon就可以使用 具体说明表格如下

![image](https://user-images.githubusercontent.com/89105781/202913190-72b852ed-0f29-4d03-bf42-aad4dfc15e15.png)

第三步：保存

此时回到所有节点界面即可看到你的订阅 点击可查看所有节点

# 二 筛选节点的使用

QR：

Q:是什么筛选节点？

R:通俗来说就是让香港的节点都集中到一起去（归类）

我的配置已经写了 但是教学一下

选择右上角[+]——[加一个名字]——[筛选类型]

具体说明如下：

![image](https://user-images.githubusercontent.com/89105781/202915346-58dcfca4-8127-43ad-af98-fa9ed231976d.png)

一般都是用NameRegex  

格式：Loon正则筛选节点：

^.*(A|B)  =  A或者B

(A.*B|B.*A)  =  有A有B

^(?!.*A)    =   不含A 

^(?!.*?B).*A  =  有A但不含B  


# 三 怎么引用他人配置文件

使用：点击最下方的[配置]——[从URL下载]——[URL]

第一步：点击配置 下滑至从URL下载 点开

![image](https://user-images.githubusercontent.com/89105781/202913458-b5eff2ff-93f9-4b13-b123-fdf934d34ae0.png)

第二步：将 [MengRain的配置](https://github.com/MengYuLianMian/Loon-configuration-file-MengRain/raw/main/Loon%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6) 粘贴至其中

PS.上方链接是全配置文件 如需简洁版请看后方 [Loom配置文件MengRain](https://github.com/MengYuLianMian/Loon-configuration-file-MengRain)

点击Loom配置文件MengRain后可选择一下版本

![image](https://user-images.githubusercontent.com/89105781/202913718-2dba8f56-8fa9-4fb4-b5ae-580ebf852972.png)

# 注意！！！引用后需要重复第一步导入订阅！！！
你也可以不用我的配置自己手搓（就是麻烦些）

# 四 分流规则的使用

QR：

Q:什么是分流规则？

R:即让指定的链接走给他规定的线路如：谷歌走香港，bilibili走中国（直连），TG走最快的代理

老样子于最下方选择[配置]——[规则大栏]

# A本地规则

此处不建议调整（麻烦）如果执意使用参考下图：

![image](https://user-images.githubusercontent.com/89105781/183360274-f295a0e2-e650-40f8-b07a-58cfeaa82390.png)

# B订阅规则

我们通常会使用这个进行分流（毕竟前人栽树了） 分流规则请访问：@blackmatrix7 [链接](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule)

我的配置已经分的很齐全了 但是依旧教学一下

[打开订阅规则]——[选择+]——[填入名字及订阅]

此处拿百度举例

![image](https://user-images.githubusercontent.com/89105781/202914772-ce52a778-0bc8-45c1-946f-c323676e9d58.png)

于别名处填入一个明白的名字（别最后忘了是什么的分流） 在URL出写入分流的订阅（如上方blackmatrix7的GH）

PS.打不开就打开解析器

# C补充：策略的使用

QR：

Q:策略是什么？

R:一个策略组分为两部部分：策略类型，子策略。策略组会根据策略类型选出流量最终使用的节点

Loon目前支持三种策略：

select 根据用户UI选择使用哪个节点

url-test 默认每隔600s向配置的url发出http请求，选择最快返回数据的节点（注：url-test不支持策略组为其子策略）

ssid，根据配置的ssid名字，在wifi切换时自动切换节点，也可以配置默认节点和在蜂窝数据下使用的节点

一个策略组可以包含任何单个节点，订阅节点，策略组（url-test不除外），内置策略（DIRECT，REJECT）

则选一个想要的即可（还是那句话 还不如用我的配置....）

如需手动看下面

点击最底下的[策略]再点击[+]

![image](https://user-images.githubusercontent.com/89105781/202916350-75bcd20e-c365-4828-aab3-65729a424106.png)

这个页面很详细就不说什么了

![image](https://user-images.githubusercontent.com/89105781/202916465-ed2423ad-64d0-48b5-970d-1e7944ddf160.png)

PS.一般用URLT不用均衡负载 （有时候开均衡会看不了Netflix，但是给TG开均衡效果会很不错）

# 五 模块(插件)的使用

QR：

Q:什么是模块？

R:模块能作的事情很多例如解锁大陆iPhone被锁的功能，比如去广告，比如给YouTube添加机翻字幕等等

因为Loon有社区制作的非官发模块仓库，使用找起来很简单（我的配置自带了这个模块）

1.复制这条链接 https://raw.githubusercontent.com/Peng-YM/Loon-Gallery/master/loon-gallery.plugin

2.添加到配置→插件中，同时，你还需要保证MitM、脚本、复写三个功能处于开启状态。

3.插件仓库的打开方法可以参考下图。

![image](https://user-images.githubusercontent.com/89105781/202915778-402172a2-74c5-4678-b1b7-e3773d29d0e5.png)

如何手动添加呢？[仪表]——[插件]——[右上角+]——[填写]

将模块的地址粘入URL即可（名字无所谓）

![image](https://user-images.githubusercontent.com/89105781/202915917-a1c1b017-afb8-4f9d-945c-4578f6866834.png)

# PS.使用模块必须打开{脚本}{复写}并配置{MitM}

# 六 MitM的使用
MitM （Man in the Middle Attack）
中间人攻击方式解密https的请求。Loon会根据配置的hostname和信任的CA证书解密相应的https请求和响应，解密后可以配合Rule和URL Rewrite进行分流。

点击[最下方配置]打开[证书管理]安装[证书]

![image](https://user-images.githubusercontent.com/89105781/202916184-73e551dc-8e97-4e93-aba6-16a7dca56de9.png)

证书绝对安全的 不用担心会有脏东西（在Safari打开！！！

# 七 如何使用网路共享

QR：

Q:什么是网路共享？

R:就是通过热点让别的设备被代理

于主页打开[网路共享] （表现为一个绿点） 点击[网路共享]将Http地址粘贴至其他设备的WiFi链接高级设置即可

# 八 更多工具的补充

见最上方的代码列表，若使用移动端观看本教程需要手动点击view code展开（会根据需求慢慢增加内容）



# 结语
好了以上就是全部教学内容 如有错误请TG找我指正

我的TG频道：[点击一键关注](https://t.me/mengyulianmian)

我的TG交流群：[点击一键加入](https://t.me/mengdelaochao)

我的Twitter：[点击一键关注](https://mobile.twitter.com/mengyulianmian)
