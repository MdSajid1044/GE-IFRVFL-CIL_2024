Please cite the following paper if you are using this code.

Reference
---------------
M. A. Ganaie, M. Sajid, A. K. Malik and M. Tanveer, "Graph Embedded Intuitionistic Fuzzy Random Vector Functional Link Neural Network for Class Imbalance Learning," in IEEE Transactions on Neural Networks and Learning Systems, doi: 10.1109/TNNLS.2024.3353531.

Bibtex
------

@ARTICLE{10431593,
  author={Ganaie, M. A. and Sajid, M. and Malik, A. K. and Tanveer, M.},
  journal={IEEE Transactions on Neural Networks and Learning Systems}, 
  title={Graph Embedded Intuitionistic Fuzzy Random Vector Functional Link Neural Network for Class Imbalance Learning}, 
  year={2024},
  volume={},
  number={},
  pages={1-10},
  keywords={Germanium;Training;Machine learning;Data models;Alzheimer's disease;Predictive models;Noise measurement;Class imbalance (CI) learning;graph embedding (GE);intuitionistic fuzzy (IF);random vector functional link (RVFL) network},
  doi={10.1109/TNNLS.2024.3353531}}

Experimental Setup
------------------

The experiments are executed on a computing system possessing MATLAB R2017b software, an Intel(R) Xeon(R) CPU E5-2697 v4 processor operating at 2.30 GHz with 128-GB Random Access Memory (RAM), and a Windows-10 operating platform.

We have put a demo of the “GE_IFRVFL_CIL” model with the “abalone9-18” dataset 

The following are the best hyperparameters set with respect to the “abalone9-18” dataset 

Opt_para.N=23; //Number of hidden nodes
Opt_para.C=10^4; //Regularization Parameter
Opt_para.kerfPara.pars=0.125; //Kernel Parameter
Opt_para.lambda=10^-3; //Lambda

Description of Files
---------------------
GE_IFRVFL_CIL_main.m: This is the main file to run selected algorithms on datasets. In the path variable specificy the path to the folder containing the codes and datasets on which you wish to run the algorithm. 

GE_IFRVFL_CIL.m: the main file calls this file, which works as an intermediator between the training and prediction process.

GE_IFRVFL_CIL_Train.m: Training file

GE_IFRVFL_CIL_Predict.m: Prediction file

IF_non_linear_score_values.m: This file assigns Intuitionistic fuzzy scores to positive and negative class samples

gesvm: This folder contains the Graph embedding files used during the training process in the GE_IFRVFL_CIL_Train.m file.

relu: Code of the relu activation function.

The codes are not optimized for efficiency. The codes have been cleaned for better readability and documented and are not exactly the same as used in our paper. For the detailed experimental setup, please follow the paper. We have re-run and checked the codes only in a few datasets, so if you find any bugs/issues, please write to Dr. M. A. Ganaie (mudasir@iitrpr.ac.in).


Some parts of the codes have been taken from:
1. Zhang, Le, and Ponnuthurai N. Suganthan. "A comprehensive evaluation of random vector functional link networks." Information Sciences 367 (2016): 1094-1105.
2. Iosifidis, Alexandros, and Moncef Gabbouj. "Multi-class support vector machine classifiers using intrinsic and penalty graphs." Pattern Recognition 55 (2016): 231-246.

29-Feb-2024

