## DEEP LEARNING FOR PAROXYSMAL ATRIAL FIBRILLATION CLASSIFICATION

This is the project showcase of Udacity - Facebook Pytorch Challenge Program. The project is a Pytorch implementation. 

### About the project

Paroxysmal atrial fibrillation (PAF), as being a type of arrhythmia of the heart that occurs spontaneously, has been the interest of researchers for more than a decade. Due to its spontaneous nature, it is hard to get ECG readings during PAF attacks. Therefore, classification methods have been developed to diagnose PAF patients, from the electrocardiogram (ECG) records with normal sinus rhythm. The purpose of this study is to utilize recent developments in deep neural network to find a better classifier to achieve higher accuracies. MLP is used to achieve classification goal of labelling the PAF subject as 1 and 0 otherwise.

If this is achieved, considering that we have data collection possibilities via mobile phones, the second step is going to be early warning to prevent many issues that may arise with a sudden PAF attack (such as while driving..)

The dataset is from Physionet "The research resource for complex physiologic signals". Retrieved from physionet.org: https://www.physionet.org and used in “The PAF Prediction Challenge” in 2001.

This database is described in Moody GB, Goldberger AL, McClennen S, Swiryn SP. Predicting the Onset of Paroxysmal Atrial Fibrillation: The Computers in Cardiology Challenge 2001. Computers in Cardiology28:113-116 (2001). Citation for PhysioNet: Goldberger AL, Amaral LAN, Glass L, Hausdorff JM, Ivanov PCh, Mark RG, Mietus JE, Moody GB, Peng C-K, Stanley HE. PhysioBank, PhysioToolkit, and PhysioNet: Components of a New Research Resource for Complex Physiologic Signals. Circulation 101(23):e215-e220 [Circulation Electronic Pages; http://circ.ahajournals.org/content/101/23/e215.full]; 2000 (June 13).

In this study, I utilized the outcome of a phd thesis. (Hilavin, I. (2016). Development of a System to Diagnose Atrial Fibrillation Patients From Arrythmia Free ECG Records. İzmir, Turkey: DEU.) In her study, Ms. Hilavin created 33 features (like Mean RR, Std RR etc) from PAF dataset and through Genetic Algorithms, she has found out the most describing 8 features. By taking these 8 features and implementing SVM classifier she achieved over 90% accuracy.

When we want to use the dataset for a DL algorithm, the first thing to realize is that the data is not big enough for the model to be trained. (50 person with PAF and 50 person without)

Hilavin’s preprocessed data is considered to be doing some part of the DL network’s job and MLP is decided to be used with that derived dataset which has 798 rows and 8 features.

### What is done in the project

The preprocessed data is used as tabular entry to our DL network. Network is created by use of Pytorch package. The dataset is splitted in to train, validation and test set after shuffling the rows with 80%, 10% and 10% respectively.

Training and testing are done with respective python + pytorch routines.

### How to install and run the project

Anaconda distribution is recommended with Python 3.7 to be downloaded. Make sure numpy, pandas, seaborn, matplotlib packages are included. If not, they need to installed by use of terminal in Mac or by Anaconda prompt in Windows.

Pytorch stable package needs the installed from it's official site.

After cloning the project, please run DLtoPAF.ipynb in Jupyter Notebook by shift + Enter every cell.

### Contributing

Project is open to contribution.