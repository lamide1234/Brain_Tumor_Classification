# Brain_Tumor_Classification

This project aims to build and evaluate Convolutional Neural Network (CNN) models for brain tumor detection and classification from MRI scans. It is structured in two stages:

Stage 1: Binary classification — Tumor vs No Tumor

Stage 2: Multi-class classification — Tumor Type (Glioma, Meningioma, Pituitary)

📁 Dataset
The dataset is split into two categories:

tumor_or_notumor/: For binary classification.

type_of_tumor/: For multi-class classification.

You can access the dataset via this Google Drive link:

🔗 [Google Drive – Brain Tumor images](https://drive.google.com/drive/folders/12hXYE9Q9Cth6C_l6XshyhWUAAAhEO4px?usp=drive_link)



🛠️ Preprocessing & Data Augmentation
Balanced the dataset by augmenting the "No Tumor" class (originally underrepresented).

Applied transformations like rotation, zoom, shift, shear, and flipping using ImageDataGenerator.

🧪 Model Architecture
The model is built using TensorFlow/Keras and consists of:

Convolutional layers with ReLU activation

Batch Normalization and MaxPooling

Fully connected Dense layers

Dropout for regularization

Softmax output for classification

The model uses the Adam optimizer and categorical crossentropy as the loss function.

📈 Training & Evaluation
Models are trained on 80% of the training data, validated on 20%.

Metrics tracked: Accuracy, Loss, Confusion Matrix, and Classification Report.

Training history is plotted to visualize performance over epochs.

🧪 Results
Performance was evaluated using:

Confusion Matrix to visualize predictions

Classification Report with precision, recall, and F1-score

Accuracy and loss plots for both training and validation


  Future Work

Apply transfer learning using pretrained models (e.g., VGG, ResNet)

Improve model robustness with more diverse datasets

Extend to real-time classification or segmentation tasks
