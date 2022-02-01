# MvtecAD supervise learning + Grad-Cam
I transformed the MvtecAD dataset into supervise learning, and use the Grad-Cam to find anomaly places.

## About data splitting
* Train  data: 2990 (728 anomaly data)
* Valid  data: 796  (182 anomaly data)
* Test   data: 1568 (348 anomaly data)


## Model Result
### 30 classes classification
* In MvtecAD Dataset, it contains 15 object category. 
* labels 0~14(0 in Binary) are the defect-free data
* labels 15~29(1 in Binary) are the defect data

|          | Test  Acc  | Test F score | Test auc |Test Binary Acc | Test Binary F score  |
| -------- | --------   | --------| -------- | --------       | --------        | 
| [VGG16](https://github.com/FieldTien/MvtecAD-supervise-learning-Grad-Cam/blob/main/VGG16_30class%2BGrad_cam.ipynb)    | 96.68%     | 96.62%  |97.83%   |96.68%            |92.37%          |
| [ResNet50](https://github.com/FieldTien/MvtecAD-supervise-learning-Grad-Cam/blob/main/ResNet50_30class%2BGrad_cam.ipynb) | 97.51%     | 97.48%  |99.26%   |97.51%            |94.27%            |


### 2 classes classification
* label 0 is the defect-free data
* label 1 is the defect data

|          | Test  Acc  | Test F score | Test auc |
| -------- | --------   | --------| -------- | 
| [VGG16](https://github.com/FieldTien/MvtecAD-supervise-learning-Grad-Cam/blob/main/VGG16_2class%2BGrad_cam.ipynb)    | 97.51%     | 94.28%  |97.97%  |
| [ResNet50](https://github.com/FieldTien/MvtecAD-supervise-learning-Grad-Cam/blob/main/ResNet50_2class%2BGrad_cam.ipynb) | 97.57%     | 94.31%  |98.96%  |



## Use Grad-CAM to find anomaly places
Here is the Grad-CAM++ result of [VGG16](https://github.com/FieldTien/MvtecAD-supervise-learning-Grad-Cam/blob/main/VGG16_2class%2BGrad_cam.ipynb) 2 class classification
![](https://i.imgur.com/NuhhoU6.png) 

## Confusion matrix
Here is the result of [ResNet50](https://github.com/FieldTien/MvtecAD-supervise-learning-Grad-Cam/blob/main/ResNet50_30class%2BGrad_cam.ipynb) 30 class classification
![](https://i.imgur.com/Y6nzDlJ.png)
![](https://i.imgur.com/pWDMCgc.png)






