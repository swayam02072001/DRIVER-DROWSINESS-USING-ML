---

# DRIVER-DROWSINESS-USING-ML

## Overview
Driver drowsiness detection is a crucial technology aimed at preventing accidents caused by fatigued drivers. This project utilizes machine learning to monitor a driver's alertness and detect signs of drowsiness, thereby enhancing road safety.

## Features
- **Real-time monitoring:** Continuously assess the driver's state using video feed.
- **Facial landmarks detection:** Identify key facial features to detect signs of drowsiness.
- **Eye closure detection:** Monitor the percentage of eye closure over time.
- **Head position analysis:** Determine head pose to identify potential signs of fatigue.
- **Alert system:** Trigger alarms when drowsiness is detected.

## Installation

### Prerequisites
- Python 3.7+
- OpenCV
- Dlib
- Scikit-learn
- Numpy
- Scipy

### Clone the Repository
```bash
git clone https://github.com/SubhrjiT/DRIVER-DROWSINESS-USING-ML.git
cd DRIVER-DROWSINESS-USING-ML
```

### Install Dependencies
It is recommended to create a virtual environment before installing the dependencies.
```bash
pip install -r requirements.txt
```

## Usage

### Step 1: Prepare Dataset
Ensure you have a dataset containing images or video of faces with annotations for drowsiness. You can use existing datasets or collect your own.

### Step 2: Train the Model
Run the training script to train the machine learning model on your dataset.
```bash
python train_model.py --dataset /path/to/dataset
```

### Step 3: Run the Detection System
Use the detection script to start monitoring for driver drowsiness.
```bash
python detect_drowsiness.py --video /path/to/video
```
Or use the webcam for real-time detection:
```bash
python detect_drowsiness.py --webcam
```

## Project Structure
```
DRIVER-DROWSINESS-USING-ML/
├── datasets/                 # Directory to store datasets
├── models/                   # Pre-trained models and training scripts
├── utils/                    # Utility functions for data processing and model evaluation
├── requirements.txt          # Required Python packages
├── train_model.py            # Script to train the machine learning model
├── detect_drowsiness.py      # Script to run the drowsiness detection
└── README.md                 # Project README file
```

## Contributing
Contributions are welcome! Please fork this repository and submit pull requests with your changes.

### Steps to Contribute:
1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`.
3. Commit your changes: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature/your-feature-name`.
5. Submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- [Dlib](http://dlib.net/) for facial landmark detection.
- [OpenCV](https://opencv.org/) for real-time video processing.
- [Scikit-learn](https://scikit-learn.org/stable/) for machine learning algorithms.

---
