---
layout: post
title: CFA Level 2 数量 Part 2
categories: CFA 
---


## 目录

1. 总结
2. 什么是协方差平稳(Covariance stationarity)？
1. 什么是随机漫步？
1. 随机漫步的特点（random walk）？
1. 什么是一阶差分（First differencing）？
2. 自相关模型的解释能力
3. 多个时间序列数据回归的Dickey-Fuller test检验（是否存在单位根）
4. 什么是协整(co-integration）？

<br><br>

## 1\. 总结

<br><br>

如果有一组数据，没有自变量，那么就使用**时间序列模型**（time series）

1\. 可以**使用时间t作为自变量**，将数据进行一元线性回归（Trend Model）

> 本质上相当于考生自行引入了自变量t

- 要考虑是否存在自相关（Autocorrelation），使用杜宾沃森检验（Durbin-Watson Test）
- 如存在自相关的话，将数据取log对数，并再用杜宾沃森检验是否存在自相关

2\. 如果以上方法不适用，使用**自回归**
> 使用自身的上一期估算下一期：AR（1）模型，但是要考虑两个问题
>
> 1. 是否存在自相关和
> 2. 协方差是否平稳



**自回归公式：X<sub>t</sub> = b<sub>0</sub> + b<sub>1</sub> X<sub>t-1</sub> + ε<sub>t</sub>**

a. 考虑是否存在自相关 （不能使用杜宾沃森检验）

- 自相关检测方法：计算n期数据之间的自相关系数（t检验，n可以是1,2,3,4）

- 假如滞后多期存在自相关（存在季节性：比如酒店的入住率和4季度前的数据存在自相关），那么就制作新的自相关模型并引入季度滞后（seasonal lag），并重新做二元回归，甚至是多元回归（假如有多个seasonal lags），不断的引入seasonal lag直至不存在自相关

b. **协方差是否平稳**(Covariance stationarity)

- 检验是否存在均值回归，使用迪基-福勒检验（Dickey-Fuller test）检验

> 本质上就是检验斜率是否等于1，是一个t-test

- 如果斜率等于1，那就存在**单位根**，那么协方差不平稳，这是一个随机漫步数据
- 随机漫步数据进行了一阶差分后，便可再进行自相关模型拟合

<br><br>

## 2\. 什么是协方差平稳(Covariance stationarity)？

<br><br>

- 仅在数据存在协方差平稳的时候才可以使用普通最小二乘法（Ordinary least squares）

- 协方差平稳的三个条件

  1. 期望值恒定(constant and finite expected value)
  2. 方差恒定(constant and finite variance)
  3. 协方差恒定(constant and finite covariance with leading or lagged value)

**均值回复：**

期望值恒定的数据存在均值回复，也就是说数据从长远来看倾向于向某个固定的均值聚拢

均值：x<sub>t</sub> = b<sub>0</sub> / (1 - b<sub>1</sub>)

<br><br>

## 3\. 什么是随机漫步（random walk）？

> 随机漫步如同一个醉汉的行走路径，他的方向完全随机

<br><br>

**定义：**

当自相关方程unit root存在单位根（b<sub>1</sub> = 1）, 意味着数据处在了随机漫步模式

随机漫步分两种情况

* Simple random walk
* random walk with drift

1\. Simple random walk 简单（无漂移的）随机漫步（b<sub>0</sub> = 0）

特点：

* X<sub>t</sub> 预期和 X<sub>t-1</sub>相同，但是存在随机误差ε<sub>t</sub>
* 公式：X<sub>t</sub> = X<sub>t-1</sub> + ε<sub>t</sub>

2\. random walk with drift 有漂移的随机漫步（b<sub>0</sub> ≠ 0 ）

特点：

* X<sub>t</sub> 总是预期比 X<sub>t-1</sub>增加（减少）一个特定的量（b<sub>0</sub>）

**检验：**

使用迪基-福勒检验（Dickey-Fuller test）检验

t = （b<sub>1</sub>(样本平均值）- 1）/ S<sub>b<sub>1</sub></sub> 总体标准差

原假设：b<sub>1</sub> = 1

<br><br>

## 4）随机漫步的特点？

<br><br>

从 Covariance stationarity的角度来看

* 随机漫步出现在当unit root等于1的时候（b<sub>1</sub> = 1）
* 随机漫步不存在均值回归（no mean reverting level）
* 无论有没有漂移的随机漫步都不存在协方差平稳（not covariance stationary）

<br><br>

## 5）什么是一阶差分 （First differencing）？

<br><br>

> 一阶差分其实是一个微分求导的过程，用于处理协方差不平稳的随机漫步。将原本不平稳的随机漫步进行一阶差分后，得出的结果是协方差平稳的（或者多阶差分，但是CFA不考这么难的内容，一般默认一阶差分即可）

* 一阶差分假设x<sub>t</sub>每一期的增量是随机值：y<sub>t</sub> = x<sub>t</sub> - x<sub>t-1</sub> = ε<sub>t</sub>
* y<sub>t</sub>存在均值回归，均值为0，因为 b<sub>0</sub>/(1-b<sub>1</sub>) = 0
* 公式：y<sub>t</sub>  = b<sub>0</sub> + b<sub>1</sub>y<sub>t</sub> + ε<sub>t</sub>  （其中b<sub>0</sub>和b<sub>1</sub>都是0）

<br><br>

## 6）自相关模型的解释能力

<br><br>

- **样本内和样本外的解释（预测）能力**

 - 对于过去已经产生的数据的解释能力&未来将会产生的数据的解释能力（in-sample forecasts and out-of-sample forecast）

- **Root mean squared error (RMSE)越小越好**

 - 本质上是Standard Error of Estimate (SEE) = Mean squared error 开根号（Mean squared error在前面ANOVA里提到过）

- **异方差（Heteroskedasticity）**

 - 自回归条件异方差 ARCH(1)
 - 将残差进行自相关拟合，如果发现拟合的模型没有解释力，说明不存在异方差（残差不存在自相关）
 - **ɛ<sup>2</sup><sub>t</sub> = α<sub>0</sub> + α<sub>1</sub>ɛ<sup>2</sup><sub>t-1</sub> + μ<sub>t</sub>**

<br><br>

## 7）多个时间序列数据回归的Dickey-Fuller test检验（是否存在单位根）

<br><br>

三种情况

1. 没有一个时间序列存在单位根
1. 至少有一个时间序列存在单位根
 * 不能回归
1. 全都存在单位根
 * 如果这些数据存在**协整(co-integration）**，可以回归，否则不能回归

<br><br>

## 8）什么是协整(co-integration）？

> 协整：时间序列数据之间存在长期的金融或者经济上的关系

<br><br>

测试协整的假设检验Dickey-Fuller Engle-Granger test (DF-EG test）

* 原假设：不存在协整 - 不可以使用多元回归
* 备择假设：存在协整 - 可以使用多元回归

<br><br>
