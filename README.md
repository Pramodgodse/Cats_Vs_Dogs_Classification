# Cats_Vs_Dogs_Classification

# DataSet
We are using dataset from Kaggale link - https://www.kaggle.com/datasets/salader/dogs-vs-cats
Dataset contains two different folders, one named as Cats which contains 2500 images of cat and other Dogs with same image count.

# Hurdels
The main hurdel was loading/importing such huge dataset. Also, we need GUI and high RAM for computing.

# Loading dataset
To resolve loading/importing huge dataset we used Kaggle & Googal Colab, We directly imported the dataset to Colab.

# Setps
1. We loaded the dataset directly from Kaggle 
2. The loaded dataset was in zip format, we unziped it
3. Imported the necessary Libraries
4. Now we need to feed the testing folder data(images) to our module but it will require hudge computational compatibility; other way is to divide the process into batches resulting on less computational compatibility, we used the concept of Generators.
5. We created Generators for Training as well as for Validation data. with 
6. The stored images/data are in the form of Numpy Array with value 0-255, we need to convert it to 0-1 i.e., pixel values between 0-1, so we need to Normalize it.
7. Create CNN module with 3 convolution layer(1st layer - 32 filters, 2nd - 64, 3rd-128 filters) & complie it.

# Overfitting

As the Epoch increases Traing accuracy increases and Validation accuracy remains constatnt cresting a gap between the curves resulting overfitting .

ways to reduce overfitting
1. Add more data
2. Data Augmentation -> next video
3. L1/L2 Regularizer
4. Dropout   ( We used)
5. Batch Norm  ( We used)
6. Reduce complexity
