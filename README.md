# Virtual-Painter

**Introduction**

Virtual Painter is a hand-tracking-based drawing application that allows users to draw on a virtual canvas using their fingers. It uses OpenCV and Mediapipe to detect hand movements and interpret gestures for drawing, erasing, and selecting colors.

**Features**

Hand Tracking: Uses Mediapipe to detect hand landmarks in real time.

Gesture-Based Drawing: Draw with your index finger and switch colors using a virtual toolbar.

Eraser Mode: Erase drawings by selecting the eraser option.

Live Video Feed: Combines the drawing canvas with the webcam feed for a real-time painting experience.

**Technologies Used**

Python

OpenCV (cv2) for video processing and drawing functions

Mediapipe for hand tracking

NumPy for image processing

**Installation**

**Prerequisites**

Ensure you have Python installed (recommended: Python 3.7 or higher).

**Install Dependencies**

Run the following command to install the required libraries:

pip install opencv-python mediapipe numpy

**Usage**

**Run the script:**

python virtual_painter.py

The webcam will open, and hand tracking will begin.

**Color Selection:**

Move your index and middle fingers to the top toolbar to select a color.

Available colors: Blue, Green, Red, Yellow, and Eraser (Black).

**Drawing:**

Keep only the index finger up to start drawing.

Move your finger across the screen to draw lines.

**Erasing:**

Select the eraser (black) and move your finger over the drawing to erase.

Exit the Program:

Press q on the keyboard to close the application.

**How It Works**

The script captures video from the webcam and detects hand landmarks.

It determines if fingers are up to classify gestures:

Both index and middle fingers up → **Selection Mode (choose color)**

Only index finger up → **Drawing Mode**

The drawing is saved on a separate canvas and blended with the webcam feed.

**Future Improvements**

Add more color options.

Implement a save option to export drawings.

Improve gesture recognition accuracy.

**License**

This project is open-source and free to use.
