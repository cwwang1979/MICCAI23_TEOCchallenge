# MICCAI23_TEOCchallenge

## Automated prediction of treatment effectiveness in ovarian cancer using histopathological images

## Introduction
Ovarian cancer is the second most common cause of gynecologic cancer death in women around the world. Epithelial ovarian cancer (EOC) accounts for over 95% of ovarian malignancies. Most women with ovarian cancer are diagnosed in advanced stage, which accounts for the high mortality rate. EOC is classified into at least five distinct histopathological subtypes, including high-grade serous, low-grade serous, clear cell, endometrioid, and mucinous ovarian cancer. High-grade serous ovarian cancer (HGSOC) is the most common histologic subtype, accounting for more than 70% of EOCs. Despite the progress made during the last two decades in the surgery and chemotherapy of ovarian cancer, more than 70 % of advanced patients are with recurrent cancer and decease. Bevacizumab is a humanized monoclonal antibody, which blocks VEGF signaling in cancer, inhibits angiogenesis and causes tumor shrinkage, and has been recently approved by FDA as a monotherapy for advanced ovarian cancer in combination with chemotherapy. Considering the cost, potential toxicity, and finding that only a portion of patients will benefit from these drugs, the identification of new predictive method for the treatment of EOC remains an urgent unmet medical need. Recent studies have shown that the challenge of applying digital whole slide image (WSI) to predict post-treatment response may be solved using deep learning (DL) technologies. Over the past few years, interest in the use of DL based approaches for drug discovery and development has increased. In this challenge, two datasets are constructed, including a whole section slide dataset and an independent TMA slide dataset. To assess the generalizability of the model, the whole section slide dataset will be used for training and the second independent TMA slide dataset will used for testing the DL based approaches. This challenge aims to build an automatic precision oncology system for patient selection and guiding ovarian cancer treatment.

## Date
- Open registration : currently open
- Training data release : available at [TCIA](https://doi.org/10.7937/tcia.985g-ey35) [1]
- Testing data release : will be available after the participant submits the [Registration Form](https://drive.google.com/file/d/1JRhSJRtDTcubmxrBThubmivysYHmQxpr/view?usp=share_link).
- Deadline for submission : August 30, 2023
the files to submit include a treatment outcome prediction file in the csv format (example shown in the table bellow and the file is available in the [link](https://drive.google.com/file/d/1fvyuJbpg6PyWJfGZb3qsZwEN4zIqLkBc/view?usp=share_link)) and a four-page paper about the methods in word or LaTex (template available at the [link](https://drive.google.com/drive/folders/1fiAdITZqX1lpImrINIwDbs0EtzUfV6rN?usp=share_link)).

| CoreID  | prediction (probability) | prediction(Binary [1:effective, 0: invalid] ) |
| :---         |     :---:      |          ---: |
| 0  | 0.75 | 1 |
| 1  | 0.6 | 1 |
| 2  | 0.25 | 0 |



## Datasets
### Training Cohorts
A large whole section whole slide image (WSI) dataset, contains 288 De-identified hematoxylin and eosin (H&E) stained whole section slides with clinical information of HGSOC patients collected from the tissue bank of the Tri-Service General Hospital and the National Defense Medical Center, Taipei, Taiwan. The large training dataset has been accepted to be stored on The Cancer Imaging Archive (TCIA) platform, and the dataset presented here is available at [the training data link](https://doi.org/10.7937/tcia.985g-ey35) [1].

### Testing Cohorts
180 tissue cores collected of HGSOC patients are collected from the tissue bank of the Tri-Service General Hospital and the National Defense Medical Center, Taipei, Taiwan. In order to test the model generalizability on unseen data, an independent and separate testing data set is provided for evaluation of models on not only sensitivity and specificity, but also on generalizability for practical usages. The data link will be released after submitting the [Registration Form](https://drive.google.com/file/d/1JRhSJRtDTcubmxrBThubmivysYHmQxpr/view?usp=share_link).

### Ethics Approval
For both training and testing datasets, ethical approvals have been obtained from the research ethics committee of the Tri-Service
General Hospital (TSGHIRB No.1???107???05???171 and No.B202005070).

## Organizers
- Prof. Ching-Wei Wang
Professor, Graduate Institute of Biomedical Engineering and Graduate Institute of Applied Science and Technology,
National Taiwan University of Science and Technology, Taipei, Taiwan.
Chair of a grand challenge for tissue microarray analysis in thyroid cancer diagnosis, IEEE International Symposium
on Biomedical Imaging (ISBI) 2017, Australia.
Chair of Grand Challenges in Dental X-ray Image Analysis, IEEE International Symposium on Biomedical Imaging
(ISBI) 2015, New York, USA.
Chair of the Grand Challenge - Automatic Cephalometric X-Ray Landmark Detection, IEEE International
Symposium on Biomedical Imaging (ISBI) 2014, Beijing, China.
- Dr. Tai-Kuang Chao
Chief, Department of Pathology, Tri-Service General Hospital, Taipei, Taiwan.
Associate Professor, College of Biochemistry, National Defense Medical Center, Taipei, Taiwan.
Director, Biobank, Tri-Service General Hospital and National Defense Medical Center
- Dr. Yi-Jia Lin
Attending Physician, Department of Pathology, Tri-Service General Hospital, Taipei, Taiwan.

## Challenge Publication and Prizes
Top-ranked teams will be invited for SCI journal publications and awarded the prizes below. 

A joint challenge paper will be prepared and submitted to journals such as Medical Image Analysis or IEEE trans on Medical Imaging, and two members from the top 10 participating teams from the leaderboards will be invited to contribute to the joint challenge paper as co-authors. 

In addition, two special Issues of the SCI-indexed journals with associated prizes (22,000 CHF in total) have been arranged for the TEOC challenge as follows. Top teams will be invited for paper submission to the arranged special issues.

The participating teams may publish their own results separately after the challenge paper is published, **but they should cite the assigned papers listed bellows**.

### Assigned Papers
- Wang et al. (2022) Histopathological whole slide image dataset for classification of treatment effectiveness to ovarian cancer, Scientific Data, 9(25), 1-5
https://doi.org/10.1038/s41597-022-01127-6
- Wang et al. (2022) Weakly Supervised Deep Learning for Prediction of Treatment Effectiveness on Ovarian Cancer from Histopathology Images, Computerized Medical Imaging and Graphics, 99.102093,1-26
https://doi.org/10.1016/j.compmedimag.2022.102093
- Wang et al. (2022) A weakly supervised deep learning method for guiding ovarian cancer treatment and identifying an effective biomarker, Cancers 14(7):1651
https://doi.org/10.3390/cancers14071651
- Wang et al. (2023) Ensemble biomarkers for guiding anti???angiogenesis therapy for ovarian cancer using deep learning, Clinical and Translational Medicine, 13(1), e1162, 1-7
https://doi.org/10.1002/ctm2.1162

### BibTeX
```
@article{wang2022histopathological,
  title={Histopathological whole slide image dataset for classification of treatment effectiveness to ovarian cancer},
  author={Wang, Ching-Wei and Chang, Cheng-Chang and Khalil, Muhammad Adil and Lin, Yi-Jia and Liou, Yi-An and Hsu, Po-Chao and Lee, Yu-Ching and Wang, Chih-Hung and Chao, Tai-Kuang},
  journal={Scientific Data},
  volume={9},
  number={1},
  pages={25},
  year={2022},
  publisher={Nature Publishing Group UK London}
}
@article{wang2022weakly,
  title={Weakly supervised deep learning for prediction of treatment effectiveness on ovarian cancer from histopathology images},
  author={Wang, Ching-Wei and Chang, Cheng-Chang and Lee, Yu-Ching and Lin, Yi-Jia and Lo, Shih-Chang and Hsu, Po-Chao and Liou, Yi-An and Wang, Chih-Hung and Chao, Tai-Kuang},
  journal={Computerized Medical Imaging and Graphics},
  volume={99},
  pages={102093},
  year={2022},
  publisher={Elsevier}
}
@article{wang2022weakly,
  title={A weakly supervised deep learning method for guiding ovarian cancer treatment and identifying an effective biomarker},
  author={Wang, Ching-Wei and Lee, Yu-Ching and Chang, Cheng-Chang and Lin, Yi-Jia and Liou, Yi-An and Hsu, Po-Chao and Chang, Chun-Chieh and Sai, Aung-Kyaw-Oo and Wang, Chih-Hung and Chao, Tai-Kuang},
  journal={Cancers},
  volume={14},
  number={7},
  pages={1651},
  year={2022},
  publisher={MDPI}
}
@article{wang2023ensemble,
  title={Ensemble biomarkers for guiding anti-angiogenesis therapy for ovarian cancer using deep learning},
  author={Wang, Ching-Wei and Lee, Yu-Ching and Lin, Yi-Jia and Chang, Chun-Chieh and Wang, Chih-Hung and Chao, Tai-Kuang and others},
  journal={Clinical and Translational Medicine},
  volume={13},
  number={1},
  year={2023},
  publisher={Wiley-Blackwell}
}
```

### Special Issues and the Prizes
Special Issues for the TEOC challenge:
1. Cancers (JCR 2021 IF = 6.575) Special Issue "Computational Pathology for Breast Cancer and Gynecologic Cancer"
2. Diagnostics (JCR2021 IF= 3.992) "Special Issue "Deep Learning in Oncological Image Analysis"

Prizes (in total 22000 CHF)

- 1st place, 2900 CHF (Swiss Francs) / 100% wavier Voucher and invited for publication in the special issue of Cancers (JCR 2021 IF = 6.575)
- 2nd place, 1450 CHF (Swiss Francs) / 50% wavier Voucher and invited for publication in the special issue of Cancers (JCR 2021 IF = 6.575)
- 3rd place, 1450 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Cancers (JCR 2021 IF = 6.575)
- 4th place, 1450 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Cancers (JCR 2021 IF = 6.575)
- 5th place, 1450 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Cancers (JCR 2021 IF = 6.575)
- 6th place, 1450 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Cancers (JCR 2021 IF = 6.575)
- 7th place, 1450 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Cancers (JCR 2021 IF = 6.575)
- 8th place, 1300 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 9th place, 1300 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 10th place, 1300 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 11th place, 1300 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 12th place, 1300 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 13th place, 1300 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 14th place, 260 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 15th place, 260 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 16th place, 260 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 17th place, 260 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 18th place, 260 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 19th place, 260 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 20th place, 260 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 21st place, 260 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 22nd place, 260 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)
- 23rd place, 260 CHF (Swiss Francs) Voucher and invited for publication in the special issue of Diagnostics (JCR2021 IF= 3.992)

## License
The challenge materials are released under a creative commons license, which allows for personal and research use only. For a commercial license please contact Prof Ching-Wei Wang. You can view a license summary here:  
http://creativecommons.org/licenses/by-nc/4.0/


## Contact
Prof. Ching-Wei Wang  
  
cweiwang@mail.ntust.edu.tw; cwwang1979@gmail.com  
  
National Taiwan University of Science and Technology

## Reference
[1] Wang et al. (2022) Histopathological whole slide image dataset for classification of treatment effectiveness to ovarian cancer, Scientific Data, 9(25), 1-5
https://doi.org/10.1038/s41597-022-01127-6
