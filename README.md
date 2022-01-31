# Neural_Network_Charity_Analysis

Overview of the Analysis
Using Machine Learning and Neural Networks for this project, I used the features in the dataset to create a binary classifier that will help to predict if the applicants that will be funded by a Charitable organization called Alphabet Soup will be successful. For this analysis we had a dataset containing various measures on 34,000 organizations that in the past have been funded by Alphabet soup over the years. within the data some of the labels is the following:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

out of this labels above we removed or drop the EIN and Name since we believe they hold no real value to our model predictions and for our attempts after that we adjust this paramaters again and removed use case.

our target was status succesful

What we had to create:
Preprocessing the data for the neural network
Compile, Train and Evaluate the Model
Optimizing the model (final result)

Results:
after preprocessing all the data and getting ready for nueral network training we created and train our initla module. The result can be view in the following image.

<img width="599" alt="Screen Shot 2022-01-30 at 9 12 44 PM" src="https://user-images.githubusercontent.com/90356052/151737996-458cb139-5ae4-49fb-8ad3-2163f579ac70.png">
 
after following the results we see our accuracy was 69% and our loss was 95% (rounding). We attempted to mitigate our loss and increased our accuracy by optimizing the model to run different activation functions, different number of layers, number of epochs, and number of neurons in each layer the results are as follow:

attempt 1 parameters: 
input activation functio: sigmoid 
output activation functio: sigmoid 
number of layers and neuros: layer1-80 layer2-30 epochs 50

<img width="599" alt="Screen Shot 2022-01-30 at 9 27 04 PM" src="https://user-images.githubusercontent.com/90356052/151738932-6540021b-dc30-4aae-acab-b4b0a8ff4464.png">

attempt 2 parameters: 
input activation functio: relu
output activation functio: sigmoid 
number of layers and neuros: layer1-100 layer2-50 layer3- 30 epochs 30

<img width="599" alt="Screen Shot 2022-01-30 at 9 27 04 PM" src="https://user-images.githubusercontent.com/90356052/151739097-d8da5fde-f4c8-4f9b-8fab-4a847b83208b.png">

attempt 3 parameters: 
input activation functio: relu
output activation functio: sigmoid 
number of layers and neuros: layer1-100 layer2-75 layer3- 50 layer4-25 epochs 30

<img width="599" alt="Screen Shot 2022-01-30 at 9 35 01 PM" src="https://user-images.githubusercontent.com/90356052/151739433-de44c9ef-feb3-4c63-bcd7-73d7acbc9dc9.png">

as you can see by all the images the results vary, but our intial model along with our third attempt seem to have had the highest accuracy scores. Is also important to point out that our intila model with the accuracy of 69% had a huge loss of 94 compared to our third attempt which had 67% and only 63% loss. By this measurements we did not reach our target model performance of 75%, but in my opinion model attempt 3 would be more effective than our original model due to how close in accuracy they both are and how low the loss is in attempt 3 next to original model.  

