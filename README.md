# Seizure Prediction using CHB-MIT Dataset

## Introduction
This project focuses on **seizure prediction** using the **CHB-MIT EEG dataset**. The preprocessing phase involves converting EEG signals into an **amino acid sequence representation** to improve feature extraction. A **lightweight 1D CNN model** is developed to ensure the implementation is suitable for wearable devices like **smartwatches**.

## Preprocessing Pipeline
1. **DNA-like Sequence Representation:**
   - Convert EEG signals into a symbolic sequence mimicking DNA structure.
2. **RNA Sequence Conversion:**
   - Transform the DNA-like sequence into an RNA-like sequence.
3. **Codon Formation:**
   - Group the RNA sequence into triplets (codons).
4. **Amino Acid Sequence Generation:**
   - Map codons to amino acids to create a meaningful sequence representation.

## Classification Task
- The model classifies EEG signals into **preictal** (before seizure) and **ictal** (during seizure) phases.
- This helps in predicting seizures before they occur, enabling timely intervention.

## Model Architecture
- **1D Convolutional Neural Network (CNN)** designed for seizure prediction.
- Optimized for **low computational cost** to run on wearable devices.
- Includes **convolutional layers, batch normalization, dropout, and fully connected layers**.

## Technologies Used
- **Python** (NumPy, Pandas, TensorFlow/Keras, Matplotlib)
- **Deep Learning** (1D CNN)
- **Data Preprocessing** (Custom sequence transformation)

## Requirements
To run this project, install dependencies using:
```sh
pip install numpy pandas tensorflow keras matplotlib
```

## Usage
Run the following command to train and evaluate the model:
```sh
python seizure_prediction.py
```

## Future Enhancements
- Further optimize the model for **real-time predictions**.
- Implement **edge AI techniques** for wearable deployment.
- Test on **different EEG datasets** for generalization.

## Author
[Bikash Konwar]

## License
This project is open-source and available under the MIT License.

