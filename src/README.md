This folder contains the Python source scripts and Flask web apps.

Files:
1. app.py - Flask server, loads the model from the models folder. This also exposes the API routes.
2. fairness_mitigation.py - This is where reweighting and group thresholds occurs. 
3. model.py - Model training utilities.
4. preprocess.py - Preprocessing utilities.
5. templates/index.html - the HTML file being launched through Flask.
