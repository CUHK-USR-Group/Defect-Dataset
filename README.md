## Our Self-Established Defect Detection Dataset: CUBIT-Det
We establish the first high-resolution dataset tailored for large-scale infrastructure defect detection, named CUBIT-Det (To be uploaded soon). The dataset comprises 5,527 visible images with a maximum resolution of $8000\times6000$ captured by the onboard cameras of the UAVs. The dataset covers the three most ubiquitous types of infrastructure, including building (65\%), pavement (29\%), and bridge (6\%), and targets for inspecting the three most critical types of surface defect, including crack (82\%), spalling (12\%), and moisture (6\%). The high-resolution images are collected from different viewpoints and distances under various illumination conditions, inherently offering more structure context information and model robustness for real-world inspection.

Image Resolution | Year | Structure Type | Number of Images | Defect Type | Annotation Level
--- | --- | --- | --- | --- | --- |
4624x3472, 8000x6000 | 2023 | Building, Pavement, Bridge | 5527 | Crack, Spalling, Moisture | Bounding-box Level

The sample images from the CUBIT-Det dataset have been showed below. The first row is crack on building surfaces and the second row includes crack on pavements (first and second column) and bridges (third and forth column). The third row is spalling and the forth is moisture.

<p align="center">
<img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Sample_Images/CUBIT-Det_Sample_Images.png" width=60% height=60%>
</p>



## [Our Self-Collected Defect Segmentation Dataset: CUBIT-Seg](https://drive.google.com/drive/folders/1ea4YqIa9mfldCLWFquAKJXnCB3QzbgId?usp=sharing)

Except for CUBIT-Seg, we also construct a pixel-level annotated defect dataset, CUBIT-Seg, for the segmentation task of common defects in building facades. We utilize UAVs and DSLRs for data collection in Hong Kong, then clean the data to remove duplicate and low-quality images, then label the rest of images pixel-by-pixel, and finally crop the images into 512x512 resolution. CUBIT-Seg contains 1160 images for spalling segmentation and 5462 images for crack segmentation.

Image Resolution | Year | Structure Type | Number of Images | Defect Type | Annotation Level
--- | --- | --- | --- | --- | --- |
512x512 | 2023 | Building | 1160 | Spalling | Pixel Level
512x512 | 2023 | Building | 5462 | Crack | Pixel Level

The sample images from the CUBIT-Seg dataset have been showed below:

<p align="center">
<img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Sample_Images/CUBIT-Seg_Sample_Images.png" width=100% height=100%>
</p>



## Visual Defect Datasets from Existing Works


To further boost research in deep learning-based defect inspection, we review and summarize **40 publicly available defect datasets**, covering common defects in various types of infrastructure. **The taxonomy of the datasets** is proposed based on **specific deep learning objectives** (classification, segmentation, and detection). Clarifications are also made for each dataset regarding its corresponding **data volume, data resolution, data source, defect categories covered, infrastructure types focused, material types targeted, algorithms adopted for validation, annotation levels, and context levels**.

<img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Sample_Images/Taxonomy.PNG">

As demonstrated in the above figure, the summarized defect datasets cover various types of infrastructure such as pavements, bridges, buildings, tunnels, and dams with different materials such as **concrete, asphalt, steel, masonry, and wood**. These datasets cover the most common defect types: **crack, spalling, delamination, corrosion, and efflorescence**. As to data types, most datasets utilize optical images, with **IRT images, IE signals, and GPR signals as alternatives**. Optical images are typically used to detect surface defects of the structure, while IRT images, IE signals, and GPR signals can reveal subsurface defects. Besides, these datasets vary in the level of image context information, i.e., the pixel level, object level, and scene level. The data contained in different datasets are collected via hand-held sensors, robotic platforms, or UAV platforms. Especially, it is promising to utilize the UAV platform with onboard sensors to conduct defect inspection and data collection in GPS-denied environment. For more detailed description of the datasets, please refer to our [review](http://www.mae.cuhk.edu.hk/~bmchen/papers/2022_CBM.pdf).

We have noticed a multi-modal defect dataset for subsurface defect detection, [SDNET-2021](https://commons.und.edu/data/19/), which contains 1,936 annotated IE signals, over 663,102 annotated GPR signals and 5 mosaic annotated IRT images containing about 4,580,680 annotated pixels collected during 2020 summer from 5 in-service bridge decks in Grand forks, ND, USA. 

Here, we concentrate on **VISUAL** defect datasets.

For ***downloading*** the dataset and corresponding reference papers, just click the name of corresponding dataset in the table below.

### Classification-Oriented Defect Dataset

Dataset | Year | Structure Type | Number of Images |
--- | --- | --- | --- |
[GAPs-v1](https://drive.google.com/drive/folders/1M_L4qxJpmaRq2QEjrEstibRYwzWwXCO4?usp=sharing) | 2017 | Pavement | 6.3 Million |
[GAPs-v2](https://drive.google.com/drive/folders/1PAs3kZ5dHkrWuwnyyFoyn0v99w7k6dAB?usp=sharing) | 2019 | Pavement | 6.7 Million |
[CBID](https://drive.google.com/drive/folders/1pW6mo5kmsfiVNmbbDo4EPuLUKwLLpelt?usp=sharing) | 2017 | Bridge | 1,028 |
[Xu](https://drive.google.com/drive/folders/1Qe0KJKscIvJO829cYwVr-LYYrst0eVD-?usp=sharing) | 2019 | Bridge | 6,069 |
[Philip](https://drive.google.com/drive/folders/1AL6lld2XAU7QTUl7FDFWABiQIBWk5QdZ?usp=sharing) | 2019 | Bridge | 3,607 |
[KrakN](https://drive.google.com/drive/folders/1pW2mF4BY-Hj2cCcbppx6RZeZTnw3L3Ob?usp=sharing) | 2020 | Bridge | 16,114 |
[DCTCD](https://drive.google.com/drive/folders/1grbTcdUZr98nFnu65Es3x9rk70N9s3Vj?usp=sharing) | 2021 | Bridge | 250 |
[CCIC](https://drive.google.com/drive/folders/14ecYMTBf8uZV4B27i4dgod1wpZ6RKHgH?usp=sharing) | 2018 | Building | 40,000 |
[Phi-Net](https://pan.baidu.com/s/15hiPmDU7OYiYlJIO801xmg?pwd=0520) | 2020 | Building | 36,413 |
[CSSC](https://pan.baidu.com/s/1yZcAdtVOaHUr7NAwQAsthA?pwd=0520) | 2017 | Bridge and Building | 89,287 |
[SDNET-2018](https://pan.baidu.com/s/1kbwFM3KTdTH_5QCvVCazuw?pwd=0520) | 2018 | Bridge, Building and Pavement | 56,092 |
[Qurishee](https://pan.baidu.com/s/1uq_au2f8Ok2Gxwskn9nd5Q?pwd=0520) | 2020 | Not Clarified | 2,088 |
| | | Total | 13,250,948

Sample images of above classification-oriented datasets are as follows:
<p align="center">
  <img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Sample_Images/Classification_Sample_Images.png" width=100% height=100%>
</p>

### Segmentation-Oriented Defect Dataset

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
[LCW](https://drive.google.com/drive/folders/1SipN8W0yc0AU2Pf-fbLqXr8xtSsfmCCR?usp=sharing) | 2021 | Bridge | 440 |
[DeepCrack](https://drive.google.com/drive/folders/1jPNGWTLYz_hYdn9KPwXHTg8MF6q8vTrb?usp=sharing) | 2019 | Building | 537 |
[Bai-2020](https://drive.google.com/drive/folders/1JnrU1eLBxl9EE3T2_e5J1W-pkzMaMm05?usp=sharing) | 2020 | Building | 853 |
[Masonry](https://drive.google.com/drive/folders/1PCZoszNupCU8IfzENF8uW7td66vWnNf3?usp=sharing) | 2021 | Building | 11,491 |
[Ren](https://drive.google.com/drive/folders/155TxDX7m68b7iokKIz2l_q2sPeXsTxLS?usp=sharing) | 2020 | Tunnel | 919 |
[Sandra (IRT)](https://drive.google.com/drive/folders/10c2lT-Q7E4FAabbEDqT5KCWbcfQe7UWs?usp=sharing) | 2020 | Dam | 517 (IRT) |
[UAV75](https://drive.google.com/drive/folders/1pXOeEmD46bYKu4XMqxdeHC7_qE7vCxLZ?usp=sharing) | 2019 | Not Clarified | 75 |
[CSD](https://drive.google.com/drive/folders/1cwao5hZANp8m6_VA8_XhQP6-qh9ksQ1X?usp=sharing) | 2020 | Multiple | 11,298 |
[Bai-2021](https://drive.google.com/drive/folders/1b-OljHOhwBpNIsuEm2ZZ13-MAEIp4EXg?usp=sharing) | 2021 | Building, Bridge | 2,229 |
[CCCD](https://drive.google.com/drive/folders/1MwRyjB9_DtJ2mxkcXeU5NuM1YyLAj2oO?usp=sharing) | 2021 | Multiple | 10,995 |
| | | Total | 517 (IRT), 60,958 (RGB)

Sample images of above segmentation-oriented datasets are as follows:

<p align="center">
<img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Sample_Images/Segmentation_Sample_Images.png" width=100% height=100%>
</p>

### Detection-Oriented Defect Dataset

Dataset | Year | Structure Type | Number of Images |
--- | --- | --- | --- |
[RDD-2020](https://drive.google.com/drive/folders/1gTK_7kUCjOTkG7lzSqrlG3z3Ft1MJ3W7?usp=sharing) | 2020 | Pavement | 26,336 |
[Qurishee (IRT)](https://drive.google.com/drive/folders/16vjyhuDscyFkXUxAurGq-iRMQI6BqD4n?usp=sharing) | 2020 | Pavement | 108 (IRT), 2620 (RGB) |
[PID](https://drive.google.com/drive/folders/1hD0XJ5Ao3FFgGuc2KwwXkb_yYPVt0M9b?usp=sharing) | 2020 | Pavement | 7,237 |
[CODEBRIM](https://drive.google.com/drive/folders/12B2ongbzxMDzrpYAXlpQuvcxCjkX-RXN?usp=sharing) | 2019 | Bridge | 1,590 |
[GC10-DET](https://drive.google.com/drive/folders/1_RFn8MT8RBYZVX5mzg0Gp-sRBEzB5vI6?usp=sharing) | 2020 | Industrial Plant | 3,570 |
| | | Total | 108 (IRT), 41,353 (RGB)

Here, the RDD-2018 and RDD-2019 are omitted.

Sample images of above detection-oriented datasets are as follows:

<p align="center">
<img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Sample_Images/Detection_Sample_Images.png" width=45% height=45%>
</p>
