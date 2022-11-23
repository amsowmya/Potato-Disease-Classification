# Potato-Disease-Classification

1. Model Building : Tensorflow, CNN, data agumentation, tf dataset
2. Backend Server : tf serving, Fast API
3. Model Optimization : Quantization, Tensorflow Lite
4. Frontend & Deployment : React JS, React Native, Deployment to GCP

#Split folder
pip install split-folders

split_folders --output dataset --ratio .7 .1 .2 -- PlantVillage

#Docker
docker pull tensorflow/serving

docker run -t --rm -v E:/DeepLearning_new/Potato-Disease-Classification:/Potato-Disease-Classification -p 8501:8501 tensorflow/serving --rest-api_port=8501 --model_config_file=/Potato-Disease-Classification/models.config
