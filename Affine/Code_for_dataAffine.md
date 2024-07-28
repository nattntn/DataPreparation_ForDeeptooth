# Data label upper 3 molar

|   Age   |   Number of images   |   Accuracy  |
|:-------:|:--------------------:|:-----------:|
|  19     |         49           |             |
|  20     |         49           |             |
|  23     |         50           |             |

|   Age   |     Sex       |   Number of images  |
|:-------:|:-------------:|:-------------------:|
|  19     |  Female       |         24          |
|  19     |  Male         |         25          |
|  20     |  Female       |         25          |
|  20     |  Male         |         24          |
|  23     |  Female       |         25          |
|  23     |  Male         |         25          |

# test data table
```
pd.read_csv (r'/content/gdrive/MyDrive/Tooth_Shap_GPT/Deep_tooth/Model/Multi_task(Age)(7-25)/Table_test_Predict.csv')
```

You can change the Path_Name column to reflect the new path using the str.replace method in pandas. Here is the code snippet to do that:

```
import pandas as pd

# Load the dataframe
df = pd.read_csv('/content/gdrive/MyDrive/Tooth_Shap_GPT/Deep_tooth/Model/Multi_task(Age)(7-25)/Table_test_Predict.csv')

# Replace the old path with the new path
df['Path_Name'] = df['Path_Name'].str.replace('/content/gdrive/MyDrive/Tooth_Shap_GPT/Deep_tooth', '/media/data/Natdata/Tooth_data')

# Display the updated dataframe
df.head()
```
