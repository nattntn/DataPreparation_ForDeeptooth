# Ratio จริง

👾ตารางรวมทุกผลการทำนายของทุกเพศ (จำนวน 762 row, ช: 465, ญ: 297)

```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Sex_UpperCanine_dataset_Ratio.csv
```

➡️ ตารางรวมผลการทำนาย กรณีตัวแบบทำนายถูก (จำนวน 662 row ช: 407, ญ: 255)  

```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Sex_correct_UpperCanine_dataset_Ratio.csv
```

➡️ ตารางรวมผลการทำนาย กรณีตัวแบบทำนายถูกด้วยความมั่นใจ 95% ขึ้นไป (จำนวน 586 แถว ช: 367 ญ: 219)  

```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Sex_correct95_UpperCanine_dataset_Ratio.csv
```

▶  ตารางรวมผลการทำนาย กรณีตัวแบบทำนายผิด  (จำนวน 100 row ช: 58, ญ: 42) (actual)
```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Sex_incorrect_UpperCanine_dataset_Ratio.csv
```

▶  ตารางรวมผลการทำนาย กรณีตัวแบบทำนายผิด  (จำนวน 100 row ช: 58, ญ: 42) (actual) ตารางรวมผลการทำนาย กรณีตัวแบบทำนายผิด  ความมั่นใจต่ำ [50-55%, 45-50) (จำนวน 5 row ช: 3, ญ: 2) (actual)
```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Sex_incorrect55_UpperCanine_dataset_Ratio.csv
```

# Adjusted data
1️⃣ Scale_X: All_data + new prediction (prediction after adjusted) (32766 row)

```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/Canine_Sex/predict_all_Predict_scale_x.csv
```
2️⃣ Scale_Y: All_data + new prediction (prediction after adjusted)
```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Data/Canine_Sex/predict_all_Predict_scale_y.csv
```

# SHAP_YOLO
## scale X
1️⃣ Positive: adjusted แล้วดูว่าตัวแบบสนใจบริเวณไหน

```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/Affine/Canine_Sex/SHAP_YOLO/all_predict_scaleX_positive_bboxes.csv
```

2️⃣ Negative: adjusted แล้วดูว่าตัวแบบสนใจบริเวณไหน

### Ratio หลังจากปรับภาพแล้วตัวแบบยังสนใจ upper canine 
1️⃣ Positive 695 จาก 762
```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/pos_all_prediction_after_adjusting_scaleX_UpperCanine_Ratio.csv
```
2️⃣ Negative: adjusted แล้วดูว่าตัวแบบสนใจบริเวณไหน

```
```
### Ratio หลังจากปรับภาพแล้วตัวแบบยังสนใจ upper canine กรณีภาพก่อนปรับทายถูก
1️⃣ Positive  611 (ช: 383 ญ:228) จาก 662  (ช: 407, ญ: 255) )
```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/pos_correct_prediction_after_adjusting_scaleX_UpperCanine_Ratio.csv
```

2️⃣ Negative

### Ratio หลังจากปรับภาพแล้วตัวแบบยังสนใจ upper canine กรณีภาพก่อนปรับทายถูก ที่ความมั่นใจ 95%  
1️⃣ Positive 550 (ช:352  ญ:198) จาก 586 (ช: 367 ญ: 219) 
```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/pos_correct95_prediction_after_adjusting_scaleX_UpperCanine_Ratio.csv
```
### Ratio หลังจากปรับภาพแล้วตัวแบบยังสนใจ upper canine กรณีภาพก่อนปรับทายผิด 
1️⃣ Positive 84 (ช: 50 , ญ:34) จาก (100 row ช: 58, ญ: 42) (actual)
```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/pos_incorrect_prediction_after_adjusting_scaleX_UpperCanine_Ratio.csv
```
2️⃣ Negative

### Ratio หลังจากปรับภาพแล้วตัวแบบยังสนใจ upper canine กรณีภาพก่อนปรับทายผิด มั่นใจต่ำ 55%
1️⃣ Positive 4 (ช: 2, ญ: 2) จาก 5 (ช: 3, ญ: 2)
```
/media/tohn/HDD/Natdata/Tooth_data/Gender_ISBI2025/pos_incorrect55_prediction_after_adjusting_scaleX_UpperCanine_Ratio.csv
```
2️⃣ Negative



