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
