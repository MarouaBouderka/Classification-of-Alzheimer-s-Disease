# **Classification of Alzheimer's Disease**

## **Classification Approach**
Our model follows a two-stage classification approach:  
1. **Initial Classification**: Determines whether a patient has **Alzheimer’s Disease** or not.  
2. **Stage Classification**: If Alzheimer's is detected, the model further categorizes the condition into one of the four stages:  
   - **Mild Dementia**  
   - **Moderate Dementia**  
   - **Non-Dementia**  
   - **Very Mild Dementia**  

## **Dataset**
The dataset used for this classification can be found here:  
[Alzheimer MRI 4 Classes Dataset](https://www.kaggle.com/datasets/marcopinamonti/alzheimer-mri-4-classes-dataset)  

This dataset contains MRI images labeled according to the Alzheimer’s stage, allowing for both binary classification (Alzheimer’s vs. Non-Alzheimer’s) and multi-class classification (four stages of Alzheimer’s).  

## **Models Used**
We experimented with various deep learning and machine learning models to identify the most effective approach:  

### **1. CNN-Based Models**  
We developed and tested two different convolutional neural network (CNN) architectures:  
- **Basic CNN Model**: A straightforward CNN with multiple convolutional layers.  
- **Complex CNN Model**: A deeper CNN with additional layers and dropout regularization to improve generalization.  

### **2. Transfer Learning**  
We leveraged pre-trained models to improve classification accuracy:  
- **ResNet**: A deep residual network capable of extracting high-level features from MRI scans.  
- **EfficientNet**: A computationally efficient model that balances depth, width, and resolution for improved performance.  

### **3. Vision Transformer (ViT)**  
- A **transformer-based model** designed for image classification.  
- Unlike CNNs, ViT **directly processes image patches as sequences**, capturing global dependencies more effectively.  

## **Best Model and Performance**  
After extensive testing, the **best-performing model** was the **Vision Transformer (ViT)** from **Notebook 2**, which achieved **98% accuracy on the test set**.  
This significantly outperformed other models, making it the most suitable choice for Alzheimer's MRI classification.

