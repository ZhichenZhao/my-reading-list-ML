# Waterbro's Reading List on Machine Learning

### Factorization Machines, ICDM, 2010
* 一个特别适用于onehot特征应用场景的因子分解机，适合广告点击率预测，推荐系统等业务。
* 它与线性分类模型的最大区别在于善于处理稀疏数据，由于进行了分解，不同点之间的关系可以通过v的内积的形式传递。
* 文章中提到的分解是cholesky分解，为了保证矩阵正定，本身可以让对角元变得足够大。


### Field-aware Factorization Machines for CTR Prediction, RecSys, 2016
* 在FM的基础上给了一个field，这个field主要解决的问题就是原来每个元素只有唯一的v，两个看起来没什么关联的field还是只能用这个来相乘，但是如果变成fv个，f是field数量，那用专门的field的v去乘就好了。

### Optimized Cost per Click in Taobao Display Advertising, KDD, 2017
* 名词：revenue，（广告）收入，CPC，cost per click，OCPC，optimized cost per click。CPM，cost per mille，KPI，key performance indicators，ROI，return of investment,CTR，click-through rate，CVR，conversion rate.small and mediumsized
advertisers 
* 阿里的文章，如果只按照cpc收费是没有办法调整bid的，这篇文章提出了ocpc，使得价格是可以变动的，即保护了中小广告主不会被大广告主挤走，也给平台注入了更多活力

### Pricing of Online Advertising: Cost-per-Click-through vs. Cost-per-Action, HICSS,2010
* incentive contracts,激励性合约
* CPC转嫁了一部分风险在广告主这边，因为是否产生点击（在没有第三方监督的情况下）是平台说了算，而有没有买东西，有没有下载去转化，则是广告主说了算的。

### Hybrid Keyword Search Auctions, WWW, 2009
impression，在广告里面指的是“曝光”，“展示”，即一个广告被看到。
 banner advertisements，横幅标语广告。
 CPM对于平台风险最小，对广告主最大，CPA对于平台风险最大，对广告主最小。而CPC则介于两者之间，因而CPC是一个比较广泛使用的方式。在CPC中，平台只负责尽量优化其点击率，而广告主则根据落地页尽量优化转化率。


## Network Initialization
### Understanding the difficulty of training deep feedforward neural networks，ICAIS，2010
* 通过会线性网络的一些分析，得到了新的初始化方法，和前一层，这一层的神经元个数都有关系，从中可以推导出xarvier的均匀分布和高斯分布

## Learning to Rank (LTR)
### Learning to Rank using Gradient Descent，ICML，2005
* learning to rank这个领域的开山之作，使用神经网络来进行这一项任务。里面提到了要用sigmoid用作概率的表示，以及用BCE loss来进行ranking。

### Learning to Rank with Nonsmooth Cost Functions，NIPS，2006
* IR领域中一些常见的衡量指标：Mean Reciprocal Rank (MRR)，如果某个query的结果rank是r，那么平均所有的r分之一。Winner
Takes All (WTA)，只看第一个对不对





