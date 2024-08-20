# 🧠 *Autism Spectrum Disorder Classification using Deep Learning* 🌟
<div align="center">
  <img src="https://github.com/user-attachments/assets/7c8b3d55-c512-41b9-b050-c6f2bf1c1349" alt="ASD title" width="400"/>
</div>

![Python](https://img.shields.io/badge/python-3.9.19-3776AB?logo=python&logoColor=white)
![Pip](https://img.shields.io/badge/pip-24.2-2C8EBB?logo=pypi&logoColor=white)
![OpenSSL](https://img.shields.io/badge/openssl-3.0.14-8A2BE2?logo=openssl&logoColor=white)
![SQLite](https://img.shields.io/badge/sqlite-3.45.3-003B57?logo=sqlite&logoColor=white)
![Setuptools](https://img.shields.io/badge/setuptools-72.1.0-FFD43B?logo=python&logoColor=black)
![Tzdata](https://img.shields.io/badge/tzdata-2024a-4A90E2?logo=timezone&logoColor=white)
![VC](https://img.shields.io/badge/vc-14.40-555555?logo=visualstudio&logoColor=white)
![VS2015_Runtime](https://img.shields.io/badge/vs2015_runtime-14.40.3.x-683D87?logo=visualstudio&logoColor=white)
![Wheel](https://img.shields.io/badge/wheel-0.43.0-007ACC?logo=python&logoColor=white)
![ca-certificates](https://img.shields.io/badge/ca--certificates-2024.7.2-3DDC84?logo=ssl&logoColor=white)

![Jupyter Notebook](https://img.shields.io/badge/Jupyter%20Notebook-71%25-F37626?logo=jupyter&logoColor=white)
![SCSS](https://img.shields.io/badge/SCSS-19%25-C76494?logo=sass&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-5.5%25-563D7C?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-3.7%25-F7DF1E?logo=javascript&logoColor=black)
![Other](https://img.shields.io/badge/Other-0.8%25-D3D3D3?logo=other&logoColor=black)


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



