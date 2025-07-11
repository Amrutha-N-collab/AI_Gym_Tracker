# AI_Gym_Tracker



## Introduction


The AI Gym Tracker project represents an innovative web application that harnesses the power of artificial intelligence to track and monitor users’ physical activities during their workout sessions. Its main goal is to provide an intuitive and user-friendly user interface that allows users to perform their physical workouts easily, obtaining detailed information about their performance in real time.
The primary goal of the application is to provide users with an interactive and highly motivating training environment. Using cutting-edge technologies such as artificial intelligence, computer vision for video analysis, and pose recognition, the application is able to count
exercise repetitions in real time, while also providing precise and accurate feedback on the speed of execution of poses.
To perform action prediction and process the stream of frames from the webcam, we developed and trained an accurate artificial intelligence
model based on **recurrent neural networks (RNNs)** and **Long Short-Term Memory (LSTM)** neural networks. We created this model through a
data collection phase during which we recorded a considerable number of videos of correctly performed exercises, thus creating an accurate custom training dataset. In this way through the use of the powerful **Mediapipe library**, we extracted the poses performed by the user in realtime



## Project Structure
This Flask project has the following structure:

- `static` folder: this folder contains various files such as audio and static that are used in the web application.

- `templates` folder: this folder contains the HTML files for all the pages of the web application. These files are used to render the web pages on the client side.

- `action.h5` file: this binary file contains the weights of the neural network, network configurations, training information and other necessary information to reconstruct the pre-trained deep learning model. This file is loaded into app.py file to use the pre-trained model.

- `README` file: this file contains a description of the project, its features, and how to use it.

- `requirements.txt` file: this file contains all the packages that need to be installed in the virtual environment for the Flask application to run.

- `app.py` file: contains all the Python code for the Flask web application.


## Setup and run the App
To setup and run AI Gym Tracker application, follow these steps:

1) Clone or download the source code

2) Create a new virtual environment for the application using the following command in your terminal:
	- On Windows: `python -m venv venv`
	- On macOS and Linux: `python3 -m venv venv`

3) Activate the virtual environment using the following command:
	- On Windows: `venv\Scripts\activate`
	- On macOS and Linux: `source venv/bin/activate`

4) Install the required packages of the application using the following command: `pip install -r requirements.txt`

5) Once all the packages have been installed successfully, you can start AI Gym Tracker application by running the following command: `python app.py`

6) After running the above command, the application will be running in the localhost at port 5000. Open your web browser and navigate to http://localhost:5000/ to see the application running.
7) Remember to deactivate the virtual environment once you're done by running the following command: `deactivate`. This will exit the virtual environment and return you to your system's default Python environment. Have fun 😄
