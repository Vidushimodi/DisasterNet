# Disaster Detection Web App Using Laptop Camera and AI

## Overview
This project is a web-based application built using Flask that allows users to detect and classify natural disasters in real-time using their laptop's camera. When you click the "Take a Pic" button, the app captures an image, processes it using deep learning models, and classifies it into various disaster categories such as cyclones, earthquakes, floods, and wildfires. The classification is powered by Convolutional Neural Networks (CNNs), a type of deep learning model that is ideal for image processing.

## Features

- **Real-Time Disaster Detection**: The app uses images captured through your laptop camera to detect natural disasters like cyclones, wildfires, floods, etc.
- **AI-Based Classification**: Leveraging deep learning models to analyze and classify disaster events from images captured by the camera.
- **Flask Web Application**: A simple and user-friendly web interface to interact with the system.
- **Portable and Easy to Use**: The system runs directly in your web browser, and it only requires a laptop camera for image capture.

## Technologies

- **Flask**: A lightweight web framework for building the web application.
- **Laptop Camera**: Real-time image capture for disaster detection through the laptop's built-in camera.
- **Convolutional Neural Networks (CNNs)**: Deep learning models used to classify disaster events based on captured images.
- **Python**: The programming language used for model development and the web application.
- **OpenCV**: Computer vision library used for image capturing and processing.
- **TensorFlow / Keras**: Deep learning libraries used to train and deploy the CNN model.

## Installation

To set up and run the project locally, follow the steps below:

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/disaster-detection-web-app.git
   cd disaster-detection-web-app
   ```

2. Create a virtual environment (optional but recommended):

   ```bash
   python -m venv env
   source env/bin/activate  # For Linux/MacOS
   .\env\Scripts\activate  # For Windows
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Install OpenCV for accessing the camera:

   ```bash
   pip install opencv-python
   ```

5. Install Flask to run the web application:

   ```bash
   pip install flask
   ```

## Usage

1. After setting up the environment and installing dependencies, run the Flask app:

   ```bash
   python app.py
   ```

2. Open your browser and navigate to `http://127.0.0.1:5000/` to access the web interface.

3. On the web page, click on the **"Take a Pic"** button. The application will activate your laptop camera and allow you to take a picture of the satellite image or scene.

4. Once the image is captured, the system will process it and classify the disaster type (e.g., cyclone, wildfire, flood, etc.), displaying the result and confidence score.

5. To stop the camera, you can either click the stop button on the page or refresh the page.

## Project Structure

- `app.py`: Main Flask application that serves the web page and handles the image capture and processing.
- `templates/`: Contains HTML templates for the web interface.
  - `index.html`: Main page of the app, which includes the camera interface.
- `static/`: Contains static files such as CSS and JavaScript for the web page.
- `models/`: Contains the trained CNN model for disaster detection.

## Data Sources

- The system uses real-time images captured via your laptop camera. Optionally, you can modify the application to work with satellite imagery datasets.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
