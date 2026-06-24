All files are uploaded in .txt, make sure it is saved in .py (python extension) so that it works.

Download Python and its all supporting libraries
Download the CIC IDS 2017 dataset

https://www.kaggle.com/datasets/chethuhn/network-intrusion-dataset

Change the path/location in between the code according to the file destination of your device

Total 5 files
Make sure all this files are saved in the same folder 
1) Preprocessing file (preprocessing_last.py)
2) Model training file (model_training_final.y)
3) Realtime detection file (realtime_final.py)
4) Backend file (nids_backend_final.py)
5) Dashboard file (nids_dashboard.html)


for the project to run successfully,
preprocessing file needs to be executed first(once only, dont have to this everytime for detection), after successful execution of this file, then

model training file has to be executed(once only, dont have to this everytime for detection),[training models take time], after successful execution of this file, then 

realtime detection file has to be executed(once only, dont have to this everytime for detection), after this is done

backend file has to be executed whenever you shut the system or close it, backend file needs to run whenever the detection has to be made, but if the backend is already running then no need start the detection directly from the dashboard

dashboard file needs to be first saved and then it directly open as localhost whenever detection needs to be done
(when opened the dashboard, if it shows system ready, models loaded it means then backend is running and you can processed further by uploading file on the dashboard)
(and if when opened it shows system not ready, model not loaded, that means you will have to first run the backend file and the access the dashboard again)
 using the dashboard, simply just upload the file, select model(best xgboost model and then ml ensemble model), select number of samples(better to keep it 5) and click on analyze with XAI and then wait for results to display.


