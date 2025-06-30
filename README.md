# Garbage Classifier System

A real-time deep learning waste detection and garbage classification system using YOLOv8 object detection framework, with an interactive Flask-based web interface.

## Features

- Automated Dataset Processing: Converts image datasets organized in class folders to YOLO format with bounding box annotations.
- Flexible Training Pipeline: Supports training from scratch, resuming previous training sessions, or loading pretrained available fine-tuned YOLOv8 models for garbage classification.
- Real-time Inference: Detects and classifies garbage in live webcam feeds with confidence scores.
- Web Interface: Facilitates a user-friendly Flask-based web app for uploading images or analyzing live camera feeds, with a responsive design for desktop and mobile.
- QR Code Access: Generates QR codes for easy mobile access to the web interface over a local network.
- Batch Processing: Processes folders of images, saves annotated results, and generates JSON summaries of predictions.
- Comprehensive Analytics: Offers detailed training metrics and model performance analysis.
- MPS/GPU Support: Automatically optimizes for Apple Silicon (MPS), NVIDIA GPUs (CUDA), with support for seamless CPU fallback.

## Project Structure

```
├── Garbage Classifier.ipynb         # Main notebook with end-to-end implementation
├── garbage_classification_yolo/     # Data, models weights and other files
├── ... other files ...
```

## How to Run

1. Clone this repository on your local machine.
2. Download the required dataset and model files using this [Google Drive Link](https://drive.google.com/file/d/1dXeYc-lT2kkoCLCo-sLE8p92jvc1s5yP/view?usp=sharing). Download and extract the `garbage_classification_yolo.zip` file and place it in the main cloned root project directory.
> The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/asdasdasasdas/garbage-classification).
3. Open and run the first cell of the `Garbage Classifier.ipynb` Jupyter Notebook file to install the required dependencies.
4. Run and execute the second cell of the file, where you can train from scratch, load existing available model, continue training existing model, test the model on sample images, upload your own images for garbage classification (or use real-time webcam for the same), or exit. 

When running the real-time inference, you can either test the model real-time on your system (using `http://localhost:5001`) via your webcam (if available) or by uploading the images; or you can scan the QR Code on your smartphone and carry out the same process through your phone camera.

If required, you may change the code's configurations to customize and tailor it to your needs too.

## Contributing

Contributions are welcome!

## License

Distributed under the MIT License.  
