# Multiclass Datasets for Anomaly Detection
*This file includes new multi-class datasets for anomaly detection tasks which have been used in previous literature, for our current anomaly detection project.*     

*🧑🏻‍🚀 represent my current coding status on that dataset.*


## 1. Numerical / Image Datasets
#### 1.1. [Retinal OCT Images](https://www.kaggle.com/paultimothymooney/kermany2018) [🧑🏻‍🚀: almost ready for training]
- **format**: images
- **volume**: 84K images in total
- **no. of labeled classes**: 1 normal class and 3 abnormal classes
- **papers using the data**: [kermany et al, 2018](https://www.cell.com/cell/fulltext/S0092-8674(18)30154-5), [Suzuki and Suzuki, 2020](https://arxiv.org/abs/2001.05859v5), [Seeböck et al, 2019](https://arxiv.org/abs/1905.12806v1), [Waldstein et al, 2020](https://www.nature.com/articles/s41598-020-69814-1).

#### 1.2. [UCI Cardiotocography Dataset](https://www.kaggle.com/propanon/uci-cardiotocography) [🧑🏻‍🚀: preprocessing for training]
- **format**: descriptive (numerical) records, 36 features per record
- **volume**: 2126 records in total
- **no. of labeled classes**: 10 (morphologic patterns) or 3 (fetal states) classes in total
- **papers using the data**: [Campos et al, 2016](http://dx.doi.org/10.1007/s10618-015-0444-8) ([results](https://www.dbs.ifi.lmu.de/research/outlier-evaluation/DAMI/semantic/Cardiotocography/))

#### 1.3. [UCI Pageblock Dataset](https://archive.ics.uci.edu/ml/datasets/Page+Blocks+Classification) [🧑🏻‍🚀: preprocessing for data]
- **format**: numerical records, 10 features per records
- **volume**: 4913 text class, 329 horiz. line class, 28 graphic class, 88 vert. line class, 115 picture class
- **no. of labeled classes**: 1 normal class (text) and 4 abnormal classes
- **papers using the data**: [Campos et al, 2016](http://dx.doi.org/10.1007/s10618-015-0444-8) ([results](https://www.dbs.ifi.lmu.de/research/outlier-evaluation/DAMI/semantic/PageBlocks/))

#### 1.4. [UNSW-NB15](https://www.unsw.adfa.edu.au/unsw-canberra-cyber/cybersecurity/ADFA-NB15-Datasets/) [Anomaly Dataset](https://www.kaggle.com/mrwellsdavid/unsw-nb15) [🧑🏻‍🚀: preprocessing for data]
- **format**: descriptive records, 49 features (processed from raw network data) per record
- **volume**: 250K records in total
- **no. of labeled classes**: 1 normal class and 9 abnormal classes (*e.g.* exploits, fuzzers, DoS, etc.)
- **papers using the data**: [Pang et al, 2020](https://arxiv.org/abs/2009.06847v1), [Moustafa et al, 2016](https://www.tandfonline.com/doi/abs/10.1080/19393555.2015.1125974)

#### 1.5 [COVID-19 Radiography Database](https://www.kaggle.com/tawsifurrahman/covid19-radiography-database) [🧑🏻‍🚀: preprocessing for data]
- **format**: images
- **volume**: 1.3K normal images, 1.2K COVID-19 positive images, and 1.3K viral pneumonia images
- **no. of labeled classes**: 1 normal class and 2 abnormal classes
- **papers using the data**: [Chowdhury et al, 2020](https://arxiv.org/abs/2003.13145)



## 2. Video Datasets
#### 2.1. [AUC Distracted Driver Dataset](https://abouelnaga.io/projects/auc-distracted-driver-dataset/) [🧑🏻‍🚀: waiting for access to data]
*Note: I've sent request forms to the authors and am still waiting for the access.*
- **format**: image (extracted from videos), 1080x1920 pixels per image
- **volume**: 17K images in total
- **no. of labeled classes**: 1 normal class and 9 abnormal classes

#### 2.2. [UCF Crime Dataset](https://webpages.uncc.edu/cchen62/dataset.html) [🧑🏻‍🚀: preparing dataset]
*Note: this dataset is in video format, and is super large (>20GB), making it a lot harder to process with our image-based anomaly detection framework.*
- **format**: videos
- **volume**: 1900 videos in total (>128 hours)
- **no. of labeled classes**: 1 normal class and 13 abnormal classes

*Note: Though the following datasets may contain multiple subtypes of anomalies, they do not have separate labels for each subtype. Also, the abnormality often occur on a specific object or motion, which usually requires object localization / optical flow analysis before detection, which is incompatible with our current anomaly detection frameworks and may introduce unnecessary artifacts. Thus, I decided to discard the following datasets for now.*
#### 2.3. [UCSD Anomaly Detection Dataset](http://www.svcl.ucsd.edu/projects/anomaly/dataset.htm) [🧑🏻‍🚀: not intend to use]
- **format**: image (extracted from videos), 234×159 pixels per image
- **volume**: 3K images for anomalies and 5K images for normal
- **no. of labeled classes**: 1 normal class and 1 abnormal class

#### 2.4. [CUHK Avenue Dataset for Abnormal Event Detection](http://www.cse.cuhk.edu.hk/leojia/projects/detectabnormal/dataset.html) [🧑🏻‍🚀: not intend to use]
- **format**: image (extracted from videos), 640×360 pixels per image
- **volume**: 30K images in total
- **no. of labeled classes**: 1 normal class and 1 abnormal class (with 47 unlabeled subtypes)

#### 2.5. [ShanghaiTech Campus Pedastrain Dataset](https://svip-lab.github.io/dataset/campus_dataset.html) [🧑🏻‍🚀: not intend to use]
- **format**: image (extracted from videos), 856×480 pixels per image
- **volume**: 400 videos in total
- **no. of labeled classes**: 1 normal class and 1 abnormal class

#### 2.6. [Street Scene Anomaly Dataset](https://www.merl.com/demos/video-anomaly-detection) [🧑🏻‍🚀: not intend to use]
- **format**: image (extracted from videos), 1280×720 pixels per image
- **volume**: 200K images in total
- **no. of labeled classes**: 1 normal class and 17 abnormal classes (*p.s.* anomalies are only annotated in bounding boxes; a single image frame may contain multiple anoamlies)



## Additional Notes
Besides the above new datasets mentioned, I have also used the following datasets. Their status and explanations for why or why not to use them are also described below:
- **Datasets in use**:
    - [FashionMNIST](https://github.com/zalandoresearch/fashion-mnist)
    - [UCI Satimage](https://www.openml.org/d/182)
    - [Spectrum](https://github.com/ZIYU-DEEP/Anomaly-Detection-for-Spectrum)
- **Datasets attempted but discarded**:
    - [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html): No downward bias found due to lack of classes with close proximity (*e.g.* `top` and `shirt` in FashionMNIST), thus we do not observe downward bias.
    - [ImageNet](https://gist.github.com/yrevar/942d3a0ac09ec9e5eb3a): No significant downward bias found for now (*p.s.* only semi-supervised trained on a few selected classes), and the training takes too long while the test results are a bit unstable.
    - [MNIST](http://yann.lecun.com/exdb/mnist/): No significant downward bias found for now (*p.s.* only tested the case when digit `7` is set to be normal) found for now. Plus, experiments on this dataset is considered when we already have FashionMNIST.
    - [Drivers' Anomaly Dataset](https://github.com/okankop/Driver-Anomaly-Detection): No significant downward bias found due to low detection rate in the unsupervised setting.
    - [UCI Covertype](https://www.openml.org/d/150): Weak downward bias found on other classes when training class 2 and class 4, but the problem is that this two classes are very *different* from each other, which is a bit inconsistent with our previous idea that downward bias is more likely to exist when training with two *similar* classes.
    - [UCI Shuttle](https://www.openml.org/d/40685): Found consistent (though weak) downward bias on One-Class models, but the training for reconstruction models are quite unstable with loss explosion problem.
    - [KDDCup99](http://odds.cs.stonybrook.edu/http-kddcup99-dataset/): No downward bias found for now (*p.s.* only semi-supervised trained on a few selected classes with sufficient data).
    - [Phish URL](https://www.openml.org/d/42641): No downward bias found. The abnormal classes (*e.g.* `spam`, `malware`, `phishing`) are similar to each other, such that semi-supervised training on one sub-class can effectively improve detection performance on others'.
    - [Gas Drift](https://www.openml.org/d/1476): Loss explosion problem exists on both One-Class and Reconstruction models.
    - [AWID](http://icsdweb.aegean.gr/awid/features.html): Loss explosion problem exists on both One-Class and Reconstruction models.
