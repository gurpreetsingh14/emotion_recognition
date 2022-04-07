# emotion_recognition
Emotion detection through facial expression recognition using CNN and Transformer architecture

The RAF-BD dataset can be downloaded from the link below (basic expressions only):

https://drive.google.com/drive/folders/0B4E10azXECctRUgwVmFPblFUdUE?resourcekey=0-SCrrCMK2lc4IDmhDsDKhRw

**About the dataset**

7 labels: Surprise, Fear, Disgust, Happiness,Sadness, Anger, Neutral

Composition:
![image](https://user-images.githubusercontent.com/84365378/162112930-0608bb99-b273-4096-bc24-a9fff7478ded.png)

**Models**

  + **VGG16 & EfficientB0** as a benchmark, we build these models with 7 output classes and we trained the weights from scratch. We then used transfer learning, and used their pre-trained ImageNet weights with the first layers frozen and only trained the top layers. Finally, we used fine-tuning.

  + **Five Layer & Deep CNN** we first started building a neural network with only five convolution layers. Then we trained deeper neural networks by varying the convolution layers hyperparameters and adding additional fully connected layers.

  + **ViT (Visual Transformer)** is a SOTA technique in image classification.We started by using the ViT model with attention architecture from the PyTorch library and trained on the RAF-BD dataset. In the second model, we used a pre-trained ViT (imagenet21k) model and fine-tuned it on the RAF-BD dataset.

More stuff will be added soon.
