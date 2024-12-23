# **Real-Time Object Detector**

This project is a Python-based implementation of a **Real-Time Object Detection System** using **YOLOv3** and **OpenCV**. The system leverages computer vision to detect multiple objects in real-time through a live webcam feed, highlights them with bounding boxes, and displays class labels along with confidence scores.

---

## **About the Project**
- **Real-Time Object Detection:** This project uses the YOLOv3 model to detect objects in a live video feed captured from a webcam.
- **Object Classes:** The model is capable of detecting 80 different objects such as `person`, `bottle`, `car`, and more, based on the COCO dataset.
- **Performance:** Utilizes Non-Maximum Suppression (NMS) to refine object detection by removing redundant bounding boxes, ensuring high accuracy.

### **Features**
- Multi-object detection in real-time.
- Displays bounding boxes with labels and confidence scores.
- Built with Python, OpenCV, and YOLOv3 for high performance and accuracy.

### **Demo**
Here is a sample output of the program detecting objects in a real-time video feed:

![Demo](Demo.png)

---

## **How to Clone and Run**

### **Step 1: Clone the Repository**
To get started, clone this repository to your local machine:
```bash
git clone https://github.com/AbhigyanRaj/RealTImeObject_Detector.git
```
Navigate to the project directory:
```bash
cd RealTImeObject_Detector
```

### **Step 2: Set Up a Virtual Environment**
Create a virtual environment to manage dependencies:
```bash
python -m venv venv
```
Activate the virtual environment:
- On Windows:
  ```bash
  venv\Scripts\activate
  ```
- On macOS/Linux:
  ```bash
  source venv/bin/activate
  ```

### **Step 3: Install Dependencies**
Install the required Python libraries:
```bash
pip install opencv-python numpy
```

### **Step 4: Download YOLO Files**
Download the following YOLOv3 files and place them in the project directory:
- `yolov3.weights` (pre-trained weights): [Download here](https://pjreddie.com/media/files/yolov3.weights)
- `yolov3.cfg` (model configuration): [Download here](https://github.com/pjreddie/darknet/blob/master/cfg/yolov3.cfg)
- `coco.names` (object class names): [Download here](https://github.com/pjreddie/darknet/blob/master/data/coco.names)

Your project structure should look like this:
```
RealTImeObject_Detector/
├── Demo.png
├── README.md
├── coco.names
├── main.py
├── venv/
├── yolov3.cfg
├── yolov3.weights
```

### **Step 5: Run the Program**
Execute the following command to start the object detection system:
```bash
python main.py
```

### **Step 6: Interact with the System**
- The webcam feed will open, and the program will detect objects in real-time.
- To exit the program, press **`q`**.

---

## **File Details**
- **`main.py`**: The main Python script that runs the real-time object detection system.
- **`yolov3.cfg`**: The YOLOv3 configuration file that defines the model architecture.
- **`yolov3.weights`**: Pre-trained weights for the YOLOv3 model.
- **`coco.names`**: A text file containing the names of the 80 object classes YOLO can detect.
- **`Demo.png`**: An example output image showing the object detection in action.
- **`venv/`**: The virtual environment directory containing all installed dependencies.

---

## **Made By**
**Abhigyan Raj ;)**
