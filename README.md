# SVD_Eigenfaces


# Eigenface Script

This script demonstrates the concept of eigenfaces in face recognition using Singular Value Decomposition (SVD) and PCA.

## Prerequisites

- NumPy
- Pandas
- Matplotlib
- PIL (Python Imaging Library)

## Description

The eigenface script follows the following steps:

1. Load the face images from the dataset folder.
2. Preprocess the images by resizing and converting them to grayscale.
3. Flatten each image into a 1D array and create a DataFrame with all the image data.
4. Calculate the average face by taking the mean of all images.
5. Compute the eigenfaces using Singular Value Decomposition (SVD) on the image data.
6. Select a test face and subtract the average face from it.
7. Project the test face onto the eigenfaces to obtain the weights.
8. Reconstruct the test face using a subset of eigenfaces and the weights.
9. Display the original test face and the reconstructed faces at different rank levels.
10. Repeat steps 7-9 for different rank levels to observe the impact on reconstruction.

## Results

The script will display the original test face and the reconstructed faces using different rank levels. You can observe how the quality of the reconstruction improves as more eigenfaces are used, however, SVD hasnt achieve a
a good approximation becuase it only considers linear relations between faces, and in the dataset I used, there are rotations and flips that cannot be consider correctly by the SVD technique.

## References

- Brunton, S. L., & Kutz, J. N. (2019). Data-Driven Science and Engineering: Machine Learning, Dynamical Systems, and Control. Cambridge University Press.
