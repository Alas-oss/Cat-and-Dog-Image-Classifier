# Cat and Dog Image Classifier (CNN)

The objective of this project was to build a convolutional neural network (CNN) that can distinguish between images of cats and dogs. It is a binary image classifier that can work with either grayscale or color images. 

## My Contribution
- Processed the dataset and separated it into different sections (training, validation, and unlabeled)
- User ImageDataGenerator to nomalize image pixel values and apply augmentation (rotation, zoom, flip, etc.) to reduce overfitting
- Built a CNN architecture using **tf.keras.Sequential**:
  - Stacked Conv2D and MaxPooling2D layers
  - Flattened the output and passed it through dense layers
  - Used a sigmoid output layer for binary classification
- Trained the model using:
  - Binary cross-entropy loss
  - Adam optimizer
  - Accuracy as the evaluation metric
- Achieved and visualized training/validation accuracy and loss across epochs
- Made predictions on unseen test images using ```model.predict()```
- Used a ```plotImages()``` helper function to display:
  - The model's predicted class ("cat" or "dog")
  - Confidence score for each test image
 
## Key skills developed
- Learned to work with image datasets and folder structures
- Built a full **CNN pipeline** for binary image classification
- Applied data augmentation to combat overfitting
- Practiced model evaluation, visualization, and prediction using TensorFlow/Keras
