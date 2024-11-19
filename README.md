# Image Super-Resolution Using Deep Learning

This repository implements an **Image Super-Resolution System** using a deep learning-based **Super-Resolution Convolutional Neural Network (SRCNN)**. The system enhances low-resolution images to high-resolution, making it ideal for tasks requiring image quality improvement.

## Features
- Implements the SRCNN architecture for super-resolution.
- Processes and trains on a subset of the **DIV2K dataset**.
- Generates low-resolution images by downscaling and reconstructs them to high resolution.
- Evaluates performance using **Peak Signal-to-Noise Ratio (PSNR)** and **Structural Similarity Index (SSIM)**.

## Results
- **PSNR**: 13.81
- **SSIM**: 0.38

These results reflect a basic implementation trained on a small dataset subset for demonstration purposes.

## Usage

### 1. Clone the Repository
```bash
git clone https://github.com/ahmdmohamedd/image-super-resolution-dl.git
cd image-super-resolution-dl
```

### 2. Install Dependencies
Ensure you have Python 3.8+ and install the required libraries:
```bash
pip install -r requirements.txt
```

### 3. Run the Notebook
Open the `image_super_resolution.ipynb` file in Jupyter Notebook or JupyterLab and run the cells step by step.

### 4. Output
The system outputs:
- Super-resolved images compared with ground truth high-resolution and input low-resolution images.
- Quantitative metrics (**PSNR** and **SSIM**) for performance evaluation.

## Dataset
The **DIV2K** dataset is used for training and evaluation:
- [DIV2K Dataset Homepage](https://data.vision.ee.ethz.ch/cvl/DIV2K/)

## Model Architecture
The SRCNN model consists of:
1. **Convolutional Layer 1**: 64 filters, 9x9 kernel, ReLU activation.
2. **Convolutional Layer 2**: 32 filters, 1x1 kernel, ReLU activation.
3. **Convolutional Layer 3**: 3 filters, 5x5 kernel, linear activation.

## Limitations
This implementation is a demonstration and may not produce state-of-the-art results:
- Trained with limited data and epochs.
- For improved performance, consider advanced architectures like **EDSR** or **ESRGAN**.

## Contributing
Feel free to fork the repository, create issues, or submit pull requests to enhance this project!

## Acknowledgements
- DIV2K Dataset creators for providing high-quality images for training and evaluation.
- The research paper [Image Super-Resolution Using Deep Convolutional Networks (SRCNN)](https://arxiv.org/abs/1501.00092) for the foundational model.

---
