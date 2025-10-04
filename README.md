# MONAITHON is a 36 Hour Workshop + Hackathon
This is one of the incredible hackathon that I have participated where we gain a hands on experience towards workshop and also towards working on 2 different Datasets in hackathon that is BRATS(Brain Tumor) and DRIVE(Retina) dataset

# 🧠 Medical Image Segmentation – Hackathon Project  

## 🚀 Overview  
This project was developed as part of a **Hackathon Challenge** focused on **medical image segmentation** using deep learning.  
The objective was to preprocess, train, and deploy segmentation models for two medical imaging datasets — **BRATS 2020 (Brain Tumor Segmentation)** and **DRIVE (Retinal Vessel Segmentation)** — while demonstrating innovation and optimization under time constraints.  

---

## 🧩 Datasets Used  
1. **BRATS 2020 (3D MRI)** – Brain tumor segmentation (multi-class)  
   - Classes: Whole Tumor (WT), Tumor Core (TC), Enhancing Tumor (ET)  
   - [Dataset Link](https://www.kaggle.com/datasets/awsaf49/brats20-dataset-training-validation)
   - [Working Model]()

2. **DRIVE (2D Fundus Images)** – Retinal vessel segmentation (binary)  
   - Classes: Vessel vs Background  
   - [Dataset Link](https://www.kaggle.com/datasets/andrewmvd/drive-digital-retinal-images-for-vessel-extraction)
   - [Working Model](https://8501-gpu-t4-s-31tc5eq1udare-c.asia-southeast1-0.prod.colab.dev/)

---

## ⚙️ Task 1: Data Preprocessing & Augmentation ✅  
**Goal:** Prepare and augment both datasets for model training using **MONAI transforms**.  

### ✔️ Implemented Steps  
- For **BRATS 2020 (3D)**:  
  - `Spacingd`, `Orientationd`, `NormalizeIntensityd`, `RandCropByPosNegLabeld`  
- For **DRIVE (2D)**:  
  - `Resize`, `NormalizeIntensity`, `RandFlip`, `RandRotate`, `RandZoom`  
- Added **custom augmentations**:  
  - Gaussian Noise  
  - Elastic Deformation  
- Visualized **3 samples before vs after** transformations for both datasets.  

**Result:** Efficient preprocessing pipeline designed to improve generalization and avoid overfitting.

---

## 🧠 Task 5: Application Development ✅  
**Goal:** Create an interactive demo app using **Streamlit**.  

### ✔️ Features  
- Upload MRI or Fundus image for inference.  
- Choose between **Baseline UNet** and **Improved Model (e.g., Attention UNet)**.  
- View **segmentation overlays** (Ground Truth vs Prediction).  
- Implemented **optimized lightweight app** for smooth performance in **Google Colab** environment.  

**Deliverable:** A fully functional web app showcasing segmentation predictions and comparison.  

---

## 📊 Evaluation Metrics  
### For BRATS  
- Dice Score per class (WT, TC, ET)  
- Hausdorff95 Distance  
- Sensitivity & Specificity  

### For DRIVE  
- Dice, Precision, Recall, F1-Score  
- ROC-AUC & PR-AUC Curves  

**Outcome:** Achieved improved Dice and AUC scores compared to baseline models, validating the effectiveness of custom augmentations and post-processing.

---

## 🧩 Technologies & Tools  
- **Frameworks:** PyTorch, MONAI, Streamlit  
- **Environment:** Google Colab (GPU)  
- **Libraries:** NumPy, Matplotlib, OpenCV, scikit-learn  
- **Visualization:** Matplotlib & MONAI utilities  
- **Deployment:** Streamlit Web App (Colab-hosted)  

---

## 🏆 Achievements  
✅ Completed both **Task 1 (Preprocessing & Augmentation)** and **Task 5 (Streamlit App(DRIVE) , Gradio(BRATS))** efficiently within the hackathon timeline.  
✅ Successfully integrated preprocessing → model training → app deployment into one smooth workflow.  
✅ Showcased creativity through **custom augmentations** and **interactive application design**.  

---

## 📸 Screenshots (Optional)
_Add visuals like preprocessed samples, training curves, and Streamlit app interface here._

---

## 👥 Team & Contributions  
**Team Name:** *AAROH*  
**Team Members:**  
- Manjunath V Poojari 
- Harsha S 
- Tarun S
- Vikyath M A 

---

## 🧭 Future Scope  
- Upgrade models to **Swin UNETR** or **SegResNet** for performance gains.  
- Integrate **explainability tools (Grad-CAM)** for medical interpretability.  
- Deploy app on **Hugging Face Spaces** or **Streamlit Cloud**.  

---

### 🏁 Conclusion  
This hackathon project demonstrates the complete pipeline — from **data preprocessing and augmentation** to **model training and real-time web deployment** — showcasing technical efficiency, innovation, and teamwork.

---

