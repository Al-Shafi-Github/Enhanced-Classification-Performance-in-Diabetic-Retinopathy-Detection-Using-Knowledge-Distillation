---

# Enhanced Classification Performance in Diabetic Retinopathy Detection Using Knowledge Distillation

**Full Paper:**  
- [IEEE Xplore](https://ieeexplore.ieee.org/document/10650642)  
- [ResearchGate](https://www.researchgate.net/publication/383883431_Enhancing_Diabetic_Retinopathy_Detection_Through_Transformer_Based_Knowledge_Distillation_and_Explainable_AI)

## Table of Contents
1. [Introduction](#introduction)  
2. [Key Features](#key-features)  
3. [Technologies Used](#technologies-used)  
4. [Methodology & Architecture](#methodology--architecture)  
5. [Results & Analysis](#results--analysis)  
6. [Explainable AI with SHAP](#explainable-ai-with-shap)  
7. [License](#license)  
8. [Contact](#contact)

---

## Introduction
This repository demonstrates an approach to **improve diabetic retinopathy detection** by leveraging **Transformer-based knowledge distillation**. The primary objective is to **boost classification performance** while maintaining efficient inference. By combining **pre-trained models**, **Transformer architectures**, and **best practices** such as early stopping, selective layer updating, and hyperparameter tuning, this project aims to offer a more reliable diagnostic tool for **retinal image analysis**.

---

## Key Features
- **Transformer-Based Knowledge Distillation**: Transfer knowledge from a high-capacity teacher model to a lighter student network.  
- **Early Stopping & Layer Freezing**: Prevent overfitting and reduce training time by selectively freezing layers.  
- **Hyperparameter Optimization**: Systematic search to find optimal learning rates, batch sizes, and regularization parameters.  
- **Robust Performance Metrics**: Evaluated using **weighted Kappa Score** and other classification metrics to ensure clinical relevance.

---

## Technologies Used
- **Programming Language**: Python  
- **Deep Learning Framework**: PyTorch  
- **Machine Learning Libraries**: scikit-learn, Keras  
- **Plotting & Visualization**: Matplotlib  

---

## Methodology & Architecture
Below is a high-level overview of the knowledge distillation process and training setups:

<img src="https://github.com/user-attachments/assets/09a09ef9-0079-4205-9f7c-59e700506bbb" alt="Architecture of KD" width="500">

1. **Teacher Model (Transformer / Vision Transformer)**  
2. **Student Model (e.g., CNN-based network)**  
3. **Distillation Loss** combining teacher outputs and ground truth.  

---

## Results & Analysis
We compared multiple models (ResNet34, MobileVitV2, DenseNet121, GoogleNet, DeiT3) under three different strategies (Imbalance, Augmented, and Cost-Sensitive Learning). The bar chart below shows **training times** for each combination:

<img src="https://github.com/user-attachments/assets/e36917cd-fb33-447a-95f9-21b99043a0c9" alt="Training Time of All The Models" width="500">

- **Cost-Sensitive Learning** offers an average of ~5% reduction in training time compared to Imbalance approaches, and ~25% faster than Augmented methods.  

---

## Explainable AI with SHAP
We employed **SHAP** (SHapley Additive exPlanations) to interpret and visualize the model’s predictions. This helps identify the **critical regions** in retinal images that drive classification decisions:

<img src="https://github.com/user-attachments/assets/0c61da1e-7fa2-45c0-9b83-4487ef64a34b" alt="Explainable AI" width="500">

---

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT). Feel free to use, modify, and distribute it as per the terms of this license.

---

## Contact
If you have any questions or suggestions, please reach out:
- **Email**: [abdullah.shafi191@gmail.com](mailto:abdullah.shafi191@gmail.com)

---

**Thank you for your interest!** If you find this project useful or have ideas for improvement, consider starring the repository or contributing.
