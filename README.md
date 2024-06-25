# Assessing Predictive Accuracy Shifts Post Oversampling in Datasets

**Writer:** Yeonsu Kim  
**Date:** 2023-12-09

This repository contains the project assignment for the Trustworthy-AI course (Prof. Park Sae-rom) during the Fall 2023 semester. This project investigates the effects of oversampling on predictive accuracy in machine learning models using the CelebA dataset.

## Abstract
This study explores the effect of oversampling on a dataset's specific properties. Predictive modeling on unbalanced datasets poses significant challenges, particularly regarding the effect of oversampling on the predictive accuracy of other properties. This investigation aims to clarify these effects and provide new insights into addressing dataset imbalances.

## Introduction
Modern machine learning technologies enhance data analysis and predictive modeling accuracy. However, handling imbalanced datasets remains a crucial challenge. This project examines how oversampling one attribute affects the prediction accuracy of another attribute using the CelebA dataset.

## Methodology
1. **Feature Engineering**: Identifying and selecting relevant features for analysis.
2. **Data Augmentation**: Applying oversampling techniques to address imbalances.
3. **Machine Learning**: Utilizing models to predict, classify, and identify anomalies based on extracted patterns.

### Experiments
- **Experiment 1**: Oversampling the 'Bald' feature.
- **Experiment 2**: Oversampling the 'Young' feature.
- **Experiment 3**: Oversampling the 'Big_Nose' feature.

Each experiment involves analyzing the impact of oversampling on prediction accuracy between male and female data using the ResNet-18 model.

## Dataset
The CelebA dataset contains images of 10,177 celebrities, each annotated with approximately 200,000 facial landmarks and more than 40 facial features. It is widely used for research and algorithm development in facial image recognition, feature extraction, and other computer vision tasks.

## Results
### Experiment 1 (Contributed by Yeonsu Kim)
Oversampling significantly impacted model accuracy in predicting genders, particularly due to the augmentation of baldness data. This led to a considerable imbalance, with the majority of bald data being male. Consequently, the oversampled dataset showed substantial differences in accuracy between genders.

### Experiment 2
Oversampling techniques were used to address unfair learning resulting from imbalances in other attributes when classifying between Gender and Old attributes. However, fairness improvement was observed only for specific attributes, indicating limitations in adjusting data ratios for a single attribute.

### Experiment 3
The appropriate oversampling ratio increased predictive accuracy and mitigated the disproportionate contribution of a specific gender to misclassified data.

## Conclusion
The study confirms that oversampling can significantly alter model performance, particularly when specific attributes correlate strongly with classification targets. While oversampling improved fairness and predictive accuracy in some cases, it also highlighted the limitations of adjusting data ratios for a single attribute.

## References
1. Rawashdeh, M. R., & Abdullah, M. (2020). Machine learning with oversampling and undersampling techniques: overview study and experimental results. In 2020 11th international conference on information and communication systems (ICICS) (pp. 243-248). IEEE.
2. Gosain, A., & Sardana, S. (2017). Handling class imbalance problem using oversampling techniques: A review. In 2017 international conference on advances in computing, communications and informatics (ICACCI) (pp. 79-85). IEEE.
3. Zhu, T., Lin, Y., & Liu, Y. (2017). Synthetic minority oversampling technique for multiclass imbalance problems. Pattern Recognition, 72, 327-340.
4. Shorten, C., & Khoshgoftaar, T. M. (2019). A survey on Image Data Augmentation for Deep Learning. J Big Data, 6, 60. https://doi.org/10.1186/s40537-019-0197-0
5. Perez, L., & Wang, J. (2017). The Effectiveness of Data Augmentation in Image Classification using Deep Learning. https://doi.org/10.48550/arXiv.1712.04621
6. Wong, S. C., Gatt, A., Stamatescu, V., & McDonnell, M. D. (2016). Understanding Data Augmentation for Classification: When to Warp? In 2016 International Conference on Digital Image Computing: Techniques and Applications (DICTA) (pp. 1-6). IEEE. doi: 10.1109/DICTA.2016.7797091
