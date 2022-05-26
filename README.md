
# Security in Recommendation System Papers Collection
### Editor: Yuni LAI
This collection will includes attack and defense for recommendation system (RS). And also some general ideas that related.  

Contents:
- Attack
- Defense
- General
- Datasets

## Attack

| Type | Paper names | Link |
| ------ | ------ | ------|
|(ACM Computing Surveys '20) Survey|A Survey on Adversarial Recommender Systems: From Attack/Defense Strategies to Generative Adversarial Networks|https://dl.acm.org/doi/10.1145/3439729|
|(CIKM'19)|Data Poisoning Attacks on Cross-domain Recommendation|https://dl.acm.org/doi/abs/10.1145/3357384.3358116|
|<sup><font color=DarkViolet>1</font></sup>(Resys'19) GAN|Adversarial Attacks on an Oblivious Recommender|https://dl.acm.org/doi/10.1145/3298689.3347031|
|(IEEE TKDE'19) Adversarial Training|Adversarial Training Towards Robust Multimedia Recommender System|https://ieeexplore.ieee.org/document/8618394|
|<sup>2</sup>(WWW'20) Influence Function|Influence Function based Data Poisoning Attacks to Top-N Recommender Systems|https://arxiv.org/abs/2002.08025|
|(WWW'20) Reinforcement Learning|Practical Data Poisoning Attack against Next-Item Recommendation|https://dl.acm.org/doi/abs/10.1145/3366423.3379992|
|<sup>3</sup> (KDD'21) GAN & influence function|Triple Adversarial Learning for Influence based Poisoning Attack in Recommender Systems |https://dl.acm.org/doi/10.1145/3447548.3467335; https://github.com/Daftstone/TrialAttack |
|(RecSys'20) Iterative gradient descend | Revisiting Adversarially Learned Injection Attacks Against Recommender Systems| https://arxiv.org/abs/2008.04876; https://github.com/graytowne/revisit_adv_rec |
|(SIGIR'20) Reinforcement Learning|Adversarial Attacks and Detection on Reinforcement Learning-Based Interactive Recommender Systems|https://arxiv.org/abs/2006.07934|
|(SIGIR'20) |Data Poisoning Attacks against Differentially Private Recommender Systems|https://dl.acm.org/doi/abs/10.1145/3397271.3401301|
|(ICDE'20) Reinforcement Learning |PoisonRec:An Adaptive Data Poisoning Framework for Attacking Black-box Recommender Systems|https://ieeexplore.ieee.org/abstract/document/9101655|
|(KDD'21) Probabilistic generative model; EM and Gradient Descent|Data Poisoning Attack against Recommender System Using Incomplete and Perturbed Data|https://dl.acm.org/doi/abs/10.1145/3447548.3467233|
|<sup>4</sup>(Information Sciences 2021) GAN|Ready for Emerging Threats to Recommender Systems? A Graph Convolution-based Generative Shilling Attack|https://arxiv.org/abs/2107.10457|
|(CCS'21) Black-box|Reverse Attack: Black-box Attacks on Collaborative Recommendation|https://dl.acm.org/doi/abs/10.1145/3460120.3484805|
|<sup>5</sup>(ICDE'21)Copy-profile; reinforcement learning|Attacking Black-box Recommendations via Copying Cross-domain User Profiles|https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9458627|


**Deal with Unnoticeable**
| Notes | Anomaly Detection | Unnoticable strategy |
| ------ | ------ | ------|
|<sup>1</sup>| Rating distribution evalueated only, no detection alg. |Adversarial Training in GAN|
|<sup>2</sup> | Featrue extraction + SVM as anomaly detection | Filler item ratings ~ original distribution|
|<sup>3</sup>|Fraudulent action propagation|Adversarial Training in GAN|
|<sup>4</sup>|PCASelectUsers,SemiSAD, DegreeSAD|Adversarial Training in GAN|
|<sup>5</sup>|Featrue extraction + SVM as anomaly detection|Copy real profiles|




## Defense

| Type | Paper names | Link |
| ------ | ------ | ------|
|(ACM Computing Surveys '20) Survey|A Survey on Adversarial Recommender Systems: From Attack/Defense Strategies to Generative Adversarial Networks|https://dl.acm.org/doi/10.1145/3439729|
|(SIGIR'20) Based on user anomaly probability |GCN-Based User Representation Learning for Unifying Robust Recommendation and Fraudster Detection |https://arxiv.org/abs/2005.10150 ; https://github.com/zsjdddhr/GraphRfi |



## General
### Graph Anomaly Detection
Anomaly detection techniques can be employed in Defense models. Especially Graph anomaly detection (GAD) on Bipartite Graph. 

| Type | Paper names | Link |
| ------ | ------ | ------|
|Survey(2020)|Shilling attacks against collaborative recommender systems: a review|https://link.springer.com/content/pdf/10.1007/s10462-018-9655-x.pdf|
|Survey(2021)| A Comprehensive Survey on Graph Anomaly Detection with Deep Learning |https://arxiv.org/pdf/2106.07178.pdf|
|(UMUAI'09) PCASelectUsers; Unsupervised;Bipartite |Unsupervised strategies for shilling detection and robust collaborative filtering|https://link.springer.com/article/10.1007/s11257-008-9050-4|
|(RecSys’11) SemiSAD; Semi-Suppervised;Bipartite|Semi-SAD: Applying Semi-supervised Learning to Shilling Attack Detection|https://dl.acm.org/doi/pdf/10.1145/2043932.2043985|
|(ICDM'12) Mutual Dependency; Unsupervised; Bipartite|Detecting Anomalies in Bipartite Graphs with Mutual Dependency Principles|https://ieeexplore.ieee.org/document/6413905|
|(WWW'13) Feature extraction + naïve Bayes + EM Alg.; semi-supervised|Shilling attack detection utilizing semi-supervised learning method for collaborative recommender system|https://link.springer.com/content/pdf/10.1007/s11280-012-0164-6.pdf|
|*(IJCAI'15) Fraudulent action propagation; Supervised; Bipartite|Catch the Black Sheep: Unified Framework for Shilling Attack Detection Based on Fraudulent Action Propagation|https://dl.acm.org/doi/10.5555/2832581.2832585|
|(IEICE Trans Info Syst. '16) PopSAD; Supervised;Bipartite|Shilling Attack Detection in Recommender Systems via Selecting Patterns Analysis|https://www.jstage.jst.go.jp/article/transinf/E99.D/10/E99.D_2015EDP7500/_pdf/-char/en|
|(TIFS'17) Features extraction; supervised/unsupervised;|A Network-Based Spam Detection Framework for Reviews in Online Social Media|https://ieeexplore.ieee.org/document/7865975|
|(TKDD'17) Greedy Optimization;Unsupervised; Bipartite|Graph-Based Fraud Detection in the Face of Camouflage(FRAUDAR)|https://dl.acm.org/doi/10.1145/3056563|
|(CIKM'20)GNN; Supervised; Bipartite|Error-Bounded Graph Anomaly Loss for GNNs|https://dl.acm.org/doi/pdf/10.1145/3340531.3411979|
|(ICDE'21)Ensemble; Unsupervised; Bipartite; Subgraph anomaly detection|EnsemFDet: An Ensemble Approach to Fraud Detection based on Bipartite Graph|https://www.computer.org/csdl/proceedings-article/icde/2021/918400c039/1uGXnraYpck|

### Label Flipping Defense

| Type | Paper names | Link |
| ------ | ------ | ------|
|(ICDM'20) community-preserving; self-supervised|Adversarial Label-Flipping Attack and Defense for Graph Neural Networks|https://ieeexplore.ieee.org/document/9338299|

### Adversarial Training Defending against Poisoning Attack
| Type | Paper names | Link |
| ------ | ------ | ------|
|(ICLR'22 Submitted) ？？ |HOW TO ADVERSARIALLY TRAIN AGAINST DATA POISONING|https://arxiv.org/pdf/2102.13624.pdf|

## Datasets in Rcommendation system

| Type | Datasets Name | Link |
| ------ | ------ | ------|
|Reviews with helpfulness votes | Amazon movie reviews |  https://snap.stanford.edu/data/web-Movies.html ; http://deepyeti.ucsd.edu/jianmo/amazon/index.html |
|Datatset collection|Recommender Systems and Personalization Datasets| https://cseweb.ucsd.edu/~jmcauley/datasets.html |
|With anomaly labels on ratings|Yelp|https://github.com/zsjdddhr/GraphRfi -> Dataset; http://odds.cs.stonybrook.edu/yelpchi-dataset/|
|943 users on 1682 movies, no labels|MovieLens 100K Dataset|https://www.kaggle.com/datasets/prajitdatta/movielens-100k-dataset|
