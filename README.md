# hair_classification
Comparing classification techniques of different hair textures

Inspired by research paper: 
@article{umar2018hair,
  title={Hair detection, segmentation, and hairstyle classification in the wild},
  author={Muhammad, Umar Riaz and Svanera, Michele and Leonardi, Riccardo and Benini, Sergio},
  journal={Image and Vision Computing},
  year={2018},
  publisher={Elsevier}
}

Utilised hair or non_hair image patches from the Figaro-1k dataset training and testing sets
Hair image patches represented 7 different classes of hair textures: straight, wavy, curly, kinky, braids, dreadlocks and short-men

Extracted tiny features from training and testing images

Extracted hog features from training and testing images

Classified each feature with KNN and SVM algorithms

SVM classifier was more accurate overall and more accurate when classifying hog features.  

KNN was more accurate when classifying tiny features than hog features and peak accuracy was k >= 20 and  k ≈ 12 respectively.

Due to the high dimensional data it is not surprisig that the SVM classifier was more accurate in deciphering between hair and non_hair images

A particularly notable result is that the accuracy of the KNN model was higher for the tiny features however had a much higher k value which would result in underfitting the data.

It was important to train both models on a diverse set of hair textures to make sure that this recognition tool was inclusive.  
