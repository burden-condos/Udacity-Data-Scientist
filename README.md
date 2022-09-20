# Disaster Response Pipeline Project
This repo contains the code for the Disaster Response Pipeline for Udacity Data Scientist Nanodegree. The project is to build a Machine Learning model to classify a piece of text into 36 categories in order to response to the disaster.

![image](https://user-images.githubusercontent.com/114002358/191294178-30fe7c26-6c53-468d-8c4f-2589e1c703c0.png)
![image](https://user-images.githubusercontent.com/114002358/191294342-4df08123-9aa9-4976-8a24-3a09ab11132b.png)



## Project Structure
```
disaster_response_pipeline
|-- app # code for the Flask app
    |-- templates
            |-- go.html
            |-- master.html
    |-- run.py
|-- data # SQLite database and preprocessed files
    |-- disaster_message.csv
    |-- disaster_categories.csv
    |-- DisasterResponse.db
    |-- process_data.py
|-- models # Machine learning models
    |-- classifier.pkl
    |-- train_classifier.py
|-- README
```

## Installation
Run: `pip install numpy pandas sqlalchemy nltk pickle scikit-learn plotly flask`

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Go to `app` directory: `cd app`

3. Run your web app: `python run.py`

4. Go to `http://0.0.0.0:3000/`

4. Click the `PREVIEW` button to open the homepage
