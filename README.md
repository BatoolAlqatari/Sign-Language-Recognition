# 🤟 Sign Language Recognition Using Image Processing and EfficientNet

A sign language recognition system using image processing and deep learning (EfficientNet), built as part of an Image Processing course.

## 📌 Overview
The system recognizes American Sign Language (ASL) gestures using RGB images. A series of image enhancement techniques were applied to preprocess hand gesture images for improved classification performance.

## 🎯 Goal
Enable robust and accurate classification of ASL letters using:
- Preprocessing (noise reduction, contrast enhancement, edge detection)
- Transfer learning with **EfficientNet-B0**
- PyTorch for deep learning implementation

## 🧪 Techniques Used

- 📦 Dataset: [ASL Fingerspelling (RGB and Depth)](https://www.kaggle.com/datasets/mrgeislinger/asl-rgb-depth-fingerspelling-spelling-it-out)
- 🖼️ Preprocessing:
  - Canny Edge Detection
  - Median Filtering (best accuracy: 95.4%)
  - Contrast Enhancement (CLAHE)
  - Thresholding
- 🧠 Model:
  - Transfer learning with EfficientNet-B0
  - Customized classifier head with dropout and ReLU
  - Accuracy comparison across filters

| Preprocessing Technique        | Accuracy |
|-------------------------------|----------|
| Median Filter                 | **95.4%** |
| CLAHE + Gaussian Filter       | 94.5%    |
| Thresholding                  | 84.8%    |
| Canny Edge Detection          | 79.3%    |
| Original Dataset (No Filters) | 86.0%    |

## 📊 Results

- Achieved best accuracy of **95.4%** using the median filter.
- Significant performance improvement through preprocessing.
- Visual and metric-based evaluation to analyze model predictions.

## 📷 Sample Screenshots

### Original Image
<img width="104" alt="image" src="https://github.com/user-attachments/assets/6adea140-794a-451e-ad75-9c77f769108c" />

### Image After Applying Canny Filter
<img width="103" alt="image" src="https://github.com/user-attachments/assets/c70598fe-dd1c-49bf-988f-3ac0211effe0" />


## 🚧 Limitations & Future Work

- Current version only supports static image classification.
- Real-time webcam input shows instability due to limited dataset diversity.
- Future improvements:
  - Real-time detection with robust background removal
  - More diverse datasets
  - Edge deployment (e.g., mobile app, webcam app)

## 👩‍💻 Team Members

- Kavya Ram Inder Mal
- Joud Adel Aldhuwaihi
- Batool Nabeel Alqatari
- Munirah Khaleel Almutlaq
- Raghad Dasman Alsubaie

Supervised by **Ms. Sara Althubaiti**

---


