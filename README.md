# become-a-data-scientist
here meant to be the central place to keep a track of my learning course (codes, articles, papers, etc.) towards a real data scientist, some day...

#### Vector Space Model algorithms
##### Term Frequency * Inverse Document Frequency, Tf-Idf
> - It therefore converts integer-valued vectors into real-valued ones, while leaving the number of dimensions intact

##### Latent Semantic Indexing, LSI (or sometimes LSA)
> - transforms documents from either bag-of-words or (preferrably) TfIdf-weighted space into a latent space of a lower dimensionality
> - LSI training is unique in that we can continue “training” at any point, simply by providing more training documents
> - This is done by incremental updates to the underlying model, in a process called online training

##### Random Projections, RP
> - aim to reduce vector space dimensionality
> - This is a very efficient (both memory- and CPU-friendly) approach to approximating TfIdf distances between documents, by throwing in a little randomness
> - Recommended target dimensionality is again in the hundreds/thousands, depending on your dataset

##### Latent Dirichlet Allocation, LDA
> - yet another transformation from bag-of-words counts into a topic space of lower dimensionality
> - LDA is a probabilistic extension of LSA (also called multinomial PCA), so LDA’s topics can be interpreted as probability distributions over words
> - These distributions are, just like with LSA, inferred automatically from a training corpus
> - Documents are in turn interpreted as a (soft) mixture of these topics (again, just like with LSA)

##### Hierarchical Dirichlet Process, HDP
> - a non-parametric bayesian method (note the missing number of requested topics)

### Tutorials
source: [如何成为阿里巴巴算法工程师？](https://www.zhihu.com/question/23724645)
算法工程师，需要机器学习及其相关数学，以及特定方向（数据挖掘，自然语言处理，图像，语音等）的领域基础知识。
推荐的资料:
> - (a). 书籍：《统计学习方法》，《Pattern Recognition and Machine Learning》，《The Elements of Statistical Learning》，《凸优化》
> - (b). 视频教程：Andrew Ng的Coursera公开课《Machine Learning》，台湾大学林轩田的《机器学习基石》和《机器学习技法》，Stanford公开课 CS229 《Machine Learning》。
> - (c). 机器学习，数据挖掘等领域的顶级会议的paper。
