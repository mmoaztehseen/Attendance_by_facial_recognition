                                                   Attendance By Facial Recognition
*****************************************************************************************************************************************
                                             Final Project: Artificial Intelligence (Python)
*****************************************************************************************************************************************

#Libraries:

I have used the folowing Libraries in this project:
1. cmake
2. dlib
3. opencv-python
4. face-recognition
5. numpy


*****************************************************************************************************************************************
Reference Article used is:

https://medium.com/@ageitgey/machine-learning-is-fun-part-4-modern-face-recognition-with-deep-learning-c3cffc121d78

*****************************************************************************************************************************************

Files/Folder in this project folder:
1. images
2. Attendance.csv
3. attendance.py
4. README.md

*****************************************************************************************************************************************
## Features

The script `attendance.py` includes the following key features:

### Loading and Preprocessing Images

- The script reads images from the `images` directory.
- Each image is processed and stored in a list, and corresponding person names are extracted from the image filenames.

### Face Encoding

- The `faceEncodings` function converts each image to RGB and encodes the facial features using the `face_recognition` library.
- Encoded faces are stored in a list for later comparison.

### Attendance Recording

- The `attendance` function logs the name of the detected individual along with the current date and time into `Attendance.csv`.
- It ensures that each individual is logged only once per day.

### Real-Time Face Recognition

- The script captures video from the default camera.
- It detects and encodes faces in each video frame, then compares them to the known encodings.
- When a match is found, the name of the individual is displayed on the video feed, and their attendance is recorded.

*****************************************************************************************************************************************

## Usage

To run the project, execute the `attendance.py` script. Ensure you have all the necessary libraries installed and the `images/` folder populated with the images of individuals to be recognized.

### Steps to Run the Project

1. **Install Dependencies**: Ensure you have all required libraries installed. You can install them using pip:
   ```sh
   pip install cmake dlib opencv-python face-recognition numpy
   ```
2. **Prepare Images**: Place the images of individuals to be recognized in the images/ folder. Ensure the image filenames correspond to the person's name.
3. **Run the Script**: Execute the attendance.py script:
   ```sh
   python attendance.py
   ```
4. **View Attendance**: Attendance records will be saved in the Attendance.csv file.

*****************************************************************************************************************************************
