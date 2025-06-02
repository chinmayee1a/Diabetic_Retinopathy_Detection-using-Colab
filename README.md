# Diabetic Retinopathy Detection - APTOS 2019

This project implements a Convolutional Neural Network (CNN) to classify retinal fundus images into 5 severity levels of diabetic retinopathy using data from the APTOS 2019 Kaggle competition. It is designed to run on Google Colab using pre-processed datasets (`train_Data_X.npy`, `train_Data_Y.npy`).

## 🧠 Severity Grading Levels

| Grade | Label             |
|-------|-------------------|
| 0     | No DR             |
| 1     | Mild              |
| 2     | Moderate          |
| 3     | Severe            |
| 4     | Proliferative DR  |

---

## 📁 Dataset

- Images are preprocessed to 300x300 pixels and saved as NumPy arrays:
  - `train_Data_X.npy` – input images
  - `train_Data_Y.npy` – labels (0–4)

- Original dataset: [APTOS 2019 Blindness Detection](https://www.kaggle.com/c/aptos2019-blindness-detection)

---

## 🚀 How to Run the Notebook

### 1. Open the Notebook in Google Colab

📎 [Open in Colab](https://colab.research.google.com/drive/1_BvUiFZlatdaZusk_MYgBF0AdpxXw8-p)

### 2. Setup Google Drive Access
The notebook uses `PyDrive` to load `.npy` files from Google Drive.

- Ensure you are logged into your Google account
- Authenticate access when prompted

### 3. Change Runtime Settings

- Go to `Runtime` > `Change runtime type`
- Set **Hardware accelerator** to **GPU**
- (Optional) Click on **Factory reset runtime** to enable high-RAM mode

### 4. Run All Cells

- Click `Runtime` > `Run all`
- The following will happen:
  - Load and display example fundus images
  - Split the dataset into training (80%) and testing (20%)
  - Build and train a CNN model
  - Evaluate and visualize predictions and performance

---

## 📦 Requirements

- Google Colab (no local install needed)
- Python libraries (already available on Colab):
  - `numpy`
  - `tensorflow`
  - `matplotlib`
  - `cv2`
  - `pydrive`

---

## 📊 Output

- Training and validation accuracy/loss plots
- Prediction titles on sample test images
- Final test accuracy & loss (e.g., ~75–85% accuracy on test set)

---

## 📜 License

This project is open-source and available under the MIT License.
