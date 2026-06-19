
# Face Recognition System using OpenCV (LBPH)

A complete face recognition system developed using Python and OpenCV. The project demonstrates the complete computer vision pipeline from image preprocessing to face recognition using the Local Binary Pattern Histogram (LBPH) algorithm.

---

## 📌 Project Overview

This project performs face recognition by following a structured machine learning workflow:

1. Data Collection
2. Image Preprocessing
3. Face Detection
4. Face Recognition (LBPH)
5. Model Evaluation

The implementation is educational and demonstrates how classical computer vision techniques can be used to build a face recognition system without deep learning.

---

## 🛠 Technologies Used

- Python 3
- OpenCV
- NumPy
- Matplotlib
- JSON
- Google Colab / Jupyter Notebook

---

## 📂 Project Structure

```
Face-Recognition-System/
│
├── dataset/
│   ├── Person1/
│   ├── Person2/
│   └── ...
│
├── preprocessing/
│
├── face_model.yml
├── label_names.json
├── haarcascade_frontalface_default.xml
│
├── Phase1_DataCollection.ipynb
├── Phase2_Preprocessing.ipynb
├── Phase3_Training.ipynb
├── Phase4_Testing.ipynb
│
├── results/
│
├── README.md
└── requirements.txt
```

---

## 📖 Project Phases

### Phase 1 – Data Collection

- Created a structured dataset.
- Stored images of multiple individuals.
- Organized images into separate folders for each person.

---

### Phase 2 – Image Preprocessing

The collected images were preprocessed to improve recognition performance.

Preprocessing techniques included:

- Conversion to grayscale
- Image resizing
- Histogram Equalization
- Gaussian Blur
- Face cropping using Haar Cascade

These steps reduce noise and normalize images before training.

---

### Phase 3 – Model Training

Face recognition was performed using the **Local Binary Pattern Histogram (LBPH)** algorithm.

Training procedure:

- Load all training images
- Detect faces
- Extract face regions
- Train the LBPH recognizer
- Save the trained model (`face_model.yml`)
- Save label mappings (`label_names.json`)

---

### Phase 4 – Model Testing & Evaluation

The trained model was evaluated on unseen test images.

The evaluation process included:

- Face detection
- Face recognition
- Confidence score calculation
- Prediction of person identity

Performance metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

## ⚙ How to Run

### 1. Clone Repository

```bash
git clone https://github.com/emanirfanbiz/Attendance-with-Face-Recognition-System
```

---

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 3. Download Haar Cascade

Download:

```
haarcascade_frontalface_default.xml
```

and place it in the project directory.

---

### 4. Train the Model

Run:

```
Phase3_Training.ipynb
```

This creates:

```
face_model.yml
label_names.json
```

---

### 5. Test the Model

Run:

```
Phase4_Testing.ipynb
```

The notebook will:

- Detect faces
- Predict identities
- Display confidence scores
- Compute evaluation metrics

---

## 📊 Results

The system successfully:

- Detects frontal faces
- Recognizes known individuals
- Stores the trained model
- Evaluates recognition performance using multiple metrics

---

## 📚 Concepts Covered

- Computer Vision
- Image Processing
- Face Detection
- Feature Extraction
- Local Binary Patterns (LBP)
- Histogram-based Recognition
- Machine Learning Evaluation Metrics

---

## 🚀 Future Improvements

- Replace Haar Cascade with MTCNN
- Use FaceNet embeddings
- Implement DeepFace
- Add real-time webcam recognition
- Improve recognition under varying lighting conditions
- Deploy as a web application using Flask or Streamlit

---

## 👨‍💻 Author

**Eman Irfan**

BS Computer Science

Machine Learning Enthusiast | Web Developer | Computer Vision

GitHub: https://github.com/emanirfanbiz

LinkedIn: www.linkedin.com/in/eman-irfan-2b5657327

---
