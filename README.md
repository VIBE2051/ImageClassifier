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
The models trained on my machine have been uploaded, and can be tested by running the following lines:
```Python
img = cv2.imread('INSERT_EXAMPLE.jpg')
resize = tf.image.resize(img, (256,256))
yhat_new = new_model.predict(np.expand_dims(resize/255, 0))
if yhat_new > 0.5: 
    print(f'Predicted class is Sad')
else:
    print(f'Predicted class is Happy')
```

The model is fairly accurate, the dataset was sourced from google images.