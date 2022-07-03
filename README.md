
# YGOAssistant
一个基于[mirai](https://github.com/mamoe/mirai)QQ机器人框架的游戏王插件

本项目旨在方便游戏王玩家(主要是萌卡的竞技玩家)

如果有bug和想要的新功能还请在issue里发布，因为代码写的跟屎一样。

所以有任何代码相关的建议也可以直接说

或者也可以直接加我QQ群和我说：[631487094](https://jq.qq.com/?_wv=1027&k=5yQoHBE0)









## 目前功能

- **查游戏王卡片信息**       
    > _卡片数据来自[百鸽](https://ygocdb.com/)_
    
    - 查卡片详细数据
    
    - 查看卡片md或者ocg的收录情况

    - 查看卡片日文的Q&A和调整
- **查看[萌卡](https://mycard.moe/)玩家信息**

    - 查看特定玩家的排名,胜率等数据
    - 查看特定玩家的对战记录   
        > *只显示最近三十条记录*
- **查看[萌卡](https://mycard.moe/)当前的对战房间信息**
    - 获得当前在进行对战的竞技匹配房间数据
        > *按玩家排名排序*
    - 在群里订阅特定玩家
        > *在这个群里获得房间列表时会优先显示群订阅玩家*
    - 单独订阅特定玩家
        > *个人订阅的玩家会在他开始对局时私聊推送给你*
## 教程/使用方法
安装方法和一般的mirai插件一样

直接把`.jar`放到安装目录的`plugins/`文件夹下就行了

> 得先运行一次这个插件来生成`配置文件`

> 然后关闭机器人打开安装目录下的`config/`文件夹的`配置文件`来手动设置机器人管理员QQ号

卡图则是存在安装目录下的`data\YGOAssistant\CardImageCache`文件夹下，可以自己添加或者修改喜欢的卡图

**指令:**

| 查卡相关指令                                              | 描述                                    |
|-------------------------------------------------|---------------------------------------|
| `卡查 关键字`                            | 开始查询并且返回一个带编号的结果列表<br />如果只有一个结果则直接返回那张卡的数据|
| `数字`                                   | 获得卡片列表后，查询列表里那个编号的卡                     |
| `md收录`                                  | 进入特定单卡后，查询那张卡的md收录情况|
| `ocg收录`                                  | 进入特定单卡后，查询那张卡的ocg收录情况|
| `日文调整`                                  | 进入特定单卡后，查询那张卡的数据库日文调整|
| `日文faq`                                  | 进入特定单卡后，查询那张卡的数据库日文F&Q|
| `释放卡查内存`                              |**插件管理员指令** 清空当前所有人的卡查记录|

| MC玩家相关指令                                   | 描述                                    |
|-------------------------------------------------|---------------------------------------|
| `查分\查成分 玩家名`                            | 查询这个玩家的胜率和排名等数据|
| `查历史\查记录 玩家名`                          | 查询这个玩家的对战记录 |

| MC观战相关指令                                   | 描述                                    |
|-------------------------------------------------|---------------------------------------|
| `Link Start!`                                   | **插件管理员指令** 开始尝试连接到MC观战服务器|
| `关闭连接`                                       | **插件管理员指令** 断开与MC观战服务器的连接|
| `连接状态`                                       | 查看当前与MC观战服务器的连接情况          |
| `添加群订阅 玩家名`                               | 添加当前玩家到群订阅 *-只能在群里用*      |
| `删除群订阅 玩家名`                               | 删除当前群订阅里的这个玩家 *-只能在群里用* |
| `显示群订阅`                                     | 显示当前群里的所有订阅玩家 *-只能在群里用* |
| `添加个人订阅 玩家名`                               | 添加当前玩家到你的个人订阅                   |
| `添加个人订阅 玩家名`                               | 删除你个人订阅里的这个玩家              |
| `显示个人订阅`                                     | 显示你的所有订阅玩家              |


## 使用例

```
卡查 流天类星龙

查分 林蒙のゲーム

添加群订阅 林蒙のゲーム
```
