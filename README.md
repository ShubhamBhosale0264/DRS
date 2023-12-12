Importing Libraries:

threading: Used for creating threads to run functions concurrently.
time: Used for introducing delays in the code.
tkinter: GUI library.
cv2: OpenCV library for computer vision tasks.
imutils: Provides convenience functions for OpenCV.
PIL: Python Imaging Library (Pillow) for image handling.
Video Initialization:

The script opens a video file ("clip.mp4") using OpenCV's VideoCapture class.
SET_WIDTH and SET_HEIGHT set the dimensions for displaying the video frames.
Functions for Playback:

play(speed): Adjusts the video playback speed based on the user's input.
pending(decision): Simulates a "pending" state by displaying an intermediate image before showing the final decision.
out(): Initiates a thread to handle the "out" decision.
not_out(): Initiates a thread to handle the "not out" decision.
GUI Initialization:

A Tkinter window titled "Shubham DRS System" is created.
The welcome image ("welcome.png") is loaded and displayed on a Tkinter canvas.
Buttons for controlling playback and making decisions ("out" or "not out") are added to the window. Each button is associated with a specific command and speed for playback.
Button Commands:

Buttons are created to navigate the video ("Previous" and "Next") with varying speeds.
Additional buttons allow the user to make decisions ("Give Out" and "Give Not Out"). These buttons trigger threads that simulate a pending state before displaying the final decision.
Main Loop:

The mainloop() function is called to start the main event loop, allowing the Tkinter application to run and respond to user interactions.
