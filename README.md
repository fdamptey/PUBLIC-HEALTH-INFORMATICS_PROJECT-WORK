
# 🧠 Breast Cancer Detection Using Deep Learning on Ultrasound Images

## 📘 Project Title:
**Exploring Deep Learning AI Ultrasound as a Primary Breast Cancer Screening Test: An Informatics Approach to Cancer Prevention**

## 👨‍🔬 Authors:
**Frederick Damptey**  
**Benjamin Odoom Asomaning**

---

## 📄 Overview

This project investigates the use of deep learning, specifically **transfer learning with convolutional neural networks (CNNs)**, to classify breast ultrasound images into **normal, benign, and malignant** categories. Using a carefully preprocessed public dataset and models like **EfficientNetB0**, we aim to provide a **low-cost, highly accurate screening tool** that can be deployed especially in **resource-limited settings**.

---

## 🎯 Objectives

- Develop and fine-tune deep learning models for breast cancer classification.
- Evaluate model performance using clinically relevant metrics: **accuracy, AUC, sensitivity, and specificity**.
- Compare AI model performance against radiologists and traditional screening methods.
- Assess feasibility of using **AI-powered ultrasound** as a **primary screening tool**, especially in LMICs (low- and middle-income countries).

---

## 📚 Dataset

- **Primary Source:** [Kaggle Breast Ultrasound Images Dataset (BUSI)](https://www.kaggle.com/datasets/aryashah2k/breast-ultrasound-images-dataset/data)
- **Secondary Source:** [Cancer Imaging Archive - Breast Lesions USG](https://www.cancerimagingarchive.net/collection/breast-lesions-usg/)

The dataset consists of **780 ultrasound images** divided into three classes:
- `normal`
- `benign`
- `malignant`

Ground truths were established through comparison with mammograms and confirmed by histopathology.

---

## 🛠️ Methods

### 🧪 Preprocessing
- Resizing images to `224x224`
- RGB conversion for model compatibility
- Image normalization and augmentation
- K-Fold Cross-Validation (K=5)

### 🧠 Models Used
All models were pretrained on ImageNet:
- ✅ **EfficientNetB0** *(Best Performing Model)*
- ResNet50
- VGG16
- InceptionV3

### 🧮 Evaluation Metrics
- **Accuracy**
- **AUC (Area Under Curve)**
- **Sensitivity**
- **Specificity**
- Confusion matrix and ROC curves

---

## 🏆 Results

| Model         | Accuracy | AUC   | Sensitivity | Specificity |
|---------------|----------|-------|-------------|-------------|
| **EfficientNetB0** | **0.95**   | **0.99** | **0.933**     | **0.970**     |
| InceptionV3   | 0.941    | 0.982 | 0.934       | 0.962       |
| VGG16         | 0.933    | 0.982 | 0.909       | 0.951       |
| ResNet50      | 0.92     | 0.964 | 0.881       | 0.945       |

---

## ✅ Conclusion

The EfficientNetB0 deep learning model achieved **high accuracy (95%)**, **sensitivity (93%)**, **specificity (97%)**, and **AUC (0.99)**, outperforming several other AI models, radiologist benchmarks, and many mammography-based systems.  

This positions **AI-enhanced ultrasound** as a **promising primary screening tool** for breast cancer, especially in regions where **mammography access is limited**.

---

## ⚠️ Limitations

- Relatively small dataset size
- Limited hardware for extensive experimentation
- Time constraints affected the depth of literature review and retraining iterations

---

## 🔭 Future Work

- Expand dataset diversity and size for better generalization
- Implement explainable AI (XAI) components
- Integrate segmentation and lesion localization
- Conduct meta-analytic performance benchmarking
- Validate models in clinical settings

---

## 💾 Installation

Clone this repository:
```bash
git clone https://github.com/yourusername/breast-cancer-ultrasound-AI.git
cd breast-cancer-ultrasound-AI
```

Install dependencies:
```bash
pip install -r requirements.txt
```

Run training:
```bash
python train_model.py
```

---

## 🔗 References

- Hijab et al. (2019), ICABME Conference  
- Li et al. (2024), Clinical Radiology  
- Yoon et al. (2023), Radiology  
- WHO (2024), Breast Cancer Fact Sheet  
- [Full reference list available in `/docs/references.bib` or project paper]

---

## 📬 Contact

For collaboration, questions, or access to supplementary materials, reach out via:

📧 **Email:** [YourEmail@example.com]  
🔗 **LinkedIn:** [Your LinkedIn Profile]
