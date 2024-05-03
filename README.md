# EVI-AI  
## Eyes for the Visually Impaired  

This project aims to assist individuals with visual impairments in their daily activities. It employs an application that uses the mobile phone's camera to identify objects and gauge their distances. The app then leverages a Large Language Model (LLM) to interpret the findings from the YOLO (You Only Look Once) object detection and ZoeDepth perception models. This information is converted into audio commands, guiding users to navigate their environment more effectively.  

## Project Overview

The main components of this project include:  

- Mobile application written in Flutter  
- YOLO object detection model  
- Depth detection model (ZoeD_N)  
- llama2 LLM model  

### Project Flow  
![pipeline](https://github.com/emre-bl/EVI-AI/assets/105359055/c6755702-0b7c-442a-83f3-564bbb13e46b)  

#### APK flow  
![APK](https://github.com/emre-bl/EVI-AI/assets/105359055/b0e182aa-1e3e-4212-905a-b563e84b8636)  

#### app flow  
![app_py png](https://github.com/emre-bl/EVI-AI/assets/105359055/3ecb45de-5cf4-41a7-8566-4e9212a117a3)  

#### user flow  
![user_py](https://github.com/emre-bl/EVI-AI/assets/105359055/98b2e9d4-d4d9-4f31-baaf-2733ec600490)  

#### server flow  
![server_py](https://github.com/emre-bl/EVI-AI/assets/105359055/d0ccfef9-c278-488f-a1d7-6a2594469259)  

## Getting Started  

### Prerequisites  
- Python 3  
- Flutter  
- Jupyter Notebook  

### Installation  

- Clone the repository
  ```bash
  git clone https://github.com/emre-bl/EVI-AI.git
  ```  

- Install dependencies
  ```bash
  pip install -r requirements.txt
  ```  

- Go to mobile app's directory  
  ```bash
  cd pipeline_scripts/mobile_app
  ```  

- Run the commands below
  ```bash
  flutter clean
  ```  
  ```bash
  flutter pub get
  ```  
  ```bash
  flutter build apk
  ```  
  ```bash
  adb install path/to/your/app-release.apk
  ```  

## Usage  

- To be the server: first run app.py, then run server.py, lastly run user.py
- To be the client: build and run the APK

## Contributors

- [Emre Belikırık](https://github.com/emre-bl)  
- [Meriç Demirörs](https://github.com/mericdemirors)  
- [Zeynep Meriç Aşık](https://github.com/meric2)  
