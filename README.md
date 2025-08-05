# 🍕 Food Recognition & Calorie Estimation System 

This project builds an end-to-end system to *recognize food items from images* and *estimate calorie content, helping users make informed dietary choices. Built for **Task-05 – Comillas Negras*, the system generates synthetic datasets and performs recognition without the need for external APIs.

---

## 🚀 Features

- 🧠 Deep Learning model with *Transfer Learning (MobileNetV2)*
- 🍽 Classifies 10 common food items
- 🔢 Estimates calorie content per portion based on 100g nutritional values
- 🎨 Generates *synthetic food images* using NumPy and noise blending
- 📊 Realistic model training & confidence estimates
- ✅ *Google Colab ready*, no API keys required
- 🖼 Interactive upload and test functionality

---

## 📦 Installation (Colab)

bash
!pip install tensorflow==2.13.0
!pip install opencv-python
!pip install pillow matplotlib seaborn scikit-learn requests numpy pandas


---

## 📁 Dataset

Synthetic images are generated for the following 10 categories:


pizza, burger, pasta, salad, sandwich,
rice, chicken, fish, apple, banana


Each category has *120+ synthetic samples* with category-specific textures and noise.

---

## 📸 Sample Output (Visual)

![Food Output](https://github.com/Vijay1097/Prodigy_ML_05/blob/main/food%20output.jpg)

*Prediction*: Pizza  
*Confidence*: ~95.6%  
*Estimated Calories*: ~412.8 kcal  
*Verdict*: ⚠ High calorie food – consider smaller portions!

---

## 🧪 Key Functionalities

| Function                | Description                                           |
|-------------------------|-------------------------------------------------------|
| create_synthetic_data| Generates realistic synthetic food images             |
| prepare_dataset       | Loads & augments dataset using ImageDataGenerator  |
| build_model           | Builds CNN using MobileNetV2 (transfer learning)      |
| train_model           | Trains model with validation and noise injection     |
| predict_food          | Predicts food type and calorie content               |
| upload_test_image     | Upload and analyze your own food image               |
| test_random_samples   | Randomly evaluates performance from generated data    |

---

## 🧠 How It Works

1. *Synthetic Dataset Generation* – Images for each food category are generated with texture and color variations.
2. *Transfer Learning* – MobileNetV2 (ImageNet pretrained) is used as the base model for efficient training.
3. *Calorie Estimation* – Each predicted class maps to a calorie-per-100g value and estimates a full portion.
4. *Interactive Testing* – User can upload an image to analyze or test with random samples from dataset.

---

## 📊 Model Info

- Input Image Size: 224x224
- Classes: 10 Food Categories
- Accuracy: ~88–95% after 10 epochs (synthetic data)
- Optimizer: Adam, Loss: Categorical Crossentropy
- Realistic noise & dropout to simulate real-world conditions

---

## 🖥 How to Use (Colab)

1. Open the notebook in Google Colab.
2. Run installation commands.
3. Execute the code cell to launch the interactive menu.
4. Train the model, test, or upload your image for predictions.

---

## 🧑‍🍳 Food Categories with Calories (per 100g)

| Food     | Calories |
|----------|----------|
| Pizza    | 266 cal  |
| Burger   | 295 cal  |
| Pasta    | 131 cal  |
| Salad    | 152 cal  |
| Sandwich | 250 cal  |
| Rice     | 130 cal  |
| Chicken  | 239 cal  |
| Fish     | 206 cal  |
| Apple    | 52 cal   |
| Banana   | 89 cal   |

---


## ✅ Future Work

- 🧠 Add real image dataset support
- 🧾 Include macro-nutrient estimates (protein, fat, carbs)
- 🌐 Web interface for mobile testing
- 📷 Use real-time webcam food prediction

---

