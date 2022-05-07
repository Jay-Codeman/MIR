# Musical-Instrument-Recognition-by-XGBoost
**这个库是自己的乐器识别方向的项目论文源码。**

### 数据集
本项目数据集采用开源数据集Medley-solos-DB。
* DOI：10.5281/zenodo.3464194
* URL：[Medley-solos-DB](https://zenodo.org/record/3464194#.Ymyk9ugza3D)
* 发布时间：September 29, 2019
### 代码部分
项目代码各部分如下：
* **Feature extraction：**用于提取音频特征，特征值保存到test.csv中。
* **Feature Description：**用于绘制图像，描述不同音色特征对乐器音色的表征程度。
* **Combined accuracy comparision：**用于对比不同域音频特征的选取对分类准确率的影响，以及不同分类模型的分类效果。

### 特征提取：
特征提取采用python开源库librosa。提取的特征包括：
##### 频域：
* 光谱质心（Spectral Centroid, SC）
* 光谱带宽（Spectral Spread, SS）
* 谱滚降（Roll-off）
* 谐波（Harmonic）

##### 时域：
* 过零率（Zero crossing rate）
* 均方根（Root Mean Square, RMS）

##### 倒谱域：
* 梅尔倒谱系数（Mel-Frequency Cepstral Coefficients, MFCC）
