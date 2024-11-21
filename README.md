Video Processing with Line Detection
This project demonstrates a simple video processing application using OpenCV and NumPy to detect and highlight lines in a video. The script applies Gaussian blur, color space conversion, and edge detection to identify lines in the video frames.

Features
Video Capture: Reads video from a file.
Image Processing: Applies Gaussian blur and HSV color space conversion.
Line Detection: Uses edge detection and Hough Line Transform to find and highlight lines.
Display: Shows the processed frames and detected edges in separate windows.
Requirements
Python 3.x
OpenCV (cv2)
NumPy
You can install the required Python packages using pip:

sh
Copy code
pip install opencv-python-headless numpy
Usage
Place your video file in the appropriate directory or update the video path in the script.

Run the script using Python:

sh
Copy code
python video_processing.py
Make sure to replace video_processing.py with the actual filename if different.

The script will open two windows:

frame: Displays the original video frame with detected lines.
edges: Displays the edges detected by the Canny edge detector.
Press Esc to exit the video processing loop and close the application.

Code Explanation
Video Capture: cv2.VideoCapture is used to read video frames from the specified file path.
Gaussian Blur: Applied to reduce noise and smooth the image.
HSV Color Space Conversion: Converts the frame from BGR to HSV color space to simplify color-based filtering.
Masking: Filters the image to detect specific colors.
Edge Detection: Uses the Canny algorithm to find edges in the masked image.
Line Detection: Applies the Hough Line Transform to detect lines in the edge-detected image.
Line Drawing: Draws the detected lines on the original frame.
Display: Uses cv2.imshow to show the original frame and edges.
Troubleshooting
No Lines Detected: Adjust the HSV range, Canny thresholds, or Hough Line Transform parameters as needed.
Video Path Issues: Ensure the video path is correct and the video file exists at the specified location.
Contributing
Feel free to open issues or submit pull requests if you have improvements or bug fixes.
![Screenshot 2024-11-21 235027](https://github.com/user-attachments/assets/76344873-2cb3-43e9-93a9-226d34cf96de)
![Screenshot 2024-11-21 235011](https://github.com/user-attachments/assets/9738ec02-a543-463c-ba9c-c2ff7fc58b8f)


License
This project is licensed under the MIT License. See the LICENSE file for details.
