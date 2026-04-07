#  Pantograph Detection

A computer vision project developed during an internship to detect and analyze the movement of a pantograph, pantobar, and cables in railway systems using YOLOv8.

##  About
This project processes railway video footage to monitor pantograph behavior in real time. It tracks horizontal and vertical movement, detects electrical sparks, measures contact points between the pantobar and cables, and logs all data into a CSV file — providing useful insights for railway maintenance and safety monitoring.

##  Features
- **Object Detection** — Detects pantograph, pantobar, and cables in each video frame using YOLOv8
- **Movement Tracking** — Calculates horizontal and vertical displacement between frames
- **Spark Detection** — Identifies electrical sparks by analyzing bright spots in the pantobar region
- **Contact Point Analysis** — Measures distances between the pantobar and cables
- **CSV Logging** — Saves timestamped movement and spark data for further analysis
- **Annotated Video Output** — Saves a processed video with visual overlays

##  Requirements

- Python 3.6+
- OpenCV (`opencv-python`)
- NumPy
- Ultralytics (YOLOv8)

Install all dependencies:
```bash
pip install opencv-python-headless numpy ultralytics
```

##  How to Run

1. Clone this repository
2. Add your trained YOLOv8 model weights and update the path in the notebook
3. Set your `input_video_path`, `output_video_path`, and `csv_output_path`
4. Open `Pantograph.ipynb` and run all cells

##  Output
- Annotated output video with bounding boxes and movement overlays
- CSV file containing per-frame movement and spark detection data

##  Notes
- The YOLO model must be trained specifically for pantograph, pantobar, and cable detection
- Detection thresholds may need tuning depending on lighting and video quality

##  License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.