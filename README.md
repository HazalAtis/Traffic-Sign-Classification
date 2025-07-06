# Traffic Sign Classification and Regularization 🚦📊

This repository contains the implementation of a deep learning project for traffic sign classification using the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset. The project includes a base CNN model and a regularized version using **Dropout** and **L2 regularization**, highlighting the importance of preventing overfitting.

---

## 📂 Dataset

The dataset used is the **GTSRB - German Traffic Sign Recognition Benchmark**.  
It was organized into:

- `train/` – contains labeled training images grouped by class.
- `val/` – validation split from the training data for performance monitoring.

---

## 🧠 Model Architectures

### 🔹 Base Model
- 3 Convolutional layers
- MaxPooling
- Fully connected layers

  ![traffic basemodel conf](https://github.com/user-attachments/assets/ba8617bc-ebe6-4158-b3aa-882f7e7ad20e)
![traffic basemodel plot](https://github.com/user-attachments/assets/d6faec7f-6468-4270-8a53-aecd0431f9b8)


### 🔹 Regularized Model
- Dropout layers added after Dense layers
- L2 Regularization applied to Conv and Dense layers
- Learning Rate Scheduler used for better convergence
![traffic reg model plot](https://github.com/user-attachments/assets/4ccecbff-3702-4659-afe7-98bcd8a8c5d2)
![traffic reg model conf](https://github.com/user-attachments/assets/7365e231-5b70-4d6d-afa3-fdf6d3d89ef0)


---

## 📈 Results

| Model            | Accuracy (Validation) | Accuracy (Test) |
|------------------|-----------------------|-----------------|
| Base Model       | ~85.8%                | ~4%             |
| Regularized Model| **~92%**              | **Significant improvement** |

- 🧪 Evaluated using: **Precision, Recall, F1-score**
- 📉 Training and validation loss/accuracy curves plotted
- 📋 Classification report included

---

## 🗂 Files Included

- `Traffic_Sign_Detection_Regularization.ipynb`: Jupyter notebook with all steps
- `Traffic_Sign_Classification_Report.docx`: Final report with explanations and results
- `README.md`: Project overview

---

## 🛠 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/Traffic-Sign-Classification.git
   cd Traffic-Sign-Classification
