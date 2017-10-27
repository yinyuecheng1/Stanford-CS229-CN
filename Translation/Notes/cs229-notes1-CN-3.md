原文：http://cs229.stanford.edu/notes/cs229-notes1.pdf  
翻译：[MIL Learning Group](https://github.com/milLearningGroup/Stanford-CS229-CN) - [San-greal](https://San-greal.github.io)

# Part III 广义线性模型(Generalized Linear Models)

到目前为止，我们已经看到了一个回归和一个分类的例子。在这个回归的例子中，我们有y|x ～ N($\mu$,$\sigma^{2}$),而在这个分类的的例子中，有y|x；$\theta$  ～ 布鲁尼(Bernoulli)($\phi$)，对于$\mu$和$\phi$的一些适当的定义可以作为函数的x和$\theta$ 。在这一节中，我们将展示这两种方法的更为广泛的家族模型的特殊情况，其称为广义线性模型（GLMS）。我们还将教授如何使用在GLM家族中的其他模型，并将他们应用于其他的分类与回归问题



## 8 The exponential family



## 9 Constructing GLMs



### 9.1 Ordinary Least Squares



### 9.2 Logistic Regression



### 9.3 Softmax Regression