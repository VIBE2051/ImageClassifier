# ImageClassifier
An image classifier, to determine whether the image presented is happy or sad

## Setting up a python environment
Setup an environment by running the following bash script, on TensorFlow's website it will say that it is compatible with Python3.12, however, only worked with 3.11:
```bash
py -3.11 -m venv tf_env
tf_env\Scripts\activate
pip install tensorflow
```
After running these commands the first line in the python notebook should be run, this will pip install all the necessary libraries, if that does not work run the follwing command:
```bash
pip install tensorflow opencv-python matplotlib
```