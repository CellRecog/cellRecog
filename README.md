# Trichomonas Vaginalis Segmentation in Microscope Images (MICCAI2022)
> Authors: Lin Li, Jingyi Liu, Shuo Wang, Xunkun Wang, and Tian-Zhu Xiang.   
> <a href="https://arxiv.org/abs/test" rel="nofollow"><img src="https://camo.githubusercontent.com/4398ed745cccb9198b5590f2d4799518bae17c2dca258419b9413789a2fd01c6/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f41727869762d50617065722d7265643f7374796c653d666c61742d737175617265" alt="ARXIV PAPER" data-canonical-src="https://img.shields.io/badge/Arxiv-Paper-red?style=flat-square" style="max-width: 100%;"></a>


## 1. Introducton

- In this work, we collect the first large-scale Microscopic Image dataset of Trichomonas Vaginalis, called ***TVMI3K***, which consists of 3,158 images covering Trichomonas of various appearances in diverse backgrounds, with high-quality annotations including object-level mask labels, object boundaries, and challenging attributes. 
- Besides, we propose a simple yet effective baseline, named ***TVNet***, to automatically segment Trichomonas from microscopic images. 



## 2. Dataset
![image](https://github.com/CellRecog/cellRecog/blob/main/Images/dataset.jpg)
Figure 1: Examples of our proposed TVMI3K. We provide different annotations, including object-level masks, object edges and challenging attributes. We use red boxes to mark Trichomonas and green boxes to mark leukocyte on images for better visualization. Leukocyte shows high similarity with Trichomonas.

TVMI3K datasets: [Download](https://zenodo.org/record/6545146#.YrcfCexBz7U)



## 3. Our Model

![image](https://github.com/CellRecog/cellRecog/blob/main/Images/tvnet.png) 
Figure 2: Overview of our proposed TVNet, which consists of high-resolution fusion (HRF) module and foreground-background attention (FBA) module. Refer to our paper for details.



## 4. Result

### 4.1 Quantitative Comparison

![image](https://github.com/CellRecog/cellRecog/blob/main/Images/res1.png)    
Table 1: Quantitative comparison on our TVMI3K dataset. The best scores are highlighted in bold.


### 4.2 Qualitative Comparison

![image](https://github.com/CellRecog/cellRecog/blob/main/Images/res.jpg)   
Figure 3: Visual comparison of different methods. Our method provides more accurate predictions than other competitors in various challenging scenarios.


### 4.3 Results Download

* Results of our TVNet. [Baidu Pan](https://pan.baidu.com/s/1LY6cNnNEL9Gi4m8UAFi_gw) (1let) [Google Drive](https://drive.google.com/file/d/1ize1Y702v655V2bBHMtiiMS48bl504BJ/view?usp=sharing)

* Performance of competing methods. [Baidu Pan](https://pan.baidu.com/s/1jwlQfScfSoBxFaq5kZ00dg) (0qv5) [Google Drive](https://drive.google.com/file/d/1qdBTRtTM10tKDMNwrSizrRF8wM2uyanf/view?usp=sharing)

## 5. Models & Evaluation

The models and source code are coming soon. 

For evaluation, we adopt 1) [PySODMetrics](https://github.com/lartpang/PySODMetrics) library and 2) [Dice and IoU](https://github.com/weijun88/SANet). They can also be found in ```Evaluation``` folder.






## 6. Citation
Please cite our paper if you find the work useful: 

```
@inproceedings{li2022TVS,
  title={Trichomonas Vaginalis Segmentation in Microscope Images},
  author={Li, Lin and Liu, Jingyi and Wang, Shuo and Wang, Xunkun and Xiang, Tian-Zhu},
  booktitle={International Conference on Medical Image Computing and Computer Assisted Intervention, MICCAI},
  year={2022}
}
```
If you have any questions about our paper, feel free to contact me via e-mail (ll198196@163.com).


