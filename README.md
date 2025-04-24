# Automatic Number Plate Recognition using YOLO-NAS and EasyOCR (Images & Videos)

<img src="./Videos/streamlit_demo.gif">

This project uses YOLO-NAS and EasyOCR to detect license plates and perform Optical Character Recognition (OCR) on them. The project includes both image and video processing capabilities, and has been deployed as a Streamlit web application.

[GitHub](https://github.com/JacobJ215/YOLO-NAS-OCR-WebApp)

## Features
* Real-time license plate detection using YOLO-NAS
* Optical Character Recognition (OCR) using EasyOCR
* Interactive user interface built with Streamlit

## Dataset
The dataset used for training and testing the YOLO-NAS model contains 484 annotated images of cars with license plates. The images were sourced from "Brave Images", "Google Images", and "https://flickr.com/". The annotations were made using [RoboFlow](https://app.roboflow.com/yolotraining-dfaoh/ocr-nsde5/deploy/1). 


## Evaluation

* 'PPYoloELoss/loss_cls': 0.9181855
* 'PPYoloELoss/loss_iou': 0.17447565
* 'PPYoloELoss/loss_dfl': 0.9500977
* 'PPYoloELoss/loss': 1.8294234

* 'Precision@0.50': 0.02825159952044487
* 'Recall@0.50': 1.0
* 'mAP@0.50': 0.9623407125473022
* 'F1@0.50': 0.05495075136423111

## Running the Web Application

1. Clone the repository:
```
git clone https://github.com/dovannam115/OCR_BKS_NAS/edit/main"
cd YOLO-NAS-OCR-WebApp
```

2. Install the required dependencies:
```
pip install -r requirements.txt
```

3. Run the Streamlit app:
```
streamlit run app.py
```

## Usage
The web application provides two main modes:
Run on Image: Upload an image containing a license plate, and the application will perform real-time detection and OCR, displaying the extracted text from the license plate.
### Run on Image
![](Screenshots/run_on_image.jpg)

Run on Video: Upload a video with license plates, and the application will perform real-time detection and OCR on the video frames, showing the extracted text and the 
frame rate.

### Run on Video
![](Screenshots/run_on_video.png)



## Acknowledgments

The YOLO-NAS model used in this project is based on Super-Gradients Repository.

EasyOCR is an excellent OCR library developed by Jaided AI.
