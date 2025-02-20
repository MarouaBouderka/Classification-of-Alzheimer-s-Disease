# **Classification of Alzheimer's Disease**

## **Classification Approach**
Our model  classifies MRI images into one of these categories:  
- **Mild Dementia**  
- **Moderate Dementia**  
- **Non-Dementia**  
- **Very Mild Dementia**  


## **Dataset**
The dataset used for this classification is available here:  
[Alzheimer MRI 4 Classes Dataset](https://www.kaggle.com/datasets/marcopinamonti/alzheimer-mri-4-classes-dataset)  

This dataset contains MRI images labeled according to the presence and severity of Alzheimer's Disease, allowing us to train models that can directly classify different stages of the condition.

## **Models Used**
We experimented with various deep learning and machine learning models to determine the best approach:  

### **1. CNN-Based Models**  
We developed and tested two different convolutional neural network (CNN) architectures:  
- **Basic CNN Model**: A straightforward CNN with multiple convolutional layers.  
- **Complex CNN Model**: A deeper CNN with additional layers and dropout regularization to improve generalization.  

### **2. Transfer Learning**  
We utilized pre-trained models to enhance feature extraction:  
- **ResNet**: A deep residual network that learns hierarchical features.  
- **EfficientNet**: A highly optimized architecture balancing accuracy and efficiency.  

### **3. Vision Transformer (ViT)**  
- A **transformer-based model** designed for image classification.  
- Unlike CNNs, ViT **processes image patches as sequences**, allowing it to capture long-range dependencies more effectively.  

## **Best Model and Performance**  
After extensive experimentation, the **best-performing model** was the **Vision Transformer (ViT)** from **Notebook 2**, which achieved **98% accuracy on the test set**.  
This significantly outperformed other models, making it the most suitable choice for Alzheimer's MRI classification.

