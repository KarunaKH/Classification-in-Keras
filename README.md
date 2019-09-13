# CLASSIFICATION-OF-CATS-&-DOGS
Trained a neural network on differentiating between a cat pic and a dog pic. Then used the trained network to classify a new pic into a cat or dog. Also, tested the model's accuracy by making the model misclassify some cat and dog pics!

# Tools:
1. Google colab
2. Jupyter Notebook
3. HDFView-2.14.0

# Instructions:
1. Use your GMail/GDrive account to log in, click on the '+ New' button at the top left of the page, look for the 'Colab' app and connect it - this will make the app (which connects to the Google Cloud on the other end!) be able to access (read, write) files and folders in your GDrive.

2. You'll notice that the above step created a folder called Colab Notebooks, inside your GDrive - this is good, because we can keep Colab-related things nicely organized inside that folder.

3. Within the Colab Notebooks subdir/folder, create a folder called cats-vs-dogs.

Now we need DATA (images of cats and dogs) for training and validation, and scripts for training+validation and classifying.

4. Download the Data, unzip the folder and upload it into the colab folder you just created.

There are 2000 pics of cats and dogs for training and 800 for validation, with the same folder name. Folder "live" is where we will place our testing data.

5. Place your code in Juptyper Notebook to the Colab folder as well. Double click on the notebook, that will open it so you can execute the code.

6. Before you run the code to kick off the training, note that you will be using GPU acceleration on the cloud (results in ~10x speedup). You'd do this via 'Edit->Notebook settings'.

7. Click the button to execute the code! The first time you run (any anytime after logging out and logging back in), you'd need to authorize Colab to access GDrive - so a dialog will pop up, asking you to click on a link, and copy and paste an authorization code that appears on the clicked page. Once you do this, the rest of the code (where the training occurs) will start to run.

8. The result is a "weights.h5" file. This file stores the weights and biases for each.

Your NEURAL NETWORK IS TRAINED!

9. Place the classify.ipynb Jupyter notebok in the same folder.

10. Supply your testing data to the live folder and Test AWAY!

PS: Output 0=cat and 1=dog.


# Code:
- The code uses the Keras NN library which runs on graph dataflow execution backends such as Tensorflow.
- The backprop loop runs 50 times(also called epochs)


# Accuracy: 82%
This is not bad! Considering there were only 2800 pictures to learn from!\
This goes without saying, the more the data, the better the accuracy of the model!

# Conclusion:
As the model is only 82% accurate, there will be some pics that will be misclassified. For example, the pics placed in this repository under "MISCLASSIFICATION" folder.
