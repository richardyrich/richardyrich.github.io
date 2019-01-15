---
layout: post
title: CFA Level 2 数量 Part 3
categories: CFA2级笔记
---


## 目录
1. 情景分析，决策树，模拟的区别
2. 模拟的步骤
3. 模拟的优势
3. 模拟的应用

<br><br>

## 1）情景分析，决策树，模拟的区别
<br><br>
离散的

- 情景分析
- 决策树  

连续的
  
- 情景分析

| Risk Approach     | Discrete/ Continuous | Correlated/ Concurrent | Sequential/ Concurrent |
|-------------------|----------------------|------------------------|------------------------|
| Scenario analysis | Discrete             | Correlated             | Concurrent             |
| Decision tree     | Discrete             | Independent            | Sequential             |
| Simulations       | Continuous           | Either                 | Either                 |

<br><br>

## 2）模拟的步骤
> 其实就是传说中的 monte carlo simulation

<br><br>

1. 指定应该使用的变量（variables）
2. 定义变量的概率分布（probabilistic distribution）
  * 历史数据（historical data）
  * 同类型数据比较（Cross section data）
  * 自行指定可能存在的概率分布模式（Statistical distribution and parameters）
3. 指定相关系数（correlation）
  * 两种处理存在着相关性的随机自变量的方法：
    * 选择对因变量影响最大的其中一个随机自变量
    * 将随机自变量的相关性的影响也建入模型内
4. 将模拟运行足够次数
  * 随机自变量的个数越多，应该运行的次数越多
<br><br>
<br><br>

## 3）模拟的优势

- 对输入参数（随机自变量）的模拟更加合理
- 输出结果不再是一个单点的估计，而是一个概率分部

<br><br>

## 4）模拟的应用
* 账面价值（book value）
  * 测试公司的资本是否满足法律要求
  * 例如：金融机构的资本是否满足资本充足率

> 巴塞尔协议，全名是资本充足协定（Capital Accord），是巴塞尔银行监理委员会成员，为了维持资本市场稳定、减少国际银行间的不公平竞争、降低银行系统信用风险和市场风险，推出的资本充足比率要求。在1988年首次订立，并于2003年作出了第二次的修订。
>   
> https://zh.wikipedia.org/zh-cn/巴塞尔协议

* 利润和现金流
  * 公司预测未来利润和现金流动向
  * 测试公司的利润和现金流是否满足贷款的要求

* 公司市值
  * 满足再融资要求

<br><br>

## 5）模拟的注意事项
* 输入参数需合理（garbage in garbage out）
* 现实数据不一定完全符合模拟的假设的模型
* 未来的数据的概率分布模式可能会与历史数据不同
* 随机自变量的相关系数可能会发生变化