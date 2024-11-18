# Lung Cancer Detection

## Dataset Details
This project uses a **histopathological image dataset** for lung cancer detection with the following details:

- **Total Images**: 15,000  
- **Image Dimensions**: 768 x 768 pixels  
- **Format**: JPEG  
- **Classes**:  
  1. **Lung Benign Tissue**: 5,000 images  
  2. **Lung Adenocarcinoma**: 5,000 images  
  3. **Lung Squamous Cell Carcinoma**: 5,000 images  

### Original Dataset Details
- The dataset was derived from **750 original images**:
  - 250 benign lung tissue images.
  - 250 lung adenocarcinoma images.
  - 250 lung squamous cell carcinoma images.
- These images were augmented to **15,000 images** using the **Augmentor package**.

![Adenocarcinoma](https://i.imgur.com/cKjHfX3.jpg)

### Citation
If you use this dataset, please cite:  
**Borkowski AA, Bui MM, Thomas LB, Wilson CP, DeLand LA, Mastorides SM. Lung and Colon Cancer Histopathological Image Dataset (LC25000). arXiv:1912.12142v1 [eess.IV], 2019**

### Relevant Links
- **Research Paper**: [arXiv:1912.12142v1](https://arxiv.org/abs/1912.12142v1)  
- **Dataset Source**: [Kaggle Dataset](https://www.kaggle.com/andrewmvd/lung-and-colon-cancer-histopathological-images)

---

## Models Used
This project leverages **state-of-the-art convolutional neural networks (CNNs)** for image classification. The following models are used:

1. **InceptionV3**  
   - Efficient for high-resolution images and reduces computational costs.
   - Uses factorized convolutions and auxiliary classifiers.

2. **VGG16**  
   - A 16-layer CNN known for simplicity and robust feature extraction.  
   - Performs well on moderate-sized datasets.  

3. **VGG19**  
   - A deeper version of VGG16 with 19 layers for complex feature extraction.  
   - Captures finer details but requires more computational resources.

4. **ResNet (Residual Network)**  
   - Employs skip connections to solve the vanishing gradient problem.  
   - Allows for training deeper networks with high accuracy and minimal overfitting.

---

## Methodology
### 1. **Data Preprocessing**
- Images resized to fit each model's input dimensions.  
- Augmentation techniques used (e.g., rotation, flipping, contrast adjustment) to improve generalization.

### 2. **Training Pipeline**
- Dataset split into **80% training** and **20% validation**.  
- Optimized using the **Adam optimizer** and **categorical cross-entropy loss**.  

### 3. **Performance Metrics**
- **Accuracy**: Measures overall classification performance.  
- **Precision & Recall**: Evaluates class-specific predictions.  
- **F1-Score**: Balances precision and recall.  
- **Confusion Matrix**: Visualizes classification results (TP, FP, TN, FN).

---

## How to Cite
If you use this repository or its components, please provide appropriate attribution. For any issues or contributions, feel free to open a pull request or issue in the repository.
