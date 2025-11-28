# Plant Disease Classification Using Deep Learning

**Graduation Project - Faculty of Computer and Information Sciences**

## Project Overview
Automated detection and classification of **38 plant diseases** using the **PlantVillage Dataset** with four deep learning architectures:
- VGG-19 (from scratch)
- ResNet-50 (transfer learning)
- Inception V3 (transfer learning)
- Vision Transformer / MobileNet (transfer learning)

**Final Test Accuracy**: **99.2%** (VGG-19 after duplicate removal)

## Dataset
- **Source**: [PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset)
- **Original Size**: 54,306 images
- **After Cleaning**: 54,284 unique images (**21 exact duplicates removed** using MD5 hashing)
- **Classes**: 38 (14 crops × healthy + diseased)

## Key Contributions
- Full duplicate removal to prevent data leakage
- Stratified train/val/test split (70/15/15)
- Data augmentation for real-world robustness
- Complete evaluation: Accuracy, Confusion Matrix, Precision/Recall/F1, ROC-AUC
- Detailed documentation and comparison between models

## Results Summary (VGG-19 from Scratch)
| Metric              | Value    |
|---------------------|----------|
| Test Accuracy       | 97.623%  |
| Test Loss           | 0.0812   |
| AUC (all classes)   | ≥ 0.999  |
| Parameters          | ~138M    |

## Project Structure
notebooks/          → All training notebooks
models/             → Saved models
report/             → Final report
logs/               → train logs &  test logs
Evaluation/         → images of model evaluation
README.md
requirements.txt

## Trained Model 
upload models on google drive (https://drive.google.com/drive/folders/1LxMFRf-8C0Po1UU-3n4LJGmgmj5QbQGH?dmr=1&ec=wgc-drive-hero-goto)