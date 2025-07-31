# facial_exp_detect

A simple Python-based facial expression detection project utilizing computer vision and deep learning. This project enables real-time detection of human faces and the classification of facial expressions through your webcam or supplied images.

## Features

- **Real-time facial expression detection** using a webcam
- Detects and classifies basic facial expressions (such as happy, sad, angry, surprised, neutral, etc.)
- Uses Haarcascade for face detection
- Deep learning model for emotion recognition
- Modular Python codebase, easy to modify and extend

## Project Structure

```
facial_exp_detect/
│
├── camera.py               # Captures webcam input, streams frames
├── model.py                # Loads/trains the deep learning model for expression classification
├── main (1).py             # Main entry script to run the detection pipeline
├── Facial_Expression_Training.ipynb  # Jupyter Notebook for model training
├── templates/              # (Optional) HTML templates for web interface
├── haarcascade_frontalface_default.xml # Face detection cascade file
├── __pycache__/
├── README.md
```

## Getting Started

### Prerequisites

- **Python 3.6 or newer**
- **OpenCV**
- **Tensorflow** and/or **Keras**
- **NumPy**

Install required packages with:

```bash
pip install opencv-python tensorflow keras numpy
```

### How to Use

1. **Clone this repository**:
   ```bash
   git clone https://github.com/sushant607/facial_exp_detect.git
   cd facial_exp_detect
   ```

2. **Model Training (Optional)**:
   - Use `Facial_Expression_Training.ipynb` to train your own expression recognition model (requires suitable dataset, e.g., FER2013).

3. **Run Real-Time Detection**:
   ```bash
   python main\ \(1\).py
   ```
   - This will activate the webcam and display real-time facial expression classification.

4. **Face Detection**:
   - The included `haarcascade_frontalface_default.xml` is used for detecting faces in each video frame.

## Model & Dataset

- The model can be trained on datasets like **FER2013** (available via Kaggle).
- Modify `model.py` and the training notebook to adjust architecture or dataset for improved results.
