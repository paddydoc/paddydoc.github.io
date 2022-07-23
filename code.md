---
title: Code and Benchmarks
subtitle: Benchamrking of AI/ML algorithms on the Paddy Doctor datasets
layout: page
show_sidebar: false
hide_hero: true
---

# Benchmarking of Deep Learning

|Model | Precision | Recall | F1-score | Accuracy |
| :--- | ---: | ---: | ---: | ---: |
| [Resnet34](https://github.com/paddydoc/paddy-docctor-dataset/blob/main/resnet34-with-fastai.ipynb)| 97.52 |  97.5 |  97.5 | 97.5  |  
| [Xception](https://github.com/paddydoc/paddy-docctor-dataset/blob/main/xception.ipynb)|96.61 |  96.58 | 96.57 | 96.58 |  
| [VGG16](https://github.com/paddydoc/paddy-docctor-dataset/blob/main/vgg16.ipynb)|  93.49  | 93.19  | 93.2 | 93.19  |  
| [MobileNet]()| - |- | - | 88.84 |  
| [CNN](https://github.com/paddydoc/paddy-docctor-dataset/blob/main/cnn.ipynb)| 89.22 | 88.84 | 88.81 | 88.84 |  

### Resnet34 results
#### Classification report
```
                          precision    recall  f1-score   support

   bacterial_leaf_blight    0.96947   0.97692   0.97318       130
   bacterial_leaf_streak    0.95146   0.98000   0.96552       100
bacterial_panicle_blight    1.00000   0.96667   0.98305        90
        black_stem_borer    0.98925   0.91089   0.94845       101
                   blast    0.97028   0.97234   0.97131       470
              brown_spot    0.98381   0.96047   0.97200       253
            downy_mildew    0.95954   0.95402   0.95677       174
                   hispa    0.96759   0.96984   0.96871       431
             leaf_roller    0.97727   0.98174   0.97950       219
                  normal    0.97951   0.99376   0.98658       481
                  tungro    0.98446   0.97436   0.97938       390
        white_stem_borer    0.95833   0.99606   0.97683       254
       yellow_stem_borer    1.00000   0.98684   0.99338       152

                accuracy                        0.97504      3245
               macro avg    0.97623   0.97107   0.97344      3245
            weighted avg    0.97520   0.97504   0.97500      3245
```
#### Confusion matrix
![resnet34 cm](https://raw.githubusercontent.com/paddydoc/paddy-docctor-dataset/main/results/cm-restnet34.png)
           

### Xception results
 ```
 precision    recall  f1-score   support

   bacterial_leaf_blight    0.96947   0.97692   0.97318       130
   bacterial_leaf_streak    0.95146   0.98000   0.96552       100
bacterial_panicle_blight    1.00000   0.96667   0.98305        90
        black_stem_borer    0.98925   0.91089   0.94845       101
                   blast    0.97028   0.97234   0.97131       470
              brown_spot    0.98381   0.96047   0.97200       253
            downy_mildew    0.95954   0.95402   0.95677       174
                   hispa    0.96759   0.96984   0.96871       431
             leaf_roller    0.97727   0.98174   0.97950       219
                  normal    0.97951   0.99376   0.98658       481
                  tungro    0.98446   0.97436   0.97938       390
        white_stem_borer    0.95833   0.99606   0.97683       254
       yellow_stem_borer    1.00000   0.98684   0.99338       152

                accuracy                        0.97504      3245
               macro avg    0.97623   0.97107   0.97344      3245
            weighted avg    0.97520   0.97504   0.97500      3245
      ```
