# Neural Network Charity Analysis
### Using machine learning and neural networks to predict whether organizations will be successful if funded by Alphabet Soup.

## Overview
This analysis consists of:
  - Preprocessing Data for a Neural Network Model
  - Compile, Train, and Evaluate the Model
  - Optimization of the Model
  
## Results
### Data Preprocessing
  - The variable IS_SUCCESSFUL is the target of the model
  - NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT are the features used in the model.
  - The columns for EIN, STATUS, and SPECIAL_CONSIDERATIONS were removed from the input data.
  
### Compiling, Training, and Evaluating the Model
  - I used three layers with the tanh activation function, because I used the keras tuner library to help me decide on the best hyperparameters.
  - I used used 100 neurons on the first layer, 30 neurons on the second layer, and 60 neurons on the third layer.
  - I was able able to achieve the target model performance of 75% accuracy.
  - My model had an accuracy score of 75.21%.
  - I did not drop the NAME column from the data. I did drop the EIN, STATUS, and SPECIAL_CONDSIDERTATIONS columns.
  - I also created more bins for rare occurences in columns, and adjusted the number of values for the bins.
  - I added an additional layer to my model, added more neurons to the layers, and changed the activation function for the hidden layers.

<img width="1326" alt="Screen Shot 2022-07-23 at 5 23 26 PM" src="https://user-images.githubusercontent.com/100643519/180624851-0d23a547-9581-4e1e-9be3-a1d83326e68d.png">
  
<img width="1077" alt="Screen Shot 2022-07-23 at 5 20 03 PM" src="https://user-images.githubusercontent.com/100643519/180624775-5439c0ef-94fb-4b8a-8c77-c6f8d702d01c.png">

<img width="930" alt="Screen Shot 2022-07-23 at 5 21 11 PM" src="https://user-images.githubusercontent.com/100643519/180624802-d117f728-c9a3-4268-b727-4d9f3cc6c128.png">

<img width="622" alt="Screen Shot 2022-07-23 at 5 22 19 PM" src="https://user-images.githubusercontent.com/100643519/180624811-7bb7f69b-d70b-416c-b2b6-f09795ae1f25.png">


### Summary
I was eventually able to optimize my model to achieve an accuracy over 75%. The model performed better with three layers than it did when I tried using more layers. When I had more layers and neurons in the model, it was overfitting the data. I tried optimizing the model several times by adjusting the input data, adding more neurons and layers, and using different activation functions, but the models did not have high accuracy scores. I think different data should be used to achieve a more accurate prediction of whether or not the organiztion will be succesful with the funding.
  
