# Emerging_Technologies_Project
## Create conda enviornment

conda create --name `<environment name>`

## Run enviornment

conda activate `<environment name>`

## Install requirements.txt

conda install --file requirements.txt

## Run flask application 

In project directory 
cd Flask
python FlaskApp.py

## The model
In the model I have taken images from the mnist data set to train a neural network on recognising numbers from images.

### Convo2D
When creating the model I used the **Conv2D** layer to create a convolutional kernel that is combined with the layer input to produce a tensor of outputs.

*filters* -  the number of output filters in the convolution
*kernel_size* - specifies the height and width of the 2D convolution window. 
	Can be a single integer to specify the same value for all spatial dimensions.

### MaxPooling2D
I used the **MaxPooling2D** to downscale the input in spacial dimension. I entered a pool_size of (2,2) to halve the horizontal and veritcal spacial dimensions.

*pool_size* - factors by which to downscale.(2, 2) will halve the input in both spatial dimension

### Flatten
I used **Flatten** to reshape the tensor to have the shape that is equal to the number of elements in tensor.

### Dense Layers
And then I had 3 **Dense layers** for the connected neural network layer
