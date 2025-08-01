---
lang: zh-CN
title: 功能-一条龙
author: DoctorReid
date: 2024-09-01
---
## 0.使用前需知

使用本页说明的功能时，建议阅读以下内容：
::: important
- 不同标签页功能不可同时启用
- 各功能使用之前需要去对应的功能页进行相关设置
:::

## 快速开始-一条龙
一条龙整合大量日常功能，使其按一定顺序进行执行。

### 一条龙运行
--- 
按需开启对应功能，点击名字跳转对应说明

|  功能   | 说明  |
|  ----  | ----  |
| [兑换码](#兑换码) | 用于兑换文件夹内已储存的长效兑换码 |
| [录像店营业](#录像店营业) | 用于完成录像店每天的开门营业 |
| [刮刮卡](#刮刮卡) | 用于完成报刊亭的每日刮刮卡 |
| [卦象集录](#卦象集录) | 用于完成卦象集录的每日抽签 |
| [体力刷本](#体力刷本) | 用于完成每日的清体力活动 |
| [咖啡店](#咖啡店) | 用于自动前往咖啡厅执行喝咖啡任务 |
| [恶名狩猎](#恶名狩猎) | 用于自动解决恶名狩猎 |
| [活跃度奖励](#活跃度奖励) | 用于自动领取活跃度奖励 |
| [枯萎之都](./feat_hollow_zero.md) | 用于自动完成零号空洞-枯萎之都的相关任务。相关配置在 [枯萎之都]中。 |
| [迷失之地](./feat_lost_void.md) | 用于自动完成零号空洞-迷失之地的相关任务 |
| [式舆防卫战](#式舆防卫战) | 用于自动完成式舆防卫战的相关任务 |
| [丽都城募](#丽都城募丽都周纪) | 用于自动领取战令活跃度 |
| [丽都周纪](#丽都城募丽都周纪) | 用于自动领取周纪奖励 |
| 邮件 | 用于自动收取邮件奖励 |
| [驱动盘分解](#驱动盘分解) | 用于自动分解驱动盘 |
| [真拿命验收](./feat_game_assistant.md#拿命验收) | 用于自动完成`拿命验收`副本 |
| [随便观](#随便观) | 用于自动完成随便观刷取任务 |
| [通知](./feat_notify.md) | 用于自动发送一条龙运行通知 |

## 预备编队

用于自动战斗时的配队，需要和游戏内的预备编队一致  
可以使用`游戏助手`-`预备编队识别`页面的工具进行自动识别填写  
需要注意编队名称尽量**不要只有一个字或者只有数字**的差异，以防识别错误  

## 体力计划
设置后可以使用一条龙功能自动战斗获取资源

1. 循环执行：开启后，将循环执行到体力用尽
1. 跳过计划：开启后，将跳过体力不足部分的体力计划
1. 使用家政券：开启后将允许定期清缴功能使用家政券
1. 新增体力计划：用于添加需要刷取的副本
   - 副本类型（如：定期清缴，恶名狩猎等）
   - 副本刷取内容（如：驱动盘，挑战的BOSS等）
   - 副本刷取编队，选择战斗使用的[预备编队](#预备编队)
   - 计划次数：当前副本计划刷取的次数（填为0时将停止当前副本的刷取）

> 体力计划内的 <font color="red">恶名狩猎 **深度追猎** </font> 是 **深度追猎** 模式  
> 需要每周三次恶名狩猎打完才可以使用

## 恶名狩猎计划

- 用于安排恶名狩猎的刷取计划
1. 恶名狩猎副本：固定的恶名狩猎副本与顺序
1. 恶名狩猎等级：默认为最高等级，可以自行选择
1. 恶名狩猎编队：默认选择游戏内编队，或手动设置要使用的[预备编队](#预备编队)
1. 恶名狩猎自动战斗：默认为全配队通用，可自行选择
1. 恶名狩猎buff配置：选择第几个buff，默认为第一个

## 咖啡计划（已随游戏版本更新而不再使用

1. 咖啡选择：优先选择符合体力计划的咖啡，默认为汀曼特调
1. 喝后挑战：喝完咖啡（加完体力）之后，进行副本挑战，分为：全都挑战、只挑战体力计划、不挑战
1. 体力计划外的数量：挑战体力计划外的数量
1. 预备编队：默认选择游戏内编队，或手动设置编队（与游戏内编队一致）
1. 自动战斗：与战斗助手内的配置方式一样，详见 [自动战斗](./feat_battle_assistant.md)
1. 结束后运行体力计划：用于设置喝咖啡（加体力）是否在体力结束后开启 

## 其他设置

- 影像店代理人：设置影像店的经营代理人
- 驱动盘拆解：自动拆解驱动盘。分为 `S级以下，A级以下，B级` 。

## 一条龙功能说明
### 兑换码
每当检测到存在新的兑换码时，自动兑换  
兑换码文件存储于： `config/redemption_codes.yml` 可以手动添加

### 录像店营业
每天自动进行一次录像店的营业上架  
可以在 `一条龙-其他设置-影像店代理人` 设置使用的角色

### 刮刮卡
每天自动进行一次刮刮卡  
**与卦象集录不能同时开启**

### 卦象集录
每天自动前往随便观获取卦象 需要解锁随便观
**与刮刮卡不能同时开启**

### 体力刷本
根据 [体力计划](#体力计划) 设置的项目自动刷取素材

### 咖啡店
自动前往咖啡店喝咖啡，喝完会自动再进行一次体力计划的刷取

### 恶名狩猎
根据 [恶名狩猎计划](#恶名狩猎计划) 的设置项目自动刷取每周三次周本素材

### 活跃度奖励
自动领取 `快捷手册-日常` 内的每日活跃度奖励

### 式舆防卫战
每个周期自动进行式舆防卫战的挑战  
需要配置了 `预备编队` 和 `一条龙-式舆防卫战` 相关节点  
保证每个弱点都至少有一个编队勾选了可以打

### 丽都城募&丽都周纪
自动领取 `丽都城募(战令)` 的活跃度和奖励

### 驱动盘分解
自动分解背包内的驱动盘，可以在 `其他设置-驱动盘拆解` 设置拆解等级

### 随便观
自动进行随便观的收菜补货等操作
- 游历收菜操作
   - 需要至少24只游历邦布以防电量不足
   - 探索会自动重复进行上次游历时的地图和时长
- 制造和售卖补货
   - 按顺序选择已有的可以制造的道具进行制造
   - 按顺序对售卖货架进行补货
- 饮茶仙自动刷新和提交道具