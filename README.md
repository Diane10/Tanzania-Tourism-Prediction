# Face Occlusion Detection

## Overview
This project aims to detect occlusion in the face area, potentially returning the fraction of the face that is occluded as a quantitative metric. By treating occlusion detection as an attribute, we can fine-tune the backbone of the Hydranet model and specifically train a head for occlusion detection.

## Table of Contents
- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Installation Steps](#installation-steps)
- [Finetuning Occlusion Head](#finetuning-occlusion-head)
  - [Data Preparation](#data-preparation)
  - [Model Training](#model-training)
  - [Evaluation and Analysis](#evaluation-and-analysis)
  - [Demo Testing](#demo-testing)

## Installation

### Prerequisites
Ensure you have the following prerequisites installed:
- PyTorch
- OpenVINO

### Installation Steps
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/face-occlusion-detection.git
   ```

2. **Navigate into the project directory:**
   ```bash
   cd face-occlusion-detection
   ```

## Finetuning Occlusion Head

### Data Preparation
1. **Run `data_preparation.py`:**
   ```bash
   python data_preparation.py
   ```
   
2. **Create a `dataloader` folder to save train and validation data:**
   ```bash
   mkdir dataloader
   ```

3. **Run `fixbbox.py`:**
   ```bash
   python fixbbox.py
   ```

4. **Run `dataloader.py`:**
   ```bash
   python dataloader.py
   ```

### Model Training
1. **Run `finetuning.py`:**
   ```bash
   python finetuning.py
   ```

### Evaluation and Analysis
1. **Run `clean.py`:**
   ```bash
   python clean.py
   ```

2. **Run `trace_model.py`:**
   ```bash
   python trace_model.py
   ```

3. **Run `evaluation.py`:**
   ```bash
   python evaluation.py
   ```

4. **Run `analysis.py`:**
   ```bash
   python analysis.py
   ```

5. **Run `compare_analysis.py`:**
   ```bash
   python compare_analysis.py
   ```

### Demo Testing
1. **Run `demo_testing.py`:**
   ```bash
   python demo_testing.py
   ```

## Contributing
Feel free to submit issues or pull requests if you have any improvements or bug fixes.

## License
This project is licensed under the MIT License.

---

By following the steps outlined above, you should be able to set up and run the face occlusion detection project. If you encounter any issues, please refer to the documentation or open an issue on GitHub. 

