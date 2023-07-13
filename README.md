# Tumor-Detection-Transfer-Learning

## Concept:
### Using Transfer Learning to import an Xception model to analyze brain MRIs and state if tumors are present or not

## What is Transfer Learning?
### Transfer learning is a machine learning technique where a model trained on one task is re-purposed on a second related task. 
### Transfer learning is a powerful technique that can be used to improve the performance of machine learning models on a variety of tasks. It is especially useful in cases where there is limited data available for the new task, like the one we're undertaking now.

### There are two main approaches to transfer learning, Fine tuning and Feature extraction. In our case, We'll be taking the Fine tuning approach, where The new model is then trained on the data for the new task, while also fine-tuning the weights of the pre-trained model.

### Some of the benefits of transfer learning are : Improved Performance, Reduced Data Requirements and Faster Training, particularly in image classification tasks.

## Working Process:
### 1) Importing the required models.
### 2) Importing the data from Google Drive and Preprocessing the data ( designing the rescaling functions using Keras layers)
### 3) Importing the pre-trained model for transfer learning (Xception)
### 4) Exclude the top layers, freeze the base layers a nd add our own custom top layers, along with rescaling layer.
### 5) Compile and Train our new model on our dataset with callbacks.
### 6) Test for our model's efficiency by plotting loss and accuracy, as well as assesing model performance using classification metrics
### 7) Saving our model in Google Drive Cloud

## Points to note :
### We have imported Xception here due to the small nature of the dataset. Depending on the type, novel features, size and other major properties of our dataset, as well as the nature of our task and our computational power, the model to be imported and the additional steps to be taken will differ. Take care to ensure you import and design your model workflow accordingly.

### We deciced to stick to just 15 epochs here due to time and computational power constraints, as well as satisfaction with obtained results of 96% accuracy and 97% F1 Score. Even with the same model and dataset, different training optimisations can be performed

## Possible Future Updates:
### 1) Deployment of model via Streamlit
### 2) Further training optimizations with our model
### 3) Attempts to try out different pre trained models for transfer learning

