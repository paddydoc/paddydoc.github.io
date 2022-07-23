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
#### Classification Report
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

#### Classification Report
 ```
                           precision    recall  f1-score   support

   bacterial_leaf_blight    0.95420   0.96154   0.95785       130
   bacterial_leaf_streak    0.94175   0.97000   0.95567       100
bacterial_panicle_blight    0.97727   0.95556   0.96629        90
        black_stem_borer    1.00000   0.91089   0.95337       101
                   blast    0.95607   0.97234   0.96414       470
              brown_spot    0.96078   0.96838   0.96457       253
            downy_mildew    0.93785   0.95402   0.94587       174
                   hispa    0.96454   0.94664   0.95550       431
             leaf_roller    0.99010   0.91324   0.95012       219
                  normal    0.96933   0.98545   0.97732       481
                  tungro    0.98454   0.97949   0.98201       390
        white_stem_borer    0.95437   0.98819   0.97099       254
       yellow_stem_borer    0.96795   0.99342   0.98052       152

                accuracy                        0.96579      3245
               macro avg    0.96606   0.96147   0.96340      3245
            weighted avg    0.96613   0.96579   0.96571      3245
```
#### Confusion matrix
![xception cm](https://raw.githubusercontent.com/paddydoc/paddy-docctor-dataset/main/results/cm-xception.png)

### VGG16 Results
#### Classification Report
```
                           precision    recall  f1-score   support

   bacterial_leaf_blight    0.85612   0.91538   0.88476       130
   bacterial_leaf_streak    0.93204   0.96000   0.94581       100
bacterial_panicle_blight    1.00000   0.86667   0.92857        90
        black_stem_borer    0.95652   0.87129   0.91192       101
                   blast    0.94017   0.93617   0.93817       470
              brown_spot    0.90310   0.92095   0.91194       253
            downy_mildew    0.95783   0.91379   0.93529       174
                   hispa    0.95792   0.89791   0.92695       431
             leaf_roller    0.99459   0.84018   0.91089       219
                  normal    0.95297   0.96881   0.96082       481
                  tungro    0.84564   0.96923   0.90323       390
        white_stem_borer    0.93585   0.97638   0.95568       254
       yellow_stem_borer    0.98013   0.97368   0.97690       152

                accuracy                        0.93190      3245
               macro avg    0.93945   0.92388   0.93007      3245
            weighted avg    0.93488   0.93190   0.93199      3245

```
#### Confusion matrix
![cm VGG16](https://raw.githubusercontent.com/paddydoc/paddy-docctor-dataset/main/results/cm-VGG16.png)

### CNN Results
#### Classification Report
```
                           precision    recall  f1-score   support

   bacterial_leaf_blight    0.84800   0.81538   0.83137       130
   bacterial_leaf_streak    0.84545   0.93000   0.88571       100
bacterial_panicle_blight    0.98630   0.80000   0.88344        90
        black_stem_borer    0.90099   0.90099   0.90099       101
                   blast    0.92601   0.87872   0.90175       470
              brown_spot    0.92511   0.83004   0.87500       253
            downy_mildew    0.94231   0.84483   0.89091       174
                   hispa    0.90281   0.81903   0.85888       431
             leaf_roller    0.78151   0.84932   0.81400       219
                  normal    0.83158   0.98545   0.90200       481
                  tungro    0.91601   0.89487   0.90532       390
        white_stem_borer    0.90672   0.95669   0.93103       254
       yellow_stem_borer    0.91824   0.96053   0.93891       152

                accuracy                        0.88844      3245
               macro avg    0.89470   0.88199   0.88610      3245
            weighted avg    0.89219   0.88844   0.88812      3245
   ```
   #### Confusion matrix
   ![CNN cm](https://raw.githubusercontent.com/paddydoc/paddy-docctor-dataset/main/results/cm-cnn.png)



