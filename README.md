# Plant-Disease-Detector

## Important Links
1. Backend API Server Docker Image: <a href="https://hub.docker.com/repository/docker/amitmaindola/plant-disease-detector-api/"> amitmaindola/plant-disease-detector-api</a>
2. API Server Link: <a href="https://potato-disease-detector-api-3dhk23ywda-uc.a.run.app/ping">Hosted on Google Cloud</a>
   *[Note: `/ping` route is to check if the server is live or not]*
3. Front-End Production Build: <a href="https://github.com/amitmaindola/PDD-Production_build">amitmaindola/PDD-Production_build</a>
4. Web Application Link: <a href="https://amitmaindola.github.io/PDD-Production_build/">amitmaindola.github.io/PDD-Production_build/</a>


## File System
1. **Model Training**: In `training/` folder you will find all files related to the training of the Deep Learning Model.
1. **Saved Model**: In `saved_models/1/` folder you will find the final saved trained model.
1. **Server**: In `server/` folder you will find `requirements.txt` and `main.py` files which will act as a backend API server for the application.
1. **Front End**: In `web_app/` folder you will find a React.js web application.

## Getting Started
### 1. Setting up the API server.
#### &emsp;There are two ways to start API server at your local device.
&emsp;1.1 **Using Docker Image** *[Prerequisites: <a href="https://www.docker.com/">Docker</a> should be installed in your machine]*<br>

&emsp; &emsp; Visit <a href="https://hub.docker.com/repository/docker/amitmaindola/plant-disease-detector-api/"> amitmaindola/plant-disease-detector-api</a> and look at the documentation to start docker container.


&emsp;1.1 **Using Python**

&emsp; &emsp; Open Terminal/Python Shell in `server/` directory and run the following command
```
pip3 install -r api/requirements.txt
```
&emsp; &emsp; Now you can run server in your local machine with command
```
python main.py
```

### 1. Using the API server.
&emsp; &emsp; Start the server in your local machine with command
```
python main.py
```
&emsp;&emsp; Now You to create a `POST` request at `https://localhost:8000/predict` with a body having a file with field name `file`

