## 🧠 Meal Nutrition Analysis using Multimodal AI  

### 📌 Overview
This project aimed to **predict lunch calorie intake** using **multimodal data**, incorporating **meal images**, **continuous glucose monitoring (CGM)** data, and **demographic details**. The dataset consisted of **40 participants observed over 10 days**, addressing limitations in traditional calorie estimation by integrating diverse data sources.

A **multimodal neural network** was developed, leveraging:
- 🖼️ **CNNs** for meal image analysis  
- 📉 **LSTMs** for glucose trend predictions  
- 🧾 **Fully Connected Networks (FCNs)** for demographic and clinical data

The model was trained using **RMSRE loss** and **outperformed established benchmarks**, showcasing the effectiveness of multimodal learning in personalized healthcare and nutrition monitoring.

---

### ✅ Key Contributions & Technical Work

#### 🔧 Data Preprocessing & Integration
- Processed meal images, CGM time-series data, and demographic details, aligning them into a unified dataset for training.  
- Normalized image data for CNN input and structured glucose readings into time-series sequences.

#### 🧠 Model Development
- Designed a multimodal neural network in **PyTorch**, combining **CNNs (ResNet-18)**, **LSTMs**, and **FCNs**.  
- Implemented **feature fusion** to integrate insights from visual, sequential, and tabular data.  
- Used pretrained **ResNet-18** for image feature extraction and adapted it for a six-channel input (combining breakfast and lunch images).

#### ⚙️ Optimization & Training
- Tuned parameters using **Adam optimizer**, **ReLU** activations, and **dropout** to prevent overfitting.  
- Selected the best model based on validation loss, achieving improved accuracy over traditional calorie prediction methods.

#### 📈 Results & Impact
- The multimodal model **significantly outperformed single-source methods** in calorie prediction.  
- Achieved a **score of 0.3218**, surpassing the **Kaggle benchmark of 0.5258**, demonstrating strong generalization through multimodal integration.

---

### 🛠 Tech Stack & Tools

📊 **Machine Learning & AI**: Python, PyTorch, CNNs, LSTMs, FCNs  
📷 **Computer Vision**: ResNet-18 for meal image processing  
📈 **Time-Series Analysis**: LSTM for glucose monitoring data  
🛠 **Data Processing**: Pandas, NumPy, StandardScaler, One-Hot Encoding  
⚡ **Deep Learning Optimization**: Adam Optimizer, RMSRE Loss, Dropout Regularization  

---

🚀 This project highlights the **power of multimodal AI** in healthcare and personalized nutrition, paving the way for **smarter dietary recommendations**.
