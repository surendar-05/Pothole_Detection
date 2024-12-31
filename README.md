Pothole Detection System

This project is a Streamlit-based application designed to detect potholes in images and videos using a YOLO (You Only Look Once) deep learning model. The system provides a user-friendly interface to upload images and videos, performs object detection, and displays the results side by side for easy comparison.

Features

Image Upload: Upload images to detect potholes, and view the annotated results.

Video Upload: Upload videos to detect potholes frame-by-frame, and watch the real-time results.

Interactive UI: Easy-to-navigate Streamlit interface with sidebar menu.

Dependencies

Ensure the following Python libraries are installed before running the application:

os

cv2 (OpenCV)

tempfile

matplotlib

pathlib

ultralytics

streamlit

streamlit-option-menu

Installation

Clone this repository to your local machine:

git clone <repository_url>

Navigate to the project directory:

cd <repository_directory>

Install the required dependencies:

pip install -r requirements.txt

Ensure the YOLO model file (pothole_segmentation.pt) is available in the project directory. If it is missing, download or place it in the directory.

Usage

Run the Application

To start the application, execute the following command:

streamlit run app.py

Image Upload

Select Image Upload from the sidebar.

Upload an image file (JPG, JPEG, or PNG).

View the input image and the detected pothole annotations side by side.

Video Upload

Select Video Upload from the sidebar.

Upload a video file (MP4, AVI, or MOV).

Watch the input video and the pothole-detected video side by side.

File Structure

├── app.py                 # Main application script
├── pothole_segmentation.pt # YOLO model file
├── requirements.txt       # List of required Python libraries
├── README.md              # Project documentation

YOLO Model

This application uses a pre-trained YOLO model (pothole_segmentation.pt) for pothole detection. Ensure that the model is compatible with the ultralytics YOLO library.

Troubleshooting

Model Not Found:
If the model file (pothole_segmentation.pt) is not found, ensure it is placed in the project directory.

Dependency Issues:
If dependencies are missing, run:

pip install -r requirements.txt

Video Playback Issues:
Ensure the uploaded video format is supported (MP4, AVI, MOV).

Future Enhancements

Add support for real-time video feed (e.g., from a webcam).

Improve model accuracy and performance.

Extend support to detect other road hazards.

License

This project is open-source and available under the MIT License.

Acknowledgments

YOLO by Ultralytics

Streamlit

Feel free to contribute and enhance the project by submitting pull requests or reporting issues.