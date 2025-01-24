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

![dataset](https://github.com/user-attachments/assets/4f84caae-71bb-4100-83c7-0856b17540c2)

The dataset used in this project is a specialized collection of images intended for the classification of Autism Spectrum Disorder (ASD). It is organized to facilitate the training and evaluation of various deep learning models.

**🔑 Key Characteristics:**

**📂 Source and Structure:** The dataset, referred to as "AutismDataset" in the notebook, is structured into directories, with subfolders representing different classes. This structure allows for easy ingestion into deep learning models using image data generators.

The data is initially stored in a consolidated folder and is then split into training and validation sets using the splitfolders library. The split ratio used is 70% for training and 30% for validation.
  
  **1. 🖼️ Image Properties:**
    
  - **📏 Image Size:** All images are resized to 128x128 pixels to ensure uniformity across the dataset, which is crucial for feeding the data into convolutional neural networks.
    
  - **🌟 Image Scaling:** The pixel values of the images are rescaled to a range of 0 to 1. This normalization helps stabilize the training process and improve the model's convergence.
  
  **2. 🔄 Data Augmentation:**
    
  - **Training Set:** Data augmentation techniques are applied to the training set to improve the generalization of the model. This includes shearing, zooming, and horizontal flipping, which artificially increases the variety of the training data and helps the model learn more robust features.
    
  - **Validation Set:** Only scaling is applied to the validation set, ensuring that the data remains representative of real-world conditions without introducing synthetic variations.
  
  **3. 🧩 Class Distribution:** The dataset is divided into different classes, each representing a specific category within the Autism Spectrum Disorder diagnosis. The exact classes are not detailed in the notebook, but they are structured to support a categorical classification task.
This dataset is well-suited for training deep learning models aimed at diagnosing Autism Spectrum Disorder, with careful consideration given to data preparation and augmentation to maximize the performance of the models.

## 🔄 **Model Workflow**

![model workflow](https://github.com/user-attachments/assets/36f47ab8-a5cb-4d49-bba0-427da05da1e0)

### 📝 **Overview:**
This section outlines the specific steps followed in the deep learning workflow used in this project for Autism Spectrum Disorder classification, as implemented in the provided Jupyter Notebook.

**1. 🗂️ Data Preparation:**
The initial stage involves organizing and preprocessing the dataset:

  - **📁 Data Splitting:** The dataset is divided into training and validation sets using the splitfolders library. This ensures a proper split between the data for training the model and validating its performance.
  - **📏 Image Rescaling:** Images are scaled to a standard size of 128x128 pixels. This uniformity is crucial for feeding the data into the neural network.
  - **🔄 Data Augmentation:** To enhance the training set, data augmentation techniques such as shearing, zooming, and horizontal flipping are applied. This helps the model generalize better by learning from a wider variety of data.

**2. 🏗️ Model Architecture:** The notebook demonstrates the use of several advanced deep learning models, each contributing unique strengths to the Autism Spectrum Disorder classification task:

  - **🔍 GoogleNet:** Also known as Inception, GoogleNet is a convolutional neural network architecture that introduces the inception module, allowing the network to consider multiple filter sizes for each convolutional layer.

  - **🔗 ResNet:** Short for Residual Networks, ResNet addresses the vanishing gradient problem in deep networks by using skip connections, allowing gradients to flow through the network more effectively and enabling the training of very deep networks.

  - **⚡ XceptionV3:** Xception is an extension of the Inception architecture that replaces the standard inception modules with depthwise separable convolutions, significantly improving performance and computational efficiency.

  - **🌐 DenseNet:** DenseNet (Densely Connected Convolutional Networks) connects each layer to every other layer in a feed-forward manner, which helps in reusing features, reducing the number of parameters, and improving gradient flow.

  - **⚙️ Xception:** Similar to XceptionV3, this model uses depthwise separable convolutions and is based on the Inception architecture. It's designed to be more efficient and achieve better performance by optimizing the convolution operations.

  - **📱 MobileNet:** MobileNet is a lightweight convolutional neural network architecture optimized for mobile and embedded vision applications, focusing on reducing the computational cost while maintaining performance.

These models were selected for their ability to handle complex image classification tasks effectively, each bringing a unique approach to feature extraction and network efficiency.

**3. 🏋️ Model Training:** The training process includes the following:

  - **🧰 Data Generators:** ImageDataGenerator is used for loading and augmenting the images in batches. This allows efficient handling of large datasets by feeding the model with data in real-time.
  - **⚙️ Training Parameters:** The model is compiled with specific loss functions and optimizers suitable for multi-class classification, such as categorical_crossentropy and optimizers like Adam.
  - **📦 Batch Processing:** The model is trained using small batches of data, with the training set providing data for learning and the validation set used to tune the model.

**4. 📊 Model Evaluation:** Post-training, the model's performance is evaluated using:

  - **📈 Accuracy Metrics:** The accuracy of the model on the validation set is calculated to assess its ability to generalize to new data.
  - **📉 Loss Curves:** The loss during training and validation is plotted to check for overfitting or underfitting.
    
**5. 🚀 Model Deployment:** Though the notebook primarily focuses on training and evaluation, deploying the model typically involves:

  - **💾 Saving the Model:** The trained model is saved in a format like .h5 for future use in production environments.
  - **🖥️ Integration with the Dashboard:** The model is integrated into an interactive dashboard where users can input new data and receive predictions in real-time.

**🛠️ Visual Workflow:**
A visual representation of this workflow, including data preprocessing, model architecture, training, and evaluation, is presented in the dashboard to offer a clear understanding of the entire process.



## 🚀 **User Interactive Dashboard**

### **Overview**

The User Interactive Dashboard is designed to provide an intuitive interface for exploring the model's performance and classification results. Users can interact with the dashboard to gain insights into the classification outcomes and understand the deep learning model's predictions in a clear and accessible manner.

### **Index Page**

This is the landing page of the dashboard where users can access the main functionalities. It provides a summary of the model's capabilities and guides the user on how to proceed with classification.

![app index page](https://github.com/user-attachments/assets/4a3e97e8-6325-42cf-9532-3fd9d5ce716e)

### **Classification Results Page:**

 The Classification Results Page displays the model's predictions, detailing whether the input data indicates a diagnosis of Autism Spectrum Disorder (ASD) or Non-Autistic. This page is critical for users looking to understand the model's decision-making process.

#### *Example - Non-Autistic Result* 
Here, the model's output indicates that the subject is non-autistic. The page visualizes the prediction along with confidence scores and relevant details.
  
![app results page na](https://github.com/user-attachments/assets/38193960-ee26-4f87-8f71-1e6b84044f5a)

### **Classification Results Page:**

#### *Example - Autistic Result*
In this scenario, the model predicts the subject as autistic. Users can view the prediction, analyze contributing factors, and see confidence levels associated with the decision.

![app results page aus](https://github.com/user-attachments/assets/b613994b-cb1a-44d6-9311-3c29573f85e0)


## 🎯 **Conclusion & Future Work**

This project implemented and compared several deep learning models, with Xception and MobileNet showing the highest accuracy. An interactive dashboard was developed to visualize and explore model performance. 

### 🔮 *Future Work*
- **Model Refinement**: Further refine the models to enhance their diagnostic accuracy.
- **Dashboard Enhancement**: Improve the interactive dashboard for better visualization and user experience.
- **Real-World Deployment**: Deploy the system in real-world applications for practical use.
- **Ensemble Techniques**: Explore ensemble techniques to further boost the accuracy of ASD detection.

## **References**

📚 References
  1. **National Institute of Mental Health (NIMH)** 🌐. [Autism Spectrum Disorder](https://www.nimh.nih.gov/health/topics/autism-spectrum-disorders-asd).
  
  2. **Jana Christina Koehler, Mark Sen Dong, Afton M. Bierlich, Stefanie Fischer, Johanna Spath, Irene Sophia Plank, Nikolaos Koutsouleris & Christine M. Falter-Wagner.** “Machine learning classification of autism spectrum disorder based on reciprocity in naturalistic social interactions.”
  
  3. **Md. Mokhlesur Rahman, Opeyemi Lateef Usman, Ravie Chandren Muniyandi, Shahnorbanun Sahran, Suziyani Mohamed, and Rogayah A Razak.** “A Review of Machine Learning Methods of Feature Selection and Classification for Autism Spectrum Disorder.”
  
  4. **Md. Zasim Uddin, Md. Arif Shahriar, Md. Nadim Mahamood, Fady Alnajjar, Md. Ileas Pramanik, Md Atiqur Rahman Ahad.** “Deep learning with image-based autism spectrum disorder analysis: A systematic review.”
  
  5. **Ibrahim Abdulrab Ahmed, Ebrahim Mohammed Senan, Taha H. Rassem, Mohammed A. H. Ali, Hamzeh Salameh Ahmad Shatnawi, Salwa Mutahar Alwazer, and Mohammed Alshahrani.** “Eye Tracking-Based Diagnosis and Early Detection of Autism Spectrum Disorder Using Machine Learning and Deep Learning Techniques.”

## 📜 **LICENSE**

This project is licensed under the MIT License. Feel free to use, modify, and distribute this project under the terms of the MIT License.

## 🤝 **Contributions**

Contributions to the project are welcome! If you have any suggestions or questions, please feel free to reach out via email at [divyatanuja17@gmail.com](mailto:divyatanuja17@gmail.com).



