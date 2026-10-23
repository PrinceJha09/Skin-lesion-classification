# HAM10000 Skin Lesion Classification with ResNet-18

This notebook explores image classification on the HAM10000 skin-lesion dataset using PyTorch and a pretrained ResNet-18 model.

## What the notebook does

- Downloads the HAM10000 dataset using `kagglehub`
- Loads metadata and maps image IDs to image files
- Splits data into training, validation, and test sets
- Applies image resizing, augmentation, and normalization
- Fine-tunes a pretrained ResNet-18 model
- Tracks training and validation loss/accuracy
- Evaluates the model using accuracy, a classification report, and a confusion matrix
- Runs a prediction on an example image

## Run in Google Colab

1. Open `Untitled11_fixed.ipynb` in Google Colab.
2. Select **Runtime → Change runtime type → T4 GPU** if a GPU is available.
3. Run cells in order from top to bottom.
4. The notebook downloads the dataset and trains the model. Training can take time.
5. The final prediction cell uses an image already found in the dataset, rather than the placeholder `your_image.jpg`.

To predict on your own image, use the optional upload snippet in the final cell after the model has been trained and the model checkpoint has been created.

## Dependencies

The notebook installs/uses PyTorch, torchvision, kagglehub, pandas, NumPy, Matplotlib, Seaborn, scikit-learn, and Pillow.

## Important note

This is an educational machine-learning project, not a medical diagnostic tool. Predictions and confidence scores should not be used to diagnose skin conditions or guide treatment.
