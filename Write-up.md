# Damaged Cars Detector


## Abstract

In our project, we wanted to develop methods using deeplearning for analyzing images of cars and detecting there body damages,but we are so determent to build a model that can be considered as an added value to any industry that is related to cars.

### Design: 

In our project, we decided to check for car damages in three separate ways, where we first determine whether or not the car is damaged, then we move forward to locate the place of the damage(front, side, or rear) and finally we try to evaluate the severity of that damage(minor, moderate, and severe)
* Damage check
* Damage location check
* Damage severity check


### Data:

Collecting data was manually, and each check had its own dataset:
* Damage check: 2540 damaged cars and 2540 not damaged cars
* Damage location chech: 498 front damages, 320 side damages and 345 rear damages
* Damage severity chech: 327 minor damages, 371 moderate damages, and 455 severe damages

### Algorithms

* Preprcessing:

  * Reshaping
  * Normalization
  * Augmentation
 
* Models:
  * Logistic Regression: we start with this model as a baseline and sometimes we used a single neuron instead
  * CNN: We tried to improve the models by applaying dropout, early stopping, learning rate and different types of optimizer
  * Transfer Learning: we have try to implement four different models, VGG16, VGG19, Inception V2 and Mobile Net V2.


* Model evaluation and selection:

  Data is splitted into train, validation, testing. Accuracy scores of the best model in every check reported as follow:
  |Split     |Damage Check   |Damage Location Check |Damage Severity Check  |
  |----------|---------------|----------------------|-----------------------|
  |Training  |0.9597         | 0.7095               | 0.7806                |
  |Validation|0.9331         | 0.7103               | 0.8587                |
  |Test      |0.9429         | 0.7634               | 0.7378                |


## Tools 
* Pandas
* Numpy
* Scikit-learn
* Matplotlib
* Seaborn
* keras
* Tensorflow

## Communication
* Discord: meeting purposes
* Notion: task management
