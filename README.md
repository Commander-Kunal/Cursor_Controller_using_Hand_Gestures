Cursor Controller using Hand Gestures

A Computer Vision utility that allows you to control your computer's cursor in real-time using hand gestures. This project uses your webcam to track hand movements and translate them into desktop cursor actions, including movement and clicking.
________________________________________
Features

•	Real-time Cursor Control: Move your mouse cursor by moving your hand.

•	Gesture-based Clicking: Perform a click action using a simple hand gesture.

•	Virtual Mouse: A complete replacement for your physical mouse, controlled entirely by your hand.
________________________________________
How it Works

The application uses the following key technologies:

•	OpenCV: To capture the video feed from your webcam.

•	MediaPipe: For robust, real-time hand tracking to detect landmarks on the hand.

•	PyAutoGUI: To programmatically control the mouse cursor (move and click) on the screen.

•	NumPy: For numerical operations and handling coordinates.

The HandTracking.py module detects the hand and its landmarks. The main script, AICursorController.py, reads these landmarks, interprets the gestures, and uses pyautogui to move the cursor and simulate clicks.
________________________________________
Gestures

The application recognizes five distinct gestures to control your computer:

* **Move Cursor:**
    * **Action:** Raise your index finger only.
    * **Result:** The mouse cursor will follow the movement of your index fingertip.

* **Left Click:**
    * **Action:** Raise your index and middle fingers. Bring the tips of these two fingers close together (distance `< 40` pixels).
    * **Result:** The system will perform a single left click.

* **Right Click:**
    * **Action:** Raise your index, middle, and ring fingers. Bring the tips of your middle and ring fingers close together (distance `< 40` pixels).
    * **Result:** The system will perform a single right click.

* **Drag and Drop:**
    * **Action:** Raise your thumb and index finger.
    * **Hold:** Bring the tips of your thumb and index finger close together (distance `< 40` pixels) to "press and hold" the left mouse button.
    * **Drag:** Move your hand while keeping your fingers pinched.
    * **Drop:** Separate your thumb and index finger (distance `> 40` pixels) to "release" the button.

* **Scrolling:**
    * **Action:** Raise all four fingers (index, middle, ring, and pinky).
    * **Scroll Up:** Move your hand towards the top of the camera's view.
    * **Scroll Down:** Move your hand towards the bottom of the camera's view.
________________________________________

Prerequisites

* You must have Python 3.x installed on your system.

Installation

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/Commander-Kunal/Cursor_Controller_using_Hand_Gestures.git](https://github.com/Commander-Kunal/Cursor_Controller_using_Hand_Gestures.git)
    cd Cursor_Controller_using_Hand_Gestures
    ```

2.  **Install the required Python libraries:**
    ```sh
    pip install opencv-python mediapipe pyautogui numpy
    ```

Usage

To run the application, simply execute the `AICursorController.py` script from your terminal:

```sh
python AICursorController.py
```
________________________________________
License

This project is open-source. See the LICENSE file for more information.
________________________________________

About Author

Kunal Gupta

MCA Data Science Student at University Institute of Computing (UIC), Chandigarh University, Mohali, Punjab – 140301

UID: 25MCD10013

Semester/Year: 1/1
