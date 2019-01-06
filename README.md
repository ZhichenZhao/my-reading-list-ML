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