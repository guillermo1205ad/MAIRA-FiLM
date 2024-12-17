# Machine Learning Pipeline

This repository contains Jupyter Notebooks for **fine-tuning**, **training**, and **testing** machine learning models.

## Notebooks Overview

### 1. Fine-Tuning
**Description:**  
Fine-tuning the model using specific configurations.

**Key Snippets:**  
```python
!wget -O CLEVR_sample_10_000.tar.gz "https://www.dropbox.com/scl/fi/l87paducv9fmmkiymjfaw/CLEVR_samp"
```
```python
!mkdir -p data
!tar -xzvf CLEVR_sample_10_000.tar.gz -C data/
```

### 2. Train
**Description:**  
Training the model using a defined dataset and hyperparameters.

**Key Snippets:**  
```python
import os
import json
import torch
import torch.nn as nn
import torch.optim as optim
import matplotlib.pyplot as plt
```

### 3. Test
**Description:**  
Testing and evaluating the trained model on specific datasets.

**Key Snippets:**  
```python
import os

# Download and extract the CLEVR dataset if it does not exist
if not os.path.exists('/home/gpe'):
    !wget -O CLEVR_sample.tar.gz "https://link_to_dataset"
    !tar -xzvf CLEVR_sample.tar.gz -C data/
```
```python
import json
import torch
import torch.nn as nn
from torchvision import models, transforms
```

## Installation

Ensure the following dependencies are installed:
```bash
pip install -r requirements.txt
```

## How to Use

1. **Fine-Tuning:** Run the `Fine-Tuning` notebook to fine-tune the base model.
2. **Train:** Use the `Train` notebook to train the model on your dataset.
3. **Test:** Execute the `Test` notebook to evaluate the model's performance.

## Requirements

- Python >= 3.8
- Jupyter Notebook
- PyTorch or TensorFlow (depending on the model used)

## License

This project is licensed under the **Apache 2.0** License. See the `LICENSE` file for more information.
