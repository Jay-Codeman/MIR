# Musical-Instrument-Recognition-by-XGBoost
**This repository is the source code of our team's project for musical instrument recognition.**

### Dataset
We use the open source dataset Medley-solos-DB in this project.
* DOI：10.5281/zenodo.3464194
* URL：[Medley-solos-DB](https://zenodo.org/record/3464194#.Ymyk9ugza3D)
* Release time：September 29, 2019
* 
### Each part
The functions of each part of the folder are as follows:
* **Feature extraction：**Is used to extract audio features, and the feature values are saved to test.csv.
* **Feature Description：**用于绘制图像，描述不同音色特征对乐器音色的表征程度。
* **Combined accuracy comparision：**Is used to draw images to describe the degree to which different timbre characteristics characterize the timbre of an instrument.

### Feature Extraction:
We use the python open source library `librosa` to extract audio features.The extracted features include:
##### Frequency domain
* Spectral Centroid(SC)
* Spectral Spread(SS)
* Roll-off
* Harmonic

##### Time domain:
* Zero crossing rate
* Root Mean Square(RMS)

##### Cepstral domain:
* Mel-Frequency Cepstral Coefficients(MFCC)
