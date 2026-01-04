# Coral Reef Health Monitoring System

## Group Information

Group Number: WS25PR14

Group Members and Roles

1) Student 1 (Technical Lead): Mihir Vinodkumar Rami

2) Student 2 (Figures & Tables): Sujal Ileshbhai Patel  

3) Student 3 (Report & Storytelling): Luvkumar Vinodbhai Patel


## Project Overview

This project presents a **hybrid AI-based system for coral reef health monitoring** using underwater imagery.  
The system integrates:
- A Convolutional Neural Network (CNN) for visual feature learning
- A meta-learning model combining CNN confidence with handcrafted image features
- A rule-based reasoning engine for improved robustness
- Explainability using Grad-CAM
- Robustness evaluation under environmental variations

## Dataset

- **Source:** Kaggle – Coral Reef Image Dataset  
- **Classes:**  
  - Healthy Coral  
  - Bleached Coral  

The dataset is preprocessed using resizing, normalization, and augmentation techniques.  
Data is split into training, validation, and testing sets.

## Research Questions (RQs)

The project defines and evaluates **exactly five research questions**:

- **RQ1:** Can a CNN effectively classify coral reef health from underwater images?
- **RQ2:** Does combining CNN predictions with handcrafted image features improve performance?
- **RQ3:** Can rule-based reasoning enhance robustness and decision reliability?
- **RQ4:** Is the model’s decision-making process interpretable?
- **RQ5:** How robust is the system under environmental variations such as brightness and blur?

## Model Architecture

### 1. Base Learner
- CNN using a pretrained **MobileNetV2**
- Fine-tuned for binary classification

### 2. Meta-Learner
- Logistic Regression
- Inputs:
  - CNN prediction probabilities
  - Handcrafted features (brightness, blue channel ratio, white pixel ratio)

### 3. Rule-Based Engine
- Expert-defined IF–THEN rules
- Applied after meta-learning to correct uncertain predictions

### 4. Explainability
- Grad-CAM visualizations to highlight image regions influencing predictions

## Figures & Tables

All figures and tables are provided in **RQ-wise folders** inside

## How to Reproduce Results

1. Clone the repository:
   ```bash
   git clone https://github.com/Mihir-MR/Coral-Reef-Health-Monitoring.git
2. Navigate to the project directory
3. Create and activate a Python environment
4. Install dependencies:
  pip install -r requirements.txt
5. Open notebook.ipynb and run all cells sequentially from top to bottom


