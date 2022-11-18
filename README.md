
# Security in Recommendation System Papers Collection
### Editor: Yuni LAI
This collection will includes attack and defense for recommendation system (RS). And also some general ideas that related.  

Contents:
- Surveys
- Attack
- Defense
- General
- Datasets

## Surveys
| Time | Paper names | Link |
| ------ | ------ | ------|
|(2020)|A Survey on Adversarial Recommender Systems: From Attack/Defense Strategies to Generative Adversarial Networks|[paper](https://dl.acm.org/doi/10.1145/3439729)|
|(2022)|Threats to Training: A Survey of Poisoning Atacks and Defenses on Machine Learning Systems|[paper](https://dl.acm.org/doi/pdf/10.1145/3538707)|
|(2022)|Adversarial Recommender Systems: Attack, Defense, and Advances|[paper](https://link.springer.com/chapter/10.1007/978-1-0716-2197-4_9)|
|(2022)|A Comprehensive Survey on Trustworthy Recommender Systems|[paper](https://arxiv.org/pdf/2209.10117.pdf)|
|(2022)|Latest trends of security and privacy in recommender systems: A comprehensive review and future perspectives|[paper](https://www.sciencedirect.com/science/article/pii/S0167404822001419)|
## Attack

| Type | Paper names | Link |
| ------ | ------ | ------|

|(CIKM'19)|Data Poisoning Attacks on Cross-domain Recommendation|[paper](https://dl.acm.org/doi/abs/10.1145/3357384.3358116)|
|<sup><font color=DarkViolet>1</font></sup>(Resys'19) GAN|Adversarial Attacks on an Oblivious Recommender|[paper](https://dl.acm.org/doi/10.1145/3298689.3347031)|
|<sup>2</sup>(WWW'20) Influence Function|Influence Function based Data Poisoning Attacks to Top-N Recommender Systems|[paper](https://arxiv.org/abs/2002.08025)|
|(WWW'20) Reinforcement Learning|Practical Data Poisoning Attack against Next-Item Recommendation|[paper](https://dl.acm.org/doi/abs/10.1145/3366423.3379992)|
|(RecSys'20) Iterative gradient descend | Revisiting Adversarially Learned Injection Attacks Against Recommender Systems| [paper](https://arxiv.org/abs/2008.04876); [code](https://github.com/graytowne/revisit_adv_rec)|
|(SIGIR'20) Reinforcement Learning|Adversarial Attacks and Detection on Reinforcement Learning-Based Interactive Recommender Systems|[paper](https://arxiv.org/abs/2006.07934)|
|(SIGIR'20) |Data Poisoning Attacks against Differentially Private Recommender Systems|[paper](https://dl.acm.org/doi/abs/10.1145/3397271.3401301)|
|(ICDE'20) Reinforcement Learning |PoisonRec:An Adaptive Data Poisoning Framework for Attacking Black-box Recommender Systems|[paper](https://ieeexplore.ieee.org/abstract/document/9101655)|
|(CIKM'20)|Attacking Recommender Systems with Augmented User Profiles|[paper](https://dl.acm.org/doi/abs/10.1145/3340531.3411884)|
|<sup>3</sup> (KDD'21) GAN & influence function|Triple Adversarial Learning for Influence based Poisoning Attack in Recommender Systems |[paper](https://dl.acm.org/doi/10.1145/3447548.3467335); [code](https://github.com/Daftstone/TrialAttack) |
|(KDD'21) Probabilistic generative model; EM and Gradient Descent|Data Poisoning Attack against Recommender System Using Incomplete and Perturbed Data|[paper](https://dl.acm.org/doi/abs/10.1145/3447548.3467233);[code](https://github.com/RUCAIBox/Recommendation-Attack-for-Partial-and-Perturbed-Data)|
|<sup>4</sup>(Information Sciences'21) GAN|Ready for Emerging Threats to Recommender Systems? A Graph Convolution-based Generative Shilling Attack|[paper](https://arxiv.org/abs/2107.10457)|
|(CCS'21) Black-box|Reverse Attack: Black-box Attacks on Collaborative Recommendation|[paper](https://dl.acm.org/doi/abs/10.1145/3460120.3484805)|
|<sup>5</sup>(ICDE'21)Copy-profile; reinforcement learning|Attacking Black-box Recommendations via Copying Cross-domain User Profiles|[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9458627)|
|(NDSS'21) rating score vector|Data Poisoning Attacks to Deep Learning Based Recommender Systems|[paper](https://arxiv.org/pdf/2101.02644.pdf);[code](https://github.com/MiracleHH/RecommPoison)|
|(TNNLS'22)|Shilling Black-Box Recommender Systems by Learning to Generate Fake User Profiles.|[paper](https://lihui.info/doc/TNNLS22.pdf);[code](https://github.com/XMUDM/ShillingAttack)|
|(WSDM '22)|PipAttack: Poisoning Federated Recommender Systems for Manipulating Item Promotion|[paper](https://dl.acm.org/doi/abs/10.1145/3488560.3498386?casa_token=USuNz00wkAUAAAAA:TEReQgIHFOR5zpi4QyZk9pm_1WiU1LNSy-LYAvDRtmvB0xGFBqmtCOhXpZmZv4QgiPO_G0PwpEkI)|
|(ACM TIST'22)|Gray-Box Shilling Attack: An Adversarial Learning Approach|[paper](https://dl.acm.org/doi/full/10.1145/3512352?casa_token=i8WwfBzvbM4AAAAA%3A8BYP0deZ9X46ybqqQAoNmzGdKEtuQmdk0ieIfh-_yLC7R3Zi_3YNtC2L6n9DW6UuviUuBFTBRSBx)|
|(KDD'22)|Knowledge-enhanced Black-box Attacks for Recommendations|[paper](https://dl.acm.org/doi/abs/10.1145/3534678.3539359?casa_token=o8mYvI3kovMAAAAA:891qkMp_5USTiJxnToTvFL3Cv7Bd12Fd5UqSM27ZdhLRB0gXoQ9I6CfwthbF8PxLqEaolrnUL3tT)|


**Deal with Unnoticeable**
| Notes | Anomaly Detection | Unnoticable strategy |
| ------ | ------ | ------|
|<sup>1</sup>| Rating distribution evalueated only, no detection alg. |Adversarial Training in GAN|
|<sup>2</sup> | Featrue extraction + SVM as anomaly detection | Filler item ratings ~ original distribution|
|<sup>3</sup>|Fraudulent action propagation (FAP)|Adversarial Training in GAN|
|<sup>4</sup>|PCASelectUsers,SemiSAD, DegreeSAD|Adversarial Training in GAN|
|<sup>5</sup>|Featrue extraction + SVM as anomaly detection|Copy real profiles|




## Defense

| Type | Paper names | Link |
| ------ | ------ | ------|
|(IEEE TKDE'19) Adversarial Training|Adversarial Training Towards Robust Multimedia Recommender System|[paper](https://ieeexplore.ieee.org/document/8618394)|
|(SIGIR'20) Based on user anomaly probability |GCN-Based User Representation Learning for Unifying Robust Recommendation and Fraudster Detection |[paper](https://arxiv.org/abs/2005.10150) ; [code](https://github.com/zsjdddhr/GraphRfi)|
|(SPAI'20)|The Majority Rule: A General Protection on Recommender System|[paper](https://dl.acm.org/doi/10.1145/3385003.3410923)|
|(SIGIR'21)* Adversarial Poisoning Training|Fight Fire with Fire: Towards Robust Recommender Systems via Adversarial Poisoning Training |[paper](https://dl.acm.org/doi/10.1145/3404835.3462914)|
|(ICAICA'21) Struc2Vec|User embedding-based approach for detecting group shilling attacks|[paper](https://ieeexplore.ieee.org/document/9497956)|
|(ICAICA'21) Dual-input CNN|Detecting group shilling attacks in recommender systems based on maximum dense subtensor mining|[paper](https://ieeexplore.ieee.org/document/9498095)|
|(FIT'22)|DefenseNet-A Resilent Network Against Adverserail Attacks On Recommendation Systems|[paper](https://ieeexplore.ieee.org/abstract/document/9701380)|
|(Neurocomputing'22)|A deep learning based trust- and tag-aware recommender system|[paper](https://www.sciencedirect.com/science/article/pii/S0925231221017410)|
|(SIGIR'22)Implicit feedback|Self-Guided Learning to Denoise for Robust Recommendation|[paper](https://arxiv.org/abs/2204.06832)|
|(JCDL'22)Causal features; Distributional shifts|Causal Factorization Machine for Robust Recommendation|[paper](https://dl.acm.org/doi/abs/10.1145/3529372.3530921)|
|(ACM TOIS'22)|Towards Robust Neural Graph Collaborative Filtering via Structure Denoising and Embedding Perturbation|[paper](https://dl.acm.org/doi/abs/10.1145/3568396)|
|(CIKM'22) sensitivity study|Rank List Sensitivity of Recommender Systems to Interaction Perturbations|[paper](https://dl.acm.org/doi/abs/10.1145/3511808.3557425)|
|(TIFS'22)|Three Birds With One Stone: User Intention Understanding and Influential Neighbor Disclosure for Injection Attack Detection|[paper](https://ieeexplore.ieee.org/abstract/document/9693911?casa_token=RN8HT_MiB3gAAAAA:xWAT4bkkWkbzYjlld0l63rLleBsQh1x3bVB8LuLfOwoYiRtAFbTAIpdNPR-TDIOWMIkZjl6E)|
|(WISE'22)|Towards Robust Recommender Systems via Triple Cooperative Defense|[paper](https://link.springer.com/chapter/10.1007/978-3-031-20891-1_40)|

## General
### Graph Anomaly Detection
Anomaly detection techniques can be employed in Defense models. Especially Graph anomaly detection (GAD) on Bipartite Graph. 

| Type | Paper names | Link |
| ------ | ------ | ------|
|Survey(2020)|Shilling attacks against collaborative recommender systems: a review|[paper](https://link.springer.com/content/pdf/10.1007/s10462-018-9655-x.pdf)|
|Survey(2021)| A Comprehensive Survey on Graph Anomaly Detection with Deep Learning |[paper](https://arxiv.org/pdf/2106.07178.pdf)|
|(UMUAI'09) PCASelectUsers; Unsupervised;Bipartite |Unsupervised strategies for shilling detection and robust collaborative filtering|[paper](https://link.springer.com/article/10.1007/s11257-008-9050-4)|
|(RecSys’11) SemiSAD; Semi-Suppervised;Bipartite|Semi-SAD: Applying Semi-supervised Learning to Shilling Attack Detection|[paper](https://dl.acm.org/doi/pdf/10.1145/2043932.2043985)|
|(ICDM'12) Mutual Dependency; Unsupervised; Bipartite|Detecting Anomalies in Bipartite Graphs with Mutual Dependency Principles|[paper](https://ieeexplore.ieee.org/document/6413905)|
|(WWW'13) Feature extraction + naïve Bayes + EM Alg.; semi-supervised|Shilling attack detection utilizing semi-supervised learning method for collaborative recommender system|[paper](https://link.springer.com/content/pdf/10.1007/s11280-012-0164-6.pdf)|
|(IJCAI'15) (FAP) Fraudulent action propagation; Supervised; Bipartite|Catch the Black Sheep: Unified Framework for Shilling Attack Detection Based on Fraudulent Action Propagation|[paper](https://dl.acm.org/doi/10.5555/2832581.2832585)|
|(IEICE Trans Info Syst. '16) PopSAD/DegreeSAD; Supervised;Bipartite|Shilling Attack Detection in Recommender Systems via Selecting Patterns Analysis|[paper](https://www.jstage.jst.go.jp/article/transinf/E99.D/10/E99.D_2015EDP7500/_pdf/-char/en)|
|(TIFS'17) Features extraction; supervised/unsupervised;|A Network-Based Spam Detection Framework for Reviews in Online Social Media|[paper](https://ieeexplore.ieee.org/document/7865975)|
|(TKDD'17) Greedy Optimization;Unsupervised; Bipartite|Graph-Based Fraud Detection in the Face of Camouflage(FRAUDAR)|[paper](https://dl.acm.org/doi/10.1145/3056563)|
|(CORR'18)OFD;Supervised;Bipartite; Neural Random Forest; Autoencoder|Opinion Fraud Detection via Neural Autoencoder Decision Forest|[paper](https://arxiv.org/pdf/1805.03379.pdf)|
|*(WSDM'18) Fairness&Reliability; Supervised/Unsupervised;Bipartite;|REV2: Fraudulent User Prediction in Rating Platforms|[paper](https://dl.acm.org/doi/pdf/10.1145/3159652.3159729)|
|(CIKM'20)GNN; Supervised; Bipartite|Error-Bounded Graph Anomaly Loss for GNNs|[paper](https://dl.acm.org/doi/pdf/10.1145/3340531.3411979)|
|(ICDE'21)Ensemble; Unsupervised; Bipartite; Subgraph anomaly detection|EnsemFDet: An Ensemble Approach to Fraud Detection based on Bipartite Graph|[paper](https://www.computer.org/csdl/proceedings-article/icde/2021/918400c039/1uGXnraYpck)|
|(ICAICA'21)Bipartite;Struc2Vec|User embedding-based approach for detecting group shilling attacks|[paper](https://ieeexplore.ieee.org/document/9497956)|
|(ICAICA'21)Bipartite;Dual-input CNN|Detecting group shilling attacks in recommender systems based on maximum dense subtensor mining|[paper](https://ieeexplore.ieee.org/document/9498095)|

### Label Flipping Defense

| Type | Paper names | Link |
| ------ | ------ | ------|
|(ICDM'20) community-preserving; self-supervised|Adversarial Label-Flipping Attack and Defense for Graph Neural Networks|[paper](https://ieeexplore.ieee.org/document/9338299)|

### Adversarial Training Defending against Poisoning Attack
| Type | Paper names | Link |
| ------ | ------ | ------|
|(ICLR'22 Submitted) ？？ |HOW TO ADVERSARIALLY TRAIN AGAINST DATA POISONING|[paper](https://arxiv.org/pdf/2102.13624.pdf)|

## Datasets in Rcommendation system

| Type | Datasets Name | Link |
| ------ | ------ | ------|
|Reviews with helpfulness votes | Amazon movie reviews |  https://snap.stanford.edu/data/web-Movies.html ; http://deepyeti.ucsd.edu/jianmo/amazon/index.html |
|Datatset collection|Recommender Systems and Personalization Datasets| https://cseweb.ucsd.edu/~jmcauley/datasets.html |
|With anomaly labels on ratings|Yelp|https://github.com/zsjdddhr/GraphRfi -> Dataset; http://odds.cs.stonybrook.edu/yelpchi-dataset/|
|943 users on 1682 movies, no labels|MovieLens 100K Dataset|https://www.kaggle.com/datasets/prajitdatta/movielens-100k-dataset|
