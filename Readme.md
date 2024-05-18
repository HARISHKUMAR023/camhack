# CamHack

CamHack is a simple Flask application that captures video from the default camera (camera index 0) and serves it as a multipart HTTP response.

## How it Works

The application uses OpenCV to capture video frames from the camera. Each frame is encoded as a JPEG image and then served as a part of a multipart HTTP response.

The main function of the application is `generate_frames` which captures the video frames and yields them as HTTP response parts.

The application has a single route (`/`) which responds with the video stream when accessed.

## How to Run

To run the application, simply execute the `camhack.py` script:

1. Ensure you have Python, Flask, and OpenCV installed.
2. Run the script using the following command:
   ```bash
   python camhack.py
# Requirements

   - Python
   - Flask
   - OpenCV

## Please ensure that these are installed before running the application.