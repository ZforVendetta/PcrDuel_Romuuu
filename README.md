# PcrDuel
2022/06/14：
	1.发送 ban(用户qq)，可以禁用用户大部分贵族决斗指令，并清空女友。
	2.发送 unban(用户qq)，可以解封用户，女友并不归还。
	3.给群主赋予了【为(用户qq)充值xx金币】指令权限。
	




创建贵族进行俄罗斯转盘决斗，提升贵族等级，争夺pcr女友的小游戏。
## 安装
把项目文件放在名称为pcr_duel文件夹里, 直接丢到hoshinobot的priconne里应该就可以了。
注意：需要保证hoshinobot的角色头像齐全，否则每次查询贵族都要下载会很卡，可以自行删掉chara里的1星和6星下载增快速度。
## 指令表
1.  发送 创建贵族 可以在本群创建自己的贵族，会被随机分配一个PCR女友。
2.  发送 查询贵族 可以查询自己的贵族状态。
3.  发送 贵族约会/招募女友 可以花费300金币招募一个女友，女友数不能超过爵位上限。
4.  发送 升级贵族/升级爵位 可以花费金币提升自己的爵位,提升爵位时女友数需已达到上限。
5.  发送 贵族决斗+艾特 可以向另一个贵族发起决斗，两个人必须都是贵族且已拥有女友，输者会随机被抢走一个女友。
6.  发送 领金币 可以在金币归零时领取50金币。
7.  发送 查金币 可以查询自己现在的金币数。
8.  发送 贵族签到 可以每天一次的领取100金币。
9.  发送 为(用户qq)充值xx金币，可以为该用户充值金币。例如 为123456充值100金币(该功能仅限机器人管理员，可以自己修改权限)
10. 发送 重置决斗 可以解锁决斗开关。(限管理员以上，这个仅用于决斗卡死无法再开的时候)
11. 发送 查女友+PCR角色名 可以查询某位pcr角色的归属。	
12. 发送 分手+PCR角色名 可以和角色分手(需要支付分手费)。
13. 发送 贵族帮助 可以查看游戏说明书。
14. 发送 声望系统帮助 可以查看声望系统说明书。
15. 发送 dlc帮助 可以查看dlc系统功能
16. 发送 本群贵族 可以查看本群贵族统计，剩余女友，及加载dlc的状况
17. 发送 查名字+女友序号(自己的第几位女友)，可以查看这个女友的名字。




## 注意
1. 目前为了方便，通过决斗获得女友是可以超过爵位上限的，这个可以自己修改。
2. 游戏可能存在bug，python新手多包涵。
3. 领金币和查金币指令，与赛跑是一样的，二者的金币也是互通的，如果两个都安可以注释掉一个。
4. 贵族签到的每日次数由于hoshino默认，不是跨群独立的，想修改可以自己修改。(现在已实现独立，此条作废)
5. 女友列表在_pcr_duel_data.py里，已与原版pcrdata分离。
6. 氪金功能没有写在说明书中，最好不要开启，开启氪金十分无聊。
7. 新增的dlc需相应的pcrdata和unit头像包，我会放在github的release里，
8. 安装dlc步骤：
	(1)release里找到dlc包
	(2)覆盖_pcr_duel_data.py(或者根据自己情况增减)
	(3)unit放在与pcr头像同文件夹
	(4)如果自行找到角色立绘，可以放在pcrduel目录下的fullcard文件夹
	(5)dlc描述和列表之类的，我已经在init文件里定义好，dlc里的dlc可以不管，如果自己制作dlc，需在init文件中照着格式定义列表和写dlc描述。
9. 新增了在招募时发送角色立绘功能，这个需要角色有立绘包。如果有的话，请在同目录下的fullcard文件夹里，按文件夹中范例，{角色id}31.png的格式添加立绘，如果没有角色立绘，则发送角色头像。
10. 魔改版的猜头像猜金币，放在了github仓库的release里，需要的自取。猜语音版本很多，需要的自行照着改就行。
 
