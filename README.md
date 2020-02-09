# 简介
在本 repo 中您可以提交 issue 反馈有关软糖的建议或者漏洞。

## 账号列表
软糖酱（七天冻结）：2862355742

软糖酱测试机（七天冻结）：3041853563

软糖酱三号机：3303997512

软糖酱四号机（限制解冻）：1840726229

软糖酱五号机（七天冻结）：3355327497

### 若五个账号均无法使用，私用机如需使用请至反馈群申请白名单。

## 反馈群
951585303

# 更新日志
## 一群两号规则（Beta）

注意：该规则仍处于设想状态，并未开始实践。

为觉得多号占用群空间的群主设计，现在只需要两个号就可享受理论不间断软糖体验。

您只需给软糖酱分流机一个管理，分流机会自动踢出离线软糖并且拉入处于在线状态的软糖，让您的群保持只有除分流机外一个账号的状态，大大减少软糖酱多个号占用群成员数量的问题。

不排除分流机无法使用的情况，分流机只有一个账号，不会有其它如二号机的情况。若分流机处于离线状态（如被冻结等）将无法自动进行操作，此时您需要手动操作。

反之您如果并没有觉得占用这相关的问题，则可以直接一次性拉入软糖酱的所有账号（除分流机），也可享受理论不间断体验。

*上文所提到的不间断指的是软糖其它账号在线的不间断，不包括所有号处于离线状态的不间断。

## 2019/10/19
新增了一些指令前缀：/arcaea（原有：/arc）、/ma（原有：/malody）

新增了退群提示（默认为关）：/group permit leave ...

新增了文本处理指令（帮助：/x help text）：
Base64 编解码、MD5 计算、简繁转换、文本转语音

修改 Pixiv 获取指令：
/send pixiv info <member|illust> ... => /send pixiv <member|illust> ...

发言排行支持显示您或群在总排名的位置。

米言支持随机关键词：/miyan query <关键词>

修复了些许漏洞。

## 2019/10/26
新增了韵律源点绑定账号（需账号、密码）：/arc bind account [...]

新增了韵律源点查询账号：/arc pinfo

新增了韵律源点默认卡片查询选项：/arc config card

修改韵律源点查询指令：
/arc bind config <选项> => /arc config <选项>

支持了韵律源点新曲与搭档（2019/10/26）。

支持了其它音游查询省略第二个参数，如：/ma、/osu、/osu pc

修改了文本转语音的 API。

修复了些许漏洞。

## 2019/11/1
新增了韵律源点随机曲目：/arc rand [难度]

新增了韵律源点搜索曲目：/arc search <曲名>

韵律源点计算潜力值现在支持俗称。

修复 osu!droid 无法查询绑定账号详情的问题。

修复查询单曲最佳成绩失败提示后出现乱码的问题。

修复私聊软糖酱提示状态异常的问题。

修改 Yande 和 Konachan 获取指令（Yande 为例）：/send yande info <illust|pool> ... => /send yande <illust|pool>

## 2019/11/2
新增查询发言记录历史月份：/rank ... 1m <月份>

修改了三条复读的规则：

自动复读 100% -> 90%；自动打断复读 0% -> 10%

修改了随机复读的规则：0.5% -> 0.2%

修复正常使用 Tweet 获取出现防滥用的问题。

修复测试机发言记录为空的问题（测试机与主号聊天记录不共通）。

现在仅 At 软糖酱不带其它文本才会自动回复。

优化了签到的速度。

## 2019/11/16
新增了 osu! 默认查询模式设置：/osu pc config mode [模式]

新增了 osu!droid 查询单曲最佳成绩：/osu info <谱面 ID> [难度]

新增了韵律源点购买绑定账号好友位和体力（强烈建议阅读帮助文档）：
/arc purchase <friend|stamina>

新增了韵律源点获取拥有付费曲目的直链下载地址。

新增了定义指令功能（强烈建议阅读帮助文档）

- 新增定义：/define add </用于替换的指令>
<^被替换的正则$>
- 删除定义：/define del <定义 ID|all>
- 定义列表：/define list

新增自定义打断复读几率：/group permit this repeat break <几率 %>

新增自定义随机复读几率：/group permit this repeat random <几率 %>

支持了文本转语音的权限项设置：/group permit - tts [true|false]

修复了部分指令提示文本错误的问题。

修复了多行文本无限复读的问题。

*帮助文档中更新内容使用 NEW 标注

修复了编译指令无法使用的问题（可能为临时方案）。

## 2019/11/22
新增了定义指令加载、导出配置：/define <load|export> [...]

新增了定义指令调试模式：/define test

/define 开头的指令现在不会受定义影响。

入群欢迎现在 @ 替换符后不会自动加空格。

支持了群管理员对自己群使用单群无视用户、群权限、定义指令。

修复了发言排行指令与定义指令冲突的问题。

修复了定义指令无法定义 @、表情等特殊消息。

## 2019/11/30
新增了以图搜图 ascii2d 备选查询 API。

打断复读与随机复读几率现在可以自定义为 0%。

文本转语音现在会自动替换表情、图片等特殊内容。

支持了编译的权限项设置：/group permit - compile [true|false]

(!) 修复了韵律源点卡片查询部分 EX 成绩时潜力值计算错误的问题。

修复了定义指令导出配置没有反斜杠的问题。

移除了以图搜图 TinEye 查询 API。

## 2019/12/14
文本转语音现在支持其它部分语言：/tts [ja|us|au|cn] <内容>

支持了群管理员对自己群使用推特 RSS 订阅。

修复了复读几率设置提示文本错误的问题。

修复了韵律源点卡片查询隐藏潜力值无法查询的问题。

修复了韵律源点卡片查询不显示唤醒角色的问题。

移除了 OSS 对象存储功能。

## 2019/12/28
新增了随机数生成：/roll \[起始值] \[结束值] \[循环次数]

新增了成语接龙统计：/x game cyjl stat

成语接龙现在会随机先后手。

计算器 (Beta) 功能暂可使用，但并无法保证能正常使用：/calc ...

支持了辅助功能 - 自动同意入群请求的权限项设置：/group permit - autoagree [true|false]

修改了发言指令的部分格式。

修复了发言排行指令，发言记录不足导致的返回结果错误的问题。

## 2020/1/10
新增しりとり（日语词语接龙）：/x game siritori <start|end|stat|词语>

成语接龙现在可以选择难度：/x game cyjl start <normal|easy>

修复了成语接龙判定部分非成语的内容为通过。

修复了成语接龙反馈内容有误的问题。

移除了 Ping 指令。

## 2020/1/29
*因消息处理量过大，导致反应延迟过大，故现已临时升级服务器配置。

新增了消息排行 - 按字数排行：/rank ... -l

*看不懂？前往 https://bot.lxns.org/help/ 查询更多帮助

新增了翻译功能：/trans [目标语言] <待翻译的文本>

新增了 osu!droid 用户名更名申请：/osu rename ...

支持了消息排行的权限项设置：/group permit - rank [true|false]

修复了韵律源点曲目查询没有显示在帮助的问题。

*另因特殊原因，反馈群群号已更改为 951585303
