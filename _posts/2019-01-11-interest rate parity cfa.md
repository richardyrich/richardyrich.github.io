---
layout: post
title: 抛补平价：CFA笔记
categories: CFA
---

### a）抛补利率平价（covered interest rate parity）

<br><br>

投资期限为一年：
F<sub>(A/B)</sub> / S<sub>(A/B)</sub> = ( 1 + R<sub>A</sub> ) / ( 1 + R<sub>B</sub> )
投资期限小于一年：
F<sub>(A/B)</sub> / S<sub>(A/B)</sub> = ( ( 1 + R<sub>A</sub> ) ( Actual / 360 ) )/ ( ( 1 + R<sub>B</sub> ) ( Actual / 360 ) )

套利收益的计算（arbitrage profit）：

如果（1）F<sub>(A/B)</sub> / S<sub>(A/B)</sub> > ( 1 + R<sub>A</sub> ) / ( 1 + R<sub>B</sub> )
套利收益 = ( F<sub>(A/B)</sub> / S<sub>(A/B)</sub> ) × ( 1 + R<sub>B</sub> ) - ( 1 + R<sub>A</sub> )

如果（2）F<sub>(A/B)</sub> / S<sub>(A/B)</sub> < ( 1 + R<sub>A</sub> ) / ( 1 + R<sub>B</sub> )
套利收益 = ( S<sub>(A/B)</sub> / F<sub>(A/B)</sub> ) × ( 1 + R<sub>A</sub> ) - ( 1 + R<sub>B</sub> )


<br><br>

### b）无抛补利率平价（uncovered interest rate parity）
> 和抛补利率平价的区别是不存在远期合约

- E[S<sub>1(A/B)</sub>] / S<sub>0(A/B)</sub>   = ( 1 + R<sub>A</sub> ) / (1 + R<sub>B</sub> )
- 公式左边是其实是汇率变化，也就是说无抛补利率平价的结论是汇率变化等于利率变化：
%△E(S) = ( R<sub>A</sub> - R<sub>B</sub> )/ (1 + R<sub>B</sub> ) ≈ R<sub>A</sub> - R<sub>B</sub>

> 假设1 + R<sub>B</sub> 近似于 1

1. 无抛补利率平价的结论是汇率变化等于利率变化
2. 汇率变化的量近似于两个国家的利率差
3. 无抛补利率平价假设投资者风险中性（risk neutral）

> 投资海外存在汇率风险，而无抛补利率平价假设这位投资者不需要汇率风险溢价

<br><br>

### c）由 抛补利率平价 和 无抛补利率平价 得到的结论

<br><br>

1. 由抛补利率平价可算出不存在套利机会的汇率远期合约（no-arbitrage forward rate），由无抛补利率平价可以算出未来的即期汇率（expected future spot rate）
2. 抛补利率平价的假设是存在套利机制
3. 如果抛补利率平价和无抛补利率平价都成立，那么远期合约得价格是未来即期汇率是无偏预测（unbiased predictor）
**F = E(S<sub>1</sub>) → ( F - S<sub>0</sub> ) / S<sub>0</sub> = ( E(S<sub>1</sub>) - S<sub>0</sub> ) / S<sub>0</sub> → f = %△E(S) ≈ R<sub>A</sub> - R<sub>B</sub>**
4. 无抛补利率平价短期内不成立，但是长期成立