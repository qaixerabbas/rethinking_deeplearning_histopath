
# Rethinking complexity in deep learning for histopathology
## Overview

This project evaluates the performance of three Convolutional Neural Networks (CNNs) and three Vision Transformers (ViTs) on histopathological image classification tasks. The focus is on distinguishing between benign and malignant tissues in lung, colon, and breast cancers using high-resolution images at 400x magnification.

## Datasets

### 1. LC25000

- **Description**: The LC25000 dataset comprises 25,000 histopathological images categorized into five classes: colon adenocarcinoma, benign colonic tissue, lung adenocarcinoma, lung squamous cell carcinoma, and benign lung tissue. Each class contains 5,000 images.
- **Image Details**: JPEG format, 768x768 pixels.
- **Source**: [LC25000 Dataset](https://github.com/tampapath/lung_colon_image_set)

### 2. BreakHis

- **Description**: The BreakHis dataset contains 7,909 microscopic images of breast tumor tissue collected from 82 patients. The images are divided into benign and malignant categories, with further subclassifications.
- **Image Details**: PNG format, 700x460 pixels, 3-channel RGB.
- **Magnification Levels**: 40X, 100X, 200X, and 400X.
- **Focus**: This project utilizes images at 400X magnification.
- **Source**: [BreakHis Dataset](https://web.inf.ufpr.br/vri/databases/breast-cancer-histopathological-database-breakhis/)

## Models Evaluated

### Convolutional Neural Networks (CNNs)

1. **ResNet-50**
2. **EfficientNet-B0**
3. **ConvNeXt**

### Vision Transformers (ViTs)

1. **ViT-B/16**
2. **DeiT-B/16**
3. **Swin Transformer v2**

## Methodology

1. **Data Preprocessing**:
   - Resizing images to 224x224 pixels.
   - Normalization using dataset-specific mean and standard deviation.

2. **Training Protocol**:
   - Split datasets into training, validation, and test sets (70/30).
   - Use of cross-entropy loss function.
   - Optimization using Adam optimizer with an initial learning rate of 1e-4.

3. **Evaluation Metrics**:
   - Accuracy
   - Precision
   - Recall
   - F1-Score
   - Area Under the Receiver Operating Characteristic Curve (AUC-ROC)
   - False Negative Rate (FNR)
   - False Positive Rate (FPR)
   - Specificity
   - Training Time (in second)

## Results

will be updated soon

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://https://github.com/qaixerabbas/rethinking_deeplearning_histopath
   cd rethinking_deeplearning_histopath
   ```

2. **Create a Virtual Environment**:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

## License

This project is licensed under the MIT License.

## Contact

For questions or collaborations, please contact: [mqaiser617@gmail.com](mailto:mqaiser617@gmail.com)
