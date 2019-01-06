---
layout: post
title: CFA Level 2 固定收益 Part 2
categories: CFA 
---

## 目录

1. 无套利估值（arbitrage-free valuation）
2. 二差利率树（binomial interest rate tree）
3. 顺向估值（pathwise valuation）
4. 蒙特卡洛模拟（monte carlo method）
5. 嵌入式期权（embedded option）
6. 可赎回债券和可卖回债券的分析和估值

<br><br>

## 无套利估值（arbitrage-free valuation）

一价定律（law of one price）

- 完全同质的商品应该有相同的价格

两种套利机会（arbitrage opportunity）

- 价值增加（value additivity）
  - 整体的价值和个体的价值之和存在差异（the value of whole differs from the sum of the value of parts）
  - 剥离（stripping）：将国债的息票拆分成独立的现金流，作为零息债券进行交易
  - 重组（reconstitution）：和剥离反过来
- 占优（dominance）：在未来存在无风险收益的金融资产的现值应该为正



## 2\. 二差利率树（binomial interest rate tree）

<br><br>

使用二差树（binomial tree）计算债券价格

- 逆向归纳估值法（backward induction valuation method）
  - 对于存在N期复利计算期的债券，该债券的现值是通过计算在第N期时可能的价值，再逐步逆推折现计算第0期的价值
- 无权债券的无套利估值（arbitrage-free valuation for option-free bond）
  - 使用基准即期利率（benchmark spot rates）定价
  - 使用二差利率树（binomial interest rate tree）定价
- 使用基准即期利率和使用二差利率树两种方法得到的定价应该都是相同的
  - 因为二差利率树是无套利机会的
- 二差利率树适合含权债券（bonds with embedded options）的定价

未来利率变动的估计需要符合以下三个条件

- 模型中利率的随机过程（random process of interest rate）符合对数正态分布（lognormal random walk）
  - 利率越高时波动性越大，而且假设利率不为负
- 波动率的设定
  - 历史利率波动率（historical interest rate volatility）：使用历史数据
  - 隐含利率波动率（implied interest rate volatility）：观察那些以利率作为标的资产（underlying asset）衍生品（derivative）的变动，逆推利率的波动性
- 利率的均值是由当前的基准收益率曲线（current benchmark yield curve）计算而得

在二差利率树中

- 同一时期的相邻分支的差别总是2个标准差，计算方法是 e<sup>2σ</sup> 的倍数
- 每个时期最中间的分支（或者说平均值）（middle forward rate）总是和远期利率大致相等
- 在正式使用前，需要找出一组定价正确的证券作为基准（benchmark security），进行微调



## 3\. 顺向估值（pathwise valuation）

- 对于有n期的二差利率树，一共有2<sup>n-1</sup>种利率演变路径，每条路径的概率都是相等的
- 计算这些路径的现值的平均值

<br><br>

## 4\. 蒙特卡洛模拟（monte carlo method）

- 蒙特卡洛模拟可以视作极为复杂的顺向估值（pathwise valuation）
- 蒙特卡洛模拟常用于计算现金流会因为路径的变化而改变的（cash flows are path dependent）证券
  - 比如含权债券

  <br><br>

## 5\. 嵌入式期权（embedded option）

**基础型期权**

1. 可赎回债券（callable bond）
2. 可卖回债券（putable bond）
3. 可展期债券（extendible bond）
4. 可转换债券（convertible bond）

**复杂型期权**

1. 财产看跌期权 / 继承人期权（estate put / survivor's option）
2. 提前偿债赎回基金（sinking fund arrangement）

**可赎回债券（callable bond）**

- 可赎回债券 = 直接债券（straight bond）- 看涨期权（call option）
- 发行人使用的期权，使用的时机为
  - 在市场利率（market interest rates）下降时
  - 发行人的信用等级（credit quality）上调时
- 投资人的义务（obligation）
  - 更高的再投资风险（reinvestment risk）
  - 更高的潜在收益，更低的发行价格

可赎回债券的特点

- 锁定期（lockout period）
  - 在锁定期内，债券的发行人不能行权
- 欧式期权（european-style）制定一个日期行权
- 美式期权（american-style）有效日期内行权
- 百慕大式期权（bermuda-style）有效日期内多个特定日期行权
- 不可调换债券（non-refundable）
  - 不允许使用存在更低的融资成本的融资赎回债券（用更低利率的债券借贷，然后赎回现有的债券）
- 赎回补偿（make-whole call）
  - 赎回的价格必须足够高，以能够补偿投资者因为债券被赎回带来的损失

**可卖回债券（putable bond）**

- 可卖回债券 = 直接债券（straight bond）+ 看跌期权（put option）
- 持有者使用的期权，使用时机为利率水平上升后
- 发行人的义务（obligation）
  - 更高的发行价格，更低的收益率

**可展期债券（extendible bond）**

- 债券的持有者在债券到期时有权要求延长债券的期限，虽然债券的其他特性会改变，比如息票（coupon）会改变

**可转换债券（convertable bond）**

- 可转换债券 = 无权债券（option-free bond）+ 权益看涨期权（embedded equity call option）
- 债权的持有者拥有将债券转化成一定比例的普通股
- 对于债券持有者的优势
  - 下行保护（downside protection） & 权益上行潜力（equity upside potential）
- 对于发行者的优势
  - 减少利息支出
  - 转换后，债务被消除
- 对现有股东的劣势
  - 股份稀释

**财产看跌期权 / 继承人期权（estate put / survivor's option）**

- 当原有债券持有者逝世，继承人可以行使期权，以票面价值（par value）卖回

**提前偿债赎回基金（sinking fund arrangement）**

- 与可赎回债券（callable bond）不同，提前偿债赎回是强制的执行的

<br><br>

## 6\. 可赎回债券和可卖回债券的分析和估值

<br><br>

- 基本原理
- 在利率零波动的（zero volatility）情况下无风险含权债券的估值
- 利率波动的对于无风险含权债券无风险含权债券的估值影响（impact of interest rate volatility）
- 使用二差利率树（binomial interest rate tree）对存在利率波动的无风险含权债券进行估值
- 对于含权风险债券（risky bonds）的估值
- 含权债券的利率风险（interest rate risk）

<br><br>

### a）基本原理

看涨期权（call option）对于发行人的价值

- = 直接债券（straight bond）的价值 - 可赎回债券（callable bond）的价值

看跌期权（put option）的价值

- = 可卖回债券（putable bond）的价值 - 直接债券（straight bond）的价值

<br><br>

### b）在利率零波动的（zero volatility）情况下无风险含权债券的估值

可赎回债券（callable bond）

- 赎回法则（call rule）：任何时间内，可赎回债券的价值都不会超过赎回价格



可卖回债券（putable bond）

- 卖回法则（call rule）：任何时间内，可卖回债券的价值都不会低于卖回价格



### c）利率波动的对于无风险含权债券无风险含权债券的估值影响（impact of interest rate volatility）

- 利率波动增大，期权的价值增大，因此
  - 可赎回债券（callable bond）的价值下降
  - 可卖回债券（putable bond）的价值上升

**可赎回债券**

收益率曲线的水平变动（changes in the level）

- 随着利率的下降，可赎回债券的价值上升的幅度没有直接债券的幅度大，限制了投资者获得上行收益的潜能

收益率曲线的形状变动（changes in the shape）（非水平移动）

- 当收益率曲线从向上倾斜（upward sloping）到水平（flat）再到向下倾斜，看涨期权的价值上升
  - 在这种条件下，计算二差利率树时更容易遇到期权被执行的状态

**可卖回债券**

收益率曲线的水平变动

- 随着利率的上升，可赎回债券的价值下降的幅度没有直接债券的幅度大，限制了投资者获得下行损失的潜能

收益率曲线的形状变动（非水平移动）

- 当收益率曲线从向上倾斜（upward sloping）到水平（flat）再到向下倾斜，看跌期权的价值下降
  - 在这种条件下，投资者使用看跌期权的机会变少

  <br><br>

### d）使用二差利率树（binomial interest rate tree）对存在利率波动的无风险含权债券进行估值



> Q4: Relative to its price at 15% interst rate volatility, the price of Bond X at a lower interest rate volatility will be:
> A. lower. B. the same. C. higher.

> Q5: Q4: Relative to its price at 15% interst rate volatility, the price of Bond Z at a lower interest rate volatility will be:
> A. lower. B. the same. C. higher.

> ### Answer

> Q1: B Q2: C Q3: B Q4: C Q5: A

（下一部分续）
