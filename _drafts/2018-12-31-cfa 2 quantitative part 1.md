---
layout: post
title: CFA Level 2 数量 Part 1
categories: CFA2级笔记
---

## 目录

1. 总结
2. 基本概念
1. 一元回归模型
2. 多元回归模型
3. 判别回归模型的解释能力 1：方差分析（ANOVA）- 量化指标
4. 判别回归模型的解释能力 2：t 检验（t test）- 定性指标
5. 判别回归模型的解释能力 3：F 检验（F test）- 定性指标
6. 虚拟变量（dummy variable）
6. 第一种违反：异方差（homoscedasticity）
1. 第二种违反：序列相关/自相关（Serial correlation/autocorrelation）
1. 第三种违反：多重共线性(Multicollinearity）

<br><br>

## 1）总结
<br><br>
**1\. 判别回归模型的解释能力** 

- 定量：方差分析（ANOVA）
- 定性：t检验（t test），F检验（F test）

**2\. 虚拟变量（dummy variable）**

- 斜率系数，截距系数
- t 检验

**3\. 前提假设的三种违反**

- 异方差（homoscedasticity）
- 自相关（Serial correlation/autocorrelation）
- 多重共线性（Multicollinearity）

<br><br>

## 2）基本概念
<br><br>
**协方差(covariance)**

- 变量和自身的协方差就是方差
- 协方差的取值范围：负无穷到正无穷 

**相关系数（Correlation）**   

- 相关系数没有单位   
- 由协方差计算而得：**-1 ≤ ρ <sub>xy</sub> = Cov(x, y)/(s<sub>x</sub> s<sub>y</sub>) ≤ 1**
- 度量的是两个变量之间的线性关系
- 相关系数和斜率是两个概念：相关系数 = 1 不代表斜率 = 1

**回归分析的局限**
 
- 异常值（outliner）  
- 伪相关（Spurious correlation）
- 非线性关系（Nonliner relationships)

<br><br>

## 3）一元回归模型
> 一元回归方程公式：**y<sub>i</sub> = b<sub>0</sub> + b<sub>1</sub> x<sub>i</sub> + ε<sub>i</sub>**

<br><br>
**回归方程的显著性检验：**
  
相关系数的假设检验：  
t 检验（t-test）  

t = r√（n - 2）/√（1 - r<sup>2</sup>）
  
- df = n - k - 1    
- r = 相关系数（correlation）
- k = 自变量的个数，在一元回归方程里 k = 1

> CFA 1级涉及4种假设检验：
> 
>  * z检验
>  * t检验
>  * F检验
>  * X<sup>2</sup>检验

**一元回归的6个前提假设：**

1. x和y之间存在线性关系
1. x和残差不相关
1. 残差的期望值为0
1. 残差的方差恒定（homoscedasticity）
1. 残差之间不存在相关性
1. 残差服从正态分布

**自变量系数的计算：**  
b<sub>1</sub> = Cov（x, y）/Var（x）  
b<sub>0</sub> = y（平均值）- b<sub>1</sub> x（平均值）

<br><br>

## 4）多元回归模型
<br><br>
**多元回归的6个前提假设：**  

1. 自变量和y之间存在线性关系  
1. 自变量之间不存在相关关系  
1. 残差的期望值为0  
1. 残差的方差恒定（homoscedasticity）  
1. 残差之间不存在相关性  
1. 残差服从正态分布  

> 对比一元回归的6个前提假设，会发现仅有2. 稍有不同

<br><br>

## 5）判别回归模型的解释能力 1：方差分析（ANOVA）- 量化指标
<br><br>
**方差分析（ANOVA）：**  

总平方和 = 回归平方和 + 残差平方和  
（Total sum of square = regression sum of square + error sum of square）

**估计标准误差（Standard error of estimate）：** 

估计标准误差 = √残差平方和  
> 平均残差平方和 = 残差平方和/（n - k - 1）

**决定系数 R<sup>2</sup>（Coefficient of determination）：**  

R<sup>2</sup> > 0.7 意味着回归关系显著   
（aka. 70%的y的变化能被x的变化解释）

a. 一元回归中：R<sup>2</sup> = r<sup>2</sup>
> 也就是说，在一元回归里，决定系数 R<sup>2</sup> 等于x和用之间的相关系数的平方

b. 多元回归中，在考虑是否要加入新的自变量时，需要对R<sup>2</sup>进行调整： adjusted R<sup>2</sup>

- 如果R<sup>2</sup>不进行调整，其他条件不变时，自变量越多，R<sup>2</sup>越大

c.如果只是单纯计算多元回归的解释能力，不需使用adjusted R<sup>2</sup>，只用R<sup>2</sup>即可

<br><br>

##6）判别回归模型的解释能力 2：t 检验（t test）- 定性指标
<br><br>
**回归系数的t 检验：** 

**t = b<sub>1</sub>**（样本估计值）**/s<sub>b<sub>1</sub></sub>**（目标总体标准差，即样本标准差除以根号下样本量）  
**df = n - k - 1**

**置信区间（confidence interval）：**  
**b<sub>1</sub>** （样本估计值）**± t<sub>c</sub> b<sub>1</sub>**

<br><br>

## 7）判别回归模型的解释能力 3：F 检验（F test）- 定性指标
> whole model significance test 
>  
> 仅用于多元回归

原假设，所有的自变量系数都 = 0，方程不具有解释力

F = 平均回归平方和/平均残差平方和  
（mean square of regression/mean square of error）  
（ =（sum square of regression/k）/（sum square of error/（n - k - 1））

df1 = k  
df2 = n - k - 1

<br><br>

##8）虚拟变量（dummy variable）
> 定性的自变量

> 例如：男/女，有/无，初中/高中/大学

虚拟变量的 t 检验：  
其他条件相同，存在和不存在该虚拟变量是否存在明显差异

<br><br>

## 9）多元回归的第一种违反：异方差（homoscedasticity）
> 异方差：残差的方差不恒定

<br><br>
**定义：**

- 无条件异方差（残差方差不恒定，但和x的值无关）
- 有条件异方差（残差方差不恒定，但和x的值有关）

**影响：**  

- CFA中默认忽略无条件异方差的影响  
- 有条件异方差对回归的结果没有影响，对于斜率和截距的估计值是对的，但是t检验的结果不对

> * 在有条件异方差的影响下，人们会可能误把原本拟合不佳的回归模型误以为拟合合理（误以为有统计学显著性，但实际上不具有）  
> 
> * 因为在 t = b<sub>j</sub>（样本估计值）/s<sub>b<sub>j</sub></sub>（目标总体标准差，即样本标准差除以根号下样本量）中   
> 有条件异方差导致s<sub>b<sub>j</sub></sub>比实际要小，所以算出来的t比实际要大  
> 
> * 增加了第一类错误的概率（Type I error），拒绝了原本不应该拒绝的原假设

**检测：**  

1\. 残差散点图  
2\. 布鲁奇-培根检验(Breusch-Pagan test)  
如果BP检测不拒绝原假设，则不存在异方差（CFA里面的假设检验一般都是想要拒绝原假设，但是BP检验除外）

> * 公式BP = nR<sup>2</sup><sub>res</sub> （自变量和残差之间的回归方程的决定系数）  
> * df = k   
> * 这是一个X<sup>2</sup>卡方检验

**修正：** 

1. 稳健的标准物（robust standard errors）（CFA指定的方法）
1. 广义最小二乘法（CFA没有提到）

> 回顾之前提到的：有条件异方差导致sbj比实际要小
> 使用了稳健的标准物，用一个更合理的标准值，但是这样依然并不能改变残差的异方差问题，所以实际上治标不治本

<br><br>
## 10）多元回归的第二种违反：序列相关/自相关（Serial correlation/autocorrelation）
> 序列相关：前期的自变量的数值会影响后期的自变量数值

<br><br>
**定义：**

- 正序列相关（Positive serial correlation）
- 负序列相关（Negative serial correlation）

**影响：**

* 对回归系数没有影响
* 对斜率的t检验有影响

**检测：**

- 画出残差散点图
- 使用杜宾沃森检验（Durbin-Watson Test）

**杜宾沃森检验（Durbin-Watson Test）：**   
**0 ≤ DW ≈ 2(1-r) ≤ 4**  
（r <- 自相关系数）

通过查阅DW table可以获得两个数值，d<sub>L</sub> 和 d<sub>U</sub>



**修正：**  

**Hanson method:** 调整系数标准差

<br><br>

## 11）多元回归的第三种违反：多重共线性（Multicollinearity）
> 多重共线性：变量之间存在明显的相关关系

<br><br>
**定义：**相关系数的绝对值大于0.7

**检测：**  

a）检测方法1：

1. 所有的t检验都不拒绝原假设（= 模型拟合不足）
2. F拒绝原假设（= 模型拟合良好，与第一个检验矛盾）
3. R<sup>2</sup> > 0.7 （= 模型拟合良好，与第一个检验矛盾）

b）检测方法2：  
（CFA提到的方法）

自变量之间的相关系数的绝对值 > 0.7

**修正：**
移除一个或多个存在相关关系的系数

<br><br>
