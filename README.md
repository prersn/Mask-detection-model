# Mask Detection System

The Mask Detection System is an AI-powered application designed to automatically detect whether individuals are wearing masks in images or live video streams. Developed to support public health initiatives and safety protocols, this system provides a reliable and efficient solution for enforcing mask-wearing policies in various environments.

## Annotation and Dataset

### Annotation
1. **Annotation Process:**
   - Annotate images of people with and without masks using Roboflow or any other annotation tool.
   - Ensure that each annotated image is labeled correctly to indicate whether the individual is wearing a mask or not.

2. **Export Dataset:**
   - After annotating the images, export the annotated dataset from Roboflow.
   - Alternatively, you can use your own dataset if you have already annotated images.

## Model Training

### Using Provided Code
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/mask-detection.git
   cd mask-detection

# Installation and Usage

2. **Install Dependencies:**
```bash
pip install -r requirements.txt

# Training the Model

1. Open the provided notebook "mask_final.ipynb" in Google Colab or any other suitable environment.
2. Follow the instructions in the notebook to execute each code cell and train the model.
3. Once training is complete, save the trained YOLOv5 model file (typically with a .pt extension) to the yolov5 directory in the project.

# Downloading the Trained Model

After training, download the trained YOLOv5 model file to your local machine.

# Running in YOLOv5 Repository

1. Clone YOLOv5 Repository:

```bash
git clone https://github.com/ultralytics/yolov5.git

# Running in YOLOv5 Repository

2. Navigate to YOLOv5 Directory:
   ```bash
   cd yolov5

# Run Detection Script

1. Choose one of the YOLOv5 script files (e.g., detect.py, detect_video.py) to run.
2. Open the chosen script file in a text editor.
3. Configure any necessary parameters or paths within the script, such as specifying the path to the trained model file.
4. Run the script in your preferred environment by executing the command similar to the one you provided earlier:
   ```bash
   python detect.py --weights /path/to/your/trained/model.pt --source /path/to/your/input
Replace `/path/to/your/trained/model.pt` with the path to your trained YOLOv5 model file.
Replace `/path/to/your/input` with the path to the input source (image or video stream).

## Contributing

Contributions to the project are welcome! Whether it's bug fixes, feature enhancements, or documentation improvements, feel free to submit pull requests to help make the Mask Detection System even better.

## License

This project is licensed under the MIT License, allowing for both personal and commercial use with proper attribution.

## Acknowledgments

We would like to thank the open-source community for their contributions and support in developing this project.

## About the Author

This project is developed and maintained by [Your Name]. For any questions, feedback, or inquiries, please contact [your email or preferred contact information].
