# Age detection of customers from a photograph

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/3aa4bea6c1e42ac87a4f471651cbefc30ebf6d9f/DS%2008%20Face%20age%20recognition/Face_age_recognition.ipynb)

## Project Description

The goal of this project is to determine the approximate age of a person based on a photograph using a dataset of labeled images of people with their ages.

## Project Execution

### Data Upload and EDA
- The data is provided in the form of photographs and labeled ages.
- The age distribution in the dataset is imbalanced, with the most common age group being between 20-30 years old.
- Photographs of people over the age of 60 are less common in the dataset, which may result in poorer model performance on such photographs.

### Model Training
- A three-layered neural network ResNet50 without augmentation was created with a ReLU activation function and an Adam optimizer.

## Skills and Tools

- **python**
- **pandas**
- **numpy**
- matplotlib.**pyplot**
- tensorflow.keras.models.**Sequential**
- tensorflow.keras.layers.**Dense** **GlobalMaxPooling2D**
- tensorflow.keras.applications.resnet.**ResNet50**
- tensorflow.keras.optimizers.**Adam**
- tensorflow.keras.preprocessing.image.**ImageDataGenerator**



## Conclusion

The model was trained on a dataset of 7591 labeled photographs. The dataset is imbalanced, with the most well-represented age group being between 20-30 years old, as well as preschool children. The validation set was 25%. A three-layered neural network ResNet50 without augmentation was used. The result for the mean absolute error metric was less than 8, which is sufficient for the age detection task for this store. The business task of determining the age of customers should be solved, as the most well-represented labeled age group corresponds to the most active age group in terms of purchasing activity.
