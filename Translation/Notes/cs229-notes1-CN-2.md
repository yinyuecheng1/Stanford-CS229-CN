原文：http://cs229.stanford.edu/notes/cs229-notes1.pdf  
翻译：[MIL Learning Group](https://github.com/milLearningGroup/Stanford-CS229-CN) - [你的GitHub ID](#对应链接地址)

# Part II 分类与逻辑回归（Classification and logistic regression）

现在让我们来讨论一下分类问题。这和回归问题很类似，不过我们现在想要预测的 $y$ 值是数量很少的一些离散值。首先，我们把目光放在 **二分类（binary classification）** 问题上，也即是说 $y$ 只有两种取值可能，0 或者 1 。（而我们提到的分类问题大多数时候是推广到多类别情形下的。）例如，如果我们想要建立一个垃圾邮件分类器，那么 $x^{(i)}$ 可能是一封邮件的某些特征，$y$ 为1则表示这是一封垃圾邮件，为0则表示不是。在这里，0也被称为 **负类（negative class）** ，1也被称为 **正类（postive class）** ，他们有时候也会用符号 “+” 和 “-” 来定义。给定 $x^{(i)}$ ，则对应的 $y^{(i)}$ 也被称作这个训练样本的 **标签（label）** 。

## 5 Logistic 回归（Logistic regression）

>  注：Logistic 回归的中文译法当前主要有“逻辑回归”和“逻辑斯蒂回归”两种，这里保留了英文原名，希望大家能够认出。

我们可以通过忽略 $y$ 是一个离散值从而解决分类问题，也即是使用原始的线性回归算法尝试在给定 $x$ 的情况下预测 $y$ 。然而，很容易用例子证明这样的方法是不靠谱的。从直觉上看，当我们知道 $y\in\{0,1\}$ 时，预测值 $h_\theta(x)$ 如果超过 1 或者小于 0 ，也就没有了意义。  

为了满足我们的需求，我们将改变假设 $h_\theta(x)$ 的形式，选择下面的函数：  

$$ h_\theta(x)=g(\theta^Tx)=\frac {1}{1+e^{-\theta^Tx}}$$

其中 $g(z)=\frac {1}{1+e^{-z}}$ 被称为



## 6 Digression: The perceptron learning algorithm



## 7 Another algorithm for maximizing ℓ(θ)

