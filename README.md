# Chest-Cancer-Detecton-CNN

<h2>Link to Data</h2>

https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images

<h2>About the Data</h2>

The images are in png to fit the model. Data contain 3 chest cancer types which are Adenocarcinoma,Large cell carcinoma, Squamous cell carcinoma , and 1 folder for the normal cell. Data folder is the main folder that contain all the step folders and inside Data folder are test , train , valid. 

- test represent testing set
- train represent training set
- valid represent validation set
- training set is 70%
- testing set is 20%
- validation set is 10%

```bash
chest-ctscan-images
   └── Data
      ├── test
      │   ├── Adenocarcinoma
      │   │   ├── image1.png
      │   │   └── image2.png
      │   ├── Large cell carcinoma
      │   ├── Squamous cell carcinoma
      │   ├── Normal
      ├── train
      └── valid
```

<h2>Adenocarcinoma</h2>

Adenocarcinoma of the lung: Lung adenocarcinoma is the most common form of lung cancer
accounting for 30 percent of all cases overall and about 40 percent
of all non-small cell lung cancer occurrences. Adenocarcinomas are
found in several common cancers, including breast, prostate and colorectal.
Adenocarcinomas of the lung are found in the outer region of the lung
in glands that secrete mucus and help us breathe.
Symptoms include coughing, hoarseness, weight loss and weakness.

<h2>Large cell carcinoma</h2>

Large-cell undifferentiated carcinoma: Large-cell undifferentiated carcinoma lung cancer grows and spreads quickly and can
be found anywhere in the lung. This type of lung cancer usually accounts for 10
to 15 percent of all cases of NSCLC.
Large-cell undifferentiated carcinoma tends to grow and spread quickly.

<h2>Squamous cell carcinoma</h2>

Squamous cell: This type of lung cancer is found centrally in the lung,
where the larger bronchi join the trachea to the lung,
or in one of the main airway branches.
Squamous cell lung cancer is responsible for about 30 percent of all non-small
cell lung cancers, and is generally linked to smoking.

And the last folder is the normal CT-Scan images 

<h2>Objective</h2>
Use machine learning and deep learning (CNN) to classify and diagnose if the patient has cancer or not. 

<h2>CNN Overview</h2>
Preprocessing Image Parameters:

    Class Names = ['adenocarcinoma_left.lower.lobe_T2_N0_M0_Ib', 'large.cell.carcinoma_left.hilum_T2_N2_M0_IIIa', 'normal', 'squamous.cell.carcinoma_left.hilum_T1_N2_M0_IIIa']
    Color Mode = grayscale (1)
    Batches are default to 32
    Label_mode is INT
    Based on Label mode of INT, need to use sparse_categorical_crossentropy

CNN Model Parameters

    Sequential Model consisting of 3 convolution blocks (Conv2D) with a max pooling layer (MaxPooling2D) in each.
    Fully connected layer (Dense) with 128 units on top and activated by a ReLu activation.
    Adam Optimizer used which is a SGD method based on adaptive Estimation of first-order and second-order moments.
    Began with 10 epochs as a base

Output

    Visualized training versus validation for accuracy over the 10 epochs
    Visualized training versus validation for loss over the 10 epochs
    Applied simple CNN to predict test data.


