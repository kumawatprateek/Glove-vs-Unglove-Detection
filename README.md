# Glove vs. Unglove Detection

## 📌 Project Overview

This project aims to detect whether a person is **wearing gloves** or **not wearing gloves** in an image. It uses a custom-trained deep learning model built on the collected dataset of gloved and ungloved hands.

The workflow includes:

1. **Dataset Preparation** – Collected and organized images into `Gloved/` and `Ungloved/`.
2. **Preprocessing** – Resized images to a consistent shape.
3. **Model Training** – Trained a CNN-based image classification/detection model.
4. **Inference Script** – A script/notebook to run predictions on new images.
5. **Output & Logs** – Sample images with predictions and JSON log files are provided.

---

## 📂 Repository Structure

```
Part_1_Glove_Detection/
├── detection_script.py or .ipynb   # Inference code (run model on test images)
├── output/                         # sample images with detection results and JSON logs for each test image (class, confidence, filename)
├── Model/                      
├── processed_dataset/   
├── date_set/     
└── README.md                       # Project documentation
```

---

## 🚀 How to Run

### 1. Clone Repo & Setup

```bash
git clone <your-repo-link>
cd Part_1_Glove_Detection
pip install -r requirements.txt
```

### 2. Run Inference

If using **Python script**:

```bash
python detection_script.py --input <path_to_image_or_folder>
```

If using **Jupyter Notebook**:

* Open `detection_script.ipynb` in Jupyter/Colab
* Run all cells to see predictions

### 3. Outputs

* Annotated images saved in `output/`
* JSON logs saved in `logs/`

---

## 🖼️ Sample Output

* **Gloved hand** → Detected with confidence (e.g., 0.94)
* **Ungloved hand** → Detected with confidence (e.g., 0.87)

(See images in `/output` for examples.)

---

## 📊 Logs Format

Each image prediction is stored in JSON format under `/logs/`. Example:

```json
{
  "filename": "sample1.jpg",
  "prediction": "Gloved",
  "confidence": 0.94
}
```

---

## 🛠️ Tools & Libraries

* Python 3.10+
* TensorFlow / Keras or PyTorch (depending on your training)
* OpenCV
* NumPy, Matplotlib
* Jupyter Notebook

---

## 👨‍💻 Author

**Prateek Kumawat**
