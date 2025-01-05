# Fashion-MNIST Interpretability

This project demonstrates the use of interpretability techniques on a Convolutional Neural Network (CNN) trained on the Fashion-MNIST dataset. Explore how models make decisions using methods like Integrated Gradients, Saliency Maps, and Feature Permutation.

## Overview

### Key Features:
- **Dataset**: Fashion-MNIST, a collection of 28x28 grayscale images of fashion items, used for classification tasks.
- **Model**: A custom CNN with three convolutional layers and fully connected layers.
- **Training**: Efficient training loop with progress tracking over 5 epochs.
- **Evaluation**: Performance metrics on test data to assess model accuracy.
- **Interpretability**:
  - Integrated Gradients
  - Saliency Maps
  - Gaussian-Smooth Saliency Maps
  - Feature Permutation Analysis

## Getting Started

### Requirements:
- Python 3.8 or higher
- Required libraries: 
  - `torch`
  - `torchvision`
  - `captum`
  - `numpy`
  - `matplotlib`
  - `tqdm`

Install dependencies using:
```bash
pip install -r requirements.txt
Project Structure:
bash
Copy code
Fashion-MNIST-Interpretability/
├── data/               # Dataset folder
├── interpretability.py # Functions for analysis and visualizations
├── model.py            # CNN architecture
├── train.py            # Training script
├── evaluate.py         # Test data evaluation
├── notebook.ipynb      # Interactive workflow
├── README.md           # Project documentation
└── requirements.txt    # Python dependencies
Usage
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/Fashion-MNIST-Interpretability.git
cd Fashion-MNIST-Interpretability
Prepare the environment:

bash
Copy code
pip install -r requirements.txt
Run the notebook: Open notebook.ipynb to train the CNN and explore interpretability techniques interactively.

Execute standalone scripts:

Train the model:
bash
Copy code
python train.py
Evaluate test data:
bash
Copy code
python evaluate.py
Interpretability Techniques
1. Integrated Gradients
Highlights input features most influential for model predictions.

2. Saliency Maps
Identifies areas of the input image that impact the output the most.

3. Gaussian-Smooth Saliency Maps
Applies Gaussian blur to saliency maps for clearer interpretations.

4. Feature Permutation
Analyzes how shuffling specific image regions affects prediction confidence.

Results
Achieved competitive accuracy on Fashion-MNIST.
Interpretability methods offer valuable insights into model decision-making.
Future Enhancements
Extend to other datasets like CIFAR-10 or ImageNet.
Implement Grad-CAM and SHAP for advanced interpretations.
Create an interactive visualization dashboard.
License
This project is licensed under the MIT License. See the LICENSE file for details.
