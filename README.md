
# BioRidge: Unlocking Blood Group via Fingerprint Ridge Analysis

## Overview

**BioRidge** presents a novel non-invasive approach to **blood group identification using fingerprint images**. By leveraging **deep learning**—specifically Convolutional Neural Networks (CNNs)—this project transforms traditional biometric systems into powerful medical tools. The system replaces conventional, time-consuming serological tests with fast, accessible fingerprint-based classification for emergency and remote applications.

##  Objectives

- Develop a non-invasive system to classify blood groups using fingerprint ridge patterns.
- Compare multiple CNN architectures (LeNet, AlexNet, VGG16, ResNet34) for model accuracy and generalization.
- Enable reliable blood group detection in emergency or resource-limited environments.

##  Key Features

- Predicts one of **8 blood groups** (A+, A−, B+, B−, AB+, AB−, O+, O−) from fingerprint images.
- Implements **image preprocessing** (grayscale conversion, resizing, normalization).
- Utilizes **data augmentation** to improve training performance.
- Benchmarks and evaluates four CNN models with performance metrics.

##  Model Architectures Used

| Model     | Description                                                                 |
|-----------|-----------------------------------------------------------------------------|
| LeNet     | Lightweight baseline CNN for simple ridge pattern recognition               |
| AlexNet   | Deeper model capturing moderate texture features                            |
| VGG16     | Deep network with strong feature extraction, used with transfer learning    |
| ResNet34  | Deepest model with residual connections for high-accuracy classification    |

##  Results Summary

| Model     | Test Accuracy | Loss    | Macro F1-Score |
|-----------|---------------|---------|----------------|
| ResNet34  | **79.03%**    | 0.6575  | **0.79**       |
| VGG16     | 75.04%        | 0.9706  | 0.75           |
| LeNet     | 70.88%        | 1.8616  | 0.71           |
| AlexNet   | 18.22%        | 2.0655  | 0.06           |

 **ResNet34** emerged as the most stable and accurate model.

##  Workflow

1. **Fingerprint Acquisition**  
2. **Image Preprocessing** (grayscale, resize, normalize, augment)  
3. **Model Training** with labeled blood group data  
4. **Prediction & Evaluation**


##  Installation & Setup

### Prerequisites
- Python 3.8+
- Virtual environment (recommended)

### Installation

```bash
# Clone the repository
git clone https://github.com/pneha244/Fingerprint-based-blood-group-detection.git

# Create virtual environment
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate

```

## Authors 
- **Neha P** – [p.neha244@gmail.com](mailto:p.neha244@gmail.com)  

