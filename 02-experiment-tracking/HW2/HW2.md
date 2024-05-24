## Q1: Install MLflow
    - version 2.13.0

## Q2: Download and preprocess the data
    - `python preprocess_data.py --raw_data_path ./taxidata --dest_path ./output`
    - 4 files were created in /output.

## Q3: Train a model with autolog
    - Start a local tracking server: `mlflow server --host 127.0.0.1 --port 8080`
    - execute `python train.py`
    - min_samples_split: 2

## Q4: Launch the tracking server locally
    - `mlflow ui --backend-store-uri sqlite:///mlflow.db --default-artifact-root ./mlruns`
    - A: `default-artifact-root`

## Q5: Tune model hyperparameters
    - A: 5.335

## Q6: Promote the best model to the model registry
    - 5.567