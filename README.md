# TensorFlow Face Recognition
Recognizes Face using Tensorflow inception_v3 model

## Installation and Setup
```pip install tensorflow
pip install opencv-python
```


Train the model using following code:
```
python -m retrain \
--output_graph=model/retrained_graph.pb \
--output_labels=model/retrained_labels.txt \
--architecture=inception_v3 \
--image_dir=dataset/images
```
Note: If error occurs while training, try removing -m


Run the detection code:
```
python detect_face.py
```
