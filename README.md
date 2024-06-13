                                                   Attendance By Facial Recognition
*****************************************************************************************************************************************
                                             Final Project: Artificial Intelligence (Python)
*****************************************************************************************************************************************

Libraries:

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

## Running the Project in PyCharm

To run the project in PyCharm, follow these steps:

1. **Clone the Repository or Copy Project Files**: Ensure you have the project files on your local machine. If you have the repository link, you can clone it using Git, or simply copy the project files.

2. **Open PyCharm**: Launch PyCharm on your machine.

3. **Open the Project**: 
   - Click on `File` -> `Open`.
   - Navigate to the directory where your project files are located and select the folder. Click `OK`.

4. **Install Dependencies**:
   - Open the terminal within PyCharm by clicking on `View` -> `Tool Windows` -> `Terminal`.
   - Install the required libraries by running the following command:
     ```sh
     pip install cmake dlib opencv-python face-recognition numpy
     ```

5. **Set Up the Project Interpreter**:
   - Go to `File` -> `Settings` (or `PyCharm` -> `Preferences` on macOS).
   - Navigate to `Project: [your_project_name]` -> `Python Interpreter`.
   - Ensure that the correct Python interpreter is selected and that all necessary packages are installed.

6. **Prepare Images**:
   - Place the images of individuals to be recognized in the `images/` folder. Ensure the image filenames correspond to the person's name.

7. **Run the Script**:
   - Locate the `attendance.py` file in the Project Explorer (usually on the left side of the PyCharm window).
   - Right-click on `attendance.py` and select `Run 'attendance'` from the context menu. Alternatively, you can open `attendance.py` and click the green play button in the upper right corner of the editor.

8. **View Attendance**:
   - After running the script, attendance records will be saved in the `Attendance.csv` file located in the project directory.
   - You can open and view this file to see the attendance records.

By following these steps, you will be able to run the facial recognition attendance system project in PyCharm successfully.


*****************************************************************************************************************************************
