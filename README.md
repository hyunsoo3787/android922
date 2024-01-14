# How to use

### 0. Install
Create conda environment

    conda env create --file environment.yaml

### 1. Run Server
    python main.py

### 2. Call API
Train MNIST model with hyperparameters

    python client.py -opt train -lr 0.001 -bs 128 -epochs 5

Register

    python client.py -opt register -run_id 'trained_model_run_id_with_mlflow'

Predict 

    python client.py -opt predict -image_path image_path_to_predict
