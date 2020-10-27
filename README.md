# ML-PHY5G-Beam-Selection
By using Coordinates as input we have added few more layers in the existing model. 



# Result
We have achieved training acuracy of 76.05% and test accuracy 72.69%. We have uploaded our predictions of s009 test dataset in output.txt file.

Output.txt Link: https://drive.google.com/file/d/1gK3KOO57GV0FJaL3sZ3eBctrgV_N9cue/view?usp=sharing 


By using Coordinates as input we have added a few more layers in the existing model.

# Model : 

We modified the model in the ModelHandler.py file for the coordinates section (‘coord_mlp’). We are training only over coordinate inputs and used the model in following structure:
4 Dense layers of size 16
2 Dense layers of size 64
2 Dense layers of size 128
2 Dense layers of size 256
Softmax layer at the end for 3 classes


# Instructions to run the code:

ITU_Beam.ipynb is the main code which includes both the beam_train_model and beam_test_model. This code can be used to generate the required output.

<b> Note : </b> Please note that we have considered only Coordinates dataset of Baseline data to train as well as test the model. 

In the third cell of ITU_Beam.ipynb, you can change the Training as well as Test data path as per the requirement (Please ensure that only coordinates dataset is provided).
The Last cell in ITU_Beam.ipynb, predicts the output of test data.



<b> Output Result :</b>

We have achieved training accuracy of 76.05% and test accuracy 72.69% for 10 best beams. We have uploaded our predictions of the s009 test dataset in the output.txt file (Pl. check the github link provided for the same). 
