# 🗣 Automatic Speech Recognition using OpenAI's Whisper ✨ [![Project Status: Active](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![](https://img.shields.io/badge/Prateek-Ralhan-brightgreen.svg?colorB=ff0000)](https://prateekralhan.github.io/)
A minimalistic automatic speech recognition streamlit based webapp powered by OpenAI's Whisper "State of the Art" models

![Animation](https://user-images.githubusercontent.com/29462447/192354340-7a242d6a-8d71-4b91-ae29-c35fbafe3ad4.gif)

## Installation:
* Simply run the command ***pip install -r requirements.txt*** to install the necessary dependencies.

## Usage:
1. Head over to [this link](https://github.com/openai/whisper) and follow the steps to get a comprehensive overview of the architecture of OpenAI's whisper models. 
2. Simply run the command: 
```
streamlit run app.py
```
3. Navigate to http://localhost:8501 in your web-browser.
4. By default, streamlit allows us to upload files of **max. 200MB**. If you want to have more size for uploading audio files, execute the command :
```
streamlit run app.py --server.maxUploadSize=1028
```

### Running the Dockerized App
1. Ensure you have Docker Installed and Setup in your OS (Windows/Mac/Linux). For detailed Instructions, please refer [this.](https://docs.docker.com/engine/install/)
2. Navigate to the folder where you have cloned this repository ( where the ***Dockerfile*** is present ).
3. Build the Docker Image (don't forget the dot!! :smile: ): 
```
docker build -f Dockerfile -t app:latest .
```
4. Run the docker:
```
docker run -p 8501:8501 app:latest
```

This will launch the dockerized app. Navigate to ***http://localhost:8501/*** in your browser to have a look at your application. You can check the status of your all available running dockers by:
```
docker ps
```
