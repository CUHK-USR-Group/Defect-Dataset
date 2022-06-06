# Defect-Dataset

Deep learning breakthrough stimulates new research trends in civil infrastructure inspection, whereas the lack of quality-guaranteed, human-annotated, free-of-charge, and publicly available defect datasets with sufficient amounts of data hinders the progress of deep learning in defect inspection. To boost research in deep learning-based defect inspection, we review and summarize 40 publicly available defect datasets, covering common defects in various types of buildings and infrastructures. The taxonomy of the datasets is proposed based on specific deep learning objectives (classification, segmentation, and detection). Clarifications are also made for each dataset regarding its corresponding data volume, data resolution, data source, defect categories covered, infrastructure types focused, material types targeted, algorithms adopted for validation, annotation levels, and context levels.

<img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Taxonomy.PNG">

As demonstrated in the above figure, the summarized defect datasets cover various types of infrastructure such as pavements, bridges, buildings, tunnels, and dams with different materials such as concrete, asphalt, steel, masonry, and wood. These datasets cover the most common defect types: crack, spalling, delamination, corrosion, and efflorescence. As to data types, most datasets utilize optical images, with IRT images, IE signals, and GPR signals as alternatives. Optical images are typically used to detect surface defects of the structure, while IRT images, IE signals, and GPR signals can reveal subsurface defects. Besides, these datasets vary in the level of image context information, i.e., the pixel level, object level, and scene level. The data contained in different datasets are collected via hand-held sensors, robotic platforms, or UAV platforms. Especially, it is promising to utilize the UAV platform with onboard sensors to conduct defect inspection and data collection in GPS-denied environment.

For more detailed description of the datasets, please refer to our paper (under review):

[Datasets and Processing Methods for Boosting Visual Inspection of Civil Infrastructure: A Comprehensive Review and Case Study on Crack Classification, Segmentation, and Detection](https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/CONBUILDMAT-S-22-06330%20(1).pdf)



## Classification-Oriented Defect Dataset

Dataset | Year | Structure Type | Number of Images |
--- | --- | --- | --- |
[GAPs-v1]() | 2017 | Pavement | 6.3 Million |
GAPs-v2 | 2019 | Pavement | 6.7 Million |
CBID | 2017 | Bridge | 1,028 |
Xu | 2019 | Bridge | 6,069 |
Philip | 2019 | Bridge | 3,607 |
KrakN | 2020 | Bridge | 16,114 |
DCTCD | 2021 | Bridge | 250 |
CCIC | 2018 | Building | 40,000 |
$\phi$-Net | 2020 | Building | 36,413 |
CSSC | 2017 | Bridge and Building | 89,287 |
SDNET-2018 | 2018 | Bridge, Building and Pavement | 56,092 |
Qurishee | 2020 | Not Clarified | 2,088 |

Sample images of above classification-oriented datasets are as follows:
<p align="center">
  <img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Classification_Sample_Images.png" width=35% height=35%>
</p>

## Segmentation-Oriented Defect Dataset

Dataset | Year | Structure Type | Number of Images |
--- | --- | --- | --- |
[Sylvie](https://drive.google.com/drive/folders/1mAzmUFpFguNng3457Ks73u5X87kfJxaU?usp=sharing) | 2011 | Pavement | 42 |
[CrackTree](https://drive.google.com/drive/folders/14ewFWnou0ZvyP9JMour3aiz0Zmc3R80x?usp=sharing) | 2012 | Pavement | 206 |
[AEL](https://drive.google.com/drive/folders/15GxhpIqdmed8q3B93KRYHhzdPHpFCId_?usp=sharing) | 2016 | Pavement | 68 |
[CFD](https://drive.google.com/drive/folders/1_PH9wFQJW_5hVnUm1xN1Xbxq3TxA1F_H?usp=sharing) | 2016 | Pavement | 118 |
[Crack500](https://drive.google.com/drive/folders/1rbGkFrIJJQ45qcFmrSoNoPfzG5yT0YYS?usp=sharing) | 2019 | Pavement | 3,368 |
[GAPs384](https://drive.google.com/drive/folders/1GpTNx7zCFbET264Ch_riqQQnfi0pEbIo?usp=sharing) | 2019 | Pavement | 384 |
[EdmCrack600](https://drive.google.com/drive/folders/1q5sXVdNruXR0ay5RU57_RYmHmgzNuAeO?usp=sharing) | 2020 | Pavement | 600 |
[GAPs-10m](https://drive.google.com/drive/folders/1bOEKVYA9i2Bx5HwNhpshK359mJuJhjdn?usp=sharing) | 2021 | Pavement | 20 |
[Highway-Crack](https://drive.google.com/drive/folders/1HyFDPPaacgsrPkMBwHhXwWL8Vtr8uabp?usp=sharing) | 2021 | Pavement | 5,275 |
[CCIC-600](https://drive.google.com/drive/folders/1hit2K12dL4s8O3qz_qA0xR2DYr1mEKz9?usp=sharing) | 2019 | Bridge | 600 |
[BCL](https://drive.google.com/drive/folders/1MkG3St6t7VjLf22IgniK3YsmIlrKgyRM?usp=sharing) | 2021 | Bridge | 11,000 |
[CCSSS](https://drive.google.com/drive/folders/1-o4nhqNonEChvYQ62B89r_WLSgZt52P3?usp=sharing) | 2021 | Bridge | 440 |
[LCW](https://drive.google.com/drive/folders/1SipN8W0yc0AU2Pf-fbLqXr8xtSsfmCCR?usp=sharing) | 221 | Bridge | 440 |
[DeepCrack](https://drive.google.com/drive/folders/1jPNGWTLYz_hYdn9KPwXHTg8MF6q8vTrb?usp=sharing) | 2019 | Building | 537 |
[Bai-2020](https://drive.google.com/drive/folders/1JnrU1eLBxl9EE3T2_e5J1W-pkzMaMm05?usp=sharing) | 2020 | Building | 853 |
[Masonry](https://drive.google.com/drive/folders/1PCZoszNupCU8IfzENF8uW7td66vWnNf3?usp=sharing) | 2021 | Building | 11,491 |
[Ren](https://drive.google.com/drive/folders/155TxDX7m68b7iokKIz2l_q2sPeXsTxLS?usp=sharing) | 2020 | Tunnel | 919 |
[Sandra (IRT)](https://drive.google.com/drive/folders/10c2lT-Q7E4FAabbEDqT5KCWbcfQe7UWs?usp=sharing) | 2020 | Dam | 517 |
[UAV75](https://drive.google.com/drive/folders/155TxDX7m68b7iokKIz2l_q2sPeXsTxLS?usp=sharing) | 2019 | Not Clarified | 75 |
[CSD](https://drive.google.com/drive/folders/1cwao5hZANp8m6_VA8_XhQP6-qh9ksQ1X?usp=sharing) | 2020 | Multiple | 11,298 |
[Bai-2021](https://drive.google.com/drive/folders/1cwao5hZANp8m6_VA8_XhQP6-qh9ksQ1X?usp=sharing) | 2021 | Building, Bridge | 2,229 |
[CCCD](https://drive.google.com/drive/folders/1cwao5hZANp8m6_VA8_XhQP6-qh9ksQ1X?usp=sharing) | 2021 | Multiple | 10,995 |

Sample images of above segmentation-oriented datasets are as follows:

<p align="center">
<img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Segmentation_Sample_Images.png" width=80% height=80%>
</p>

## Detection-Oriented Defect Dataset

Dataset | Year | Structure Type | Number of Images |
--- | --- | --- | --- |
[RDD-2020](https://drive.google.com/drive/folders/1cwao5hZANp8m6_VA8_XhQP6-qh9ksQ1X?usp=sharing) | 2020 | Pavement | 26,336 |
[Qurishee (IRT)](https://drive.google.com/drive/folders/1hD0XJ5Ao3FFgGuc2KwwXkb_yYPVt0M9b?usp=sharing) | 2020 | Pavement | 108 (IRT), 2620 (RGB) |
[PID](https://drive.google.com/drive/folders/1hD0XJ5Ao3FFgGuc2KwwXkb_yYPVt0M9b?usp=sharing) | 2020 | Pavement | 7,237 |
[CODEBRIM](https://drive.google.com/drive/folders/1hD0XJ5Ao3FFgGuc2KwwXkb_yYPVt0M9b?usp=sharing) | 2019 | Bridge | 1,590 |
[GC10-DET](https://drive.google.com/drive/folders/1_RFn8MT8RBYZVX5mzg0Gp-sRBEzB5vI6?usp=sharing) | 2020 | Industrial Plant | 3,570 |

Here, the RDD-2018 and RDD-2019 are omited.

Sample images of above detection-oriented datasets are as follows:

<p align="center">
<img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Detection_Sample_Images.png" width=40% height=40%>
</p>
