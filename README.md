# Mask Detection System

The Mask Detection System is an AI-powered application designed to automatically detect whether individuals are wearing masks in images or live video streams. Developed to support public health initiatives and safety protocols, this system provides a reliable and efficient solution for enforcing mask-wearing policies in various environments.

## Key Features

- **Real-time Mask Detection:** Utilizes deep learning algorithms to analyze input images or video streams in real-time, accurately identifying the presence or absence of masks on individuals' faces.
- **High Accuracy:** Trained on diverse datasets, the model achieves high accuracy in detecting masks under various conditions, including different lighting, angles, and types of masks.
- **Scalable Deployment:** The system can be deployed on edge devices or cloud platforms, offering scalability to meet the requirements of different deployment scenarios.
- **Customizable:** Users have the flexibility to customize the system according to specific use cases, such as adjusting detection thresholds or integrating with existing security systems.

## Getting Started

Follow these instructions to get the Mask Detection System up and running on your local machine or preferred environment.

### Prerequisites

- Python 3.6+
- pip package manager

### Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/mask-detection.git
    ```
2. **Navigate to the project directory:**
    ```bash
    cd mask-detection
    ```
3. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Obtain Dataset

- Annotate images of people with and without masks using Roboflow or any other annotation tool.
- Export the annotated dataset from Roboflow and place it in the `data` directory of the project.
- Alternatively, you can use an alternate dataset provided as a zip file downloaded from Roboflow. Extract the contents of the zip file and place them in the `data` directory of this repository.

### Train Model

- Open the provided notebook `mask_final.ipynb` in Google Colab or any other suitable environment.
- Follow the instructions in the notebook to execute each code cell and train the model.
- Once training is complete, save the trained YOLOv5 model file (typically with a `.pt` extension) to the `yolov5` directory in the project.

### Downloading Trained Model

- After training, download the trained YOLOv5 model file to your local machine.

### Running in YOLOv5 Repository

1. **Clone YOLOv5 Repository:**
    ```bash
    git clone https://github.com/ultralytics/yolov5.git
    ```
2. **Navigate to YOLOv5 Directory:**
    ```bash
    cd yolov5
    ```
3. **Run Detection Script:**
    - Choose one of the YOLOv5 script files (e.g., `detect.py`, `detect_video.py`) to run.
    - Open the chosen script file in a text editor.
    - Configure any necessary parameters or paths within the script, such as specifying the path to the trained model file.
    - Run the script in your preferred environment by executing the command similar to the one you provided earlier:
        ```bash
        python detect.py --weights /path/to/your/trained/model.pt --source /path/to/your/input
        ```
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
