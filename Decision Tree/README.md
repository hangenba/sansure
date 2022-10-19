# `决策树模型`

* 将`PreprocX.xlsx`文件作为输入，其大小为$103\times103$
* 将`relapse_label_103.dat`文件作为标签进行训练，大小$103\times 1$
* `ID3`、`C4.5`采用信息增益的算法中有对数运算，会增加时间开销，而使用基尼指数采用指数运算，其时间效率大约是对数运算的100倍。
* 设置了决策树的分类方法为基尼指数。
* 将整体拆分为`7:3`的数据进行训练和测试

# `第一次训练`

* 只设置了分类的方式，得到以下结果
* 训练集准确率: 1.0
* 测试集准确率: 0.5483870967741935
* 生成树的形状如下图：
* ![](https://raw.githubusercontent.com/hangenba/sansure/ylh/Decision%20Tree/images/DecisionTreeV1.svg)

# `第二次训练`

* 设置了分类的最小样本数为5，叶子节点所需的最少样本数为5，得到以下结果

* 训练集准确率: 0.7638888888888888 

* 测试集准确率: 0.6451612903225806

* 生成树的形状如下图：

  * ![](https://raw.githubusercontent.com/hangenba/sansure/ylh/Decision%20Tree/images/DecisionTreeV2.svg)

    