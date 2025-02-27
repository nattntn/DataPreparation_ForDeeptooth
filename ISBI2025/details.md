# Data

|   Age   |   Number of images   |   Accuracy  |
|:-------:|:--------------------:|:-----------:|
|   7     |         50           |   84.00%    |
|   8     |         48           |   85.42%    |
|   9     |         50           |   82.00%    |
|   10    |         49           |   83.67%    |
|   11    |         50           |   82.00%    |
|   12    |         48           |   79.17%    |
|   13    |         50           |   80.00%    |
|   14    |         47           |   68.09%    |
|   15    |         51           |   82.35%    |
|   16    |         50           |   90.00%    |
|   17    |         51           |   96.08%    |
|   18    |         50           |   96.00%    |
|  19     |         49           |   95.92%    |
|  20     |         49           |   95.92%    |
|  21     |         50           |   92.00%    |
|  22     |         49           |   94.00%    |
|  23     |         50           |   98.00%    |
|  24     |         51           |   94.12%    |
|  25     |         50           |   80.00%    |

|   Age   |     Sex       |   Number of images  |
|:-------:|:-------------:|:-------------------:|
|  7      |  Female       |         25          |
|  7      |  Male         |         25          |
|  8      |  Female       |         26          |
|  8      |  Male         |         22          |
|  9      |  Female       |         26          |
|  9      |  Male         |         24          |
|  10     |  Female       |         25          |
|  10     |  Male         |         24          |
|  11     |  Female       |         24          |
|  11     |  Male         |         26          |
|  12     |  Female       |         23          |
|  12     |  Male         |         25          |
|  13     |  Female       |         25          |
|  13     |  Male         |         25          |
|  14     |  Female       |         25          |
|  14     |  Male         |         22          |
|  15     |  Female       |         26          |
|  15     |  Male         |         25          |
|  16     |  Female       |         25          |
|  16     |  Male         |         25          |
|  17     |  Female       |         25          |
|  17     |  Male         |         26          |
|  18     |  Female       |         25          |
|  18     |  Male         |         25          |
|  19     |  Female       |         24          |
|  19     |  Male         |         25          |
|  20     |  Female       |         25          |
|  20     |  Male         |         24          |
|  21     |  Female       |         25          |
|  21     |  Male         |         25          |
|  22     |  Female       |         25          |
|  22     |  Male         |         25          |
|  23     |  Female       |         25          |
|  23     |  Male         |         25          |
|  24     |  Female       |         26          |
|  24     |  Male         |         25          |+
|  25     |  Female       |         25          |
|  25     |  Male         |         25          |

# Upper Canine
| **upper cannine** | Negative (569) |              |Positive (557)  |              |
|:-----------------:|:--------------:|:------------:|:--------------:|:------------:|
| **Sex**           |**Female (273)**|**Male (296)**|**Female (264)**|**Male (293)**|
|      Correct      |       233      |     257      |       224      |     254      |
|     Incorrect     |       40       |     39       |       40       |     39       |
|    Age correct    |                |              |                |              |
|   Age incorrect   |                |              |                |              |

# data SHAP YOLO ภาพ original
[Colab](https://colab.research.google.com/drive/17xrR2P9VTEYq7zstCFRPQZudOc5VLJIT?authuser=0#scrollTo=4BvXrVng8Hpy&uniqifier=1)
```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025 #path

# ผล SHAP+YOLO+ผลการทำนาย ผู้หญิง 1-prob **negative**
final_result_gender_negative_bboxes.csv

# ผล SHAP+YOLO+ผลการทำนาย ผู้หญิง 1-prob **positive**
final_result_gender_positive_bboxes.csv

# data ที่ label region of Upper Canine
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/merge_result_UpperCanine_dataset.csv
```

## code
```
#ย้าย folder จากpc  ไป server
scp -r ./{folder name} natt@10.177.191.29:/media/tohn/HDD/Natdata/Tooth_data/Data_Label/.
scp -r ./Gender_ISBI2025 natt@10.177.191.29:/media/tohn/HDD/Natdata/Tooth_data/.
```

```
# path data original of test cut images (943 images)
/media/tohn/HDD/Natdata/Tooth_data/Data_Label/ #path
7Y
.
.
.
25Y
```
```
#ผลการทำนาย 943 ภาพ
/content/gdrive/MyDrive/Tooth_Shap_GPT/Deep_tooth/Model/Multi_task(Age)(7-25)/Table_test_Predict.csv
pd.read_csv('/media/tohn/HDD/Natdata/Tooth_data/Table/Result_Predict/Table_test_Predict.csv') 

# ผล SHAP+YOLO+ผลการทำนาย ผู้หญิง 1-prob **positive**
pd.read_csv (r'/content/gdrive/My Drive/Tooth_Shap_GPT/Deep_tooth/OPG_SHAPer/Result_ALL/final_result_gender_positive_bboxes.csv')

# ผล SHAP+YOLO+ผลการทำนาย ผู้หญิง 1-prob **negative**
pd.read_csv (r'/content/gdrive/My Drive/Tooth_Shap_GPT/Deep_tooth/OPG_SHAPer/Result_ALL/final_result_gender_negative_bboxes.csv')

```
# Threshold 15-9-2567
## path data
```
# negative ตาม threshold
## correct
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/Neg_correct_male_UC_90percent.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/Neg_correct_male_UC_55percent.csv

## incorrect
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/Neg_incorrect_male_UC_10percent.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/Neg_incorrect_male_UC_45percent.csv


# positive ตาม threshold
## correct
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/Pos_correct_male_UC_90percent.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/Pos_correct_male_UC_55percent.csv


## incorrect
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/Pos_incorrect_male_UC_10percent.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/Pos_incorrect_male_UC_45percent.csv
```
## path data scale x
```
# negative ตาม threshold
## correct
### correct 95% (232*43=9976)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/neg_cor_scale_x.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_neg_cor_scale_x.csv

### correct 55% (3*43=129)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/neg_cor55_scale_x.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_neg_cor55_scale_x.csv


## incorrect
### incorrect 5% (22*43=946)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/neg_incor_scale_x.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_neg_incor_scale_x.csv

### incorrect 45% (3*43=129)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/neg_incor45_scale_x.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_neg_incor45_scale_x.csv




# positive
## correct
### correct 95% (230*43=9890)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/pos_cor_scale_x.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_pos_cor_scale_x.csv

### correct 55% (3*43=129)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/pos_cor55_scale_x.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_pos_cor55_scale_x.csv

## incorrect
### incorrect 5% (22*43=946)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/pos_incor_scale_x.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_pos_incor_scale_x.csv

### incorrect 45% (3*43=129) 
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/pos_incor45_scale_x.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_pos_incor45_scale_x.csv
```

## path data scale y
```
# negative ตาม threshold
## correct
### correct 95% (232*43=9976)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/neg_cor_scale_y.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_neg_cor_scale_y.csv

### correct 55% (3*43=129)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/neg_cor55_scale_y.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_neg_cor55_scale_y.csv



## incorrect

### incorrect 5% (22*43=946)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/neg_incor_scale_y.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_neg_incor_scale_y.csv

### incorrect 45% (3*43=129)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/neg_incor45_scale_y.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_neg_incor45_scale_y.csv


# positive
## correct
### correct 95% (230*43=9890)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/pos_cor_scale_y.cs
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_pos_cor_scale_y.csv

### correct 55% (3*43=129)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/pos_cor55_scale_y.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_pos_cor55_scale_y.csv

## incorrect
### incorrect 5% (22*43=946)
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/pos_incor_scale_y.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_pos_incor_scale_y.csv

### incorrect 45%  (3*43=129) 
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/pos_incor45_scale_y.csv
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/predict_pos_incor45_scale_y.csv

```


