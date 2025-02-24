# Air-canvas-using-opencv

This project creates an "Air Canvas" application using OpenCV, MediaPipe, and Python.  It uses hand tracking to detect the user's hand movements in real-time. By tracking the tip of the index finger (or another designated finger), the program allows the user to "draw" in the air. The drawing appears on the screen as if the finger were a virtual pen.  The project can be expanded to include features like color selection, an eraser, and different brush sizes, all controlled by hand gestures.

# Algorithm

1.Start reading the frames and convert the captured frames to HSV colour space.(Easy for colour detection)
2.Prepare the canvas frame and put the respective ink buttons on it.
3.Adjust the values of teh mediapipe intilization to detect one hand only.
4.Detect teh landmarks by passing the RGB frame to the mediapipe hand detector
5.Detect the landmarks, find the forefinger coordinates and keep storing them in the array for successive frames .(Arrays for drawing points on canvas)
6.Finally draw the points stored in array on the frames and canvas 

