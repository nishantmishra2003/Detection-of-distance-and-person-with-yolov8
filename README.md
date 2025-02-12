# Detection-of-distance-and-person-with-yolov8

Overview

This project utilizes YOLOv8 (You Only Look Once) to detect people in real-time and estimate their distance from the camera. The model processes video input, detects persons, and calculates the approximate distance using object size or depth estimation techniques.

Features

>Real-time person detection using YOLOv8.

>Distance estimation based on object size or depth perception.

>Supports webcam & video input for live detection.

>Customizable threshold settings for detection confidence and distance alerts.

>Visual overlays to display bounding boxes, labels, and distance.

2. Key Arguments

--source: Specify the input source (0 for webcam, video file path for pre-recorded videos).

--model: Path to the YOLOv8 model (yolov8n.pt, yolov8s.pt, etc.).

--conf: Set confidence threshold (default: 0.5).

Distance Estimation

Method Used:

If depth sensors are available, we use stereo vision or depth maps.

If only a single camera is used, distance estimation is based on pixel size vs real-world size scaling.

Calibration techniques may be used to improve accuracy.

Example Output

>The detection window will display:

>Bounding boxes around detected persons.

>Distance overlays showing approximate distances.

Future Improvements

>Improve distance accuracy with depth estimation techniques.

>Add multi-object tracking for consistent measurements.

>Enhance speed optimization for real-time performance.

Acknowledgments

>Built using Ultralytics YOLOv8

>OpenCV for video processing

License

>MIT License
