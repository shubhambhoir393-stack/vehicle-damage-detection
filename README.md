# Vehicle Damage Detection 🚗💥

This project is a **Streamlit web application** that classifies vehicle images into different **damage categories** using a **deep learning (CNN / ResNet) model**.

The application allows users to upload a vehicle image and predicts the type of damage present.

---

## 🔍 Problem Statement

Given an image of a car, classify it into one of the following categories:

- Front Breakage
- Front Crushed
- Front Normal
- Rear Breakage
- Rear Crushed
- Rear Normal

This is an **image classification problem**, not object detection.

---

## 🧠 Model Details

- Architecture: **ResNet (transfer learning)**
- Framework: **PyTorch**
- Image size: **224 × 224**
- Normalization: ImageNet mean & std
- Output: 6 damage classes

> ⚠️ Note:  
> The model performs **image-level classification**.  
> It does **not localize or detect exact damage areas**, so some misclassifications are expected.

---

## 🖥️ Streamlit Application

### Features
- Upload `.jpg` / `.png` vehicle images
- Display uploaded image
- Predict vehicle damage category
- Simple and clean UI using Streamlit

---
vehicle-damage-detection/
│
├── app.py # Streamlit app
├── model_helper.py # Model loading & prediction logic
├── requirements # Python dependencies
├── README.md # Project documentation
├── app_screenshot.jpg # App UI screenshot
└── .gitignore # Ignored files (models, temp files)


---

## ⚙️ Installation & Run Locally

### 1️⃣ Create virtual environment (optional)
```bash
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

2️⃣ Install dependencies
pip install -r requirements

3️⃣ Run the Streamlit app
streamlit run app.py

Open browser at:
http://localhost:8501

📸 Sample Outpu
Predicted Class: Front Breakage

⚠️ Limitations

Model accuracy depends on training data quality
Misclassification can occur for:
Different lighting conditions
Unseen angles
Clean vehicles with reflections
Not suitable for insurance-grade damage estimation

🧑‍💻 Tech Stack

Python
PyTorch
Torchvision
Streamlit
Pillow
## 📂 Project Structure

