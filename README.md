# bilibili_kaios

bilibili for kaios

如需使用请下载 release 版本，master 分支可能存在实验性特性！

|    文件夹    |    用途    |
| :-: | :--: |
|    allive    |  直播分区  |
|  attention   |  关注的人  |
|  bandetail   |  番剧详细  |
|    bangmi    |  番剧首页  |
|  collection  |   收藏夹   |
| contribution |  用户投稿  |
|   dydetail   |  动态详细  |
|   dynamic    |    动态    |
|     live     | 直播间页面 |
|    lives     |  直播列表  |
|    music     |  音乐首页  |
|    player    |  播放页面  |
|     user     |  用户页面  |
|     web      |  网站页面  |
|     lib      |   引用库   |

## TODO List

- [ ] FLV 播放支持（最高 720P、但实测在线播放最高 480P，否则容易崩溃）

## Update

<details>
<summary>更新日志</summary>

### 1.0
版本：1.0
更新时间：2020-10-3
更新简介：
因为电脑文件丢失，不得不重写软件。更改了配色（从粉色变为蓝色）和原来丑不拉几的UI，增加了可用左右键操作的顶栏。提升了代码的可维护性。
主要功能如下：
1.获取B站电脑端首页视频
2.播放视频和观看弹幕（透明度不可调，弹幕无法关闭）
更新内容：
1.修改了UI
2.由使用<div>存储临时数据改为了用列表存储（我都不知道我是怎么想到用自定义标签的阴间方法的……）
3.提升了网络体验（更换服务器）


### 1.1
版本：1.1
更新时间：2020-10-31
更新简介：
为了让大家快点用上新版本，再加上马上期中考，更新有些仓促，新增的功能比较少。
本次更新添加了“关注”功能，完整的直播观看系统在做了
更新内容： 1.找回了关注功能，能在本地直接使用 UID 添加喜欢的 UP 主（不能和 B 站账号同步！） 2.在“直播”选项卡按“观看”键可以试试正在制作的看直播功能（用来测试的是“KPL 官方赛事直播间”），目前看直播功能如下： 1.如果 UP 主有在直播，可以正常低画质观看直播流（高画质 8110 带不动） 2.全屏观看直播


### 1.2
版本：1.2
更新时间：2021-1-30
更新简介：
这次更新间隔有点长，因为我有严重拖延症（沉迷 Arcara）。这次更新改进了一些细节，填了一些坑。
视频暂停神马的还暂时做不到（能获取到视频的文件位置，但叔叔做了跨域限制，只有 B 站自己的网址能正常访问。转发视频流神马的小带宽吃不消 Σ:3，以后试一下伪装包名）
有反馈说弹幕太多了看不到视频，含泪把弹幕关闭了
更新内容：
1.“首页推荐”选项卡更名“热门” 2.修复了无法正常退出程序的 bug 3.视频播放页面可以查看视频详情了 4.软件启动会自动检查更新，下一次更新可以直接在手机安装了（前提是安装了 Omni SD） 5.在非全屏页面下能看到状态栏了 6.可以观看已关注的 UP 主的直播流（暂时不提供 UP 主是否正在直播的查询）（反正出错你就退出来 Σ;3） 7.关闭了弹幕功能 8.视频播放窗口的音量调节按钮改到了右软键（直播页面仍然是 2 键）


### 1.3
版本：1.3
更新时间：2021-3-14
更新简介：
【应急更新】云服务器到期了，学生机续费次数用完了（哭）。马上之前的版本用不了了，现在用的是我自己搭建的服务器，使用体验会非常差，希望大家可以理解。
这期间应用响应时间多半在 10 秒以上，希望大家能等一下……
可能会有家里人拔电源线的情况，希望大家能够理解……
更新内容： 1.更换了服务器


### 1.4
版本：1.4
更新时间：等亿下
更新简介：



更新内容： 1.能显示关注的 UP 主的完整的视频列表 2.增加了搜索视频的功能 3.能播放分 P 视频的其它分集 4.能手动输入直播间号观看直播视频
1.4 更新补充：
更改接口请求方式，直接请求 b 站官方接口，不再由服务器中转！


### 1.5
版本：1.5
更新人：zixing
更新内容： 1.修改快捷键，播放界面 2 键提高音量，8 键降低音量。 2.可以删除添加或清空关注的主播和直播内容 3.直播更改为通过直播间 id 或者直播的用户进行添加,可以删除添加的直播间 4.注意：本版本更新更改了关注和直播的数据结构，会自动转化旧版的数据！ 5.修复视频评论内容，支持下一页操作 6.修改获取图片时的默认分辨率，使网络加载图片更加顺畅 7.主页视频支持切换三天热点或者七天热点 8.搜索支持下一页操作 9.查看 UP 主视频支持下一页操作


### 1.6
版本：1.6
更新人：zixing
更新内容： 1.现在直播可以加载出直播间信息并且可以查看直播弹幕了(需要手动刷新) 2.切换菜单时记住当前选中的项目。 3.视频可以暂停了（解析了视频直链，不再使用 B 站播放器）


### 1.8
版本 1.8
更新人：michael_eddy 1.现在你可以登录了。 2.登录后的一些操作：关注列表、评论、收藏夹、投稿。 3.支持看直播和发弹幕。 4.支持通过按钮“4”、“6”进行视频“快退”、“快进”。 5.支持番剧、国创、直播列表/分区。 6.番剧可以用 480P 看了，虽然支持 720P 但是实测很容易崩溃


### 1.8.1
版本 1.8.1
更新人：michael_eddy 1.添加视频弹幕，可以在分区-设置中开启或者关闭


### 1.8.2
版本 1.8.2
更新人：michael_eddy 1.添加直播弹幕，可以在分区-设置中开启或者关闭（视频弹幕关闭则直播弹幕也会关闭，但列表中弹幕仍会更新）

### 1.8.3
版本 1.8.3
更新人：michael_eddy 1.修改主界面去掉旧无用代码提高效率 2.增加播放器失败重新播放功能

### 1.8.5
版本 1.8.5
更新时间：2022-9-3
更新人：白羊座的一只狼（TonyLang）
更新内容：紧急修复了视频搜索功能的API调用错误。该错误由B站服务端升级引起。
  </details>
