# Classifying Images of Dogs and Cats

## Data
**Data source** = https://www.kaggle.com/c/dogs-vs-cats

The data contain 25000 images which are contain 12500 images of cat and 12500 images of dog:

![alt text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Image%20Classification/Assets/Cat.png)

![alt text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Image%20Classification/Assets/Dog.png)

## Data Preprocessing

**Data Augmentation**

I randomly transform the images of the train data to be rotated, zoomed, shifted, sheared, and flipped.  It was done to make the model to be more robust to recognize the object. I also make the size of the image to rescale into 224 x 224. 

![alt text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Image%20Classification/Assets/Original%20vs%20Augmented.png)

## Model Architecture

![alt text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Image%20Classification/Assets/Model%20Architecture.png)

## Results

**Learning Graph**

![alt_text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Image%20Classification/Assets/Learning%20Graph.png)

**Confussion Matrix and Classification Report**

![alt text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Image%20Classification/Assets/Result.png)
