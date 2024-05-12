# Face Recognition

This repository contains the implementation of a face recognition assignment as part of a university course. The assignment involves using Principal Component Analysis (PCA) and Linear Discriminant Analysis (LDA) for classification on the ORL dataset, as well as exploring various aspects of classifier tuning and comparing results with non-face images.

## Dataset
The ORL dataset, consisting of grayscale images of size 92x112, with 10 images per each of the 40 subjects, is utilized for this assignment. You can download the dataset from [Kaggle](https://www.kaggle.com/kasikrit/att-database-of-faces/).

## Steps Implemented

1. **Generate Data Matrix and Label Vector**
    - Convert images into vectors and stack them into a data matrix `D`. Generate the label vector `y` corresponding to subject IDs.

2. **Split Dataset into Training and Test Sets**
    - Keep odd rows for training and even rows for testing, resulting in 5 instances per person for both training and testing.

3. **Classification using PCA**
    - Compute the projection matrix `U` for different values of `alpha`.
    - Project the training and test sets using `U`.
    - Utilize the nearest neighbor classifier and report accuracy for each `alpha`.
    - Investigate the relation between `alpha` and classification accuracy.

4. **Classification using LDA**
    - Modify LDA pseudocode for multiclass LDA.
    - Project training and test sets using the projection matrix `U`.
    - Utilize nearest neighbor classifier and report accuracy for multiclass LDA.
    - Compare results with PCA.

5. **Classifier Tuning**
    - Explore different number of neighbors (`K`) for K-NN classifier.
    - Plot accuracy against `K` for both PCA and LDA.

6. **Comparison with Non-Face Images**
    - Attempt classification of faces vs. non-faces using non-face images of the same size.
    - Analyze success and failure cases.
    - Determine the number of dominant eigenvectors for LDA.
    - Plot accuracy vs. number of non-face images.
    - Critique accuracy measure for large numbers of non-face images in the training data.

7. **Bonus**
    - Implement different training and test splits, comparing results with the original split.
    - Utilize variations of PCA and LDA algorithms (QDA), comparing time complexity and accuracy.

## Contributors
- [Mostafa M. Galal](https://github.com/MostafaGalal1)
- [Mohamed H. Sadik](https://github.com/mohamedhassan279)
- [Joseph S. Soliman](https://github.com/josephShokry)

## Report
The detailed report for this assignment can be found [here](link_to_report_pdf).

For any inquiries or suggestions, feel free to contact us through GitHub.
