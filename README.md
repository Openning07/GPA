# GPA
Online photography assistance, tailored for food photograph.

To support the research and applications that are related to image aesthetic assessment on food photos and calls for aesthetic-aware visual feature, we establish the first large-scale dataset, namely, **Gourmet Photography Dataset** (GPD).

For further details, please refer to our paper [[pdf](https://www.researchgate.net/profile/Kekai_Sheng3/publication/329329757_Gourmet_photography_dataset_for_aesthetic_assessment_of_food_images/links/5c0dc00c92851c39ebe1d0f9/Gourmet-photography-dataset-for-aesthetic-assessment-of-food-images.pdf)].

## Background
![HighQualityFoodPhotosIsObvious](http://chongyangma.com/publications/gp/2018_gp_thumbnail.jpg "真 * 秀色可餐")

## Overview
### Sources of food photos
We collect food photos from both the online photo-sharing websites (*e.g.*, Flickr, Pinterest, 500px, Pexels) and from several existing food categorization benchmarks (*e.g.*, Food-101, [[ChineseFoodNet](https://sites.google.com/view/chinesefoodnet/)]).

### Configuration of GPD

|  | Train | Test | Overall |
| :------: | :------: | :------: | :------: |
| Positive | 11,791 | 1,311 | 13,102 |
| Negative | 9,809 | 1,089 | 10,898 |
| Overall | 21,600 | 2,400 | 24,000 |

For the convenience of file transfer, we resize the images first, and then upload the resized images on *Google Drive*:
 * [[Positive Partition (Resized)](https://drive.google.com/open?id=1hQUtgNBXijFP1ET82AazlhxQ6Rz38DgY)]
 * [[Negative Partition (Resized)](https://drive.google.com/open?id=1vlPalmsrkHRUJ3razt4tR-V3w7FJGrqi)]

```
ACCESS TERMS 
Researcher has requested permission to use the GPD.
In exchange for such permission, Researcher hereby agrees to the following terms and conditions:
1. Researcher shall use the Database only for non-commercial research and educational purposes.
2. Researcher may provide research associates and colleagues with access to the Database provided that they first agree to be bound by these terms and conditions.
3. If Researcher is employed by a for-profit, commercial entity, Researcher's employer shall also be bound by these terms and conditions, and Researcher hereby represents that he or she is fully authorized to enter into this agreement on behalf of such employer.

```

#### NOTE
In order to support further research and make aesthetic-aware applications on food photos practical, we will enlarge the scale of GPD and enrich the information it contains (e.g., introduce some aesthetic-related attributes). Hence, your feedback means a lot to us. Let's together make GPD better, and create interesting applications based on it.

## Application of GPD
### Food Photograph Triage
![FoodPhotoTriage](https://github.com/Openning07/GPA/blob/master/TeaserOfSA2018.png "With the help of GPD, we can now enable AI to pick high-quality food photos automatically!")

When we train a CNN model (*e.g.*, VGG-16 or ResNet-18) on our proposed GPD dataset, we can equip AI with the ability to assess the visual aesthetic of food photos, and therefore make it possible to create several practical aesthetic-aware task scenarios in the specific domain of food photographs.

For quantitative analysis and comparisons, we conduct another generalization ability test experiment. We collect *825* food photos from *WeChat*, and invite *50* interviewees, who are qualified for the task of food image aesthetic assessment, and collect their responses on those *825* images. Based on their judgements, we can evaluate how the trained model perform on unseen food photos.

| Solution | V(S_{pos}) | V(S_{neg}) |
| :--- | :-----: | :-----: |
| Best | 75.5 | 83.9 |
| Random | 37.3 | 62.5 |
| Worst | 16.1 | 24.5 |
| Human (Expert) | 72.1 | 81.0 |
| ResNet-18 + AVA | 38.5 | 65.7 |
| ResNet-18 + GPD | 61.1 | 72.5 |

For further details and discussions of the table shown above, please refer to [[our paper](https://www.researchgate.net/profile/Kekai_Sheng3/publication/329329757_Gourmet_photography_dataset_for_aesthetic_assessment_of_food_images/links/5c0dc00c92851c39ebe1d0f9/Gourmet-photography-dataset-for-aesthetic-assessment-of-food-images.pdf)].

### Assistance in Food Image Generation
![AssistanceInFoodImageGeneration](https://github.com/Openning07/GPA/blob/master/HelpToDiminishBadCaseGeneration.png "TODO")

### Enhancement of food photos (Raw -> Better)
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

@inproceedings{sheng2018attention,
  title={Attention-based multi-patch aggregation for image aesthetic assessment},
  author={Sheng, Kekai and Dong, Weiming and Ma, Chongyang and Mei, Xing and Huang, Feiyue and Hu, Bao-Gang},
  booktitle={2018 ACM Multimedia Conference on Multimedia Conference},
  pages={879--886},
  year={2018},
  organization={ACM}
}
```

## Concate & Feedback
If you have any suggenstions about papers, feel free to mail me :)
 * Email : shengkekai_D@163.com (personal), saulsheng@tencent.com (company)
 * QQ contact : 2309310604
