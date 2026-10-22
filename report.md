# YOLO Object Detection and Tracking Technical Report

## 1. Introduction
This report documents the object detection pipeline implemented using YOLOv8 to process static images and video streams.

## 2. Functions & Implementation Details
- **Model Initialisation**: Used `YOLOv8n` pretrained model on COCO dataset.
- **Image Processing Routine**: Reads images, extracts bounding box coordinates, tallies detected objects per class, and renders visual annotations.
- **Video Processing Routine**: Frame-by-frame analysis with OpenCV, rendering bounding boxes and dynamic class tally overlays using `cv2.putText`.
- **Transcoding**: Processed raw video streams converted via FFmpeg (`libx264`) into web-standard MP4 format.

## 3. Deliverables Summary
- `output_processed_video.mp4`: Complete video output featuring bounding boxes and real-time class counts.
- `screenshot_*.jpg`: Visual evidence/screenshots of static image and video detection results.
- `report.md`: Detailed documentation.
