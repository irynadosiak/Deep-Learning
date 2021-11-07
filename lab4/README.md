# Homework #4 - Training (Dense) Neural Networks

**Theory.ipynb** 

Contains summaries of the following chapters:
 - Model Selection, Underfitting, and Overfitting
 - Weight Decay
 - Dropout
 - Forward Propagation, Backward Propagation, and Computational Graphs
 - Numerical Stability and Initialization
 - Environment and Distribution Shift

**Code.ipynb**

Contains the source code from the chapter (where appropriate).

**Predicting House Prices.ipynb**

Contains implementing DNN for Predicting House Prices. K-Fold cross-validation, model selection were used. Besides, the work contains different weights initializations, at least:
- RandomNormal 
- GlorotNormal
- HeNormal
- LeCunNormal
- 
Also the work contains different activation functions to all your layers (at once) - except the output layer: 
- sigmoid
- tanh
- relu
- elu
- selu
- gelu
Moreover, the notebook Predicting House Prices.ipynb includes the implementations of all the callbacks (Early Stopping, LR Decay on Plateau, ModelCheckpoint) in all the subsequent setups.
TensorBoard dashboards with learning curves (train and validation) are included to every experiment reported in the notebook.

**Callbacks.ipynb**
Contains implementing and brief explanation of Early Stopping, LR Decay on Plateau, ModelCheckpoint.

**Set up TensorBoard.ipynb**
Shows how to install and use TensorBoard dashboard.

**Exercises.ipynb**
Includes every exercise execution (https://d2l.ai/chapter_multilayer-perceptrons/kaggle-house-price.html#exercises). In addition, there is a brief summary of what approach worked best and what was the most influential change.
