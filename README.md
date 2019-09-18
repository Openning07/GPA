# GPA
Online photography assistance, tailored for food photograph.

For further details, please refer to our paper [[pdf](https://www.researchgate.net/profile/Kekai_Sheng3/publication/329329757_Gourmet_photography_dataset_for_aesthetic_assessment_of_food_images/links/5c0dc00c92851c39ebe1d0f9/Gourmet-photography-dataset-for-aesthetic-assessment-of-food-images.pdf)].

## Background
![HighQualityFoodPhotosIsObvious](http://chongyangma.com/publications/gp/2018_gp_thumbnail.jpg "真 * 秀色可餐")

## Overview
### Sources of food photos

### Configuration of GPD24K

|  | Train | Test | Overall |
| :------: | :------: | :------: | :------: |
| Positive | 11,791 | 1,311 | 13,102 |
| Negative | 9,809 | 1,089 | 10,898 |
| Overall | 21,600 | 2,400 | 24,000 |

For the convenience of file transfer, we resize the images first, and then upload the resized images on Google Drive:
 * [[Positive Partition (Resized)](https://drive.google.com/open?id=10VFCKLoEl3Qq10RiPW68SQ0HXMfXbcwS)]
 * [[Negative Partition (Resized)](https://drive.google.com/open?id=14rwugQ2nbpQRHN5ipyWKT7bLcAhTvIJq)]

## Application of GPD24K
### Food Photograph Triage
![FoodPhotoTriage](https://github.com/Openning07/GPA/blob/master/TeaserOfSA2018.png "With the help of GPD24K, we can now enable AI to pick high-quality food photos automatically!")

When we train a CNN model (*e.g.*, VGG-16 or ResNet-18) on our proposed GPD24 dataset, we can equip AI with the ability to assess the visual aesthetic of food photos, and therefore make it possible to create several practical aesthetic-aware task scenarios in the specific domain of food photographs.

For quantitative analysis and comparisons, we conduct another generalization ability test experiment. We collect *825* food photos from *WeChat*, and invite *50* interviewees, who are qualified for the task of food image aesthetic assessment, and collect their responses on those *825* images. Based on their judgements, we can evaluate how the trained model perform on unseen food photos.

| Solution | V(S_{pos}) | V(S_{neg}) |
| :--- | :--: | :--: |
| Best | x | x |
| Random | x | x |
| Worst | x | x |
| Human (Expert) | x | x |
| ResNet-18 + AVA | x | x |
| ResNet-18 + GPD24K | x | x |

### Online Food Photography Assistance
TODO

### Enhancement of food photos
![FoodPhotoEnhancement](https://github.com/Openning07/GPA/blob/master/FoodPhotoEnhancement_PlaceHolder.jpg "Much better than the original images, and save your time from the endless attempts with existing PS tools!")

TODO

## Citation
If you find this useful in your research, please consider citing:
```
@inproceedings{sheng2018gourmet,
  title={Gourmet photography dataset for aesthetic assessment of food images},
  author={Sheng, Kekai and Dong, Weiming and Huang, Haibin and Ma, Chongyang and Hu, Bao-Gang},
  booktitle={SIGGRAPH Asia 2018 Technical Briefs},
  pages={20},
  year={2018},
  organization={ACM}
}
```
