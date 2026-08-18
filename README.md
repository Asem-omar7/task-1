# Image Recognition with Teachable Machine

A simple image classification project trained using [Google's Teachable Machine](https://teachablemachine.withgoogle.com/) and run locally with TensorFlow/Keras and Python.

## Overview

This project trains an image recognition model with at least two classes using Teachable Machine, exports it in TensorFlow → Keras format, and uses a Python script to load the model and classify a new input image.

## Files in this Repository

| File | Description |
|---|---|
| `Ai.py` | Python script that loads the trained model and predicts the class of an input image |
| `keras_model.h5` | Exported trained model (Keras format) from Teachable Machine |
| `labels.txt` | Class labels used by the model |
| `screenshot.png` | Screenshot of the script output |

## Requirements

- Python 3.10 (Anaconda environment)
- TensorFlow / Keras
- Pillow (PIL)
- NumPy

Install dependencies:
```bash
pip install tensorflow pillow numpy
```

## How to Run

1. Clone this repository:
   ```bash
   git clone <your-repo-link>
   cd <repo-folder>
   ```

2. Activate the Anaconda environment:
   ```bash
   conda activate Teachable_machine
   ```

3. Update the image path inside `Ai.py` (line ~20) to point to the image you want to classify:
   ```python
   image = Image.open(r"path\to\your\image.jpg").convert("RGB")
   ```

4. Run the script:
   ```bash
   python Ai.py
   ```

## Example Output

```
1/1 [==============================] - 1s 626ms/step
Class: cat
Confidence Score: 0.9999988
```

## Model Training

The model was trained using Teachable Machine's image project with at least two classes, then exported in **TensorFlow → Keras** format and downloaded as `keras_model.h5` + `labels.txt`.

## Author

Submitted as part of a SmartMethods training task.
