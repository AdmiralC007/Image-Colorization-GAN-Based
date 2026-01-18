🎨 Image Colorisation Using GAN
===============================

This project implements a **Generative Adversarial Network (GAN)** to perform **automatic colorization of black-and-white images**. The system learns to map grayscale images to realistic RGB color images using deep learning.

📂 Project Directory Structure (Exact)
--------------------------------------
```
Image Colorisation using GAN 2/
│
├── models/
│   ├── generator.py          # Generator network architecture
│   ├── discriminator.py      # Discriminator network architecture
│   └── __pycache__/           # Python cache files
│
├── utils/
│   ├── data_loader.py        # Dataset loading and preprocessing
│   └── __pycache__/           # Python cache files
│
├── outputs/
│   ├── checkpoints/
│   │   └── gen_epoch_99.pth  # Final retained generator checkpoint
│   └── images/
│       └── colorized_output.png  # Sample colorized output
│
├── train.py                  # Training script
├── test.py                   # Model testing script
├── test1.py                  # Additional testing / experimentation
├── 1.py                      # Initial or experimental script
├── tempCodeRunnerFile.py     # IDE auto-generated file
├── requirements.txt          # Required Python dependencies
└── README.md

```

🧠 Model Description
--------------------

### 🔹 Generator (models/generator.py)

*   Accepts **grayscale images** as input
    
*   Learns to generate corresponding **RGB color images**
    
*   Uses convolutional layers to extract spatial features
    

### 🔹 Discriminator (models/discriminator.py)

*   Takes real and generated color images
    
*   Classifies them as **real** or **fake**
    
*   Helps the generator improve realism through adversarial training
    

⚙️ Utilities
------------

### 📦 Data Loader (utils/data\_loader.py)

*   Handles dataset loading
    
*   Converts images to grayscale where required
    
*   Applies necessary preprocessing and tensor conversion
    
*   Supplies data to training and testing pipelines
    

🚀 Training the Model
---------------------

### 1️⃣ Install Dependencies

`   pip install -r requirements.txt   `

### 2️⃣ Start Training

`   python train.py   `

*   Generator and Discriminator are trained simultaneously
    
*   Model weights are periodically saved in:
    

`   outputs/checkpoints/   `

🧪 Testing & Inference
----------------------

### Run Testing Script

`   python test.py   `

or

`   python test1.py   `

*   Loads the trained generator model
    
*   Produces colorized outputs
    
*   Output images are saved in:
    

`   outputs/images/   `

🖼️ Sample Output
-----------------

A sample generated output is provided:

`   outputs/images/colorized_output.png   `

This image demonstrates the model’s ability to infer and apply realistic colors to grayscale inputs.

⚠️ Checkpoint Notice (Important)
--------------------------------

To manage repository size and avoid large uploads:

*   **Intermediate epoch checkpoints were removed**
    
*   Only the **final trained generator checkpoint** is retained:
    

`   outputs/checkpoints/gen_epoch_99.pth   `

### ✅ This means:

*   The project is **fully functional**
    
*   Training can be reproduced by rerunning train.py
    
*   Model performance is preserved using the final checkpoint
    

🛠️ Dependencies
----------------

All dependencies are listed in:

`   requirements.txt   `

Typical libraries include:

*   Python
    
*   PyTorch
    
*   NumPy
    
*   OpenCV / PIL
    
*   Torchvision
    

📌 Notes
--------

*   1.py and test1.py were used for experimentation and validation
    
*   tempCodeRunnerFile.py is IDE-generated and not required for execution
    
*   \_\_pycache\_\_ folders can be safely ignored
    

🔮 Future Enhancements
----------------------

*   Improve color accuracy using perceptual loss
    
*   Add support for high-resolution images
    
*   Create a web-based UI for image upload and colorization
    
*   Optimize training speed and memory usage
    

👤 Authors
----------

**Maddikatla Chaitanya (VCE)**

**Vanapalli Darpad Sai (VCE)**
