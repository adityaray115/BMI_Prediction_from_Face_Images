
# BMI Prediction from Face Images

BMI - Body Mass Index is a value which is used to determine whether a person is underweight, overweight or in normal range when compared to their body height. 
## Dependencies
* Python 3.6
* matplotlib
* numpy 
* Pandas
* face-recognition

face-recognition does not give native support to windows. It is available for linux ans MacOS, and can be installed simply with pip command. 

For windows follow this link: https://www.youtube.com/watch?v=xaDJ5xnc8dc 

They have explained in step-by-step manner on how to install it for windows.
## Dataset

Since this project uses sensitive information like person's photographs, weight and height, data is not readily available over internet. Therfore dataset was created from scratch using publically available photographs of celebrities and famous personalities.

200 photographs (100 of males and females each) along with their weight and height from various different websites. This can probably introduce inaccuracy into the model but this is no other way to obtain such information.
## Models Trained

Following models were selected and they gave accuracies as shown in the table.

| Model  | Height Accuracy | Weight Accuracy | BMI Accuracy | 
| --- | --- | --- | --- |
| Linear Regression | 94.30% | 12.67% | 17.02% |
| Ridge Linear Regression | 93.30% | 97.58% | 96.15% |
| Random Forest Regression | 93.95% | 97.78% | 96.43% |
| Kernel Ridge Regression | 93.48% | 97.75% | 96.32% |
| Support Vector Regression | 91.53% | 98.07% | 97.25% |

Among all these I concluded SVR as the best model since it performed best in terms of BMI Accuracy.
