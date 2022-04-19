# Project Name
> To build a CNN based model which can accurately detect melanoma.
Melanoma is a type of cancer that can be deadly if not detected early.It accounts for 75% of skin cancer deaths.
A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Steps and Observations
* Imported Skin Cancer Data from Google Drive in google colab
* Data Visualisation of all the nine classes present in the dataset
* Rescaling of the data to normalize pixel values between (0,1).
* Create model using appropirate optimiser and loss function for model training
* Training accuracy is at 84% and validation accuracy around 77%. 
Loss function for validation dataset is higher than train data. There may be a possibilty of model overfit which needs to be checked further
* Data Augmentation startegy applied to reduced the possibility of overfit.
* After rebuilding the model with augumented data, there is drop in accuracy to 42% and the model is underfitting as accuracy is less than random guess.
We need to check the class ditribution to improve our accuracy rate
* On checking class imbalance, Seborrheic keratosis has less the 20 numbers and Melanoma and pigmented benign keratosis has close to 100 samples
* Class imbalance rectified by adding more images to maintain class balance
* Model trained using augmented data and batch Normalisation and the accuracy improved to 82% but the validation accuracy is still at 62% indicating overfit issue.
* By further adding layers in the network and hyper parameter tuning

## Contact
Created by [@sindhus123] - feel free to contact me!
