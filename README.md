
# Road Damage Detection Using YOLOv7 and Coordinate Attention

## Project Overview

This project focuses on detecting road damages such as cracks, potholes, and other surface defects using state-of-the-art deep learning techniques. We use **YOLOv7**, a cutting-edge object detection model, enhanced with **Coordinate Attention** modules to improve the model’s focus on relevant features and spatial information. This combination boosts detection accuracy and robustness, especially in challenging environments with varying lighting and complex backgrounds.

## Key Features

* **YOLOv7 Architecture:** Provides fast and accurate real-time object detection.
* **Coordinate Attention Module:** Enhances feature representation by capturing precise positional information along with channel attention.
* **Multi-class Detection:** Detects different types of road damages for better road maintenance planning.
* **Custom Dataset:** Trained on a curated dataset of road images with annotated damages to improve model generalization.

## Repository Contents

```
├── dataset/                # Annotated road damage images
├── weights/                # Pretrained YOLOv7 models
├── train.py                # Training script integrating coordinate attention
├── detect.py               # Script for detecting damages on new images/videos
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
```

## Installation & Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/road-damage-detection.git
   cd road-damage-detection
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Train the model (optional):

   ```bash
   python train.py --data dataset.yaml --weights yolov7.pt
   ```

4. Run inference on images or videos:

   ```bash
   python detect.py --source path/to/image_or_video
   ```

## Results

* High precision and recall in detecting multiple damage types.
* Robust detection under various lighting and weather conditions.
* Enables efficient road maintenance scheduling by accurately locating damages.

## Future Work

* Integrate with drone or vehicle-mounted cameras for real-time monitoring.
* Expand dataset with more damage types and varied road conditions.
* Optimize model for embedded or edge devices.

## License

MIT License

