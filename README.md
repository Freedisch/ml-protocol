# Breast Cancer Image Classification using Transfer Learning

## Dataset

The dataset contains images related to bread cancer. Each image has a corresponding mask image.

## Pre-trained Models

We selected the following pre-trained models:

- **VGG16**: Known for its simplicity and effectiveness in image classification tasks.
- **ResNet50**: Utilizes residual learning, which allows training of very deep networks.
- **InceptionV3**: Combines multiple filter sizes and network-in-network architectures, providing high accuracy.

## Fine-Tuning

We fine-tuned the models by modifying the top layers and training them on the dataset. The following layers were modified:

- **GlobalAveragePooling2D**: To reduce the feature maps.
- **Dense (1024 units)**: Added for high-level features.
- **Dense (1 unit)**: Output layer for binary classification with sigmoid activation.

## Usage

To use this project:

1. Clone the repository to your local machine.
2. Ensure that the dataset is stored at the correct path, as specified in the notebook.
3. Open the `Transfer_Learning_Assignment.ipynb` notebook in Jupyter or another IPython notebook viewer.
4. Run the cells sequentially to perform the data preprocessing, model training, and evaluation.

## Evaluation Metrics

The models are evaluated based on the following metrics:

- Accuracy
- Loss
- Precision
- Recall
- F1 Score

These metrics are crucial for assessing the performance of the models, particularly in a medical context where accuracy and reliability are paramount.

## Results

The results section will contain tables and charts generated from the notebook, providing a visual and quantitative comparison of the performance of the different models.

## Contributions

Contributions to this project are welcome. You can contribute by improving the model training pipeline, introducing new models, or enhancing the data preprocessing steps.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
