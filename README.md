# Neural_Network_Charity_Analysis

Overview of the Analysis
---------------------

In the challenge I had to preprocess the data for the neural network, compile, train and evaluate the model, and lastly optimize the model in order to predict if the 
applicants being funded by Apple Soup Charity, would be successful.

Results
--------

Data Processing
----
* Variable considered the target for the model: IS_SUCCESSFUL column.
* Variables that are considered to be features: All columns minus IS_SUCCESFUL column and the columns that were dropped.
* Variables neither targets or features and should be removed from input data: EIN and NAME.


Compiling, Training and Evaluating 
-----
* For my model I had 2 hidden layers, the first one had 80 neurons and the second, 30 neurons.

<img width="660" alt="image" src="https://user-images.githubusercontent.com/106127571/193434967-f336a9b2-baa5-405d-9633-0272231206d1.png">


* The model was not able to reach the target 75%. The accuracy for my model was 69%.

<img width="669" alt="image" src="https://user-images.githubusercontent.com/106127571/193434984-8d384155-5cbe-4168-8de6-49f59375e4a5.png">


Steps Taken to Try and Increase Model Performance
-----

* 1st Attempt: Remove the 'USE_CASE' columns. Model accuracy increased to 63%.

* 2nd Attempt: Adding more neurons to hidden layers and adding additional hidden layers. Model accuracy increased to 71%.

<img width="675" alt="image" src="https://user-images.githubusercontent.com/106127571/193435106-5a1cef57-7a9b-4d88-9906-2dd030db477e.png">


<img width="671" alt="image" src="https://user-images.githubusercontent.com/106127571/193435135-5aac871f-b68d-4a0a-8eca-bf2876da06c4.png">

* 3rd Attempt: Change outer layer from "sigmoid" to "tanh". Model accuracy decreased to 47%.

<img width="639" alt="image" src="https://user-images.githubusercontent.com/106127571/193435188-3624a12a-11b9-4aa9-9830-645ddc206957.png">

<img width="668" alt="image" src="https://user-images.githubusercontent.com/106127571/193435203-9ffdc16c-ed96-46e0-926f-0d4fe0ea0cb1.png">


Summary
-------

After optimization the model ended up with an accuracy of 47%; dramatically decreased from the first neural network accuracy of 69%.




