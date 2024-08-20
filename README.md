# 🧠 *Autism Spectrum Disorder Classification using Deep Learning* 🌟
<div align="center">
  <img src="https://github.com/user-attachments/assets/7c8b3d55-c512-41b9-b050-c6f2bf1c1349" alt="ASD title" width="400"/>
</div>

## 📚 **Introduction**

Autism Spectrum Disorder (ASD) is a developmental disorder that affects communication, behavior, and social interaction. Individuals with ASD may exhibit a wide range of abilities and challenges. Some common features include difficulty with social interactions, repetitive behaviors, and sensitivity to sensory input. However, the presentation of ASD varies greatly between individuals.

In this project, we explore the use of deep learning techniques combined with eye-tracking technology for the early detection of Autism Spectrum Disorder (ASD). Early diagnosis is crucial for effective intervention, yet it often occurs around the age of 4, despite earlier symptom onset. Eye-tracking technology offers a promising, cost-effective, and non-invasive method for early diagnosis by capturing eye movement data that can serve as biomarkers for ASD. 

We analyze an eye-tracking dataset using enhanced image processing techniques to extract critical visual features. This study introduces a hybrid classification approach that integrates multiple deep learning models, including GoogleNet, ResNet, XceptionV3, DenseNet, Xception, and MobileNet, to enhance the diagnostic accuracy of Autism Spectrum Disorder (ASD) detection. These features are processed through a hybrid model that leverages the strengths of multiple deep learning architectures, significantly improving the accuracy of ASD diagnosis. This approach successfully distinguishes ASD cases from typical development (TD) cases, offering a robust tool for early detection and contributing to better treatment strategies.

## 📊 **Dataset Overview**
The dataset was meticulously preprocessed to optimize the training and evaluation of the deep learning models. The process involved several key steps:

  - **Data Splitting**: The dataset was initially split into training and validation sets, ensuring a balanced representation of classes in each subset.

  - **Image Augmentation**:
    - For the training set, images underwent augmentation to increase the model's robustness and generalization capabilities. This included:
      - **Rescaling**: Standardizing pixel values.
      - **Shearing**: Applying affine transformations to simulate perspective shifts.
      - **Zooming**: Randomly zooming in on images to enhance feature detection.
    - For the test set, a simpler preprocessing was applied, involving only rescaling to maintain consistency during model evaluation.
    
  - **Data Loading**: The preprocessed images were then loaded into the model pipeline using ImageDataGenerator, which facilitated real-time data augmentation during training.
    - A target image size of 128x128 pixels was set, balancing the trade-off between computational efficiency and preserving critical visual features.
    - This comprehensive setup enabled the effective training and evaluation of multiple deep learning models, ensuring that the models were exposed to a diverse range of image variations during the training phase while maintaining a consistent evaluation process.

## 🎯 **Conclusion & Future Work**

This project implemented and compared several deep learning models, with Xception and MobileNet showing the highest accuracy. An interactive dashboard was developed to visualize and explore model performance. 

### 🔮 *Future Work*
- **Model Refinement**: Further refine the models to enhance their diagnostic accuracy.
- **Dashboard Enhancement**: Improve the interactive dashboard for better visualization and user experience.
- **Real-World Deployment**: Deploy the system in real-world applications for practical use.
- **Ensemble Techniques**: Explore ensemble techniques to further boost the accuracy of ASD detection.

## 📜 **LICENSE**

This project is licensed under the MIT License. Feel free to use, modify, and distribute this project under the terms of the MIT License.

## 🤝 **Contributions**

Contributions to the project are welcome! If you have any suggestions or questions, please feel free to reach out via email at [divya.pariti@ucdconnect.ie](mailto:divya.pariti@ucdconnect.ie).



