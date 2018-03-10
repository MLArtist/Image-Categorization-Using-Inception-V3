# Image-Categorization-Using-Inception-V3

## Pre requisits: 
1) Python 3.6.3
2) Tensorflow 1.4

## Archetecture of used algorithm for image processing: Inception V3 
Approch: 
1) Retrain the final layer of the avaible inception v3 model [Transfer Learning]
2) Use the such trained model to predict the test data		

## Trainiing: 
python tensorflow/tensorflow/examples/image_retraining/retrain.py --image_dir test_61326

## Test
python tensorflow/tensorflow/examples/label_image/label_image_updated.py --graph=saved_models/output_graph.pb --labels=saved_models/output_labels.txt --input_layer=Mul --output_layer=final_result --image_dir="D:\DataSci\projects\JBM\mydata\test_61326"
