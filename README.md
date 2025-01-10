<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
</head>
<body style="font-family: Arial, sans-serif; line-height: 1.6; margin: 0; padding: 20px; background-color: #f4f4f9;">

<h1 style="color: #333;">Pothole Detection System</h1>

<p>This project is a Streamlit-based application designed to detect potholes in images and videos using a YOLO (You Only Look Once) deep learning model. The system provides a user-friendly interface to upload images and videos, performs object detection, and displays the results side by side for easy comparison.</p>

<h2 style="color: #333;">Features</h2>
<ul>
    <li><strong>Image Upload</strong>: Upload images to detect potholes, and view the annotated results.</li>
    <li><strong>Video Upload</strong>: Upload videos to detect potholes frame-by-frame, and watch the real-time results.</li>
    <li><strong>Interactive UI</strong>: Easy-to-navigate Streamlit interface with a sidebar menu.</li>
</ul>

<h2 style="color: #333;">Dependencies</h2>
<p>Ensure the following Python libraries are installed before running the application:</p>
<ul>
    <li><code>os</code></li>
    <li><code>cv2</code> (OpenCV)</li>
    <li><code>tempfile</code></li>
    <li><code>matplotlib</code></li>
    <li><code>pathlib</code></li>
    <li><code>ultralytics</code></li>
    <li><code>streamlit</code></li>
    <li><code>streamlit-option-menu</code></li>
</ul>

<h2 style="color: #333;">Installation</h2>
<ol>
    <li>Clone this repository to your local machine:
        <pre style="background: #333; color: #fff; padding: 10px; overflow-x: auto;"><code>git clone &lt;repository_url&gt;</code></pre>
    </li>
    <li>Navigate to the project directory:
        <pre style="background: #333; color: #fff; padding: 10px; overflow-x: auto;"><code>cd &lt;repository_directory&gt;</code></pre>
    </li>
    <li>Install the required dependencies:
        <pre style="background: #333; color: #fff; padding: 10px; overflow-x: auto;"><code>pip install -r requirements.txt</code></pre>
    </li>
    <li>Ensure the YOLO model file (<code>pothole_segmentation.pt</code>) is available in the project directory. If it is missing, download or place it in the directory.</li>
</ol>

<h2 style="color: #333;">Usage</h2>

<h3 style="color: #333;">Run the Application</h3>
<p>To start the application, execute the following command:</p>
<pre style="background: #333; color: #fff; padding: 10px; overflow-x: auto;"><code>streamlit run app.py</code></pre>

<h3 style="color: #333;">Image Upload</h3>
<ol>
    <li>Select <strong>Image Upload</strong> from the sidebar.</li>
    <li>Upload an image file (JPG, JPEG, or PNG).</li>
    <li>View the input image and the detected pothole annotations side by side.</li>
</ol>

<h3 style="color: #333;">Video Upload</h3>
<ol>
    <li>Select <strong>Video Upload</strong> from the sidebar.</li>
    <li>Upload a video file (MP4, AVI, or MOV).</li>
    <li>Watch the input video and the pothole-detected video side by side.</li>
</ol>

<h2 style="color: #333;">File Structure</h2>
<pre style="background: #333; color: #fff; padding: 10px; overflow-x: auto;"><code>
├── app.py                 # Main application script
├── pothole_segmentation.pt # YOLO model file
├── requirements.txt       # List of required Python libraries
├── README.md              # Project documentation
</code></pre>

<h2 style="color: #333;">YOLO Model</h2>
<p>This application uses a pre-trained YOLO model (<code>pothole_segmentation.pt</code>) for pothole detection. Ensure that the model is compatible with the <code>ultralytics</code> YOLO library.</p>

<h2 style="color: #333;">Troubleshooting</h2>
<ul>
    <li><strong>Model Not Found</strong>: If the model file (<code>pothole_segmentation.pt</code>) is not found, ensure it is placed in the project directory.</li>
    <li><strong>Dependency Issues</strong>: If dependencies are missing, run:
        <pre style="background: #333; color: #fff; padding: 10px; overflow-x: auto;"><code>pip install -r requirements.txt</code></pre>
    </li>
    <li><strong>Video Playback Issues</strong>: Ensure the uploaded video format is supported (MP4, AVI, MOV).</li>
</ul>

<h2 style="color: #333;">Future Enhancements</h2>
<ul>
    <li>Add support for real-time video feed (e.g., from a webcam).</li>
    <li>Improve model accuracy and performance.</li>
    <li>Extend support to detect other road hazards.</li>
</ul>

<h2 style="color: #333;">License</h2>
<p>This project is open-source and available under the <a href="LICENSE" style="color: #3498db; text-decoration: none;">MIT License</a>.</p>

<h2 style="color: #333;">Acknowledgments</h2>
<ul>
    <li><a href="https://ultralytics.com/" style="color: #3498db; text-decoration: none;">YOLO by Ultralytics</a></li>
    <li><a href="https://streamlit.io/" style="color: #3498db; text-decoration: none;">Streamlit</a></li>
</ul>

<p>Feel free to contribute and enhance the project by submitting pull requests or reporting issues.</p>

</body>
</html>
