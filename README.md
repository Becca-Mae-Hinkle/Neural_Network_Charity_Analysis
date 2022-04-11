# Neural_Network_Charity_Analysis

## Overview

The Alphabet Soup Company is wanting to provide funding to applicants but wants to use machine learning to predict whether aplicants will be succesful or not. We received a CSV containing 34,000 organizations that have received funding over the years. We will take this data and compile, train and evaluate the neural network model.

## Deliverable 1

* Data Processing
      * To clean the data I removed the EIN and NAME columns since they are "noisy" columns and don't contribute any value to the model.
      * A list of categorical variables was made with: 'STATUS', 'ASK_AMT', 'IS_SUCCESSFUL', 'APPLICATION_TYPE', 'CLASSIFICATION', 'USE_CASE',                     'ORGANIZATION', 'INCOME_AMT'as the target variables and dropping "USE_CASE_Other","AFFILIATION_Other".
      * My dependent variable is "IS_SUCCESFUL" since we want to predict high accuracy.       

<img width="1184" alt="Deliverable 1" src="https://user-images.githubusercontent.com/94575416/162646591-fff346ba-18a7-4347-81b7-e2d2e76aa6a4.png">

## Deliverable 2

* Compile, Train and Evaluate
      * Continuing to use the data from Deliverable 1 we are ready to start using the neural network. After evaluating the model using the test data we             ended up with a Loss: 0.5686031579971313 and Accuracy: 0.7222157716751099.
      
<img width="850" alt="Deliverable 2" src="https://user-images.githubusercontent.com/94575416/162646920-f50a0002-80e5-4a07-8fbb-3687c7ddd908.png">


## Deliverable 3

We will attempt 4 different ways to reach the accuracy the client is asking for by manipulating the data inside the neural network.

   * Attempt 1:
        * 2 hidden layers
        * 80 neurons (Layer 1), 30 neurons(Layer 2)
        * Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for nonlinear datasets.
        * Removed "USE_CASE_Other","AFFILIATION_Other" columns.

  <img width="759" alt="Attempt 1" src="https://user-images.githubusercontent.com/94575416/162647298-2a5a8a1e-0f0b-4ef0-a12c-20e735754237.png">
  
  * Attempt 2:
        * 3 Hidden Layers
        * 80 neurons (Layer1), 30 neurons(Layer2), 15 neurons(Layer3)
        * Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for nonlinear datasets.
        * Removed "USE_CASE_Other","AFFILIATION_Other" columns.

<img width="867" alt="Attempt 2" src="https://user-images.githubusercontent.com/94575416/162651915-e5a87720-b82d-4b50-ab29-7a4c1a41eedf.png">


  * Attempt 3:
        * 3 Hidden Layers
        * 80 neurons(Layer1), 35 neurons(Layer2), 10 neurons (Layer3)
        * Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for nonlinear datasets.
        * Went back to original dataset

<img width="844" alt="Attempt 3" src="https://user-images.githubusercontent.com/94575416/162652456-f33cad32-428f-4942-b4b3-b851eb2d6b5b.png">

  * Attempt 4:
        * 3 Hidden Layers
        * 80 neurons (Layer1), 30 neurons(Layer2), 15 neurons (Layer3)
        * Reordered Relu and Sigmoid Activations
        * Went back to original dataset

<img width="767" alt="Attempt 4" src="https://user-images.githubusercontent.com/94575416/162652627-931fbaad-aeb5-4cd3-b8d0-368b37cfa09d.png">


I made changes to try to get as close to a 75% accuracy rate but was unable to achieve that. Changing the hidden layers, number of neurons and the features were unable to reach that output.

## Summary

The deep learning neural network did not reach the targeted 75% accuracy. Considering that this target level is pretty average we could say that the model is not outperforming. If given more than a day and more changes maybe we could reach the accuracy the client was wanting. I am pretty happy with what we were able to achieve. Since we are in a binary classification situation, we could use a multitude of decision trees to generate a classified output and evaluate its performance.
















