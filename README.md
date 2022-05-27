# BAFNet: Bottleneck Attention Based Fusion Network for Sleep Apnea Detection

## Abstract
Sleep apnea (SA) is a common sleep disorder that occurs during sleep, leading to the decrease of oxygen saturation in the blood. It would develop a variety of complications like diabetes, chronic kidney disease, depression, cardiovascular diseases, or even sudden death. Early SA detection can help physicians to take interventions for SA patients to prevent malignant events. This paper proposes a lightweight SA detection method of multi-scaled fusion network named SE-MSCNN based on single-lead ECG signals. The proposed SE-MSCNN mainly includes multi-scaled convolutional neural network (CNN) module and channel-wise attention module. In order to facilitate the SA detection performance, various scaled ECG information with different-length adjacent segments are extracted by three sub-neural networks. To overcome the problem of local concentration of feature fusion with concatenation, a channel-wise attention module with a squeeze-to-excitation block is employed to fuse the different scaled features adaptively. Furthermore, the ablation study and computational complexity analysis of the SE-MSCNN are conducted. Extensive experiment results show that the proposed SEMSCNN has the performance superiority to the state-of-the-art methods for SA detection on the Apnea-ECG benchmark dataset. The SE-MSCNN with the merits of quick response and lightweight parameters can be potentially embedded into a wearable device to provide an SA detection service for individuals in home sleep test (HST).
![img](pic/model_if.png)


## Dataset
[Apnea-ECG Database](https://physionet.org/content/apnea-ecg/1.0.0/)

## Usage

1. Get the pkl file
- Download the dataset Apnea-ECG Database
- Run [Preprocessing.py](Preprocessing.py) to get a file named apnea-ecg.pkl

2. Per-segment classification
- Run [MCAFNet.py](MCAFNet.ipynb)

3. Per-recording classification  
- Run [evaluate.py](utils/code_for_calculating_per-recording/evaluate.py)
- The performance is shown in [Table.csv](utils/code_for_calculating_per-recording/output/Table.csv)

## Cite
Not yet published
<!-- If our work is helpful to you, please cite: -->

## Email
If you have any questions, please email to: [xhchen@m.scnu.edu.cn](mailto:xhchen@m.scnu.edu.cn)
