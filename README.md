# Smart Traffic Analyzer with YOLOv8
![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![YOLOv8](https://img.shields.io/badge/YOLOv8-ultralytics-orange?logo=github)
![Colab](https://img.shields.io/badge/Runs%20in-Google%20Colab-brightgreen?logo=googlecolab)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green?logo=opencv)
![Status](https://img.shields.io/badge/Status-Prototype-yellow)

This project demonstrates object detection and tracking on traffic video footage using the YOLOv8 deep learning model. The system processes a video file frame-by-frame, identifies objects such as vehicles and pedestrians, and outputs annotated videos with bounding boxes, class labels, and persistent tracking IDs. Additional visualizations such as heatmaps are generated to highlight high-traffic areas over time.

---

## 🚦 Features
- 🔍 Real-time object detection and object tracking with YOLOv8
- ⚡ ByteTrack integration for consistent object IDs across frames
- 🎥 Annotated `.mp4` output videos with bounding boxes and tracking overlays
- 🌡️ Cumulative heatmap visualization to highlight object density
- 🧊 Side-by-side visual comparison of original vs. tracked frames

---

## 🛠️ Technologies Used
- Python
- [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)
- ByteTrack (built into YOLOv8's tracker)
- OpenCV
- Google Colab

---

## 📋 How It Works
1. Upload a short `.mp4` traffic video to Colab.
2. YOLOv8 detects objects and applies ByteTrack to assign consistent IDs.
3. Detection results are saved to annotated videos.
4. A cumulative heatmap is generated based on detection history.
5. All outputs can be previewed inline or downloaded.

---

## 🧪 Sample Outputs

<table>
  <tr>
    <td><strong>Input Video</strong></td>
    <td><strong>YOLOv5 Detection</strong></td>
    <td><strong>YOLOv8 + ByteTrack</strong></td>
  </tr>
  <tr>
    <td><img src="assets/traffic_input_gif.gif" width="320"/></td>
    <td><img src="assets/yolo_output_gif.gif" width="320"/></td>
    <td><img src="assets/yolo_output_2.gif" width="320"/></td>
  </tr>
</table>

- **YOLOv5** shows raw object detection without tracking.
- **YOLOv8 + ByteTrack** enhances the output with persistent object IDs for each tracked entity.

---

## 🌡️ Heatmap Visualizations

<table>
  <tr>
    <td><strong>Object Density Heatmap</strong></td>
    <td><strong>Overlay on Sample Frame</strong></td>
  </tr>
  <tr>
    <td><img src="assets/heatmap.png" width="400"/></td>
    <td><img src="assets/heatmap_overlay_blurred.png" width="400"/></td>
  </tr>
</table>

- The heatmap shows areas of frequent detection across all frames.
- The overlay visualizes traffic density directly on a representative frame.

---

<table>
  <tr>
    <td><strong>Heatmap Overlay (All Frames)</strong></td>
    <td><strong>Side-by-Side Comparison</strong></td>
  </tr>
  <tr>
    <td><img src="assets/heatmap_video_gif.gif" width="400"/></td>
    <td><img src="assets/heatmap_side_gif.gif" width="600"/></td>
  </tr>
</table>

- Heatmap accumulation builds up over time and blends with live footage.
- Side-by-side comparison helps visualize the impact of heatmap overlays and detection labels in real-time.

---

## 🚀 Run It in Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DP6W3bgCwbKlj6UQw8aJOKavvJw8cfBW?usp=sharing)

---

## 👤 Author
Built by **Jalen Gilbert** as a demonstration of fundamental computer vision techniques using modern deep learning libraries.