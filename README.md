# Vehicle Damage Detection App

This application allows users to drag and drop an image of a car and predicts the type of damage present in the vehicle.

The model is trained on **third-quarter front and rear view images**, so for best results, the uploaded image should capture either the **front-quarter** or **rear-quarter** view of the car.

![App Screenshot](app_screenshot.jpg)

---

## 🧠 Model Details

1. Transfer learning using **ResNet50**
2. Trained on approximately **1,700 images**
3. Total **6 target classes**:
   - Front Normal  
   - Front Crushed  
   - Front Breakage  
   - Rear Normal  
   - Rear Crushed  
   - Rear Breakage  
4. Validation accuracy achieved: **~80%**

> ⚠️ Note:  
> This is an **image-level classification model**, not an object detection model.  
> It does not locate the exact damaged area and may misclassify some images depending on lighting, angle, or reflections.

---

## ⚙️ Setup Instructions

### 1️⃣ Install dependencies
```bash
pip install -r requirements.txt
2️⃣ Run the Streamlit app
bash
Copy code
streamlit run app.py
The application will be available at:

arduino
Copy code
http://localhost:8501
🛠 Tech Stack
Python

PyTorch

Torchvision

Streamlit

Pillow
