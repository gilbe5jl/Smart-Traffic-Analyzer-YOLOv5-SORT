# Smart Traffic Analyzer with YOLOv5

This project demonstrates object detection on traffic video footage using the YOLOv5 deep learning model. The system processes a video file frame-by-frame, identifies objects such as cars and pedestrians, and outputs an annotated video with bounding boxes and class labels.

## Features
- 🔍 Real-time object detection with YOLOv5
- 🎞️ Frame-by-frame video processing using OpenCV
- 📦 Outputs annotated `.mp4` video showing detection results

## Technologies Used
- Python
- OpenCV
- PyTorch
- YOLOv5 (via `torch.hub`)

## How It Works
1. Upload a short `.mp4` video to Colab.
2. YOLOv5 detects objects in each frame.
3. Detected objects are annotated and written to a new output video.
4. Final result is previewed inline or downloaded.



## Sample Output

**Input Video:**
![input](assets/traffic_input_gif.gif)

**Annotated Output with YOLOv5:**
![output](assets/yolo_output_gif.gif)

*Detection results showing bounding boxes and class labels over real traffic footage.*

---

### 🚀 Run It in Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

---

### Author
Built by Jalen Gilbert as a demonstration of fundamental computer vision techniques using modern deep learning libraries.