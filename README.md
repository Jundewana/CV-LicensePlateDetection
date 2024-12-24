# CV-LicensePlateDetection

This project aims to detect vehicle license plates using the YOLOv8 model.

## Environment Setup

1. Clone this repository.
2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

## Using Roboflow

This project uses Roboflow to manage the dataset. Here is an example code to download the dataset using Roboflow:

```python
from roboflow import Roboflow

rf = Roboflow(api_key="YOUR_API_KEY")
project = rf.workspace("general-pdvg1").project("sca-kel.-3-tugas-p12")
version = project.version(3)
dataset = version.download("yolov8")
