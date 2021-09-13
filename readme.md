# This application uses TensorFlow Serving to serve an image classifier model

## Run Requirements.txt

## Tensor FlOw Server

docker pull tensorflow/serving

## Docker 

docker run -it -v C:\Users\harik\OneDrive\Documents\ProductionCode\TFServing\img_classifier:/img_classifier -p 8605:8605 --entrypoint /bin/bash tensorflow/serving

tensorflow_model_server --rest_api_port=8605 --model_name=classifier --model_base_path=/img_classifier/saved_models/

## Predict 

Run python predict.py

## Results

Saved to img_classifier/saved_models

