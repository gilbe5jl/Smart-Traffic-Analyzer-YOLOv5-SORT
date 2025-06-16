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
4. 



## Sample Output

**Input Video:**
![input](assets/traffic_input_gif.gif)

**Annotated Output with YOLOv5:**
![output](assets/yolo_output_gif.gif)
*Detection results showing bounding boxes and class labels over real traffic footage.*

switched from YOLOv5+SORT → YOLOv8+ByteTrack

![output](assets/yolo_output_2.gif)





video 1/1 (frame 53/750) /content/yolov5/traffic_input.mp4: 384x640 1 person, 3 cars, 142.1ms
video 1/1 (frame 54/750) /content/yolov5/traffic_input.mp4: 384x640 1 person, 3 cars, 1 truck, 145.2ms
video 1/1 (frame 55/750) /content/yolov5/traffic_input.mp4: 384x640 1 person, 2 cars, 1 truck, 149.0ms
video 1/1 (frame 56/750) /content/yolov5/traffic_input.mp4: 384x640 1 person, 3 cars, 145.0ms
video 1/1 (frame 57/750) /content/yolov5/traffic_input.mp4: 384x640 1 person, 3 cars, 1 truck, 149.6ms
video 1/1 (frame 58/750) /content/yolov5/traffic_input.mp4: 384x640 1 person, 3 cars, 158.2ms
video 1/1 (frame 59/750) /content/yolov5/traffic_input.mp4: 384x640 1 person, 3 cars, 142.4ms
video 1/1 (frame 60/750) /content/yolov5/traffic_input.mp4: 384x640 1 person, 3 cars, 145.4ms
---

### 🚀 Run It in Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DP6W3bgCwbKlj6UQw8aJOKavvJw8cfBW?usp=sharing)

---

### Author
Built by Jalen Gilbert as a demonstration of fundamental computer vision techniques using modern deep learning libraries.