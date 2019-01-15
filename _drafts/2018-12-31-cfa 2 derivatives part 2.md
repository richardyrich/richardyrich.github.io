---
layout: post
title: CFA Level 2 衍生 Part 2
categories: CFA2级笔记
---

## 目录

1. 掉期期权合约（swaption）
2. 信用违约掉期（credit default swap）

<br><br>

## 1\. 掉期期权合约（swaption）

<br><br>

掉期期权合约（swaption）

- 本质是期权
- 固定利率也是提前约定的

掉期期权合约的价值变化

- 支付方掉期期权（payer swaption），执行后，期权持有者变为固定利率支付方，当利率上升时，期权的价值上升
- 接受方掉期期权（receiver swaption），执行后，期权持有者变为浮动利率支付方，当利率下降时，期权的价值下降

掉期期权合约的作用

- 提前结束已有的掉期合约
  - 因为想要的，与现有合约想法的掉期合约不易寻找

掉期合约的违约风险

- 利率掉期合约：随时间，刚开始小，期间变大，快结束时再变小
- 货币掉期合约：越逼近结束时，风险越大，在快结束时稍微下降
- 使用钆差（netting）可以降低违约风险

掉期利率利差（swap spread）

- = 掉期利率 - 相同期限的新发行（on-the-run）国债的到期收益率

> 在固定收益部分也提及到掉期利率利差，批发银行间的拆放利率，用于计量离岸市场大型金融机构的平均信用风险

<br><br>

## 信用违约掉期（credit default swap）

<br><br>

信用违约掉期

- 可以理解为保险
- 标的资产物叫做参考债务（reference obligation）
  - 参考债务可以是债券（bond）或者贷款（loan）

信用违约掉期的保险费用（premium）

- 保险费用（premium），支付的是一个百分比，所以也成为利差（spread）
- 虽然信用违约掉期是场外交易的，但是被高度标准化了，监管机构叫做国际掉期交易协会（international swaps and derivatives association (ISDA)）
  - 由于实际上，每个机构的信用风险都不同，所以存在保费缴纳过度或者缴纳不足的情况，于是需要进行多还少补

单一信用违约掉期（single-name credit default swap）vs 一揽子信用违约掉期（index credit default swap）

- 一揽子信用违约掉期保护的是一系列债券的违约风险

触发信用违约掉期的条件

- 破产（bankruptcy）
- 未履行付款义务（failure to pay）
- 重组（restructuring）

信用违约掉期的赔偿/交割（settlement）

- 可以分为现金交割（cash settlement）或者实物交割（physical settlement）
- 偿付率（payout ratio）
  - 1 - 恢复率（recovery rate）
- 偿付金额（payout amount）
  - 偿付率（payout ratio）× 名义本金（notional principal）

信用违约掉期的保险费用（premium）的特点

- 和违约概率正相关
- 和违约损失率（loss given default）（= 偿付率相等）正相关

信用利差曲线（credit spread curve）

- 横坐标时间，纵坐标信用利差

裸信贷违约掉期（naked credit default swap）

- 即使和标的资产物没有有任何相关债权债务关系（have no exposure to the reference entity），也可以购入信贷违约掉期

长短仓交易策略（long/short trade）

- 做多一个参考实体（reference entity）（公司，或者机构等），同时做多另一个参考实体（reference entity）
- 可以是使用单一信用违约掉期或者一揽子信用违约掉期

曲线交易策略（curve trade）

- 可以分为陡峭化交易策略（steepening trade）或者平缓化交易策略（flatening trade）
- 发生在同一个参考实体（reference entity），不同的期限

基差交易策略（basis trade）

- 信用违约掉期和债券之间的交易
- 理论上信用违约掉期的保金（=利差）应该等于债券的信用利差，否则存在套利机制
- 无风险证券（default-free securities）+ 做空信用违约掉期 可以合成担保债务凭证（synthetic collateralized debt obligation (CDO)）
