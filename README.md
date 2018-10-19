# Waterbro's Reading List on Machine Learning

### Factorization Machines, ICDM, 2010
* 一个特别适用于onehot特征应用场景的因子分解机，适合广告点击率预测，推荐系统等业务。
* 它与线性分类模型的最大区别在于善于处理稀疏数据，由于进行了分解，不同点之间的关系可以通过v的内积的形式传递。
* 文章中提到的分解是cholesky分解，为了保证矩阵正定，本身可以让对角元变得足够大。


### Field-aware Factorization Machines for CTR Prediction, RecSys, 2016
* 在FM的基础上给了一个field，这个field主要解决的问题就是原来每个元素只有唯一的v，两个看起来没什么关联的field还是只能用这个来相乘，但是如果变成fv个，f是field数量，那用专门的field的v去乘就好了。


