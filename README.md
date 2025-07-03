# MFC
Multi-Feature Combined Cloud and Cloud Shadow Detection

Rebuild and redirected from [https://sendimage.whu.edu.cn/en/mfc](https://sendimage.whu.edu.cn/en/mfc)


**Introduction**

The wide field of view (WFV) imaging system onboard the Chinese GaoFen-1 (GF-1) optical satellite has a 16-m resolution and four-day revisit cycle for large-scale Earth observation. The advantages of the high temporal-spatial resolution and the wide field of view make the GF-1 WFV imagery very popular. However, cloud cover is an inevitable problem in GF-1 WFV imagery, which influences its precise application. Accurate cloud and cloud shadow detection in GF-1 WFV imagery is quite difficult due to the fact that there are only three visible bands and one near-infrared band.

In this paper, an automatic multi-feature combined (MFC) method is proposed for cloud and cloud shadow detection in GF-1 WFV imagery. The MFC algorithm first implements threshold segmentation based on the spectral features and mask refinement based on guided filtering to generate a preliminary cloud mask. The geometric features are then used in combination with the texture features to improve the cloud detection results and produce the final cloud mask. Finally, the cloud shadow mask can be acquired by means of the cloud and shadow matching and follow-up correction process. The method was validated using 108 globally distributed scenes. The results indicate that MFC performs well under most conditions, and the average overall accuracy of MFC cloud detection is as high as 96.8%. In the contrastive analysis with the official provided cloud fractions, MFC shows a significant improvement in cloud fraction estimation, and achieves a high accuracy for the cloud and cloud shadow detection in the GF-1 WFV imagery with fewer spectral bands. The proposed method could be used as a preprocessing step in the future to monitor land-cover change, and it could also be easily extended to other optical satellite imagery which has a similar spectral setting.

<br>

**Method**

**Li, Z., Shen, H., Li, H., Xia, G., Gamba, P., & Zhang, L. (2017). [Multi-feature combined cloud and cloud shadow detection in GaoFen-1 wide field of view imagery](https://zhiweili.net/assets/pdf/2017.3_RSE_Multi-feature%20combined%20cloud%20and%20cloud%20shadow%20detection%20in%20GaoFen-1%20wide%20field%20of%20view%20imagery.pdf). *Remote Sensing of Environment*, 191, 342-358.**

![img](https://raw.githubusercontent.com/dr-lizhiwei/MFC/main/Flowchart.jpg)Fig. 1. Overall framework of the MFC algorithm

<br>

**Example results**

![img](https://raw.githubusercontent.com/dr-lizhiwei/MFC/main/barren.gif)

![img](https://raw.githubusercontent.com/dr-lizhiwei/MFC/main/forest.gif)

![img](https://raw.githubusercontent.com/dr-lizhiwei/MFC/main/urban.gif)

<br>

**Download Links**

- **GF1_WHU**: Gaofen-1 WFV Cloud and Cloud Shadow Detection Dataset ([Link](https://github.com/dr-lizhiwei/GF1_WHU))
- MFC cloud and cloud shadow detection tool ([MFC_CCSD_Tool_V1.0](https://github.com/dr-lizhiwei/MFC/raw/main/MFC_CCSD_Tool_V1.0.zip))
