#### CS867-Assignment 3: Image Classification Using Convolutional Neural Network

## Pre-Requisites
1. Anaconda (https://www.anaconda.com/products/individual)
2. Pytorch (https://pytorch.org/get-started/locally/)
3. Natural Scene Classification Dataset (https://www.kaggle.com/puneet6060/intel-image-classification/version/2)

## Data Augmentation

To add more diversity in dataset, I have performed four types of data augmentations including,

- Gaussian Blur
- Horizontal Flip
- Contrast
- Saturation

You can use the **Augmentation.ipynb** in **Train_Notebooks** to perform augmentation on the provided dataset.

## Training

To this end, three state-of-the-art CNNs i.e. **Alexnet** , **Resnet-152**, and **VGG** are employed to perform classification. It is important to mention here that, pre-trained CNNs are downloaded, and trained through transfer learning to achieve effective results. All the networks are available in above-folder named **Trained Notebooks**. All the trained models are available in above-folder **models**.

## Results
The experiments are performed on both i.e. the base and augmented datasets to analyse the difference through adaptive and static learning rate. The experiments showed that Resnet-152 achieved better accuracy on augmented dataset with adaptive learning rate.

#### Alexnet
- With Adaptive Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/CS867-Assignment3/blob/main/graphs/Alex_Aug_AL.PNG?raw=true)

- With Constant Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/CS867-Assignment3/blob/main/graphs/Alex_Aug_CLR.PNG?raw=true)

- With Adaptive Learning Rate on Base Dataset

![alt text](https://github.com/aatiibutt/CS867-Assignment3/blob/main/graphs/Alex_Base_AL.PNG?raw=true)

- With Constant Learning Rate on Base Dataset

![alt text](https://github.com/aatiibutt/CS867-Assignment3/blob/main/graphs/Alex_Base_CLR.PNG?raw=true)

#### Resnet

- With Adaptive Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/CS867-Assignment3/blob/main/graphs/Res_Aug_AL.PNG?raw=true)

- With Constant Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/CS867-Assignment3/blob/main/graphs/Res_Aug_AL.PNG?raw=true)

#### VGG

- With Adaptive Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/CS867-Assignment3/blob/main/graphs/VGG_Aug_AL.PNG?raw=true)

- With Constant Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/CS867-Assignment3/blob/main/graphs/Res_Aug_AL.PNG?raw=true)
