# Object_detection
Engineered a full Computer Vision desktop application using TensorFlow (SSD MobileNet V2) and OpenCV for real-time object detection across 90+ COCO classes.
# 👁️ Real-Time Deep Learning Object Recognition System (Desktop App)

A comprehensive Computer Vision application built in Python that uses a pre-trained Deep Learning model for real-time object detection via a camera or static images, featuring an intuitive GUI and voice feedback.

## ✨ Features

* **Real-Time Detection:** Utilizes the camera feed (cv2) for instantaneous object detection and analysis.
* **Deep Learning Model:** Employs the **SSD MobileNet V2** (Single Shot MultiBox Detector) model, pre-trained on the COCO dataset, for high-speed, accurate detection of **90+ object classes**.
* **Interactive GUI:** Built with **Tkinter** for an intuitive, multi-function desktop interface (Start System, Capture Image, Detect Object, Exit).
* **Voice Feedback:** Integrates **pyttsx3** (Text-to-Speech) to verbally announce system status and detected object names and classes.
* **Image Processing:** Draws real-time bounding boxes, class labels, and confidence scores directly onto the image using **OpenCV** and **NumPy**.
* **System Integrity:** Uses `subprocess` to manage the launch and flow between different application modules.

## 🛠️ Technologies Used

| Category | Technology | Purpose |
| :--- | :--- | :--- |
| **Primary Language** | Python 3.x | Core application logic and scripting. |
| **Deep Learning** | **TensorFlow** | Model loading and inference (ssd_mobilenet_v2). |
| **Computer Vision** | **OpenCV (cv2)** | Camera capture, image manipulation, and drawing bounding boxes. |
| **GUI** | **Tkinter** | Creating the cross-platform desktop application interface. |
| **Core Libraries** | NumPy, PIL (Pillow) | Image data handling, array manipulation, and image loading. |
| **Voice Output** | pyttsx3 | Text-to-Speech integration for hands-free feedback. |

## 🚀 Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You will need Python 3.x installed, along with the following libraries:

```bash
pip install opencv-python tensorflow numpy pillow pyttsx3

🖼️ Application Flow (Example)
1. Start: The system initializes and greets the user via voice output.

2. Capture Image: Opens the webcam and captures a frame after 3 seconds or when the user presses 'a'.

3. Detect Object: Opens a file dialog to select an image (.jpg, .png, etc.). The model runs inference, and the resulting image with bounding boxes is displayed using matplotlib.

4. Voice Feedback: The system announces the success and the name(s) of the detected object(s).

## 🚀 Getting Started

### Installation

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/ak-11bhardwaj/Object_detection](https://github.com/ak-11bhardwaj/Object_detection)
    ```

2.  **Download the Model:**

    * Download the pre-trained `ssd_mobilenet_v2_fpnlite_640x640_coco17_tpu-8` model directory and place it inside the cloned `Object_detection` folder. *(Note: You will need to specify the path to your model file.)*

3.  **Run the application:**

    ```bash
    python your_main_script_name.py
    ```
