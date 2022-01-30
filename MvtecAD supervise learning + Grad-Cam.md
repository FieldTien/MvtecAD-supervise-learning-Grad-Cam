# MvtecAD supervise learning + Grad-Cam
I transformed the MvtecAD dataset into supervise learning, and use the Grad-Cam to find anomaly places.

## About data splitting
* Train  data: 2990 (728 anomaly data)
* Valid  data: 796  (182 anomaly data)
* Test   data: 1568 (348 anomaly data)


## Model Result
### 30 classes classification

|          | Test  Acc  | Test F score | Test auc |Test Binary Acc | Test Binary F score  |
| -------- | --------   | --------| -------- | --------       | --------        | 
| VGG16    | 96.68%     | 96.62%  |97.83%   |96.68%            |92.37%          |
| ResNet50 | 97.51%     | 97.48%  |99.26%   |97.51%            |94.27%            |


### 2 classes classification

|          | Test  Acc  | Test F score | Test auc |
| -------- | --------   | --------| -------- | 
| VGG16    | 97.51%     | 94.28%  |97.97%   |
| ResNet50 | 97.57%     | 94.31%  |98.96%   |


