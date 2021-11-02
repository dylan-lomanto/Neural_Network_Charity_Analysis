# Neural_Network_Charity_Analysis

### Overview
This anaylsis is completed on behalf of the investment firm Alphabet Soup. The client has provided a CSV of 34,000 organizations that they have funded. The aim of the analysis is to use this data to develop a neural network that can predict whether or not an organization will achieve its goal if funded by Alphabet Soup based upon the data fields provided in the CSV.

### Results

##### Data Preprocessing
1. The target variable is 'IS_SUCCESSFUL'. This variable determines whether or not the funding money provided by Alphabet Soup was used effectively.
2. The feature variables for the first model are all variables other than 'IS_SUCCESSFUL', except for the columns that were dropped.
3. The variables that were removed from the first model are 'EIN', and 'NAME'.  'SPECIAL_CONSIDERATIONS' and 'STATUS' were dropped for subsequent models.
![drop columns original](https://user-images.githubusercontent.com/86164867/139950037-0d1e5c87-0435-4171-b95e-fd0dee13e697.PNG)
![drop columns optimized](https://user-images.githubusercontent.com/86164867/139950052-ffb66ccc-4e0b-4bda-a3b8-0cf4641983e1.PNG)


##### Compiling, Training, and Evaluating the Model
1. The initial model had two hidden layers, with 80 neurons in the first layer and 30 in the second. The activation functions for both hidden layers were ReLU and the funtion for the output layer was sigmoid.  Subsequent models added a hidden layer, increased the neurons to 120, 60, and 20, and changed the activation functions for all three hidden layers to sigmoid. The additional layer, extra neurons, and activation funciton change were all excecuted with the hope of increasing the accuracy fo the model to greater than 75%.
![original model](https://user-images.githubusercontent.com/86164867/139957315-cec13524-2c93-43dc-88f0-f0c29b646336.PNG)
2. Despite the changes, the model was never able to achieve the the target accuracy. The original model came the closest, with an accuracy of 72.97%. The optimization models had accuracy scores of 72.92%, 72.71%, and 72.8%.
![original model accuracy](https://user-images.githubusercontent.com/86164867/139957594-a01eb472-579a-4b54-a681-91996a82c9c6.PNG)
3. The optimized models added a hidden layer, increased the neurons to 120, 60, and 20, and changed the activation functions for all three hidden layers to sigmoid.
![3rd optimized model](https://user-images.githubusercontent.com/86164867/139957192-91df19bd-ede0-49e4-bc8a-e91e1fc4c183.PNG)


### Summary
The deep learning model was never able to surpass the initial accuracy score of 72.97%.  
