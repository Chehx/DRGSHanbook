# DRGSHanbook
# **DR grading survival handbook**

## **DR dataset link:**
https://hkustconnect-my.sharepoint.com/:f:/g/personal/ychengbj_connect_ust_hk/Etvtx9dSgClMoEcQZgKEwXkBBs6d6wzT0beCpXS0vT_wDQ?e=jpsaH3
There are four datasets inside this link (Messidor-2, APTOS, IDRID, DeepDR)

## papers:
This paper 'CANet: Cross-Disease Attention Network for Joint Diabetic Retinopathy and Diabetic Macular Edema Grading' about CANet by Prof. Li Xiaomeng could be followed.
https://ieeexplore.ieee.org/abstract/document/8892667
This paper is about DR and DME jointly grading. You can only focus on DR grading and follow the format the baseline.py in CANet.

other papers available:
1. CABNet: Category Attention Block for Imbalanced Diabetic Retinopathy Grading
https://ieeexplore.ieee.org/abstract/document/9195035


## preparation:
To run a deep learning algorithm by GPU, there are something need to be prepared.
#### 1. make sure you have a gpu
#### 2. download the correct version of cuda
link: https://developer.nvidia.com/cuda-downloads
usually we download the newest version of cuda
#### 3. download the corresponding version of pytorch
link: https://pytorch.org/get-started/previous-versions/
if your gpu is old, something error may occur. you need to find the corresponding version of pytorch
#### 4. check if the cuda could be used
open your terminal, type 'python' to get into python, then type like this:
![avatar](pics\terminal.png)
the output should be true

## some hints about DR grading
#### 1. you can learn how Resnet is realized
link: https://zh.d2l.ai/chapter_convolutional-modern/resnet.html
the d2l library contains some basic codes about the training process, how to compute the accuracy, how to visualize the output... you can check the codes for reference
#### 2. install the tensorboard and learn how to use tensorboard to visualize the output
link: https://github.com/tensorflow/tensorboard
![avatar](pics\tensorboard.png)
#### 3. the framework
1. a dataloader to load your DR dataset
2. use parsers to imput as commands
3. load your model (usually Resnet) and use pretrained model
4. the training process
5. compute the accuracy and auc score
6. visualize the output
### my output for reference
![avatar](pics\output.png)