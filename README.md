# Age_and_Gender_Classification

This projetc is a reimplementation of this [paper](https://ieeexplore.ieee.org/document/7301352). Actually in our implementation, an attempt is made to modify the architecture of the paper in a way to be able to train the modlel with fewer parameters and training time with comparable performance. In this project we have compared the efficiency of using CNN and ResNet-18 for Age and Gender Classification task.
 
## Dataset

In this project, to test the efficiency of the model we have used the Adience benchmark which is designed for age and gender classification task. The dataste needs some preprocessing which has been done as a part of the project. The preprocessed version of the dataset which consists of 16249 data can be downloaded from [here](https://drive.google.com/drive/folders/1d0qAw7UvqKhXcu_7I6yTv3mGrxhSLD2Z?usp=sharing
). Consider that after downloading the dataset, you must put all images in Data/ALLFOLDS folder.

We splited the data into training and testing set with 13000 and 3249 data smaples, respectively.

## Test the code

You can run the following code to test the system:
```
cd Code
python CNN_A.py    #for age classification using CNN
python CNN_G.py    #for Gender classification using CNN
```

## Model Accuracy

### for gender classification

| Model  |  Accuracy |
| ------------- | ------------- |
| CNN  | 77.72  |
| ResNet-18  | 71.96  |
| VGG-16  | 79.31  |
| Original Paper  | 85.9  |

### for age classification

| Model  |  Accuracy |
| ------------- | ------------- |
| CNN  | 46.66  |
| ResNet-18  | 48.11  |
| Original Paper  | 49.5  |



