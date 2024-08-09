# Hand Gesture-Based Screen Brightness Control

This Python application allows you to control your computer's screen brightness using hand gestures. The application leverages OpenCV and MediaPipe to detect hand landmarks in real-time, adjusting brightness based on the distance between the thumb and index finger.

## Features

- **Real-Time Gesture Recognition**: Detects and processes hand gestures in real-time using a webcam.
- **Brightness Adjustment**: Dynamically adjusts screen brightness by calculating the distance between the thumb and index finger.
- **Visual Feedback**: Displays the hand landmarks and a line connecting the thumb and index finger on the video feed.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.x installed on your system.
- A working webcam.
- Install the necessary Python libraries using `pip`.

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/aditikute24/Brightness-Control-Python.git
   ```
2. Navigate to the project directory:
   ```sh
   cd Hand-Gesture-Brightness-Control
   ```

3. Install the required Python libraries:
   ```sh
   pip install opencv-python mediapipe screen-brightness-control numpy
   ```
   
## Running the Application
   Run the Python script:
   ```sh
   python hand_gesture_brightness.py
   ```

## Usage:

1. Place your hand in front of the webcam.
2. Adjust the distance between your thumb and index finger to control the screen brightness.
3. The brightness will change dynamically as you move your fingers closer together or farther apart.
4. Press the 'q' key to exit the application.

## How It Works

1. **Hand Detection:** The application uses MediaPipe to detect the landmarks on your hand.
2. **Distance Measurement:** The Euclidean distance between the tips of your thumb and index finger is calculated using the hypot function from the math module.
3. **Brightness Control:** The distance is mapped to a brightness level between 0 and 100 using numpy.interp, and the screen brightness is set using the screen-brightness-control library.


   
