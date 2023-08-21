# Attendance_system

This project represents an attendance system using face recognition. Here's a breakdown of the code:

1. Import the necessary libraries: `cv2` for computer vision tasks, `datetime` for time-related operations, `face_recognition` for face recognition functionalities, `csv` for CSV file operations, and `os` for interacting with the operating system.

1. Load the face images and their corresponding names from the "faces" directory. The code uses the `face_recognition` library to encode the faces and store them in the `faces` list. The names are stored in the `names` list.

1. Initialize the CSV file and create a header row for the attendance records.

1. Initialize variables and lists to keep track of recorded attendees.

1. Initialize the video capture using the default camera (index 0).

1. Start an infinite loop to capture frames from the video.

1. Convert each captured frame to RGB format.

1. Detect faces in the frame by using the `face_recognition` library.

1. Iterate through each detected face and compare it with the known faces. If a match is found and the attendee has not been recorded yet, update the attendance record.

1. Save the frame containing the recognized face to a file with a unique name.

1. Add the attendance record (name, time, and image filename) to the CSV file.

1. Draw a rectangle around the detected face and display the name label on the frame.

1. Display the resulting image in a window named "Attendance System".

1. Exit the loop if the 'q' key is pressed.

1. Release the video capture and destroy the windows.

This code allows real-time face recognition and attendance tracking by comparing detected faces with the pre-loaded face images. It saves the attendance records in a CSV file and stores the corresponding face images as well.


