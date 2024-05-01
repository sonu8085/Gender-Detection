# Gender detection using deep learning models 
The keras model is created by training model from scratch on around 2200 face images (~1100 for each class). Face region is cropped by applying `face detection` using `cvlib` on the images gathered from Google Images. It acheived around 96% training accuracy and ~90% validation accuracy. (20% of the dataset is used for validation)


## Python packages used

* keras
* tensorflow
* numpy
* opencv-python
* cvlib
* scikit-learn
* matplotlib
* protobuf

Install the required packages by executing the following command.

`$ pip install -r requirements.txt`

**Note: Python 2.x is not supported** 

Make sure `pip` is linked to Python 3.x  (`pip -V` will display this info).

If `pip` is linked to Python 2.7. Use `pip3` instead. 
`pip3` can be installed using the command `sudo apt-get install python3-pip`

Using **Python virtual environment** is highly recommended.

## Usage

### image input
`$ python detect_gender.py -i <input_image>`

### webcam
`$ python detect_gender_webcam.py`

### Sample output :

![](sample_output.jpg)

## Training
You can download the dataset I gathered from Google Images from this [link](https://github.com/arunponnusamy/gender-detection-keras/releases/download/v0.1/gender_dataset_face.zip) and train the network from scratch on your own if you are interested. You can add more images and play with the hyper parameters to experiment different ideas. 

# Gender detection (from scratch) using deep learning with keras and cvlib
The keras model is created by training [SmallerVGGNet](model.png) from scratch on around 2200 face images (~1100 for each class). Face region is cropped by applying `face detection` using `cvlib` on the images gathered from Google Images. It acheived around 96% training accuracy and ~90% validation accuracy. (20% of the dataset is used for validation)

## Update :
Checkout the gender detection functionality implemented in [cvlib](https://github.com/arunponnusamy/cvlib) which can be accessed through a single function call `detect_gender()`. 

## Python packages
* numpy
* opencv-python
* tensorflow
* keras
* requests
* progressbar
* cvlib



## Usage

### image input
`$ python detect_gender.py -i <input_image>`

### webcam
`$ python detect_gender_webcam.py`

When you run the script for the first time, it will download the pre-trained model from this [link](https://github.com/arunponnusamy/cvlib/releases/download/v0.2.0/gender_detection.model) and place it under `pre-trained` directory in the current path.

(If `python` command invokes default Python 2.7, use `python3` instead)

### Sample output :

![](sample_output.jpg)

## Training
You can download the dataset I gathered from Google Images from this [link](https://github.com/arunponnusamy/gender-detection-keras/releases/download/v0.1/gender_dataset_face.zip) and train the network from scratch on your own if you are interested. You can add more images and play with the hyper parameters to experiment different ideas. 