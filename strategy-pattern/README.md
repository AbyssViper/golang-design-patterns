# 策略模式

## 定义

> wiki: 策略模式作为一种软件设计模式，指对象有某个行为，但是在不同的场景中，该行为有不同的实现算法。比如每个人都要“交个人所得税”，但是“在美国交个人所得税”和“在中国交个人所得税”就有不同的算税方法.

特点:
 - 定义了一族算法（业务规则）
 - 封装了每个算法
 - 这族的算法可互换代替（interchangeable）

策略模式，和其他设计模式的优点相同，都是为了解耦。 可以让客户端自行选择某一行为要使用的策略，我们可以针对不同的情况，来使用不同的策略（方式不同，但是目的相同，这也是第三个特点，算法族中的算法可互相替换）。

## 类图

![](https://gss1.bdstatic.com/-vo3dSag_xI4khGkpoWK1HF6hhy/baike/c0%3Dbaike72%2C5%2C5%2C72%2C24/sign=3c1919f176094b36cf9f13bfc2a517bc/5366d0160924ab189a9f061935fae6cd7b890b16.jpg)

(图源百度百科)

由一个策略接口，从接口延伸出一个策略族，由上下文`Context`来调用策略族中的具体策略

## 举个栗子
