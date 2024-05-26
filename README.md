# Real-Time Facial Expression Recognition Using VGG16 Convolutional Neural Network

## 📚 Introduction
Facial expression recognition (FER) is a significant area of research within computer vision and artificial intelligence due to its practical applications in various fields. Recent advancements in deep learning, particularly convolutional neural networks (CNNs), have significantly enhanced FER capabilities by leveraging large-scale facial expression datasets to automatically learn discriminative features associated with different emotions. This study aims to develop a robust real-time FER system utilizing the VGG16 architecture, evaluated primarily on the FER2013 dataset, to classify distinct facial expressions effectively.

## 💻 Tools and Analysis
The primary dataset used in this study is the Facial Expression Recognition 2013 (FER2013) dataset. This dataset is widely used for training and evaluating FER models. FER2013 comprises 35,887 grayscale facial images, each resized to 48x48 pixels, categorized into seven emotions: angry, disgust, fear, happy, sad, surprise, and neutral. 

![image](https://github.com/hengkisan/FER-python/assets/122197570/3071849b-be3b-4da9-82de-e44e0ba8bcb6)

The development environment chosen is Google Colaboratory (Colab), a cloud-based platform that allows Python code execution in a web browser with GPU acceleration, crucial for training deep learning models requiring significant computational resources. The study adapts the VGG16 architecture, known for its effectiveness in image classification tasks, with modifications to suit the FER2013 dataset's input size and the specific task of emotion classification. 

## 💡 Conclusion
The study evaluates the performance of the developed FER system using metrics like accuracy, precision, and confusion matrices. Key findings can be summarized as below:
- The VGG16 architecture was adapted, featuring 13 convolutional layers and 3 fully connected layers. Batch normalization and L2 regularization were applied to mitigate overfitting. The performance of the models shown in table below.
  
![image](https://github.com/hengkisan/FER-python/assets/122197570/a9463337-bb72-4682-a132-e7ace4b19c43)

- Confusion Matrix: Revealed that 'Happy' and 'Surprise' emotions were most accurately classified, while 'Angry', 'Fear', and 'Sad' were often misclassified among each other.

  ![image](https://github.com/hengkisan/FER-python/assets/122197570/2472dd0c-dacf-4ade-a81e-828b4a7894e6)

- Saliency Maps: Showed that regions around the mouth and eyes were most significant for emotion classification, indicating the model's focus areas.
  
![image](https://github.com/hengkisan/FER-python/assets/122197570/8313c3ea-7b58-464b-80db-786276705ce4)

- The final product includes a real-time FER system using OpenCV for video input processing. The system, detects faces using the Haar Cascade Classifier then crops detected face regions and inputs them to the trained VGG16 model for emotion prediction. Lastly it provides real-time feedback on the predicted emotional state. Figures below are resulted from the model.
  
![image](https://github.com/hengkisan/FER-python/assets/122197570/7f754647-b414-4673-9df8-9989b6ea60ac)
