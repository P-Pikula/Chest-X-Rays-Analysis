# Chest-X-Rays-Analysis
Identifying Pneumonia in Chest X-Rays by Image-Based Deep Learning (Classification problem)

Dataset: https://www.kaggle.com/datasets/tolgadincer/labeled-chest-xray-images

## Inspiration

X-Ray imaging is one of the oldest and still one of the most prevalent methods of medical imaging. X-ray is the life-saving technology that was actually invented by accident.

The risk of pneumonia is immense for many, especially in developing nations where billions face energy poverty and rely on polluting forms of energy. The WHO estimates that over 4 million premature deaths occur annually from household air pollution-related diseases including pneumonia.

Fast diagnosis can guarantee timely access to treatment and save much needed time and money for those already experiencing poverty.

## The goal

Build an algorithm to automatically identify whether a patient is suffering from pneumonia or not by looking at chest X-ray images. The algorithm had to be extremely accurate because lives of people is at stake.

## Approach

Dataset comes from Kaggle. It contains 5856 samples divided into train and test sets categorized into two groups: Normal and Pneumonia. Both sets seem imbalanced having more samples with "Pnenumonia" label. After data exploration train dataset is being divided to create a validation set.

Due to low number of samples data augmentation is being used to tackle the imbalance problem by presenting larger number of cases to the model.

Models are convolutional neural networks compromising of different number of convolutional layers. First two models are built from scratch. Third one is using pre-trained model provided by Keras - DenseNet121.

## Result

The second model attained good capabilities having only 3,715,169 parameters and size of 42,7 MB.


## Libriaries used
- ML: Tensorflow / Keras
- Data visualisation and manipulation: Pandas, Numpy, Matplotlib, Seaborn, CV2
