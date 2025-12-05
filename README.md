# Real-Time Plant Disease Detection in Smart Agriculture Using a YOLO11x-Based Deep Learning Model

This repository contains the complete implementation, evaluation scripts, and supplementary materials for the research work:

**"Real-Time Plant Disease Detection in Smart Agriculture Using a YOLO11-Based Deep Learning Model"**

The system uses **YOLO11x** trained on a **23-class multi-crop dataset** consisting of:
- Chili  
- Eggplant  
- Potato  
- Tomato  

The model achieves:
- **Precision: 99%**
- **Recall: 97%**
- **mAP50: 96%**
- **Real-time inference: 16–17 FPS on NVIDIA Tesla T4**

---

##  Repository Contents

### **1. `training_script_yolo11x.ipynb`**
Main training notebook used for YOLO11x model training (Kaggle environment).

### **2. `config_files/`**
Contains dataset and training configuration:
- `data.yaml`
- `args.yaml`

### **3. `Ablation_study/`**
Includes 4 ablation experiment notebooks:
- Batch size effect  
- Image size variation  
- Mosaic disabled  
- Strong augmentation  

### **4. `cross_dataset_test_samples/`**
Manually tested images from publicly available sources to verify generalization.

### **5. `evaluation_and_tests/`**
Includes FPS measurement and class balance analysis.

---

##  Model Weights (Zenodo DOI)

The trained YOLO11x model weights are hosted on Zenodo:

 **https://doi.org/10.5281/zenodo.17829240**

Files available:
- `best.pt` – Best performing weight  
- `last.pt` – Final epoch weight  

> These weights are required to reproduce inference results.

---

##  Training Environment
- Python 3.11  
- Ultralytics YOLO11x  
- NVIDIA Tesla T4 (Kaggle)  
- AMP enabled  
- Batch size: 24  
- Image size: 640×640  

---

##  Key Features
- Real-time disease detection  
- 23-class multi-crop dataset  
- Ablation experiments included  
- Failure case analysis  
- Cross-dataset performance testing  
- Fully open-source reproducible workflow  

---

##  Citation

If you use this work, please cite the Zenodo weight repository:

**IEEE Format:**
